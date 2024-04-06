# Comparing `tmp/scalifiai-client-1.3.0a5.tar.gz` & `tmp/scalifiai-client-1.3.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalifiai-client-1.3.0a5.tar", last modified: Sat Apr  6 16:08:57 2024, max compression
+gzip compressed data, was "scalifiai-client-1.3.0a6.tar", last modified: Sat Apr  6 16:22:23 2024, max compression
```

## Comparing `scalifiai-client-1.3.0a5.tar` & `scalifiai-client-1.3.0a6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.754268 scalifiai-client-1.3.0a5/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/LICENSE
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1299 2024-04-06 16:08:57.754268 scalifiai-client-1.3.0a5/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/README.md
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1194 2024-04-06 16:08:35.000000 scalifiai-client-1.3.0a5/pyproject.toml
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.742267 scalifiai-client-1.3.0a5/scalifiai/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6439 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/credentials.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.742267 scalifiai-client-1.3.0a5/scalifiai/mcs/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.742267 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/base.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-06 12:51:10.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/exceptions.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.746267 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/keras/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/keras/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       24 2024-04-06 12:51:24.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/keras/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/keras/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8462 2024-04-06 14:18:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/keras/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.746267 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/pytorch/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 12:49:28.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/pytorch/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       26 2024-04-06 12:51:17.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/pytorch/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5657 2024-04-06 12:58:51.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/pytorch/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     7717 2024-04-06 15:11:51.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/pytorch/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/schema.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2576 2024-04-06 14:22:40.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/utils.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/main.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.746267 scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13424 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.746267 scalifiai-client-1.3.0a5/scalifiai/mcs/model/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34065 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model/schemas.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.750268 scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/__init__.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/constants.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/exceptions.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28720 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/main.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/schemas.py
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a5/scalifiai/request_manager.py
-drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:08:57.750268 scalifiai-client-1.3.0a5/scalifiai_client.egg-info/
--rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1299 2024-04-06 16:08:57.000000 scalifiai-client-1.3.0a5/scalifiai_client.egg-info/PKG-INFO
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1570 2024-04-06 16:08:57.000000 scalifiai-client-1.3.0a5/scalifiai_client.egg-info/SOURCES.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-06 16:08:57.000000 scalifiai-client-1.3.0a5/scalifiai_client.egg-info/dependency_links.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      282 2024-04-06 16:08:57.000000 scalifiai-client-1.3.0a5/scalifiai_client.egg-info/requires.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-06 16:08:57.000000 scalifiai-client-1.3.0a5/scalifiai_client.egg-info/top_level.txt
--rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-06 16:08:57.754268 scalifiai-client-1.3.0a5/setup.cfg
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.417606 scalifiai-client-1.3.0a6/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/LICENSE
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1299 2024-04-06 16:22:23.417606 scalifiai-client-1.3.0a6/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/README.md
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1194 2024-04-06 16:22:00.000000 scalifiai-client-1.3.0a6/pyproject.toml
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.409607 scalifiai-client-1.3.0a6/scalifiai/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     6439 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      440 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      597 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/credentials.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    19269 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.409607 scalifiai-client-1.3.0a6/scalifiai/mcs/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      101 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       27 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8244 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.409607 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      459 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/base.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-06 12:51:10.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     9873 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/exceptions.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.409607 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/keras/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/keras/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       24 2024-04-06 12:51:24.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/keras/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5589 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/keras/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     8462 2024-04-06 14:18:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/keras/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.409607 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/pytorch/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 12:49:28.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/pytorch/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       26 2024-04-06 12:51:17.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/pytorch/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     5657 2024-04-06 12:58:51.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/pytorch/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     7734 2024-04-06 16:21:26.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/pytorch/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1233 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/schema.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2576 2024-04-06 14:22:40.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/utils.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     2894 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/main.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.413607 scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      396 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    32685 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    13424 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1790 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.413607 scalifiai-client-1.3.0a6/scalifiai/mcs/model/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      848 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    26835 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    34065 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      812 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model/schemas.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.413607 scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/__init__.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      607 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/constants.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    23552 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/exceptions.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)    28720 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/main.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      599 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/schemas.py
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1927 2024-04-05 06:13:21.000000 scalifiai-client-1.3.0a6/scalifiai/request_manager.py
+drwxrwxr-x   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        0 2024-04-06 16:22:23.413607 scalifiai-client-1.3.0a6/scalifiai_client.egg-info/
+-rw-r--r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1299 2024-04-06 16:22:23.000000 scalifiai-client-1.3.0a6/scalifiai_client.egg-info/PKG-INFO
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)     1570 2024-04-06 16:22:23.000000 scalifiai-client-1.3.0a6/scalifiai_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)        1 2024-04-06 16:22:23.000000 scalifiai-client-1.3.0a6/scalifiai_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)      282 2024-04-06 16:22:23.000000 scalifiai-client-1.3.0a6/scalifiai_client.egg-info/requires.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       10 2024-04-06 16:22:23.000000 scalifiai-client-1.3.0a6/scalifiai_client.egg-info/top_level.txt
+-rw-rw-r--   0 ai-bloq-founder  (1000) ai-bloq-founder  (1000)       38 2024-04-06 16:22:23.417606 scalifiai-client-1.3.0a6/setup.cfg
```

### Comparing `scalifiai-client-1.3.0a5/PKG-INFO` & `scalifiai-client-1.3.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.3.0a5
+Version: 1.3.0a6
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scalifiai-client-1.3.0a5/pyproject.toml` & `scalifiai-client-1.3.0a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scalifiai-client"
-version = "1.3.0-alpha.5"
+version = "1.3.0-alpha.6"
 description = "SCALIFI AI NO CODE PLATFORM"
 readme = "README.md"
 authors = [{ name = "Scalifi Ai", email = "helpdesk@scalifiai.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `scalifiai-client-1.3.0a5/scalifiai/base.py` & `scalifiai-client-1.3.0a6/scalifiai/base.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/credentials.py` & `scalifiai-client-1.3.0a6/scalifiai/credentials.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/exceptions.py` & `scalifiai-client-1.3.0a6/scalifiai/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/exceptions.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/exceptions.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/keras/exceptions.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/keras/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/keras/main.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/keras/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/pytorch/exceptions.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/pytorch/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/pytorch/main.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/pytorch/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             temp_dir_path = Path(temp_dir)
             model_save_file_path = temp_dir_path / Path(MODEL_SAVE_FOLDER_NAME)
 
             if not model_save_file_path.exists():
                 model_save_file_path.mkdir()
 
             try:
-                torch.jit.script(self.model).save(model_save_file_path / Path("model.pt"))
+                torch.jit.script(self.model).save(f"{model_save_file_path.absolute()}/model.pt")
             except Exception as ex:
                 print(f"type(ex): {type(ex)}")
                 print(f"ex: {ex}")
                 try:
                     raise PytorchInvalidModelException(extra_info=str(ex))
                 except Exception as ex:
                     raise PytorchInvalidModelException()
@@ -201,9 +201,9 @@
         import torch
 
         model_file = next((item for item in model_path.iterdir() if item.is_file()), None)
 
         if model_file == None:
             raise PytorchInvalidModelException(extra_info="No valid model file found")
 
-        return torch.jit.load(model_file)
+        return torch.jit.load(model_file.absolute())
```

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/schema.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/schema.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/frameworks/utils.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/frameworks/utils.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/main.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/exceptions.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/main.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/metadata/schemas.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/metadata/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/model/constants.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/model/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/model/exceptions.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/model/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/model/main.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/model/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/model/schemas.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/model/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/constants.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/constants.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/exceptions.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/main.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/main.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/mcs/model_version/schemas.py` & `scalifiai-client-1.3.0a6/scalifiai/mcs/model_version/schemas.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai/request_manager.py` & `scalifiai-client-1.3.0a6/scalifiai/request_manager.py`

 * *Files identical despite different names*

### Comparing `scalifiai-client-1.3.0a5/scalifiai_client.egg-info/PKG-INFO` & `scalifiai-client-1.3.0a6/scalifiai_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalifiai-client
-Version: 1.3.0a5
+Version: 1.3.0a6
 Summary: SCALIFI AI NO CODE PLATFORM
 Author-email: Scalifi Ai <helpdesk@scalifiai.com>
 Project-URL: Homepage, https://github.com/Ai-Bloc-24
 Keywords: ai,ml,artificial intelligence,machine learning,no-code,no code,low-code,low code,big-data,big data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scalifiai-client-1.3.0a5/scalifiai_client.egg-info/SOURCES.txt` & `scalifiai-client-1.3.0a6/scalifiai_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

