# Comparing `tmp/deepgram-sdk-3.2.3.tar.gz` & `tmp/deepgram-sdk-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepgram-sdk-3.2.3.tar", last modified: Wed Mar 27 15:53:17 2024, max compression
+gzip compressed data, was "deepgram-sdk-3.2.4.tar", last modified: Fri Apr  5 22:31:44 2024, max compression
```

## Comparing `deepgram-sdk-3.2.3.tar` & `deepgram-sdk-3.2.4.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.690265 deepgram-sdk-3.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-03-27 15:53:17.686265 deepgram-sdk-3.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.678265 deepgram-sdk-3.2.3/deepgram/
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.678265 deepgram-sdk-3.2.3/deepgram/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/audio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.678265 deepgram-sdk-3.2.3/deepgram/audio/microphone/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/audio/microphone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/audio/microphone/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/audio/microphone/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/audio/microphone/microphone.py
--rw-r--r--   0 runner    (1001) docker     (127)     9593 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.678265 deepgram-sdk-3.2.3/deepgram/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/abstract_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/abstract_sync_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.678265 deepgram-sdk-3.2.3/deepgram/clients/analyze/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.682265 deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/listen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.682265 deepgram-sdk-3.2.3/deepgram/clients/live/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.682265 deepgram-sdk-3.2.3/deepgram/clients/live/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20773 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/live/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.682265 deepgram-sdk-3.2.3/deepgram/clients/manage/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/manage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/manage/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.682265 deepgram-sdk-3.2.3/deepgram/clients/manage/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/manage/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/manage/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33112 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/manage/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/manage/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/manage/v1/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.682265 deepgram-sdk-3.2.3/deepgram/clients/onprem/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/onprem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/onprem/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.682265 deepgram-sdk-3.2.3/deepgram/clients/onprem/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/onprem/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/onprem/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/onprem/v1/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.686265 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.686265 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.686265 deepgram-sdk-3.2.3/deepgram/clients/speak/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.686265 deepgram-sdk-3.2.3/deepgram/clients/speak/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/v1/async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/v1/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/v1/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/clients/speak/v1/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/deepgram/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:53:17.686265 deepgram-sdk-3.2.3/deepgram_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-03-27 15:53:17.000000 deepgram-sdk-3.2.3/deepgram_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-27 15:53:17.000000 deepgram-sdk-3.2.3/deepgram_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:53:17.000000 deepgram-sdk-3.2.3/deepgram_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-27 15:53:17.000000 deepgram-sdk-3.2.3/deepgram_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 15:53:17.000000 deepgram-sdk-3.2.3/deepgram_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:53:17.690265 deepgram-sdk-3.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-27 15:53:08.000000 deepgram-sdk-3.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.882693 deepgram-sdk-3.2.4/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.882693 deepgram-sdk-3.2.4/deepgram/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.886693 deepgram-sdk-3.2.4/deepgram/audio/microphone/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/microphone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/microphone/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/microphone/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/audio/microphone/microphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.886693 deepgram-sdk-3.2.4/deepgram/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/abstract_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/abstract_sync_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.886693 deepgram-sdk-3.2.4/deepgram/clients/analyze/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.886693 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12291 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12411 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8228 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/listen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/live/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/live/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21558 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20861 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4419 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/live/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/manage/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33519 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33112 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/manage/v1/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/onprem/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.890693 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12830 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12762 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21250 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/deepgram/clients/speak/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/clients/speak/v1/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/deepgram/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11366 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 22:31:44.000000 deepgram-sdk-3.2.4/deepgram_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:31:44.894693 deepgram-sdk-3.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 22:31:35.000000 deepgram-sdk-3.2.4/setup.py
```

### Comparing `deepgram-sdk-3.2.3/LICENSE` & `deepgram-sdk-3.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/PKG-INFO` & `deepgram-sdk-3.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 3.2.3
+Version: 3.2.4
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Deepgram
 Author-email: devrel@deepgram.com
 License: MIT
 Keywords: deepgram,deepgram speech-to-text
 Classifier: Intended Audience :: Developers
```

### Comparing `deepgram-sdk-3.2.3/README.md` & `deepgram-sdk-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/__init__.py` & `deepgram-sdk-3.2.4/deepgram/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023-2024 Deepgram SDK contributors. All Rights Reserved.
 # Use of this source code is governed by a MIT license that can be found in the LICENSE file.
 # SPDX-License-Identifier: MIT
 
 # version
-__version__ = "v3.2.3"
+__version__ = "v3.2.4"
 
 # entry point for the deepgram python sdk
 from .client import Deepgram, DeepgramClient
 from .options import DeepgramClientOptions, ClientOptionsFromEnv
 import logging, verboselogs
 
 # listen client
@@ -19,16 +19,17 @@
 from .client import LiveOptions
 from .client import (
     OpenResponse,
     LiveResultResponse,
     MetadataResponse,
     SpeechStartedResponse,
     UtteranceEndResponse,
-    ErrorResponse,
     CloseResponse,
+    UnhandledResponse,
+    ErrorResponse,
 )
 
 # prerecorded
 from .client import PreRecordedClient, AsyncPreRecordedClient
 from .client import (
     FileSource,
     PrerecordedSource,
```

### Comparing `deepgram-sdk-3.2.3/deepgram/audio/microphone/errors.py` & `deepgram-sdk-3.2.4/deepgram/audio/microphone/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/audio/microphone/microphone.py` & `deepgram-sdk-3.2.4/deepgram/audio/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/client.py` & `deepgram-sdk-3.2.4/deepgram/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 # live client responses
 from .clients import (
     OpenResponse,
     LiveResultResponse,
     MetadataResponse,
     SpeechStartedResponse,
     UtteranceEndResponse,
-    ErrorResponse,
     CloseResponse,
+    ErrorResponse,
+    UnhandledResponse,
 )
 
 # prerecorded
 from .clients import PreRecordedClient, AsyncPreRecordedClient
 from .clients import (
     FileSource,
     PrerecordedSource,
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 from .live import LiveTranscriptionEvents
 from .live import (
     OpenResponse,
     LiveResultResponse,
     MetadataResponse,
     SpeechStartedResponse,
     UtteranceEndResponse,
-    ErrorResponse,
     CloseResponse,
+    ErrorResponse,
+    UnhandledResponse,
 )
 
 # prerecorded
 from .prerecorded import PreRecordedClient, AsyncPreRecordedClient
 from .prerecorded import PrerecordedOptions
 from .prerecorded import Sentiment
 from .prerecorded import (
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/abstract_async_client.py` & `deepgram-sdk-3.2.4/deepgram/clients/abstract_async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/abstract_sync_client.py` & `deepgram-sdk-3.2.4/deepgram/clients/abstract_sync_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/errors.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/async_client.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/helpers.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/options.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/analyze/v1/response.py` & `deepgram-sdk-3.2.4/deepgram/clients/analyze/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/errors.py` & `deepgram-sdk-3.2.4/deepgram/clients/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/helpers.py` & `deepgram-sdk-3.2.4/deepgram/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/listen.py` & `deepgram-sdk-3.2.4/deepgram/clients/listen.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,22 @@
     AsyncLiveClient,
     LiveOptions,
     LiveTranscriptionEvents,
 )
 
 # responses
 from .live import (
+    OpenResponse,
     LiveResultResponse,
     MetadataResponse,
     SpeechStartedResponse,
     UtteranceEndResponse,
+    CloseResponse,
     ErrorResponse,
+    UnhandledResponse,
 )
 
 
 class Listen:
     """
     Represents a client for interacting with the Deepgram API.
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 from .client import LiveTranscriptionEvents
 from .client import (
     OpenResponse,
     LiveResultResponse,
     MetadataResponse,
     SpeechStartedResponse,
     UtteranceEndResponse,
-    ErrorResponse,
     CloseResponse,
+    ErrorResponse,
+    UnhandledResponse,
 )
 
 from ...options import DeepgramClientOptions
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from .enums import LiveTranscriptionEvents
 from .v1.response import (
     OpenResponse as OpenResponseLatest,
     LiveResultResponse as LiveResultResponseLatest,
     MetadataResponse as MetadataResponseLatest,
     SpeechStartedResponse as SpeechStartedResponseLatest,
     UtteranceEndResponse as UtteranceEndResponseLatest,
-    ErrorResponse as ErrorResponseLatest,
     CloseResponse as CloseResponseLatest,
+    ErrorResponse as ErrorResponseLatest,
+    UnhandledResponse as UnhandledResponseLatest,
 )
 
 """
 The vX/client.py points to the current supported version in the SDK.
 Older versions are supported in the SDK for backwards compatibility.
 """
 
@@ -68,25 +69,33 @@
     """
     pass through for UtteranceEndResponse based on API version
     """
 
     pass
 
 
+class CloseResponse(CloseResponseLatest):
+    """
+    pass through for CloseResponse based on API version
+    """
+
+    pass
+
+
 class ErrorResponse(ErrorResponseLatest):
     """
     pass through for ErrorResponse based on API version
     """
 
     pass
 
 
-class CloseResponse(CloseResponseLatest):
+class UnhandledResponse(UnhandledResponseLatest):
     """
-    pass through for CloseResponse based on API version
+    pass through for UnhandledResponse based on API version
     """
 
     pass
 
 
 # clients
 class LiveClient(LiveClientLatest):
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/enums.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/enums.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,8 +13,9 @@
     Open: str = "Open"
     Close: str = "Close"
     Transcript: str = "Results"
     Metadata: str = "Metadata"
     UtteranceEnd: str = "UtteranceEnd"
     SpeechStarted: str = "SpeechStarted"
     Error: str = "Error"
+    Unhandled: str = "Unhandled"
     Warning: str = "Warning"
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/errors.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/helpers.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/v1/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/v1/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 from ....options import DeepgramClientOptions
 from .response import (
     OpenResponse,
     LiveResultResponse,
     MetadataResponse,
     SpeechStartedResponse,
     UtteranceEndResponse,
-    ErrorResponse,
     CloseResponse,
+    ErrorResponse,
+    UnhandledResponse,
 )
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/v1/async_client.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/v1/async_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 
 from .response import (
     OpenResponse,
     LiveResultResponse,
     MetadataResponse,
     SpeechStartedResponse,
     UtteranceEndResponse,
-    ErrorResponse,
     CloseResponse,
+    ErrorResponse,
+    UnhandledResponse,
 )
 from .options import LiveOptions
 
 ONE_SECOND = 1
 DEEPGRAM_INTERVAL = 5
 PING_INTERVAL = 20
 
@@ -240,42 +241,45 @@
                         result = UtteranceEndResponse.from_json(message)
                         self.logger.verbose("UtteranceEndResponse: %s", result)
                         await self._emit(
                             LiveTranscriptionEvents.UtteranceEnd,
                             utterance_end=result,
                             **dict(self.kwargs),
                         )
-                    case LiveTranscriptionEvents.Error.value:
-                        result = ErrorResponse.from_json(message)
-                        self.logger.verbose("LiveTranscriptionEvents: %s", result)
-                        await self._emit(
-                            LiveTranscriptionEvents.Error,
-                            error=result,
-                            **dict(self.kwargs),
-                        )
                     case LiveTranscriptionEvents.Close.value:
                         result = CloseResponse.from_json(message)
                         self.logger.verbose("CloseResponse: %s", result)
                         await self._emit(
                             LiveTranscriptionEvents.Close,
                             close=result,
                             **dict(self.kwargs),
                         )
+                    case LiveTranscriptionEvents.Error.value:
+                        result = ErrorResponse.from_json(message)
+                        self.logger.verbose("LiveTranscriptionEvents: %s", result)
+                        await self._emit(
+                            LiveTranscriptionEvents.Error,
+                            error=result,
+                            **dict(self.kwargs),
+                        )
                     case _:
                         self.logger.warning(
                             "Unknown Message: response_type: %s, data: %s",
                             response_type,
                             data,
                         )
-                        error = ErrorResponse(
-                            type="UnhandledMessage",
-                            description="Unknown message type",
-                            message=f"Unhandle message type: {response_type}",
+                        unhandled = UnhandledResponse(
+                            type=LiveTranscriptionEvents.Unhandled.value,
+                            raw=message,
+                        )
+                        self._emit(
+                            LiveTranscriptionEvents.Unhandled,
+                            unhandled=unhandled,
+                            **dict(self.kwargs),
                         )
-                        await self._emit(LiveTranscriptionEvents.Error, error=error)
 
             except websockets.exceptions.ConnectionClosedOK as e:
                 self.logger.notice(f"_listening({e.code}) exiting gracefully")
                 self.logger.debug("AsyncLiveClient._listening LEAVE")
                 return
 
             except websockets.exceptions.WebSocketException as e:
@@ -481,23 +485,35 @@
 
     # signals the WebSocket connection to exit
     async def _signal_exit(self) -> None:
         # send close event
         self.logger.verbose("closing socket...")
         if self._socket is not None:
             self.logger.verbose("send CloseStream...")
-            await self._socket.send(json.dumps({"type": "CloseStream"}))
-
-            await asyncio.sleep(0.5)
+            try:
+                # if the socket connection is closed, the following line might throw an error
+                await self._socket.send(json.dumps({"type": "CloseStream"}))
+            except websockets.exceptions.ConnectionClosedOK as e:
+                self.logger.notice(f"_signal_exit  - connection closed: {e.code}")
+            except websockets.exceptions.WebSocketException as e:
+                self.logger.error(f"_signal_exit - WebSocketException: {str(e)}")
+            except Exception as e:
+                self.logger.error(f"_signal_exit - Exception: {str(e)}")
 
             # push close event
-            await self._emit(
-                LiveTranscriptionEvents.Close,
-                CloseResponse(type=LiveTranscriptionEvents.Close.value),
-            )
+            try:
+                await self._emit(
+                    LiveTranscriptionEvents.Close,
+                    CloseResponse(type=LiveTranscriptionEvents.Close.value),
+                )
+            except Exception as e:
+                self.logger.error(f"_signal_exit - Exception: {str(e)}")
+
+            # wait for task to send
+            await asyncio.sleep(0.5)
 
         # signal exit
         self._exit_event.set()
 
         # closes the WebSocket connection gracefully
         self.logger.verbose("clean up socket...")
         if self._socket is not None:
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/v1/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/v1/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 
 from .response import (
     OpenResponse,
     LiveResultResponse,
     MetadataResponse,
     SpeechStartedResponse,
     UtteranceEndResponse,
-    ErrorResponse,
     CloseResponse,
+    ErrorResponse,
+    UnhandledResponse,
 )
 from .options import LiveOptions
 
 ONE_SECOND = 1
 DEEPGRAM_INTERVAL = 5
 PING_INTERVAL = 20
 
@@ -240,42 +241,45 @@
                         result = UtteranceEndResponse.from_json(message)
                         self.logger.verbose("UtteranceEndResponse: %s", result)
                         self._emit(
                             LiveTranscriptionEvents.UtteranceEnd,
                             utterance_end=result,
                             **dict(self.kwargs),
                         )
-                    case LiveTranscriptionEvents.Error.value:
-                        result = ErrorResponse.from_json(message)
-                        self.logger.verbose("ErrorResponse: %s", result)
-                        self._emit(
-                            LiveTranscriptionEvents.Error,
-                            error=result,
-                            **dict(self.kwargs),
-                        )
                     case LiveTranscriptionEvents.Close.value:
                         result = CloseResponse.from_json(message)
                         self.logger.verbose("CloseResponse: %s", result)
                         self._emit(
                             LiveTranscriptionEvents.Close,
                             close=result,
                             **dict(self.kwargs),
                         )
+                    case LiveTranscriptionEvents.Error.value:
+                        result = ErrorResponse.from_json(message)
+                        self.logger.verbose("ErrorResponse: %s", result)
+                        self._emit(
+                            LiveTranscriptionEvents.Error,
+                            error=result,
+                            **dict(self.kwargs),
+                        )
                     case _:
                         self.logger.warning(
                             "Unknown Message: response_type: %s, data: %s",
                             response_type,
                             data,
                         )
-                        error = ErrorResponse(
-                            type="UnhandledMessage",
-                            description="Unknown message type",
-                            message=f"Unhandle message type: {response_type}",
+                        unhandled = UnhandledResponse(
+                            type=LiveTranscriptionEvents.Unhandled.value,
+                            raw=message,
+                        )
+                        self._emit(
+                            LiveTranscriptionEvents.Unhandled,
+                            unhandled=unhandled,
+                            **dict(self.kwargs),
                         )
-                        self._emit(LiveTranscriptionEvents.Error, error=error)
 
             except websockets.exceptions.ConnectionClosedOK as e:
                 self.logger.notice(f"_listening({e.code}) exiting gracefully")
                 self.logger.debug("LiveClient._listening LEAVE")
                 return
 
             except websockets.exceptions.WebSocketException as e:
@@ -469,23 +473,35 @@
 
     # signals the WebSocket connection to exit
     def _signal_exit(self) -> None:
         # closes the WebSocket connection gracefully
         self.logger.notice("closing socket...")
         if self._socket is not None:
             self.logger.notice("sending CloseStream...")
-            self.send(json.dumps({"type": "CloseStream"}))
-
-            time.sleep(0.5)
+            try:
+                # if the socket connection is closed, the following line might throw an error
+                self._socket.send(json.dumps({"type": "CloseStream"}))
+            except websockets.exceptions.ConnectionClosedOK as e:
+                self.logger.notice(f"_signal_exit  - connection closed: {e.code}")
+            except websockets.exceptions.WebSocketException as e:
+                self.logger.error(f"_signal_exit - WebSocketException: {str(e)}")
+            except Exception as e:
+                self.logger.error(f"_signal_exit - Exception: {str(e)}")
 
             # push close event
-            self._emit(
-                LiveTranscriptionEvents.Close,
-                CloseResponse(type=LiveTranscriptionEvents.Close.value),
-            )
+            try:
+                self._emit(
+                    LiveTranscriptionEvents.Close,
+                    CloseResponse(type=LiveTranscriptionEvents.Close.value),
+                )
+            except Exception as e:
+                self.logger.error(f"_signal_exit - Exception: {str(e)}")
+
+            # wait for task to send
+            time.sleep(0.5)
 
         # signal exit
         self._exit_event.set()
 
         # closes the WebSocket connection gracefully
         self.logger.verbose("clean up socket...")
         if self._socket is not None:
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/v1/options.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/v1/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     )
     punctuate: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     profanity_filter: Optional[bool] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
-    redact: Optional[bool] = field(
+    redact: Optional[Union[List[str], bool, str]] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     replace: Optional[str] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
     )
     sample_rate: Optional[int] = field(
         default=None, metadata=config(exclude=lambda f: f is None)
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/live/v1/response.py` & `deepgram-sdk-3.2.4/deepgram/clients/live/v1/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,37 @@
     def __setitem__(self, key, val):
         self.__dict__[key] = val
 
     def __str__(self) -> str:
         return self.to_json(indent=4)
 
 
+# Close Message
+
+
+@dataclass_json
+@dataclass
+class CloseResponse:
+    """
+    Close Message from the Deepgram Platform
+    """
+
+    type: str = ""
+
+    def __getitem__(self, key):
+        _dict = self.to_dict()
+        return _dict[key]
+
+    def __setitem__(self, key, val):
+        self.__dict__[key] = val
+
+    def __str__(self) -> str:
+        return self.to_json(indent=4)
+
+
 # Error Message
 
 
 @dataclass_json
 @dataclass
 class ErrorResponse:
     """
@@ -313,22 +336,26 @@
     def __setitem__(self, key, val):
         self.__dict__[key] = val
 
     def __str__(self) -> str:
         return self.to_json(indent=4)
 
 
+# Unhandled Message
+
+
 @dataclass_json
 @dataclass
-class CloseResponse:
+class UnhandledResponse:
     """
-    Close Message from the Deepgram Platform
+    Unhandled Message from the Deepgram Platform
     """
 
     type: str = ""
+    raw: str = ""
 
     def __getitem__(self, key):
         _dict = self.to_dict()
         return _dict[key]
 
     def __setitem__(self, key, val):
         self.__dict__[key] = val
```

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/manage/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/manage/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/manage/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/manage/v1/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/manage/v1/async_client.py` & `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/manage/v1/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/manage/v1/options.py` & `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/manage/v1/response.py` & `deepgram-sdk-3.2.4/deepgram/clients/manage/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/onprem/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/onprem/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/onprem/v1/async_client.py` & `deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/onprem/v1/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/onprem/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/errors.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/__init__.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/async_client.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/helpers.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/helpers.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/options.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/prerecorded/v1/response.py` & `deepgram-sdk-3.2.4/deepgram/clients/prerecorded/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/read.py` & `deepgram-sdk-3.2.4/deepgram/clients/read.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/speak/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/speak/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/speak/errors.py` & `deepgram-sdk-3.2.4/deepgram/clients/speak/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/speak/v1/async_client.py` & `deepgram-sdk-3.2.4/deepgram/clients/speak/v1/async_client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/speak/v1/client.py` & `deepgram-sdk-3.2.4/deepgram/clients/speak/v1/client.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/speak/v1/options.py` & `deepgram-sdk-3.2.4/deepgram/clients/speak/v1/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/clients/speak/v1/response.py` & `deepgram-sdk-3.2.4/deepgram/clients/speak/v1/response.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/errors.py` & `deepgram-sdk-3.2.4/deepgram/errors.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram/options.py` & `deepgram-sdk-3.2.4/deepgram/options.py`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/deepgram_sdk.egg-info/PKG-INFO` & `deepgram-sdk-3.2.4/deepgram_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepgram-sdk
-Version: 3.2.3
+Version: 3.2.4
 Summary: The official Python SDK for the Deepgram automated speech recognition platform.
 Home-page: https://github.com/deepgram/deepgram-python-sdk
 Author: Deepgram
 Author-email: devrel@deepgram.com
 License: MIT
 Keywords: deepgram,deepgram speech-to-text
 Classifier: Intended Audience :: Developers
```

### Comparing `deepgram-sdk-3.2.3/deepgram_sdk.egg-info/SOURCES.txt` & `deepgram-sdk-3.2.4/deepgram_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/pyproject.toml` & `deepgram-sdk-3.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deepgram-sdk-3.2.3/setup.py` & `deepgram-sdk-3.2.4/setup.py`

 * *Files identical despite different names*

