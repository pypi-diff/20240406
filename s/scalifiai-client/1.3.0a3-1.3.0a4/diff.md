# Comparing `tmp/scalifiai-client-1.3.0a3.tar.gz` & `tmp/scalifiai-client-1.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalifiai-client-1.3.0a3.tar", last modified: Fri Apr  5 09:36:21 2024, max compression
+gzip compressed data, was "scalifiai-client-1.3.0a4.tar", last modified: Sat Apr  6 16:04:54 2024, max compression
```

## Comparing `scalifiai-client-1.3.0a3.tar` & `scalifiai-client-1.3.0a4.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.707047 scalifiai-client-1.3.0a3/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/LICENSE
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      908 2024-04-05 09:36:21.707047 scalifiai-client-1.3.0a3/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/README.md
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      982 2024-04-05 09:35:58.000000 scalifiai-client-1.3.0a3/pyproject.toml
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.699047 scalifiai-client-1.3.0a3/scalifiai/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6439 2024-04-02 08:09:54.000000 scalifiai-client-1.3.0a3/scalifiai/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/credentials.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.699047 scalifiai-client-1.3.0a3/scalifiai/mcs/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.699047 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.703047 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       63 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9490 2024-04-05 09:32:04.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/schema.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2144 2024-04-05 09:33:28.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/utils.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.703047 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13424 2024-04-02 08:09:54.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.703047 scalifiai-client-1.3.0a3/scalifiai/mcs/model/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34065 2024-04-02 08:09:55.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.703047 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28720 2024-04-02 08:09:54.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/schemas.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-04-02 07:17:38.000000 scalifiai-client-1.3.0a3/scalifiai/request_manager.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 09:36:21.707047 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      908 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1353 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      147 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/requires.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-05 09:36:21.000000 scalifiai-client-1.3.0a3/scalifiai_client.egg-info/top_level.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-05 09:36:21.707047 scalifiai-client-1.3.0a3/setup.cfg
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.950530 scalifiai-client-1.3.0a4/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/LICENSE
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1173 2024-04-06 16:04:54.950530 scalifiai-client-1.3.0a4/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/README.md
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1119 2024-04-06 16:04:33.000000 scalifiai-client-1.3.0a4/pyproject.toml
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.938530 scalifiai-client-1.3.0a4/scalifiai/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6439 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/credentials.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.938530 scalifiai-client-1.3.0a4/scalifiai/mcs/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.942530 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-06 12:51:10.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.942530 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/keras/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/keras/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       24 2024-04-06 12:51:24.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/keras/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/keras/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8462 2024-04-06 14:18:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/keras/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.942530 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/pytorch/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 12:49:28.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/pytorch/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       26 2024-04-06 12:51:17.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/pytorch/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5657 2024-04-06 12:58:51.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/pytorch/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     7717 2024-04-06 15:11:51.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/pytorch/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/schema.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2576 2024-04-06 14:22:40.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/utils.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.946530 scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13424 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.946530 scalifiai-client-1.3.0a4/scalifiai/mcs/model/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34065 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.946530 scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28720 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/schemas.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a4/scalifiai/request_manager.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:04:54.946530 scalifiai-client-1.3.0a4/scalifiai_client.egg-info/
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1173 2024-04-06 16:04:54.000000 scalifiai-client-1.3.0a4/scalifiai_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1570 2024-04-06 16:04:54.000000 scalifiai-client-1.3.0a4/scalifiai_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-06 16:04:54.000000 scalifiai-client-1.3.0a4/scalifiai_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      234 2024-04-06 16:04:54.000000 scalifiai-client-1.3.0a4/scalifiai_client.egg-info/requires.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-06 16:04:54.000000 scalifiai-client-1.3.0a4/scalifiai_client.egg-info/top_level.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-06 16:04:54.950530 scalifiai-client-1.3.0a4/setup.cfg
```

### Comparing `scalifiai-client-1.3.0a3/PKG-INFO` & `scalifiai-client-1.3.0a4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.3.0a3
+Version: 1.3.0a4
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,7 +17,13 @@
 Requires-Dist: tzlocal>=2.1
 Provides-Extra: tf
 Requires-Dist: tensorflow<=2.15.1,>=2.2.0; extra == "tf"
 Requires-Dist: pydantic>=2.0; extra == "tf"
 Requires-Dist: pandas>=1.3.0; extra == "tf"
 Requires-Dist: humanize>=2.0.0; extra == "tf"
 Requires-Dist: tzlocal>=2.1; extra == "tf"
+Provides-Extra: torch
+Requires-Dist: torch<=2.2.2,>=1.3.0; extra == "torch"
+Requires-Dist: pydantic>=2.0; extra == "torch"
+Requires-Dist: pandas>=1.3.0; extra == "torch"
+Requires-Dist: humanize>=2.0.0; extra == "torch"
+Requires-Dist: tzlocal>=2.1; extra == "torch"
```

### Comparing `scalifiai-client-1.3.0a3/pyproject.toml` & `scalifiai-client-1.3.0a4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scalifiai-client"
-version = "1.3.0-alpha.3"
+version = "1.3.0-alpha.4"
 description = "SCALIFI AI NO CODE PLATFORM"
 readme = "README.md"
 authors = [{ name = "Scalifi Ai", email = "helpdesk@scalifiai.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,10 +27,17 @@
 tf = [
     "tensorflow >= 2.2.0, <= 2.15.1",
     "pydantic >= 2.0",
     "pandas >= 1.3.0",
     "humanize >= 2.0.0",
     "tzlocal >= 2.1",
 ]
+torch = [
+    "torch >= 1.3.0, <= 2.2.2",
+    "pydantic >= 2.0",
+    "pandas >= 1.3.0",
+    "humanize >= 2.0.0",
+    "tzlocal >= 2.1",
+]
 
 [project.urls]
 Homepage = "https://github.com/Ai-Bloc-24"
```

### Comparing `scalifiai-client-1.3.0a3/scalifiai/base.py` & `scalifiai-client-1.3.0a4/scalifiai/base.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/credentials.py` & `scalifiai-client-1.3.0a4/scalifiai/credentials.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/exceptions.py` & `scalifiai-client-1.3.0a4/scalifiai/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/exceptions.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/exceptions.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/exceptions.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/keras/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/keras/main.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/keras/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import tempfile
 from pathlib import Path
 import os
-import requests
 
 from scalifiai.mcs.frameworks.base import ModelWrapper
 from scalifiai.mcs.frameworks.schema import TensorSpec, DataType
+from scalifiai.mcs.frameworks.constants import MODEL_SAVE_FOLDER_NAME
 from scalifiai.mcs.model.exceptions import (
     raise_custom_exception as raise_custom_exception__model,
 )
-from scalifiai.mcs.metadata.exceptions import (
-    raise_custom_exception as raise_custom_exception__metadata,
-)
 from .exceptions import KerasInvalidDataTypeModelException, KerasInvalidModelException
-from .constants import MODEL_SAVE_FOLDER_NAME, FRAMEWORK_KEY
+from .constants import FRAMEWORK_KEY
 
 
 # TODO[VIMPORTANT] SEGREGATE `ModelWrapper` class into deep learning and machine learning wrapper class and model following function to appropriate model class: [infer_data_type, infer_signature, serialize_signature]
 class KerasModelWrapper(ModelWrapper):
 
     framework_key = FRAMEWORK_KEY
 
@@ -48,15 +45,15 @@
             tf.double: DataType.FLOAT64,
             tf.complex64: DataType.COMPLEX64,
             tf.complex128: DataType.COMPLEX128,
             tf.string: DataType.STRING,
             tf.bool: DataType.BOOL,
             tf.variant: DataType.VARIANT,
         }
-    
+
     @classmethod
     def check_model_instance(cls, *, model_instance):
 
         try:
             import tensorflow as tf
         except Exception:
             print("Skipping Tensorflow check as Tensorflow installation is not detected")
@@ -111,36 +108,14 @@
             if self.signature[key] != None:
                 signature[key] = []
                 for spec in self.signature[key]:
                     signature[key].append(spec.to_dict())
 
         return signature
 
-    @classmethod
-    def get_all_files_and_size(cls, *, search_dir_path=None, base_path=None):
-        files_relative_paths = []
-        files_data = []
-        total_size = 0
-        for dirpath, _, filenames in os.walk(search_dir_path):
-            for filename in filenames:
-                file_path = os.path.join(dirpath, filename)
-                if os.path.isfile(file_path):
-                    file_relative_path = str(Path(file_path).relative_to(base_path))
-                    file_size = os.path.getsize(file_path)
-                    files_relative_paths.append(file_relative_path)
-                    files_data.append(
-                        {
-                            "file_relative_path": file_relative_path,
-                            "file_full_path": Path(file_path).resolve(),
-                            "file_size": file_size,
-                        }
-                    )
-                    total_size += file_size
-        return total_size, files_relative_paths, files_data
-
     def get_total_params(self):
         # TODO[VIMPORTANT] MAKE A FUNCTION FOR IMPORTING DEPENDENT LIBRARIES FOR EACH FRAMEWORK IN THEIR CLASS AND USE THAT FUNCTION OR ELSE RAISE ERROR WITH PROPER INSTALLATION MENTIONED VIA OUR LIBRARY ONLY VIA OTHER DEPENDENCIEZS IN project.toml FILE
         import tensorflow as tf
 
         return {
             "trainable": {
                 "verbose": "Trainable",
@@ -164,14 +139,15 @@
         request_manager=None,
         upload_url=None,
         parent_action=None,
         model_instance=None,
     ):
 
         from scalifiai.mcs.model_version.main import ModelVersion
+        from scalifiai.mcs.frameworks.utils import get_all_files_and_size
 
         with tempfile.TemporaryDirectory(dir=base_dir_path) as temp_dir:
 
             temp_dir_path = Path(temp_dir)
             model_save_file_path = temp_dir_path / Path(MODEL_SAVE_FOLDER_NAME)
 
             try:
@@ -183,15 +159,15 @@
                     raise KerasInvalidModelException(extra_info=str(ex))
                 except Exception as ex:
                     raise KerasInvalidModelException()
 
             self.signature = self.infer_signature()
 
             total_files_size, files_relative_paths, files_data = (
-                self.get_all_files_and_size(
+                get_all_files_and_size(
                     search_dir_path=model_save_file_path, base_path=model_save_file_path
                 )
             )
 
             create_version_request_body = {
                 "framework": self.framework_key,
                 "variation_name": variation,
```

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/frameworks/schema.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/main.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/exceptions.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/main.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/metadata/schemas.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/metadata/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/model/constants.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/model/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/model/exceptions.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/model/main.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/model/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/model/schemas.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/model/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/constants.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/exceptions.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/main.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/mcs/model_version/schemas.py` & `scalifiai-client-1.3.0a4/scalifiai/mcs/model_version/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai/request_manager.py` & `scalifiai-client-1.3.0a4/scalifiai/request_manager.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a3/scalifiai_client.egg-info/PKG-INFO` & `scalifiai-client-1.3.0a4/scalifiai_client.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.3.0a3
+Version: 1.3.0a4
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,7 +17,13 @@
 Requires-Dist: tzlocal>=2.1
 Provides-Extra: tf
 Requires-Dist: tensorflow<=2.15.1,>=2.2.0; extra == "tf"
 Requires-Dist: pydantic>=2.0; extra == "tf"
 Requires-Dist: pandas>=1.3.0; extra == "tf"
 Requires-Dist: humanize>=2.0.0; extra == "tf"
 Requires-Dist: tzlocal>=2.1; extra == "tf"
+Provides-Extra: torch
+Requires-Dist: torch<=2.2.2,>=1.3.0; extra == "torch"
+Requires-Dist: pydantic>=2.0; extra == "torch"
+Requires-Dist: pandas>=1.3.0; extra == "torch"
+Requires-Dist: humanize>=2.0.0; extra == "torch"
+Requires-Dist: tzlocal>=2.1; extra == "torch"
```

### Comparing `scalifiai-client-1.3.0a3/scalifiai_client.egg-info/SOURCES.txt` & `scalifiai-client-1.3.0a4/scalifiai_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,26 @@
 scalifiai/request_manager.py
 scalifiai/mcs/__init__.py
 scalifiai/mcs/constants.py
 scalifiai/mcs/exceptions.py
 scalifiai/mcs/main.py
 scalifiai/mcs/frameworks/__init__.py
 scalifiai/mcs/frameworks/base.py
+scalifiai/mcs/frameworks/constants.py
 scalifiai/mcs/frameworks/exceptions.py
 scalifiai/mcs/frameworks/schema.py
 scalifiai/mcs/frameworks/utils.py
 scalifiai/mcs/frameworks/keras/__init__.py
 scalifiai/mcs/frameworks/keras/constants.py
 scalifiai/mcs/frameworks/keras/exceptions.py
 scalifiai/mcs/frameworks/keras/main.py
+scalifiai/mcs/frameworks/pytorch/__init__.py
+scalifiai/mcs/frameworks/pytorch/constants.py
+scalifiai/mcs/frameworks/pytorch/exceptions.py
+scalifiai/mcs/frameworks/pytorch/main.py
 scalifiai/mcs/metadata/__init__.py
 scalifiai/mcs/metadata/constants.py
 scalifiai/mcs/metadata/exceptions.py
 scalifiai/mcs/metadata/main.py
 scalifiai/mcs/metadata/schemas.py
 scalifiai/mcs/model/__init__.py
 scalifiai/mcs/model/constants.py
```

