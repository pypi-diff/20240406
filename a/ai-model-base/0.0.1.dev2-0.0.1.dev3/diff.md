# Comparing `tmp/ai_model_base-0.0.1.dev2.tar.gz` & `tmp/ai_model_base-0.0.1.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_model_base-0.0.1.dev2.tar", max compression
+gzip compressed data, was "ai_model_base-0.0.1.dev3.tar", max compression
```

## Comparing `ai_model_base-0.0.1.dev2.tar` & `ai_model_base-0.0.1.dev3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/__init__.py
--rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/model/__init__.py
--rw-r--r--   0        0        0      358 2024-03-29 08:47:46.646854 ai_model_base-0.0.1.dev2/ai_model_base/model/BaseModel.py
--rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/resource/__init__.py
--rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/resource/factory/__init__.py
--rw-r--r--   0        0        0      227 2024-03-29 09:11:48.035112 ai_model_base-0.0.1.dev2/ai_model_base/resource/factory/ModelFactory.py
--rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/resource/pool/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-06 13:27:03.872205 ai_model_base-0.0.1.dev2/ai_model_base/resource/pool/ModelPool.py
--rw-r--r--   0        0        0        0 2024-04-06 13:04:03.951902 ai_model_base-0.0.1.dev2/ai_model_base/resource/proxy/__init__.py
--rw-r--r--   0        0        0      727 2024-04-06 13:26:00.660212 ai_model_base-0.0.1.dev2/ai_model_base/resource/proxy/DynamicProxy.py
--rw-r--r--   0        0        0      482 2024-04-06 13:28:05.364032 ai_model_base-0.0.1.dev2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/README.md
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 ai_model_base-0.0.1.dev2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev3/ai_model_base/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev3/ai_model_base/model/__init__.py
+-rw-r--r--   0        0        0      358 2024-03-29 08:47:46.646854 ai_model_base-0.0.1.dev3/ai_model_base/model/BaseModel.py
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev3/ai_model_base/resource/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev3/ai_model_base/resource/factory/__init__.py
+-rw-r--r--   0        0        0      227 2024-03-29 09:11:48.035112 ai_model_base-0.0.1.dev3/ai_model_base/resource/factory/ModelFactory.py
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev3/ai_model_base/resource/pool/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-06 13:27:03.872205 ai_model_base-0.0.1.dev3/ai_model_base/resource/pool/ModelPool.py
+-rw-r--r--   0        0        0        0 2024-04-06 13:04:03.951902 ai_model_base-0.0.1.dev3/ai_model_base/resource/proxy/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-06 13:26:00.660212 ai_model_base-0.0.1.dev3/ai_model_base/resource/proxy/DynamicProxy.py
+-rw-r--r--   0        0        0      519 2024-04-06 14:13:15.976007 ai_model_base-0.0.1.dev3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev3/README.md
+-rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 ai_model_base-0.0.1.dev3/PKG-INFO
```

### Comparing `ai_model_base-0.0.1.dev2/ai_model_base/resource/pool/ModelPool.py` & `ai_model_base-0.0.1.dev3/ai_model_base/resource/pool/ModelPool.py`

 * *Files identical despite different names*

### Comparing `ai_model_base-0.0.1.dev2/ai_model_base/resource/proxy/DynamicProxy.py` & `ai_model_base-0.0.1.dev3/ai_model_base/resource/proxy/DynamicProxy.py`

 * *Files identical despite different names*

### Comparing `ai_model_base-0.0.1.dev2/PKG-INFO` & `ai_model_base-0.0.1.dev3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ai-model-base
-Version: 0.0.1.dev2
+Version: 0.0.1.dev3
 Summary: 
 Home-page: https://github.com/hackty/ai-model-base
 License: MIT
 Author: taoyang
 Author-email: hackty@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: ai-model-dispatcher (>=0.0.1.dev4,<0.0.2)
 Project-URL: Repository, https://github.com/hackty/ai-model-base
 Description-Content-Type: text/markdown
```

