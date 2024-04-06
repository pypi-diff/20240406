# Comparing `tmp/galileo_core-0.4.0.tar.gz` & `tmp/galileo_core-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_core-0.4.0.tar", max compression
+gzip compressed data, was "galileo_core-0.4.1.tar", max compression
```

## Comparing `galileo_core-0.4.0.tar` & `galileo_core-0.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10946 2024-04-06 07:59:08.614448 galileo_core-0.4.0/LICENSE
--rw-r--r--   0        0        0       80 2024-04-06 07:59:08.614448 galileo_core-0.4.0/README.md
--rw-r--r--   0        0        0     2323 2024-04-06 07:59:09.618449 galileo_core-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-06 07:59:09.618449 galileo_core-0.4.0/src/galileo_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/constants/__init__.py
--rw-r--r--   0        0        0      573 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/constants/http_headers.py
--rw-r--r--   0        0        0      362 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/helpers/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/helpers/api_client.py
--rw-r--r--   0        0        0     5322 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/helpers/config.py
--rw-r--r--   0        0        0       60 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/helpers/logger.py
--rw-r--r--   0        0        0        0 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/protect/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/protect/action.py
--rw-r--r--   0        0        0      488 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/protect/metric.py
--rw-r--r--   0        0        0      772 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/protect/payload.py
--rw-r--r--   0        0        0     2075 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/protect/request.py
--rw-r--r--   0        0        0     1934 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/protect/rule.py
--rw-r--r--   0        0        0     1034 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/protect/ruleset.py
--rw-r--r--   0        0        0     1124 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/protect/stage.py
--rw-r--r--   0        0        0        0 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/shared/__init__.py
--rw-r--r--   0        0        0      149 2024-04-06 07:59:08.614448 galileo_core-0.4.0/src/galileo_core/schemas/shared/metric.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-06 08:05:55.033620 galileo_core-0.4.1/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-06 08:05:55.033620 galileo_core-0.4.1/README.md
+-rw-r--r--   0        0        0     2323 2024-04-06 08:05:57.557616 galileo_core-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-06 08:05:57.557616 galileo_core-0.4.1/src/galileo_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/constants/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/constants/http_headers.py
+-rw-r--r--   0        0        0      362 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/helpers/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/helpers/api_client.py
+-rw-r--r--   0        0        0     5322 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/helpers/config.py
+-rw-r--r--   0        0        0       60 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/helpers/logger.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/protect/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/protect/action.py
+-rw-r--r--   0        0        0      488 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/protect/metric.py
+-rw-r--r--   0        0        0      902 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/protect/payload.py
+-rw-r--r--   0        0        0     2075 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/protect/request.py
+-rw-r--r--   0        0        0     1934 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/protect/rule.py
+-rw-r--r--   0        0        0     1034 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/protect/ruleset.py
+-rw-r--r--   0        0        0     1124 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/protect/stage.py
+-rw-r--r--   0        0        0        0 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/shared/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-06 08:05:55.037620 galileo_core-0.4.1/src/galileo_core/schemas/shared/metric.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.4.1/PKG-INFO
```

### Comparing `galileo_core-0.4.0/LICENSE` & `galileo_core-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/pyproject.toml` & `galileo_core-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-core"
-version = "0.4.0"
+version = "0.4.1"
 description = "Shared schemas and configuration for Galileo's Python packages."
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_core", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
```

### Comparing `galileo_core-0.4.0/src/galileo_core/constants/http_headers.py` & `galileo_core-0.4.1/src/galileo_core/constants/http_headers.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/src/galileo_core/helpers/api_client.py` & `galileo_core-0.4.1/src/galileo_core/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/src/galileo_core/helpers/config.py` & `galileo_core-0.4.1/src/galileo_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/src/galileo_core/schemas/protect/action.py` & `galileo_core-0.4.1/src/galileo_core/schemas/protect/action.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/src/galileo_core/schemas/protect/payload.py` & `galileo_core-0.4.1/src/galileo_core/schemas/protect/payload.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import cached_property
 from typing import Optional
 
 from pydantic import BaseModel, Field, computed_field, model_validator
 
 
 class Payload(BaseModel):
     input: Optional[str] = Field(default=None, description="Input text to be processed.")
@@ -9,15 +10,17 @@
 
     @model_validator(mode="after")
     def ensure_input_or_output(self) -> "Payload":
         if not self.input and not self.output:
             raise ValueError("Either input or output must be set.")
         return self
 
-    @computed_field
+    # https://github.com/python/mypy/issues/1362
+    @computed_field  # type: ignore[misc]
+    @cached_property
     def text(self) -> str:
         if self.output:
             return self.output
         elif self.input:
             return self.input
         else:
             raise ValueError("Either input or output must be set.")
```

### Comparing `galileo_core-0.4.0/src/galileo_core/schemas/protect/request.py` & `galileo_core-0.4.1/src/galileo_core/schemas/protect/request.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/src/galileo_core/schemas/protect/rule.py` & `galileo_core-0.4.1/src/galileo_core/schemas/protect/rule.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/src/galileo_core/schemas/protect/ruleset.py` & `galileo_core-0.4.1/src/galileo_core/schemas/protect/ruleset.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/src/galileo_core/schemas/protect/stage.py` & `galileo_core-0.4.1/src/galileo_core/schemas/protect/stage.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.4.0/PKG-INFO` & `galileo_core-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galileo-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: Shared schemas and configuration for Galileo's Python packages.
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

