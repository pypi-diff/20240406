# Comparing `tmp/primula-0.2.tar.gz` & `tmp/primula-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primula-0.2.tar", last modified: Tue Mar 19 13:30:10 2024, max compression
+gzip compressed data, was "primula-0.3.tar", last modified: Sat Apr  6 05:13:19 2024, max compression
```

## Comparing `primula-0.2.tar` & `primula-0.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-03-19 13:30:10.127091 primula-0.2/
--rw-r--r--   0 hattya    (1000) users      (100)      218 2024-03-19 13:28:15.000000 primula-0.2/CHANGES.rst
--rw-r--r--   0 hattya    (1000) users      (100)    11358 2024-02-17 12:18:15.000000 primula-0.2/LICENSE.txt
--rw-r--r--   0 hattya    (1000) users      (100)      129 2024-03-17 06:37:02.000000 primula-0.2/MANIFEST.in
--rw-r--r--   0 hattya    (1000) users      (100)     2948 2024-03-19 13:30:10.127091 primula-0.2/PKG-INFO
--rw-r--r--   0 hattya    (1000) users      (100)     2003 2024-03-17 06:37:02.000000 primula-0.2/README.rst
-drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-03-19 13:30:10.115091 primula-0.2/primula/
--rw-r--r--   0 hattya    (1000) users      (100)      378 2024-03-03 06:33:33.000000 primula-0.2/primula/__init__.py
--rw-r--r--   0 hattya    (1000) users      (100)      155 2024-03-06 12:07:13.000000 primula-0.2/primula/__main__.py
--rw-r--r--   0 hattya    (1000) users      (100)       58 2024-03-19 13:30:10.000000 primula-0.2/primula/__version__.py
--rw-r--r--   0 hattya    (1000) users      (100)      343 2024-02-17 12:18:15.000000 primula-0.2/primula/_typing.py
--rw-r--r--   0 hattya    (1000) users      (100)     6479 2024-03-17 07:36:47.000000 primula-0.2/primula/cli.py
--rw-r--r--   0 hattya    (1000) users      (100)    10244 2024-03-18 13:07:16.000000 primula-0.2/primula/core.py
--rw-r--r--   0 hattya    (1000) users      (100)      399 2024-02-17 12:18:15.000000 primula-0.2/primula/exception.py
--rw-r--r--   0 hattya    (1000) users      (100)     2598 2024-03-03 06:33:33.000000 primula-0.2/primula/plugin.py
--rw-r--r--   0 hattya    (1000) users      (100)        0 2024-02-17 12:18:15.000000 primula-0.2/primula/py.typed
-drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-03-19 13:30:10.127091 primula-0.2/primula.egg-info/
--rw-r--r--   0 hattya    (1000) users      (100)     2948 2024-03-19 13:30:10.000000 primula-0.2/primula.egg-info/PKG-INFO
--rw-r--r--   0 hattya    (1000) users      (100)     2117 2024-03-19 13:30:10.000000 primula-0.2/primula.egg-info/SOURCES.txt
--rw-r--r--   0 hattya    (1000) users      (100)        1 2024-03-19 13:30:10.000000 primula-0.2/primula.egg-info/dependency_links.txt
--rw-r--r--   0 hattya    (1000) users      (100)       44 2024-03-19 13:30:10.000000 primula-0.2/primula.egg-info/entry_points.txt
--rw-r--r--   0 hattya    (1000) users      (100)       14 2024-03-19 13:30:10.000000 primula-0.2/primula.egg-info/requires.txt
--rw-r--r--   0 hattya    (1000) users      (100)        8 2024-03-19 13:30:10.000000 primula-0.2/primula.egg-info/top_level.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1673 2024-03-06 12:07:13.000000 primula-0.2/pyproject.toml
--rw-r--r--   0 hattya    (1000) users      (100)      198 2024-03-19 13:30:10.128091 primula-0.2/setup.cfg
-drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-03-19 13:30:10.118091 primula-0.2/tests/
--rw-r--r--   0 hattya    (1000) users      (100)      553 2024-03-03 06:33:33.000000 primula-0.2/tests/base.py
-drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-03-19 13:30:10.124091 primula-0.2/tests/profiles/
--rw-r--r--   0 hattya    (1000) users      (100)     1554 2024-03-07 13:02:00.000000 primula-0.2/tests/profiles/autoload.v7.4.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1668 2024-02-25 13:48:04.000000 primula-0.2/tests/profiles/autoload.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1658 2024-02-18 06:32:35.000000 primula-0.2/tests/profiles/autoload.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1755 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/autoload.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1202 2024-03-07 13:02:00.000000 primula-0.2/tests/profiles/dict.v7.4.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1290 2024-02-25 13:48:04.000000 primula-0.2/tests/profiles/dict.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1280 2024-02-18 06:32:35.000000 primula-0.2/tests/profiles/dict.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1359 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/dict.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1084 2024-03-07 13:02:00.000000 primula-0.2/tests/profiles/duplicate.v7.4.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1182 2024-02-25 13:48:04.000000 primula-0.2/tests/profiles/duplicate.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1172 2024-02-25 13:48:04.000000 primula-0.2/tests/profiles/duplicate.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1248 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/duplicate.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)     2636 2024-03-07 13:02:00.000000 primula-0.2/tests/profiles/execute.v7.4.txt
--rw-r--r--   0 hattya    (1000) users      (100)     3136 2024-02-25 13:48:04.000000 primula-0.2/tests/profiles/execute.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)     3105 2024-02-21 11:55:00.000000 primula-0.2/tests/profiles/execute.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)     3337 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/execute.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1121 2024-03-07 13:02:00.000000 primula-0.2/tests/profiles/global.v7.4.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1213 2024-02-25 13:48:04.000000 primula-0.2/tests/profiles/global.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1203 2024-02-18 06:32:35.000000 primula-0.2/tests/profiles/global.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1279 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/global.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)      659 2024-03-09 13:49:49.000000 primula-0.2/tests/profiles/lambda.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)      654 2024-03-09 13:49:49.000000 primula-0.2/tests/profiles/lambda.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)      697 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/lambda.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)      974 2024-03-07 13:02:00.000000 primula-0.2/tests/profiles/line_continuation.v7.4.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1096 2024-02-25 13:48:04.000000 primula-0.2/tests/profiles/line_continuation.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1091 2024-02-19 13:11:50.000000 primula-0.2/tests/profiles/line_continuation.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1146 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/line_continuation.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)     5320 2024-03-07 13:02:00.000000 primula-0.2/tests/profiles/nested.v7.4.txt
--rw-r--r--   0 hattya    (1000) users      (100)     5740 2024-02-27 13:36:18.000000 primula-0.2/tests/profiles/nested.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)     5695 2024-02-27 13:36:18.000000 primula-0.2/tests/profiles/nested.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)     6161 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/nested.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1175 2024-03-07 13:02:00.000000 primula-0.2/tests/profiles/script_local.v7.4.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1279 2024-02-25 13:48:04.000000 primula-0.2/tests/profiles/script_local.v8.1.0365.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1269 2024-02-18 06:32:35.000000 primula-0.2/tests/profiles/script_local.v9.0.0000.txt
--rw-r--r--   0 hattya    (1000) users      (100)     1345 2024-03-18 13:07:16.000000 primula-0.2/tests/profiles/script_local.v9.0.1411.txt
--rw-r--r--   0 hattya    (1000) users      (100)     8975 2024-03-06 12:07:13.000000 primula-0.2/tests/test_cli.py
--rw-r--r--   0 hattya    (1000) users      (100)    35969 2024-03-09 13:49:49.000000 primula-0.2/tests/test_core.py
--rw-r--r--   0 hattya    (1000) users      (100)     2573 2024-03-03 06:33:33.000000 primula-0.2/tests/test_plugin.py
-drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-03-19 13:30:10.126091 primula-0.2/tests/vimfiles/
-drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-03-19 13:30:10.127091 primula-0.2/tests/vimfiles/autoload/
--rw-r--r--   0 hattya    (1000) users      (100)      216 2024-02-17 12:18:15.000000 primula-0.2/tests/vimfiles/autoload/autoload.vim
--rw-r--r--   0 hattya    (1000) users      (100)       21 2024-02-17 12:18:15.000000 primula-0.2/tests/vimfiles/autoload.vim
--rw-r--r--   0 hattya    (1000) users      (100)      184 2024-02-17 12:18:15.000000 primula-0.2/tests/vimfiles/dict.vim
--rw-r--r--   0 hattya    (1000) users      (100)      120 2024-02-25 13:48:04.000000 primula-0.2/tests/vimfiles/duplicate.vim
--rw-r--r--   0 hattya    (1000) users      (100)      508 2024-02-21 11:55:00.000000 primula-0.2/tests/vimfiles/execute.vim
--rw-r--r--   0 hattya    (1000) users      (100)      136 2024-02-17 12:18:15.000000 primula-0.2/tests/vimfiles/global.vim
--rw-r--r--   0 hattya    (1000) users      (100)       48 2024-03-09 13:49:49.000000 primula-0.2/tests/vimfiles/lambda.vim
--rw-r--r--   0 hattya    (1000) users      (100)      112 2024-02-19 13:11:50.000000 primula-0.2/tests/vimfiles/line_continuation.vim
--rw-r--r--   0 hattya    (1000) users      (100)      625 2024-02-27 13:36:18.000000 primula-0.2/tests/vimfiles/nested.vim
--rw-r--r--   0 hattya    (1000) users      (100)      142 2024-02-17 12:18:15.000000 primula-0.2/tests/vimfiles/script_local.vim
--rw-r--r--   0 hattya    (1000) users      (100)      338 2024-02-17 12:18:15.000000 primula-0.2/tests/vimfiles/vimrc
+drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-04-06 05:13:19.677920 primula-0.3/
+-rw-r--r--   0 hattya    (1000) users      (100)      305 2024-04-06 05:11:16.000000 primula-0.3/CHANGES.rst
+-rw-r--r--   0 hattya    (1000) users      (100)    11358 2024-02-17 12:18:15.000000 primula-0.3/LICENSE.txt
+-rw-r--r--   0 hattya    (1000) users      (100)      129 2024-03-17 06:37:02.000000 primula-0.3/MANIFEST.in
+-rw-r--r--   0 hattya    (1000) users      (100)     2948 2024-04-06 05:13:19.677920 primula-0.3/PKG-INFO
+-rw-r--r--   0 hattya    (1000) users      (100)     2003 2024-03-17 06:37:02.000000 primula-0.3/README.rst
+drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-04-06 05:13:19.661920 primula-0.3/primula/
+-rw-r--r--   0 hattya    (1000) users      (100)      378 2024-03-03 06:33:33.000000 primula-0.3/primula/__init__.py
+-rw-r--r--   0 hattya    (1000) users      (100)      155 2024-03-06 12:07:13.000000 primula-0.3/primula/__main__.py
+-rw-r--r--   0 hattya    (1000) users      (100)       58 2024-04-06 05:13:19.000000 primula-0.3/primula/__version__.py
+-rw-r--r--   0 hattya    (1000) users      (100)      343 2024-02-17 12:18:15.000000 primula-0.3/primula/_typing.py
+-rw-r--r--   0 hattya    (1000) users      (100)     6547 2024-04-03 12:37:19.000000 primula-0.3/primula/cli.py
+-rw-r--r--   0 hattya    (1000) users      (100)    10244 2024-03-18 13:07:16.000000 primula-0.3/primula/core.py
+-rw-r--r--   0 hattya    (1000) users      (100)      399 2024-02-17 12:18:15.000000 primula-0.3/primula/exception.py
+-rw-r--r--   0 hattya    (1000) users      (100)     2598 2024-03-03 06:33:33.000000 primula-0.3/primula/plugin.py
+-rw-r--r--   0 hattya    (1000) users      (100)        0 2024-02-17 12:18:15.000000 primula-0.3/primula/py.typed
+drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-04-06 05:13:19.676921 primula-0.3/primula.egg-info/
+-rw-r--r--   0 hattya    (1000) users      (100)     2948 2024-04-06 05:13:19.000000 primula-0.3/primula.egg-info/PKG-INFO
+-rw-r--r--   0 hattya    (1000) users      (100)     2117 2024-04-06 05:13:19.000000 primula-0.3/primula.egg-info/SOURCES.txt
+-rw-r--r--   0 hattya    (1000) users      (100)        1 2024-04-06 05:13:19.000000 primula-0.3/primula.egg-info/dependency_links.txt
+-rw-r--r--   0 hattya    (1000) users      (100)       44 2024-04-06 05:13:19.000000 primula-0.3/primula.egg-info/entry_points.txt
+-rw-r--r--   0 hattya    (1000) users      (100)       14 2024-04-06 05:13:19.000000 primula-0.3/primula.egg-info/requires.txt
+-rw-r--r--   0 hattya    (1000) users      (100)        8 2024-04-06 05:13:19.000000 primula-0.3/primula.egg-info/top_level.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1673 2024-03-06 12:07:13.000000 primula-0.3/pyproject.toml
+-rw-r--r--   0 hattya    (1000) users      (100)      198 2024-04-06 05:13:19.677920 primula-0.3/setup.cfg
+drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-04-06 05:13:19.664920 primula-0.3/tests/
+-rw-r--r--   0 hattya    (1000) users      (100)      553 2024-03-03 06:33:33.000000 primula-0.3/tests/base.py
+drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-04-06 05:13:19.673920 primula-0.3/tests/profiles/
+-rw-r--r--   0 hattya    (1000) users      (100)     1554 2024-03-07 13:02:00.000000 primula-0.3/tests/profiles/autoload.v7.4.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1668 2024-02-25 13:48:04.000000 primula-0.3/tests/profiles/autoload.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1658 2024-02-18 06:32:35.000000 primula-0.3/tests/profiles/autoload.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1755 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/autoload.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1202 2024-03-07 13:02:00.000000 primula-0.3/tests/profiles/dict.v7.4.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1290 2024-02-25 13:48:04.000000 primula-0.3/tests/profiles/dict.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1280 2024-02-18 06:32:35.000000 primula-0.3/tests/profiles/dict.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1359 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/dict.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1084 2024-03-07 13:02:00.000000 primula-0.3/tests/profiles/duplicate.v7.4.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1182 2024-02-25 13:48:04.000000 primula-0.3/tests/profiles/duplicate.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1172 2024-02-25 13:48:04.000000 primula-0.3/tests/profiles/duplicate.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1248 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/duplicate.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     2636 2024-03-07 13:02:00.000000 primula-0.3/tests/profiles/execute.v7.4.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     3136 2024-02-25 13:48:04.000000 primula-0.3/tests/profiles/execute.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     3105 2024-02-21 11:55:00.000000 primula-0.3/tests/profiles/execute.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     3337 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/execute.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1121 2024-03-07 13:02:00.000000 primula-0.3/tests/profiles/global.v7.4.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1213 2024-02-25 13:48:04.000000 primula-0.3/tests/profiles/global.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1203 2024-02-18 06:32:35.000000 primula-0.3/tests/profiles/global.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1279 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/global.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)      659 2024-03-09 13:49:49.000000 primula-0.3/tests/profiles/lambda.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)      654 2024-03-09 13:49:49.000000 primula-0.3/tests/profiles/lambda.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)      697 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/lambda.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)      974 2024-03-07 13:02:00.000000 primula-0.3/tests/profiles/line_continuation.v7.4.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1096 2024-02-25 13:48:04.000000 primula-0.3/tests/profiles/line_continuation.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1091 2024-02-19 13:11:50.000000 primula-0.3/tests/profiles/line_continuation.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1146 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/line_continuation.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     5320 2024-03-07 13:02:00.000000 primula-0.3/tests/profiles/nested.v7.4.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     5740 2024-02-27 13:36:18.000000 primula-0.3/tests/profiles/nested.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     5695 2024-02-27 13:36:18.000000 primula-0.3/tests/profiles/nested.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     6161 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/nested.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1175 2024-03-07 13:02:00.000000 primula-0.3/tests/profiles/script_local.v7.4.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1279 2024-02-25 13:48:04.000000 primula-0.3/tests/profiles/script_local.v8.1.0365.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1269 2024-02-18 06:32:35.000000 primula-0.3/tests/profiles/script_local.v9.0.0000.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     1345 2024-03-18 13:07:16.000000 primula-0.3/tests/profiles/script_local.v9.0.1411.txt
+-rw-r--r--   0 hattya    (1000) users      (100)     8975 2024-03-06 12:07:13.000000 primula-0.3/tests/test_cli.py
+-rw-r--r--   0 hattya    (1000) users      (100)    35969 2024-03-09 13:49:49.000000 primula-0.3/tests/test_core.py
+-rw-r--r--   0 hattya    (1000) users      (100)     2573 2024-03-03 06:33:33.000000 primula-0.3/tests/test_plugin.py
+drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-04-06 05:13:19.676921 primula-0.3/tests/vimfiles/
+drwxr-xr-x   0 hattya    (1000) users      (100)        0 2024-04-06 05:13:19.676921 primula-0.3/tests/vimfiles/autoload/
+-rw-r--r--   0 hattya    (1000) users      (100)      216 2024-02-17 12:18:15.000000 primula-0.3/tests/vimfiles/autoload/autoload.vim
+-rw-r--r--   0 hattya    (1000) users      (100)       21 2024-02-17 12:18:15.000000 primula-0.3/tests/vimfiles/autoload.vim
+-rw-r--r--   0 hattya    (1000) users      (100)      184 2024-02-17 12:18:15.000000 primula-0.3/tests/vimfiles/dict.vim
+-rw-r--r--   0 hattya    (1000) users      (100)      120 2024-02-25 13:48:04.000000 primula-0.3/tests/vimfiles/duplicate.vim
+-rw-r--r--   0 hattya    (1000) users      (100)      508 2024-02-21 11:55:00.000000 primula-0.3/tests/vimfiles/execute.vim
+-rw-r--r--   0 hattya    (1000) users      (100)      136 2024-02-17 12:18:15.000000 primula-0.3/tests/vimfiles/global.vim
+-rw-r--r--   0 hattya    (1000) users      (100)       48 2024-03-09 13:49:49.000000 primula-0.3/tests/vimfiles/lambda.vim
+-rw-r--r--   0 hattya    (1000) users      (100)      112 2024-02-19 13:11:50.000000 primula-0.3/tests/vimfiles/line_continuation.vim
+-rw-r--r--   0 hattya    (1000) users      (100)      625 2024-02-27 13:36:18.000000 primula-0.3/tests/vimfiles/nested.vim
+-rw-r--r--   0 hattya    (1000) users      (100)      142 2024-02-17 12:18:15.000000 primula-0.3/tests/vimfiles/script_local.vim
+-rw-r--r--   0 hattya    (1000) users      (100)      338 2024-02-17 12:18:15.000000 primula-0.3/tests/vimfiles/vimrc
```

### Comparing `primula-0.2/LICENSE.txt` & `primula-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/PKG-INFO` & `primula-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primula
-Version: 0.2
+Version: 0.3
 Summary: A code coverage tool for Vim script
 Author-email: Akinori Hattori <hattya@gmail.com>
 License: ALv2
 Project-URL: Homepage, https://github.com/hattya/primula
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `primula-0.2/README.rst` & `primula-0.3/README.rst`

 * *Files identical despite different names*

### Comparing `primula-0.2/primula/cli.py` & `primula-0.3/primula/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,19 +59,20 @@
             proc = subprocess.run(args)
             self.coverage.combine([os.environ[name]])
         finally:
             self.coverage.save()
         return coverage.cmdline.ERR if proc.returncode else coverage.cmdline.OK
 
     def _which(self, name: str) -> str:
+        parent, name = os.path.split(name)
         cands: List[str] = []
         if sys.platform == 'win32':
             cands += (name + ext for ext in os.environ['PATHEXT'].split(os.pathsep))
         cands.append(name)
-        for p in os.environ['PATH'].split(os.pathsep):
+        for p in (parent,) if parent else os.environ['PATH'].split(os.pathsep):
             for n in cands:
                 path = os.path.join(p, n)
                 if os.path.isfile(path):
                     return path
         raise coverage.CoverageException(f'Could not find command: {name}')
```

### Comparing `primula-0.2/primula/core.py` & `primula-0.3/primula/core.py`

 * *Files identical despite different names*

### Comparing `primula-0.2/primula/plugin.py` & `primula-0.3/primula/plugin.py`

 * *Files identical despite different names*

### Comparing `primula-0.2/primula.egg-info/PKG-INFO` & `primula-0.3/primula.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primula
-Version: 0.2
+Version: 0.3
 Summary: A code coverage tool for Vim script
 Author-email: Akinori Hattori <hattya@gmail.com>
 License: ALv2
 Project-URL: Homepage, https://github.com/hattya/primula
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `primula-0.2/primula.egg-info/SOURCES.txt` & `primula-0.3/primula.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/pyproject.toml` & `primula-0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/base.py` & `primula-0.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/autoload.v7.4.txt` & `primula-0.3/tests/profiles/autoload.v7.4.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/autoload.v8.1.0365.txt` & `primula-0.3/tests/profiles/autoload.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/autoload.v9.0.0000.txt` & `primula-0.3/tests/profiles/autoload.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/autoload.v9.0.1411.txt` & `primula-0.3/tests/profiles/autoload.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/dict.v7.4.txt` & `primula-0.3/tests/profiles/dict.v7.4.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/dict.v8.1.0365.txt` & `primula-0.3/tests/profiles/dict.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/dict.v9.0.0000.txt` & `primula-0.3/tests/profiles/dict.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/dict.v9.0.1411.txt` & `primula-0.3/tests/profiles/dict.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/duplicate.v7.4.txt` & `primula-0.3/tests/profiles/duplicate.v7.4.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/duplicate.v8.1.0365.txt` & `primula-0.3/tests/profiles/duplicate.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/duplicate.v9.0.0000.txt` & `primula-0.3/tests/profiles/duplicate.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/duplicate.v9.0.1411.txt` & `primula-0.3/tests/profiles/duplicate.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/execute.v7.4.txt` & `primula-0.3/tests/profiles/execute.v7.4.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/execute.v8.1.0365.txt` & `primula-0.3/tests/profiles/execute.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/execute.v9.0.0000.txt` & `primula-0.3/tests/profiles/execute.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/execute.v9.0.1411.txt` & `primula-0.3/tests/profiles/execute.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/global.v7.4.txt` & `primula-0.3/tests/profiles/global.v7.4.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/global.v8.1.0365.txt` & `primula-0.3/tests/profiles/global.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/global.v9.0.0000.txt` & `primula-0.3/tests/profiles/global.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/global.v9.0.1411.txt` & `primula-0.3/tests/profiles/global.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/lambda.v8.1.0365.txt` & `primula-0.3/tests/profiles/lambda.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/lambda.v9.0.0000.txt` & `primula-0.3/tests/profiles/lambda.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/lambda.v9.0.1411.txt` & `primula-0.3/tests/profiles/lambda.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/line_continuation.v7.4.txt` & `primula-0.3/tests/profiles/line_continuation.v7.4.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/line_continuation.v8.1.0365.txt` & `primula-0.3/tests/profiles/line_continuation.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/line_continuation.v9.0.0000.txt` & `primula-0.3/tests/profiles/line_continuation.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/line_continuation.v9.0.1411.txt` & `primula-0.3/tests/profiles/line_continuation.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/nested.v7.4.txt` & `primula-0.3/tests/profiles/nested.v7.4.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/nested.v8.1.0365.txt` & `primula-0.3/tests/profiles/nested.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/nested.v9.0.0000.txt` & `primula-0.3/tests/profiles/nested.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/nested.v9.0.1411.txt` & `primula-0.3/tests/profiles/nested.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/script_local.v7.4.txt` & `primula-0.3/tests/profiles/script_local.v7.4.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/script_local.v8.1.0365.txt` & `primula-0.3/tests/profiles/script_local.v8.1.0365.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/script_local.v9.0.0000.txt` & `primula-0.3/tests/profiles/script_local.v9.0.0000.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/profiles/script_local.v9.0.1411.txt` & `primula-0.3/tests/profiles/script_local.v9.0.1411.txt`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/test_cli.py` & `primula-0.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/test_core.py` & `primula-0.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/test_plugin.py` & `primula-0.3/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `primula-0.2/tests/vimfiles/nested.vim` & `primula-0.3/tests/vimfiles/nested.vim`

 * *Files identical despite different names*

