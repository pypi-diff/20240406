# Comparing `tmp/ai_model_base-0.0.1.dev1.tar.gz` & `tmp/ai_model_base-0.0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_model_base-0.0.1.dev1.tar", max compression
+gzip compressed data, was "ai_model_base-0.0.1.dev2.tar", max compression
```

## Comparing `ai_model_base-0.0.1.dev1.tar` & `ai_model_base-0.0.1.dev2.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0        0 2023-10-20 07:03:06.325079 ai_model_base-0.0.1.dev1/ai_model_base/__init__.py
--rw-r--r--   0        0        0        0 2023-08-18 19:10:04.219233 ai_model_base-0.0.1.dev1/ai_model_base/model/__init__.py
--rw-r--r--   0        0        0      358 2023-10-24 08:55:50.943365 ai_model_base-0.0.1.dev1/ai_model_base/model/BaseModel.py
--rw-r--r--   0        0        0        0 2023-08-30 09:15:13.699810 ai_model_base-0.0.1.dev1/ai_model_base/resource/__init__.py
--rw-r--r--   0        0        0        0 2023-10-26 06:59:46.695817 ai_model_base-0.0.1.dev1/ai_model_base/resource/factory/__init__.py
--rw-r--r--   0        0        0      227 2023-10-26 07:02:29.914425 ai_model_base-0.0.1.dev1/ai_model_base/resource/factory/ModelFactory.py
--rw-r--r--   0        0        0        0 2023-08-30 09:15:53.204504 ai_model_base-0.0.1.dev1/ai_model_base/resource/pool/__init__.py
--rw-r--r--   0        0        0      873 2023-10-26 07:02:29.914425 ai_model_base-0.0.1.dev1/ai_model_base/resource/pool/ModelPool.py
--rw-r--r--   0        0        0      482 2023-10-26 07:19:23.945587 ai_model_base-0.0.1.dev1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-26 06:32:41.998399 ai_model_base-0.0.1.dev1/README.md
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 ai_model_base-0.0.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/model/__init__.py
+-rw-r--r--   0        0        0      358 2024-03-29 08:47:46.646854 ai_model_base-0.0.1.dev2/ai_model_base/model/BaseModel.py
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/resource/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/resource/factory/__init__.py
+-rw-r--r--   0        0        0      227 2024-03-29 09:11:48.035112 ai_model_base-0.0.1.dev2/ai_model_base/resource/factory/ModelFactory.py
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/ai_model_base/resource/pool/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-06 13:27:03.872205 ai_model_base-0.0.1.dev2/ai_model_base/resource/pool/ModelPool.py
+-rw-r--r--   0        0        0        0 2024-04-06 13:04:03.951902 ai_model_base-0.0.1.dev2/ai_model_base/resource/proxy/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-06 13:26:00.660212 ai_model_base-0.0.1.dev2/ai_model_base/resource/proxy/DynamicProxy.py
+-rw-r--r--   0        0        0      482 2024-04-06 13:28:05.364032 ai_model_base-0.0.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-04 09:02:59.729894 ai_model_base-0.0.1.dev2/README.md
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 ai_model_base-0.0.1.dev2/PKG-INFO
```

### Comparing `ai_model_base-0.0.1.dev1/ai_model_base/resource/pool/ModelPool.py` & `ai_model_base-0.0.1.dev2/ai_model_base/resource/pool/ModelPool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from ai_model_base.model.BaseModel import BaseModel
 from ai_model_base.resource.factory.ModelFactory import ModelFactory
+from ai_model_base.resource.proxy.DynamicProxy import DynamicProxy
 
 
 class ModelPool:
     pool: dict[str, BaseModel] = {}
 
+    def get_model_by_name(self, model_name):
+        return DynamicProxy(model_name)
+
     def get_model_by_class(self, model_class):
         model_name = model_class.__name__
         if model_name in self.pool:
             pass
         else:
             model = ModelFactory.create_by_class(model_class)
             self.pool[model_name] = model
```

### Comparing `ai_model_base-0.0.1.dev1/PKG-INFO` & `ai_model_base-0.0.1.dev2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: ai-model-base
-Version: 0.0.1.dev1
+Version: 0.0.1.dev2
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
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/hackty/ai-model-base
 Description-Content-Type: text/markdown
```

