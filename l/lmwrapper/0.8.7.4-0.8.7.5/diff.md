# Comparing `tmp/lmwrapper-0.8.7.4.tar.gz` & `tmp/lmwrapper-0.8.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmwrapper-0.8.7.4.tar", last modified: Tue Apr  2 23:25:38 2024, max compression
+gzip compressed data, was "lmwrapper-0.8.7.5.tar", last modified: Sat Apr  6 05:14:02 2024, max compression
```

## Comparing `lmwrapper-0.8.7.4.tar` & `lmwrapper-0.8.7.5.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-02 23:25:38.120724 lmwrapper-0.8.7.4/
--rw-r--r--   0 dgros      (501) staff       (20)     6726 2024-04-02 23:25:38.120484 lmwrapper-0.8.7.4/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     5308 2024-04-02 23:18:51.000000 lmwrapper-0.8.7.4/README.md
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-02 23:25:38.116179 lmwrapper-0.8.7.4/lmwrapper/
--rw-r--r--   0 dgros      (501) staff       (20)     2416 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/_TokenStoppingCriteria.py
--rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     4259 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/abstract_predictor.py
--rw-r--r--   0 dgros      (501) staff       (20)     1654 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/caching.py
--rw-r--r--   0 dgros      (501) staff       (20)      294 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/env.py
--rw-r--r--   0 dgros      (501) staff       (20)     3646 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/prompt_trimming.py
--rw-r--r--   0 dgros      (501) staff       (20)      583 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/runtime.py
--rw-r--r--   0 dgros      (501) staff       (20)     1149 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/secrets_manager.py
--rw-r--r--   0 dgros      (501) staff       (20)    16083 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/structs.py
--rw-r--r--   0 dgros      (501) staff       (20)      710 2024-03-19 21:15:58.000000 lmwrapper-0.8.7.4/lmwrapper/togethertoy.py
--rw-r--r--   0 dgros      (501) staff       (20)     2532 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/utils.py
--rw-r--r--   0 dgros      (501) staff       (20)     1098 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/lmwrapper/wrapping_config.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-02 23:25:38.119451 lmwrapper-0.8.7.4/lmwrapper.egg-info/
--rw-r--r--   0 dgros      (501) staff       (20)     6726 2024-04-02 23:25:38.000000 lmwrapper-0.8.7.4/lmwrapper.egg-info/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)      700 2024-04-02 23:25:38.000000 lmwrapper-0.8.7.4/lmwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 dgros      (501) staff       (20)        1 2024-04-02 23:25:38.000000 lmwrapper-0.8.7.4/lmwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 dgros      (501) staff       (20)      402 2024-04-02 23:25:38.000000 lmwrapper-0.8.7.4/lmwrapper.egg-info/requires.txt
--rw-r--r--   0 dgros      (501) staff       (20)       10 2024-04-02 23:25:38.000000 lmwrapper-0.8.7.4/lmwrapper.egg-info/top_level.txt
--rw-r--r--   0 dgros      (501) staff       (20)     4743 2024-04-02 23:19:23.000000 lmwrapper-0.8.7.4/pyproject.toml
--rw-r--r--   0 dgros      (501) staff       (20)       38 2024-04-02 23:25:38.120767 lmwrapper-0.8.7.4/setup.cfg
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-02 23:25:38.119045 lmwrapper-0.8.7.4/test/
--rw-r--r--   0 dgros      (501) staff       (20)     1244 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.4/test/test_caching.py
--rw-r--r--   0 dgros      (501) staff       (20)      547 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/test/test_docs.py
--rw-r--r--   0 dgros      (501) staff       (20)    30472 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.4/test/test_huggingface.py
--rw-r--r--   0 dgros      (501) staff       (20)     6534 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.4/test/test_huggingface_memory.py
--rw-r--r--   0 dgros      (501) staff       (20)    17741 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.4/test/test_models_common.py
--rw-r--r--   0 dgros      (501) staff       (20)    10251 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.4/test/test_openai.py
--rw-r--r--   0 dgros      (501) staff       (20)      512 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.4/test/test_prompt_trimming.py
--rw-r--r--   0 dgros      (501) staff       (20)     2080 2024-02-10 07:57:44.000000 lmwrapper-0.8.7.4/test/test_structs.py
--rw-r--r--   0 dgros      (501) staff       (20)      237 2024-02-10 00:21:07.000000 lmwrapper-0.8.7.4/test/test_util.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 05:14:02.715180 lmwrapper-0.8.7.5/
+-rw-r--r--   0 dgros      (501) staff       (20)     6730 2024-04-06 05:14:02.714852 lmwrapper-0.8.7.5/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     5312 2024-04-06 05:06:05.000000 lmwrapper-0.8.7.5/README.md
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 05:14:02.707861 lmwrapper-0.8.7.5/lmwrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)     2416 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/_TokenStoppingCriteria.py
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4259 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/abstract_predictor.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1654 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/caching.py
+-rw-r--r--   0 dgros      (501) staff       (20)      294 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/env.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 05:14:02.710100 lmwrapper-0.8.7.5/lmwrapper/huggingface_wrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)      177 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/lmwrapper/huggingface_wrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1712 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/lmwrapper/huggingface_wrapper/prediction.py
+-rw-r--r--   0 dgros      (501) staff       (20)    34279 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/lmwrapper/huggingface_wrapper/predictor.py
+-rw-r--r--   0 dgros      (501) staff       (20)    27210 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/lmwrapper/huggingface_wrapper/wrapper.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 05:14:02.710591 lmwrapper-0.8.7.5/lmwrapper/openai_wrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)      139 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/lmwrapper/openai_wrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)    18610 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/lmwrapper/openai_wrapper/wrapper.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3646 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/prompt_trimming.py
+-rw-r--r--   0 dgros      (501) staff       (20)      583 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/runtime.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1149 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/secrets_manager.py
+-rw-r--r--   0 dgros      (501) staff       (20)    16083 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/structs.py
+-rw-r--r--   0 dgros      (501) staff       (20)      710 2024-03-19 21:15:58.000000 lmwrapper-0.8.7.5/lmwrapper/togethertoy.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2532 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/utils.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1098 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/lmwrapper/wrapping_config.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 05:14:02.713433 lmwrapper-0.8.7.5/lmwrapper.egg-info/
+-rw-r--r--   0 dgros      (501) staff       (20)     6730 2024-04-06 05:14:02.000000 lmwrapper-0.8.7.5/lmwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)      943 2024-04-06 05:14:02.000000 lmwrapper-0.8.7.5/lmwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 dgros      (501) staff       (20)        1 2024-04-06 05:14:02.000000 lmwrapper-0.8.7.5/lmwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 dgros      (501) staff       (20)      402 2024-04-06 05:14:02.000000 lmwrapper-0.8.7.5/lmwrapper.egg-info/requires.txt
+-rw-r--r--   0 dgros      (501) staff       (20)       10 2024-04-06 05:14:02.000000 lmwrapper-0.8.7.5/lmwrapper.egg-info/top_level.txt
+-rw-r--r--   0 dgros      (501) staff       (20)     4819 2024-04-06 05:05:16.000000 lmwrapper-0.8.7.5/pyproject.toml
+-rw-r--r--   0 dgros      (501) staff       (20)       38 2024-04-06 05:14:02.715246 lmwrapper-0.8.7.5/setup.cfg
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 05:14:02.712878 lmwrapper-0.8.7.5/test/
+-rw-r--r--   0 dgros      (501) staff       (20)     1244 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/test/test_caching.py
+-rw-r--r--   0 dgros      (501) staff       (20)      547 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/test/test_docs.py
+-rw-r--r--   0 dgros      (501) staff       (20)    30472 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/test/test_huggingface.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6534 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/test/test_huggingface_memory.py
+-rw-r--r--   0 dgros      (501) staff       (20)    17741 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/test/test_models_common.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10251 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.5/test/test_openai.py
+-rw-r--r--   0 dgros      (501) staff       (20)      512 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.5/test/test_prompt_trimming.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2080 2024-02-10 07:57:44.000000 lmwrapper-0.8.7.5/test/test_structs.py
+-rw-r--r--   0 dgros      (501) staff       (20)      237 2024-02-10 00:21:07.000000 lmwrapper-0.8.7.5/test/test_util.py
```

### Comparing `lmwrapper-0.8.7.4/PKG-INFO` & `lmwrapper-0.8.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwrapper
-Version: 0.8.7.4
+Version: 0.8.7.5
 Summary: Wrapper around language model APIs
 Author-email: David Gros <DNGros@users.noreply.github.com>, Claudio Spiess <claudiosv@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/DaiseyCode/lmwrapper
 Keywords: large language models,openai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -51,21 +51,21 @@
 ```bash
 pip install lmwrapper
 ```
 
 For usage with HuggingFace models as well:
 
 ```bash
-pip install lmwrapper[hf]
+pip install 'lmwrapper[hf]'
 ```
 
 For development dependencies:
 
 ```bash
-pip install lmwrapper[dev]
+pip install 'lmwrapper[dev]'
 ```
 
 <!---
 If you prefer using `conda`/`mamba` to manage your environments, you may edit the `environment.yml` file to your liking & setup and create a new environment based on it:
 
 ```bash
 mamba env create -f environment.yml
```

### Comparing `lmwrapper-0.8.7.4/README.md` & `lmwrapper-0.8.7.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 ```bash
 pip install lmwrapper
 ```
 
 For usage with HuggingFace models as well:
 
 ```bash
-pip install lmwrapper[hf]
+pip install 'lmwrapper[hf]'
 ```
 
 For development dependencies:
 
 ```bash
-pip install lmwrapper[dev]
+pip install 'lmwrapper[dev]'
 ```
 
 <!---
 If you prefer using `conda`/`mamba` to manage your environments, you may edit the `environment.yml` file to your liking & setup and create a new environment based on it:
 
 ```bash
 mamba env create -f environment.yml
```

### Comparing `lmwrapper-0.8.7.4/lmwrapper/_TokenStoppingCriteria.py` & `lmwrapper-0.8.7.5/lmwrapper/_TokenStoppingCriteria.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/abstract_predictor.py` & `lmwrapper-0.8.7.5/lmwrapper/abstract_predictor.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/caching.py` & `lmwrapper-0.8.7.5/lmwrapper/caching.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/prompt_trimming.py` & `lmwrapper-0.8.7.5/lmwrapper/prompt_trimming.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/runtime.py` & `lmwrapper-0.8.7.5/lmwrapper/runtime.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/secrets_manager.py` & `lmwrapper-0.8.7.5/lmwrapper/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/structs.py` & `lmwrapper-0.8.7.5/lmwrapper/structs.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/togethertoy.py` & `lmwrapper-0.8.7.5/lmwrapper/togethertoy.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/utils.py` & `lmwrapper-0.8.7.5/lmwrapper/utils.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper/wrapping_config.py` & `lmwrapper-0.8.7.5/lmwrapper/wrapping_config.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/lmwrapper.egg-info/PKG-INFO` & `lmwrapper-0.8.7.5/lmwrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwrapper
-Version: 0.8.7.4
+Version: 0.8.7.5
 Summary: Wrapper around language model APIs
 Author-email: David Gros <DNGros@users.noreply.github.com>, Claudio Spiess <claudiosv@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/DaiseyCode/lmwrapper
 Keywords: large language models,openai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -51,21 +51,21 @@
 ```bash
 pip install lmwrapper
 ```
 
 For usage with HuggingFace models as well:
 
 ```bash
-pip install lmwrapper[hf]
+pip install 'lmwrapper[hf]'
 ```
 
 For development dependencies:
 
 ```bash
-pip install lmwrapper[dev]
+pip install 'lmwrapper[dev]'
 ```
 
 <!---
 If you prefer using `conda`/`mamba` to manage your environments, you may edit the `environment.yml` file to your liking & setup and create a new environment based on it:
 
 ```bash
 mamba env create -f environment.yml
```

### Comparing `lmwrapper-0.8.7.4/lmwrapper.egg-info/SOURCES.txt` & `lmwrapper-0.8.7.5/lmwrapper.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 lmwrapper/utils.py
 lmwrapper/wrapping_config.py
 lmwrapper.egg-info/PKG-INFO
 lmwrapper.egg-info/SOURCES.txt
 lmwrapper.egg-info/dependency_links.txt
 lmwrapper.egg-info/requires.txt
 lmwrapper.egg-info/top_level.txt
+lmwrapper/huggingface_wrapper/__init__.py
+lmwrapper/huggingface_wrapper/prediction.py
+lmwrapper/huggingface_wrapper/predictor.py
+lmwrapper/huggingface_wrapper/wrapper.py
+lmwrapper/openai_wrapper/__init__.py
+lmwrapper/openai_wrapper/wrapper.py
 test/test_caching.py
 test/test_docs.py
 test/test_huggingface.py
 test/test_huggingface_memory.py
 test/test_models_common.py
 test/test_openai.py
 test/test_prompt_trimming.py
```

### Comparing `lmwrapper-0.8.7.4/pyproject.toml` & `lmwrapper-0.8.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 [build-system]
 requires = ["setuptools>=68.2.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-packages = ["lmwrapper"]
+packages = [
+    "lmwrapper",
+    "lmwrapper.huggingface_wrapper",
+    "lmwrapper.openai_wrapper",
+]
 #py-modules = ["lmwrapper"]
 
 [project]
 name = "lmwrapper"
-version = "0.8.7.4"
+version = "0.8.7.5"
 authors = [
     { name = "David Gros", email = "DNGros@users.noreply.github.com" },
     { name = "Claudio Spiess", email = "claudiosv@users.noreply.github.com" },
 ]
 description = "Wrapper around language model APIs"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lmwrapper-0.8.7.4/test/test_caching.py` & `lmwrapper-0.8.7.5/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/test/test_docs.py` & `lmwrapper-0.8.7.5/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/test/test_huggingface.py` & `lmwrapper-0.8.7.5/test/test_huggingface.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/test/test_huggingface_memory.py` & `lmwrapper-0.8.7.5/test/test_huggingface_memory.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/test/test_models_common.py` & `lmwrapper-0.8.7.5/test/test_models_common.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/test/test_openai.py` & `lmwrapper-0.8.7.5/test/test_openai.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/test/test_prompt_trimming.py` & `lmwrapper-0.8.7.5/test/test_prompt_trimming.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.4/test/test_structs.py` & `lmwrapper-0.8.7.5/test/test_structs.py`

 * *Files identical despite different names*

