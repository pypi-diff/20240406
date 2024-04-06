# Comparing `tmp/not_again_ai-0.4.5.tar.gz` & `tmp/not_again_ai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "not_again_ai-0.4.5.tar", max compression
+gzip compressed data, was "not_again_ai-0.5.0.tar", max compression
```

## Comparing `not_again_ai-0.4.5.tar` & `not_again_ai-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.4.5/LICENSE
--rw-r--r--   0        0        0    14318 2024-01-29 00:33:04.305624 not_again_ai-0.4.5/README.md
--rw-r--r--   0        0        0     4103 2024-03-31 23:07:46.384202 not_again_ai-0.4.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.4.5/src/not_again_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.4.5/src/not_again_ai/base/__init__.py
--rw-r--r--   0        0        0      344 2023-10-22 01:25:46.292824 not_again_ai-0.4.5/src/not_again_ai/base/file_system.py
--rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.4.5/src/not_again_ai/base/parallel.py
--rw-r--r--   0        0        0      451 2024-03-31 23:12:37.684279 not_again_ai-0.4.5/src/not_again_ai/llm/__init__.py
--rw-r--r--   0        0        0     8545 2024-02-10 21:35:57.581631 not_again_ai-0.4.5/src/not_again_ai/llm/chat_completion.py
--rw-r--r--   0        0        0     3424 2024-02-04 00:26:08.346905 not_again_ai-0.4.5/src/not_again_ai/llm/context_management.py
--rw-r--r--   0        0        0     2500 2024-01-29 00:33:04.305624 not_again_ai-0.4.5/src/not_again_ai/llm/embeddings.py
--rw-r--r--   0        0        0     2470 2024-01-28 00:29:53.278594 not_again_ai-0.4.5/src/not_again_ai/llm/openai_client.py
--rw-r--r--   0        0        0     2295 2024-02-11 18:48:34.797432 not_again_ai-0.4.5/src/not_again_ai/llm/prompts.py
--rw-r--r--   0        0        0     4244 2024-02-04 00:27:48.412079 not_again_ai-0.4.5/src/not_again_ai/llm/tokens.py
--rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.4.5/src/not_again_ai/py.typed
--rw-r--r--   0        0        0      466 2024-03-31 23:13:12.512750 not_again_ai-0.4.5/src/not_again_ai/statistics/__init__.py
--rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.4.5/src/not_again_ai/statistics/dependence.py
--rw-r--r--   0        0        0      447 2024-03-31 23:13:45.949200 not_again_ai-0.4.5/src/not_again_ai/viz/__init__.py
--rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.4.5/src/not_again_ai/viz/barplots.py
--rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.4.5/src/not_again_ai/viz/distributions.py
--rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.4.5/src/not_again_ai/viz/scatterplot.py
--rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.4.5/src/not_again_ai/viz/time_series.py
--rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.4.5/src/not_again_ai/viz/utils.py
--rw-r--r--   0        0        0    15883 1970-01-01 00:00:00.000000 not_again_ai-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-28 17:31:42.037063 not_again_ai-0.5.0/LICENSE
+-rw-r--r--   0        0        0    14318 2024-04-01 23:35:34.781252 not_again_ai-0.5.0/README.md
+-rw-r--r--   0        0        0     4103 2024-04-06 02:20:49.177649 not_again_ai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-20 15:38:49.234719 not_again_ai-0.5.0/src/not_again_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-22 01:25:46.292824 not_again_ai-0.5.0/src/not_again_ai/base/__init__.py
+-rw-r--r--   0        0        0      344 2023-10-22 01:25:46.292824 not_again_ai-0.5.0/src/not_again_ai/base/file_system.py
+-rw-r--r--   0        0        0     3448 2023-10-22 01:25:46.292824 not_again_ai-0.5.0/src/not_again_ai/base/parallel.py
+-rw-r--r--   0        0        0      451 2024-03-31 23:12:37.684279 not_again_ai-0.5.0/src/not_again_ai/llm/__init__.py
+-rw-r--r--   0        0        0     8410 2024-04-06 14:52:22.933014 not_again_ai-0.5.0/src/not_again_ai/llm/chat_completion.py
+-rw-r--r--   0        0        0     4266 2024-04-06 15:17:52.192357 not_again_ai-0.5.0/src/not_again_ai/llm/chat_completion_vision.py
+-rw-r--r--   0        0        0     3424 2024-02-04 00:26:08.346905 not_again_ai-0.5.0/src/not_again_ai/llm/context_management.py
+-rw-r--r--   0        0        0     2500 2024-01-29 00:33:04.305624 not_again_ai-0.5.0/src/not_again_ai/llm/embeddings.py
+-rw-r--r--   0        0        0     2470 2024-01-28 00:29:53.278594 not_again_ai-0.5.0/src/not_again_ai/llm/openai_client.py
+-rw-r--r--   0        0        0     9496 2024-04-06 15:19:28.097571 not_again_ai-0.5.0/src/not_again_ai/llm/prompts.py
+-rw-r--r--   0        0        0     4244 2024-02-04 00:27:48.412079 not_again_ai-0.5.0/src/not_again_ai/llm/tokens.py
+-rw-r--r--   0        0        0       93 2022-11-20 15:38:49.234719 not_again_ai-0.5.0/src/not_again_ai/py.typed
+-rw-r--r--   0        0        0      466 2024-03-31 23:13:12.512750 not_again_ai-0.5.0/src/not_again_ai/statistics/__init__.py
+-rw-r--r--   0        0        0     4429 2024-01-28 00:06:13.617140 not_again_ai-0.5.0/src/not_again_ai/statistics/dependence.py
+-rw-r--r--   0        0        0      447 2024-03-31 23:13:45.949200 not_again_ai-0.5.0/src/not_again_ai/viz/__init__.py
+-rw-r--r--   0        0        0     3382 2023-11-19 21:07:35.038071 not_again_ai-0.5.0/src/not_again_ai/viz/barplots.py
+-rw-r--r--   0        0        0     4354 2023-10-22 01:25:46.292824 not_again_ai-0.5.0/src/not_again_ai/viz/distributions.py
+-rw-r--r--   0        0        0     2290 2023-10-22 01:25:46.292824 not_again_ai-0.5.0/src/not_again_ai/viz/scatterplot.py
+-rw-r--r--   0        0        0     5212 2024-01-27 23:36:54.323725 not_again_ai-0.5.0/src/not_again_ai/viz/time_series.py
+-rw-r--r--   0        0        0      238 2022-11-20 15:38:49.234719 not_again_ai-0.5.0/src/not_again_ai/viz/utils.py
+-rw-r--r--   0        0        0    15883 1970-01-01 00:00:00.000000 not_again_ai-0.5.0/PKG-INFO
```

### Comparing `not_again_ai-0.4.5/LICENSE` & `not_again_ai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/README.md` & `not_again_ai-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/pyproject.toml` & `not_again_ai-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "not-again-ai"
-version = "0.4.5"
+version = "0.5.0"
 description = "Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place."
 authors = ["DaveCoDev <dave.co.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DaveCoDev/not-again-ai"
 documentation = "https://github.com/DaveCoDev/not-again-ai"
 classifiers = [
@@ -24,18 +24,18 @@
 # Some packages, such as scipy, constrain their upper bound of Python versions they support.
 # Without also constraining the upper bound here, Poetry will not select those versions and will
 # result in an old version being resolved/locked.
 python = "^3.11, <3.13"
 
 # Optional dependencies are defined here, and groupings are defined below.
 numpy = { version = "^1.26.4", optional = true }
-openai = { version = "^1.14.3", optional = true }
+openai = { version = "^1.16.2", optional = true }
 pandas = { version = "^2.2.1", optional = true }
 python-liquid = { version = "^1.12.1", optional = true }
-scipy = { version = "^1.12.0", optional = true }
+scipy = { version = "^1.13.0", optional = true }
 scikit-learn = { version = "^1.4.1.post1", optional = true }
 seaborn = { version = "^0.13.2", optional = true }
 tiktoken = { version = "^0.6.0", optional = true }
 
 [tool.poetry.extras]
 llm = ["openai", "python-liquid", "tiktoken"]
 statistics = ["numpy", "scikit-learn", "scipy"]
```

### Comparing `not_again_ai-0.4.5/src/not_again_ai/base/parallel.py` & `not_again_ai-0.5.0/src/not_again_ai/base/parallel.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/llm/chat_completion.py` & `not_again_ai-0.5.0/src/not_again_ai/llm/chat_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,16 +101,15 @@
 
     response_data: dict[str, Any] = {"choices": []}
     for response_choice in response.choices:
         response_data_curr = {}
         finish_reason = response_choice.finish_reason
         response_data_curr["finish_reason"] = finish_reason
 
-        # Not checking finish_reason=="tool_calls" here because when a user provides function name as tool_choice,
-        # the finish reason is "stop", not "tool_calls"
+        # We first check for tool calls because even if the finish_reason is stop, the model may have called a tool
         tool_calls = response_choice.message.tool_calls
         if tool_calls:
             tool_names = []
             tool_args_list = []
             for tool_call in tool_calls:
                 tool_names.append(tool_call.function.name)
                 tool_args_list.append(json.loads(tool_call.function.arguments))
@@ -155,12 +154,11 @@
         response_data["completion_tokens"] = usage.completion_tokens
         response_data["prompt_tokens"] = usage.prompt_tokens
 
     if seed is not None and response.system_fingerprint is not None:
         response_data["system_fingerprint"] = response.system_fingerprint
 
     if len(response_data["choices"]) == 1:
-        # Add all the fields in the first choice dict to the response_data dict
         response_data.update(response_data["choices"][0])
         del response_data["choices"]
 
     return response_data
```

### Comparing `not_again_ai-0.4.5/src/not_again_ai/llm/context_management.py` & `not_again_ai-0.5.0/src/not_again_ai/llm/context_management.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/llm/embeddings.py` & `not_again_ai-0.5.0/src/not_again_ai/llm/embeddings.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/llm/openai_client.py` & `not_again_ai-0.5.0/src/not_again_ai/llm/openai_client.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/llm/tokens.py` & `not_again_ai-0.5.0/src/not_again_ai/llm/tokens.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/statistics/dependence.py` & `not_again_ai-0.5.0/src/not_again_ai/statistics/dependence.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/viz/barplots.py` & `not_again_ai-0.5.0/src/not_again_ai/viz/barplots.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/viz/distributions.py` & `not_again_ai-0.5.0/src/not_again_ai/viz/distributions.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/viz/scatterplot.py` & `not_again_ai-0.5.0/src/not_again_ai/viz/scatterplot.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/src/not_again_ai/viz/time_series.py` & `not_again_ai-0.5.0/src/not_again_ai/viz/time_series.py`

 * *Files identical despite different names*

### Comparing `not_again_ai-0.4.5/PKG-INFO` & `not_again_ai-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: not-again-ai
-Version: 0.4.5
+Version: 0.5.0
 Summary: Designed to once and for all collect all the little things that come up over and over again in AI projects and put them in one place.
 Home-page: https://github.com/DaveCoDev/not-again-ai
 License: MIT
 Author: DaveCoDev
 Author-email: dave.co.dev@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Development Status :: 3 - Alpha
@@ -17,19 +17,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Provides-Extra: llm
 Provides-Extra: statistics
 Provides-Extra: viz
 Requires-Dist: numpy (>=1.26.4,<2.0.0) ; extra == "statistics" or extra == "viz"
-Requires-Dist: openai (>=1.14.3,<2.0.0) ; extra == "llm"
+Requires-Dist: openai (>=1.16.2,<2.0.0) ; extra == "llm"
 Requires-Dist: pandas (>=2.2.1,<3.0.0) ; extra == "viz"
 Requires-Dist: python-liquid (>=1.12.1,<2.0.0) ; extra == "llm"
 Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0) ; extra == "statistics"
-Requires-Dist: scipy (>=1.12.0,<2.0.0) ; extra == "statistics"
+Requires-Dist: scipy (>=1.13.0,<2.0.0) ; extra == "statistics"
 Requires-Dist: seaborn (>=0.13.2,<0.14.0) ; extra == "viz"
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0) ; extra == "llm"
 Project-URL: Documentation, https://github.com/DaveCoDev/not-again-ai
 Project-URL: Repository, https://github.com/DaveCoDev/not-again-ai
 Description-Content-Type: text/markdown
 
 # not-again-ai
```

