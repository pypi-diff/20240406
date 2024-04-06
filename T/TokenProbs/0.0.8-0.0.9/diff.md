# Comparing `tmp/TokenProbs-0.0.8.tar.gz` & `tmp/TokenProbs-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TokenProbs-0.0.8.tar", last modified: Thu Apr  4 00:58:22 2024, max compression
+gzip compressed data, was "TokenProbs-0.0.9.tar", last modified: Thu Apr  4 01:20:59 2024, max compression
```

## Comparing `TokenProbs-0.0.8.tar` & `TokenProbs-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:58:22.036741 TokenProbs-0.0.8/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-0.0.8/LICENSE
--rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 00:58:22.036303 TokenProbs-0.0.8/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     2999 2024-04-02 20:06:10.000000 TokenProbs-0.0.8/README.md
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-04 00:58:22.036811 TokenProbs-0.0.8/setup.cfg
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     1194 2024-04-04 00:58:10.000000 TokenProbs-0.0.8/setup.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:58:22.032310 TokenProbs-0.0.8/src/
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:58:22.034121 TokenProbs-0.0.8/src/TokenProbs/
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-04 00:57:59.000000 TokenProbs-0.0.8/src/TokenProbs/__init__.py
--rw-rw-r--   0 faf32    (50383) faf32    (50391)     8847 2024-04-02 22:14:09.000000 TokenProbs-0.0.8/src/TokenProbs/logit_extraction.py
-drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 00:58:22.035979 TokenProbs-0.0.8/src/TokenProbs.egg-info/
--rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 00:58:22.034684 TokenProbs-0.0.8/src/TokenProbs.egg-info/PKG-INFO
--rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-04 00:58:22.035045 TokenProbs-0.0.8/src/TokenProbs.egg-info/SOURCES.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-04 00:58:22.035373 TokenProbs-0.0.8/src/TokenProbs.egg-info/dependency_links.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-04 00:58:22.035709 TokenProbs-0.0.8/src/TokenProbs.egg-info/requires.txt
--rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-04 00:58:22.036037 TokenProbs-0.0.8/src/TokenProbs.egg-info/top_level.txt
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 01:20:59.460533 TokenProbs-0.0.9/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        0 2024-04-01 19:16:35.000000 TokenProbs-0.0.9/LICENSE
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 01:20:59.459986 TokenProbs-0.0.9/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     2999 2024-04-02 20:06:10.000000 TokenProbs-0.0.9/README.md
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       38 2024-04-04 01:20:59.460606 TokenProbs-0.0.9/setup.cfg
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     1194 2024-04-04 01:20:52.000000 TokenProbs-0.0.9/setup.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 01:20:59.455346 TokenProbs-0.0.9/src/
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 01:20:59.457385 TokenProbs-0.0.9/src/TokenProbs/
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-04 01:15:43.000000 TokenProbs-0.0.9/src/TokenProbs/__init__.py
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)     8847 2024-04-02 22:14:09.000000 TokenProbs-0.0.9/src/TokenProbs/logit_extraction.py
+drwxrwxr-x   0 faf32    (50383) faf32    (50391)        0 2024-04-04 01:20:59.459506 TokenProbs-0.0.9/src/TokenProbs.egg-info/
+-rw-r--r--   0 faf32    (50383) faf32    (50391)     3559 2024-04-04 01:20:59.457986 TokenProbs-0.0.9/src/TokenProbs.egg-info/PKG-INFO
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)      277 2024-04-04 01:20:59.458407 TokenProbs-0.0.9/src/TokenProbs.egg-info/SOURCES.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)        1 2024-04-04 01:20:59.458796 TokenProbs-0.0.9/src/TokenProbs.egg-info/dependency_links.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       63 2024-04-04 01:20:59.459197 TokenProbs-0.0.9/src/TokenProbs.egg-info/requires.txt
+-rw-rw-r--   0 faf32    (50383) faf32    (50391)       11 2024-04-04 01:20:59.459575 TokenProbs-0.0.9/src/TokenProbs.egg-info/top_level.txt
```

### Comparing `TokenProbs-0.0.8/PKG-INFO` & `TokenProbs-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `TokenProbs-0.0.8/README.md` & `TokenProbs-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `TokenProbs-0.0.8/setup.py` & `TokenProbs-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Extract token-level probabilities from LLMs for classification-type outputs.'
 LONG_DESCRIPTION = 'A package that allows one to extract token-level probabilities. This method can be used for example to extract sentiment class probabilities or other probability-based queries instead of parsing text-generation outputs.'
 
 # Setting up
 setup(
     name="TokenProbs",
     version=VERSION,
```

### Comparing `TokenProbs-0.0.8/src/TokenProbs/logit_extraction.py` & `TokenProbs-0.0.9/src/TokenProbs/logit_extraction.py`

 * *Files identical despite different names*

### Comparing `TokenProbs-0.0.8/src/TokenProbs.egg-info/PKG-INFO` & `TokenProbs-0.0.9/src/TokenProbs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TokenProbs
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extract token-level probabilities from LLMs for classification-type outputs.
 Author: Francesco A. Fabozzi
 Author-email: francescoafabozzi@gmail.com
 Keywords: python,LLMs,finance,forecasting,language models,huggingface
 Classifier: Development Status :: 1 - Planning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

