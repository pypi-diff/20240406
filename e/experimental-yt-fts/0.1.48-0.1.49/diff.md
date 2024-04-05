# Comparing `tmp/experimental-yt-fts-0.1.48.tar.gz` & `tmp/experimental-yt-fts-0.1.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimental-yt-fts-0.1.48.tar", last modified: Fri Apr  5 23:19:26 2024, max compression
+gzip compressed data, was "experimental-yt-fts-0.1.49.tar", last modified: Fri Apr  5 23:36:26 2024, max compression
```

## Comparing `experimental-yt-fts-0.1.48.tar` & `experimental-yt-fts-0.1.49.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:19:26.599696 experimental-yt-fts-0.1.48/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-05 23:19:26.599696 experimental-yt-fts-0.1.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:19:26.599696 experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-05 23:19:26.000000 experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 23:19:26.000000 experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:19:26.000000 experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 23:19:26.000000 experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 23:19:26.000000 experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 23:19:26.000000 experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:19:26.599696 experimental-yt-fts-0.1.48/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:19:26.595697 experimental-yt-fts-0.1.48/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/tests/test_export_transcripts.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/tests/test_parse_vtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/tests/test_split_subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/tests/test_vector_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:19:26.599696 experimental-yt-fts-0.1.48/yt_fts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/vector_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-04-05 23:19:22.000000 experimental-yt-fts-0.1.48/yt_fts/yt_fts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:26.439130 experimental-yt-fts-0.1.49/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-05 23:36:26.439130 experimental-yt-fts-0.1.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:26.439130 experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-05 23:36:26.000000 experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-05 23:36:26.000000 experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:36:26.000000 experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 23:36:26.000000 experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-05 23:36:26.000000 experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 23:36:26.000000 experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:36:26.439130 experimental-yt-fts-0.1.49/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:26.435130 experimental-yt-fts-0.1.49/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/tests/test_export_transcripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/tests/test_parse_vtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/tests/test_split_subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/tests/test_vector_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:26.435130 experimental-yt-fts-0.1.49/yt_fts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8800 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/vector_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11651 2024-04-05 23:36:21.000000 experimental-yt-fts-0.1.49/yt_fts/yt_fts.py
```

### Comparing `experimental-yt-fts-0.1.48/LICENSE` & `experimental-yt-fts-0.1.49/LICENSE`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/PKG-INFO` & `experimental-yt-fts-0.1.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimental-yt-fts
-Version: 0.1.48
+Version: 0.1.49
 Summary: Search all of a YouTube channel from the command line
 Author-email: NotJoeMartinez <notjoemartinez@protonmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `experimental-yt-fts-0.1.48/README.md` & `experimental-yt-fts-0.1.49/README.md`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/PKG-INFO` & `experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimental-yt-fts
-Version: 0.1.48
+Version: 0.1.49
 Summary: Search all of a YouTube channel from the command line
 Author-email: NotJoeMartinez <notjoemartinez@protonmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `experimental-yt-fts-0.1.48/experimental_yt_fts.egg-info/SOURCES.txt` & `experimental-yt-fts-0.1.49/experimental_yt_fts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/pyproject.toml` & `experimental-yt-fts-0.1.49/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=46.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "experimental-yt-fts"
-version = "0.1.48" 
+version = "0.1.49" 
 description = "Search all of a YouTube channel from the command line"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
     { name = "NotJoeMartinez", email = "notjoemartinez@protonmail.com" }
 ]
@@ -26,8 +26,8 @@
     "requests==2.31.0",
     "rich==13.7.0",
     "sqlite-utils==3.36",
     "beautifulsoup4==4.12.2"
 ]
 
 [project.scripts]
-yt-fts = "yt_fts.yt_fts:cli"
+yt-fts = "yt_fts.yt_fts:cli"
```

### Comparing `experimental-yt-fts-0.1.48/tests/test_export_transcripts.py` & `experimental-yt-fts-0.1.49/tests/test_export_transcripts.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/tests/test_vector_search.py` & `experimental-yt-fts-0.1.49/tests/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/config.py` & `experimental-yt-fts-0.1.49/yt_fts/config.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/db_utils.py` & `experimental-yt-fts-0.1.49/yt_fts/db_utils.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/download.py` & `experimental-yt-fts-0.1.49/yt_fts/download.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/embeddings.py` & `experimental-yt-fts-0.1.49/yt_fts/embeddings.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/export.py` & `experimental-yt-fts-0.1.49/yt_fts/export.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/list.py` & `experimental-yt-fts-0.1.49/yt_fts/list.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/search.py` & `experimental-yt-fts-0.1.49/yt_fts/search.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/update.py` & `experimental-yt-fts-0.1.49/yt_fts/update.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/utils.py` & `experimental-yt-fts-0.1.49/yt_fts/utils.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/vector_search.py` & `experimental-yt-fts-0.1.49/yt_fts/vector_search.py`

 * *Files identical despite different names*

### Comparing `experimental-yt-fts-0.1.48/yt_fts/yt_fts.py` & `experimental-yt-fts-0.1.49/yt_fts/yt_fts.py`

 * *Files identical despite different names*

