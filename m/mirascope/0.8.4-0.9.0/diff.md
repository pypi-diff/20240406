# Comparing `tmp/mirascope-0.8.4.tar.gz` & `tmp/mirascope-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirascope-0.8.4.tar", max compression
+gzip compressed data, was "mirascope-0.9.0.tar", max compression
```

## Comparing `mirascope-0.8.4.tar` & `mirascope-0.9.0.tar`

### file list

```diff
@@ -1,57 +1,62 @@
--rw-r--r--   0        0        0     1072 2024-04-05 05:54:10.645911 mirascope-0.8.4/LICENSE
--rw-r--r--   0        0        0    10093 2024-04-05 05:54:10.645911 mirascope-0.8.4/docs/README.md
--rw-r--r--   0        0        0      472 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/__init__.py
--rw-r--r--   0        0        0      270 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/__init__.py
--rw-r--r--   0        0        0     6596 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/calls.py
--rw-r--r--   0        0        0     4068 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/extractors.py
--rw-r--r--   0        0        0        0 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/py.typed
--rw-r--r--   0        0        0     3549 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/tools.py
--rw-r--r--   0        0        0     6006 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/anthropic/types.py
--rw-r--r--   0        0        0      453 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/__init__.py
--rw-r--r--   0        0        0     3645 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/calls.py
--rw-r--r--   0        0        0     8304 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/extractors.py
--rw-r--r--   0        0        0     5696 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/prompts.py
--rw-r--r--   0        0        0        0 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/py.typed
--rw-r--r--   0        0        0     2890 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/tools.py
--rw-r--r--   0        0        0     5313 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/types.py
--rw-r--r--   0        0        0     5615 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/base/utils.py
--rw-r--r--   0        0        0       97 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/__init__.py
--rw-r--r--   0        0        0      199 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/__init__.py
--rw-r--r--   0        0        0     4213 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/add.py
--rw-r--r--   0        0        0     3002 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/init.py
--rw-r--r--   0        0        0        0 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/py.typed
--rw-r--r--   0        0        0     3101 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/remove.py
--rw-r--r--   0        0        0     2008 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/status.py
--rw-r--r--   0        0        0     2801 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/commands/use.py
--rw-r--r--   0        0        0      118 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/constants.py
--rw-r--r--   0        0        0       86 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/generic/__init__.py
--rw-r--r--   0        0        0      494 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/generic/mirascope.ini.j2
--rw-r--r--   0        0        0     1554 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/generic/prompt_template.j2
--rw-r--r--   0        0        0     1067 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/py.typed
--rw-r--r--   0        0        0     1197 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/schemas.py
--rw-r--r--   0        0        0    24322 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/cli/utils.py
--rw-r--r--   0        0        0     1552 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/enums.py
--rw-r--r--   0        0        0      241 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/__init__.py
--rw-r--r--   0        0        0     6333 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/calls.py
--rw-r--r--   0        0        0     3730 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/extractors.py
--rw-r--r--   0        0        0     4081 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/tools.py
--rw-r--r--   0        0        0     4950 2024-04-05 05:54:10.649911 mirascope-0.8.4/mirascope/gemini/types.py
--rw-r--r--   0        0        0      239 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/__init__.py
--rw-r--r--   0        0        0     5900 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/calls.py
--rw-r--r--   0        0        0     3940 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/extractors.py
--rw-r--r--   0        0        0        0 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/py.typed
--rw-r--r--   0        0        0     3896 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/tools.py
--rw-r--r--   0        0        0     6389 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/mistral/types.py
--rw-r--r--   0        0        0      232 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/__init__.py
--rw-r--r--   0        0        0     9068 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/calls.py
--rw-r--r--   0        0        0     3932 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/extractors.py
--rw-r--r--   0        0        0        0 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/py.typed
--rw-r--r--   0        0        0     3860 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/tools.py
--rw-r--r--   0        0        0     9087 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/openai/types.py
--rw-r--r--   0        0        0        0 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/py.typed
--rw-r--r--   0        0        0      151 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/wandb/__init__.py
--rw-r--r--   0        0        0     9593 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/wandb/wandb.py
--rw-r--r--   0        0        0     1921 2024-04-05 05:54:10.653911 mirascope-0.8.4/mirascope/wandb/weave.py
--rw-r--r--   0        0        0     2763 2024-04-05 05:54:10.653911 mirascope-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    11526 1970-01-01 00:00:00.000000 mirascope-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 17:20:31.993416 mirascope-0.9.0/LICENSE
+-rw-r--r--   0        0        0    10203 2024-04-05 17:20:31.993416 mirascope-0.9.0/docs/README.md
+-rw-r--r--   0        0        0      524 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/__init__.py
+-rw-r--r--   0        0        0      270 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/calls.py
+-rw-r--r--   0        0        0     4068 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/py.typed
+-rw-r--r--   0        0        0     3549 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/tools.py
+-rw-r--r--   0        0        0     6006 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/types.py
+-rw-r--r--   0        0        0      453 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/__init__.py
+-rw-r--r--   0        0        0     3645 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/calls.py
+-rw-r--r--   0        0        0     8304 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/extractors.py
+-rw-r--r--   0        0        0     5696 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/prompts.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/py.typed
+-rw-r--r--   0        0        0     2890 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/tools.py
+-rw-r--r--   0        0        0     5313 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/types.py
+-rw-r--r--   0        0        0     5615 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/utils.py
+-rw-r--r--   0        0        0       97 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4213 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/add.py
+-rw-r--r--   0        0        0     3002 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/init.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/py.typed
+-rw-r--r--   0        0        0     3101 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/remove.py
+-rw-r--r--   0        0        0     2008 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/status.py
+-rw-r--r--   0        0        0     2801 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/use.py
+-rw-r--r--   0        0        0      118 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/constants.py
+-rw-r--r--   0        0        0       86 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/generic/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/generic/mirascope.ini.j2
+-rw-r--r--   0        0        0     1554 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/generic/prompt_template.j2
+-rw-r--r--   0        0        0     1067 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/py.typed
+-rw-r--r--   0        0        0     1197 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/schemas.py
+-rw-r--r--   0        0        0    24322 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/utils.py
+-rw-r--r--   0        0        0     1552 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/enums.py
+-rw-r--r--   0        0        0      241 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/__init__.py
+-rw-r--r--   0        0        0     6333 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/calls.py
+-rw-r--r--   0        0        0     3730 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/extractors.py
+-rw-r--r--   0        0        0     4081 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/tools.py
+-rw-r--r--   0        0        0     4950 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/types.py
+-rw-r--r--   0        0        0      223 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/__init__.py
+-rw-r--r--   0        0        0     7211 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/calls.py
+-rw-r--r--   0        0        0     3537 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/extractors.py
+-rw-r--r--   0        0        0     3954 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/tools.py
+-rw-r--r--   0        0        0     8845 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/types.py
+-rw-r--r--   0        0        0      239 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/__init__.py
+-rw-r--r--   0        0        0     5900 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/calls.py
+-rw-r--r--   0        0        0     3940 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/py.typed
+-rw-r--r--   0        0        0     3898 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/tools.py
+-rw-r--r--   0        0        0     6389 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/types.py
+-rw-r--r--   0        0        0      232 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/__init__.py
+-rw-r--r--   0        0        0     8720 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/calls.py
+-rw-r--r--   0        0        0     3932 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/py.typed
+-rw-r--r--   0        0        0     3860 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/tools.py
+-rw-r--r--   0        0        0     9087 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/types.py
+-rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/py.typed
+-rw-r--r--   0        0        0      151 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/wandb/__init__.py
+-rw-r--r--   0        0        0     9593 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/wandb/wandb.py
+-rw-r--r--   0        0        0     1921 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/wandb/weave.py
+-rw-r--r--   0        0        0     2861 2024-04-05 17:20:32.001416 mirascope-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11730 1970-01-01 00:00:00.000000 mirascope-0.9.0/PKG-INFO
```

### Comparing `mirascope-0.8.4/LICENSE` & `mirascope-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/docs/README.md` & `mirascope-0.9.0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -288,29 +288,34 @@
 def root(book_recommender: BookRecommender) -> Book:
     """Generates a book based on provided `genre`."""
     return book_recommender.extract()
 ```
 
 ## Roadmap
 
-- [x]  Extracting structured information using LLMs
+- [X]  Extracting structured information using LLMs
+- [ ]  RAG
+- [ ]  Agents
 - [ ]  Streaming extraction for tools (function calling)
 - [ ]  Additional template parsing for more complex messages
-    - [x]  Chat History
+    - [X]  Chat History
+    - [ ]  Better Tool Messages
     - [ ]  Additional Metadata
     - [ ]  Vision
-- [ ]  RAG
-- [ ]  Agents
 - [ ]  Support for more LLM providers:
-    - [X]  Anthropic Function Calling
-    - [ ]  Mistral
+    - [X]  Anthropic
+    - [X]  Gemini
+    - [X]  Mistral
+    - [X]  Groq
+    - [ ]  Cohere
     - [ ]  HuggingFace
 - [ ]  Integrations
-    - [x]  Weights & Biases
-    - [x]  LangChain / LangSmith
+    - [X]  Weights & Biases Trace
+    - [X]  Weave by Weights & Biases
+    - [X]  LangChain / LangSmith
     - [ ]  … tell us what you’d like integrated!
 - [ ]  Evaluating prompts and their quality by version
 
 ## Versioning
 
 Mirascope uses [Semantic Versioning](https://semver.org/).
```

### Comparing `mirascope-0.8.4/mirascope/anthropic/calls.py` & `mirascope-0.9.0/mirascope/anthropic/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/anthropic/extractors.py` & `mirascope-0.9.0/mirascope/anthropic/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/anthropic/tools.py` & `mirascope-0.9.0/mirascope/anthropic/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/anthropic/types.py` & `mirascope-0.9.0/mirascope/anthropic/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/base/calls.py` & `mirascope-0.9.0/mirascope/base/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/base/extractors.py` & `mirascope-0.9.0/mirascope/base/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/base/prompts.py` & `mirascope-0.9.0/mirascope/base/prompts.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/base/tools.py` & `mirascope-0.9.0/mirascope/base/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/base/types.py` & `mirascope-0.9.0/mirascope/base/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/base/utils.py` & `mirascope-0.9.0/mirascope/base/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/commands/add.py` & `mirascope-0.9.0/mirascope/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/commands/init.py` & `mirascope-0.9.0/mirascope/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/commands/remove.py` & `mirascope-0.9.0/mirascope/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/commands/status.py` & `mirascope-0.9.0/mirascope/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/commands/use.py` & `mirascope-0.9.0/mirascope/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/generic/prompt_template.j2` & `mirascope-0.9.0/mirascope/cli/generic/prompt_template.j2`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/main.py` & `mirascope-0.9.0/mirascope/cli/main.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/schemas.py` & `mirascope-0.9.0/mirascope/cli/schemas.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/cli/utils.py` & `mirascope-0.9.0/mirascope/cli/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/enums.py` & `mirascope-0.9.0/mirascope/enums.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/gemini/calls.py` & `mirascope-0.9.0/mirascope/gemini/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/gemini/extractors.py` & `mirascope-0.9.0/mirascope/gemini/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/gemini/tools.py` & `mirascope-0.9.0/mirascope/gemini/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/gemini/types.py` & `mirascope-0.9.0/mirascope/gemini/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/mistral/calls.py` & `mirascope-0.9.0/mirascope/mistral/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/mistral/extractors.py` & `mirascope-0.9.0/mirascope/mistral/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/mistral/tools.py` & `mirascope-0.9.0/mirascope/mistral/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,19 +105,19 @@
             raise ValueError() from e
 
         model_json["tool_call"] = tool_call
         return cls.model_validate(model_json)
 
     @classmethod
     def from_model(cls, model: Type[BaseModel]) -> Type[MistralTool]:
-        """Constructs a `OpenAITool` type from a `BaseModel` type."""
+        """Constructs a `MistralTool` type from a `BaseModel` type."""
         return convert_base_model_to_tool(model, MistralTool)
 
     @classmethod
     def from_fn(cls, fn: Callable) -> Type[MistralTool]:
-        """Constructs a `OpenAITool` type from a function."""
+        """Constructs a `MistralTool` type from a function."""
         return convert_function_to_tool(fn, MistralTool)
 
     @classmethod
     def from_base_type(cls, base_type: Type[BaseTypeT]) -> Type[MistralTool]:
         """Constructs a `MistralTool` type from a `BaseType` type."""
         return convert_base_type_to_tool(base_type, MistralTool)
```

### Comparing `mirascope-0.8.4/mirascope/mistral/types.py` & `mirascope-0.9.0/mirascope/mistral/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/openai/calls.py` & `mirascope-0.9.0/mirascope/openai/calls.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,22 +90,21 @@
         messages = self._update_messages_if_json(self.messages(), tool_types)
         start_time = datetime.datetime.now().timestamp() * 1000
         completion = client.chat.completions.create(
             messages=messages,
             stream=False,
             **kwargs,
         )
-        openai_call_response = OpenAICallResponse(
+        return OpenAICallResponse(
             response=completion,
             tool_types=tool_types,
             start_time=start_time,
             end_time=datetime.datetime.now().timestamp() * 1000,
+            response_format=self.call_params.response_format,
         )
-        openai_call_response.response_format = self.call_params.response_format
-        return openai_call_response
 
     async def call_async(self, **kwargs: Any) -> OpenAICallResponse:
         """Makes an asynchronous call to the model using this `OpenAICall`.
 
         Args:
             **kwargs: Additional keyword arguments parameters to pass to the call. These
                 will override any existing arguments in `call_params`.
@@ -113,33 +112,32 @@
         Returns:
             An `OpenAICallResponse` instance.
 
         Raises:
             OpenAIError: raises any OpenAI errors, see:
                 https://platform.openai.com/docs/guides/error-codes/api-errors
         """
-        kwargs, tool_types = self._setup(kwargs, OpenAITool)
+        kwargs, tool_types = self._setup_openai_kwargs(kwargs)
         client = AsyncOpenAI(api_key=self.api_key, base_url=self.base_url)
         if self.call_params.wrapper_async is not None:
             client = self.call_params.wrapper_async(client)
         messages = self._update_messages_if_json(self.messages(), tool_types)
         start_time = datetime.datetime.now().timestamp() * 1000
         completion = await client.chat.completions.create(
             messages=messages,
             stream=False,
             **kwargs,
         )
-        openai_call_response = OpenAICallResponse(
+        return OpenAICallResponse(
             response=completion,
             tool_types=tool_types,
             start_time=start_time,
             end_time=datetime.datetime.now().timestamp() * 1000,
+            response_format=self.call_params.response_format,
         )
-        openai_call_response.response_format = self.call_params.response_format
-        return openai_call_response
 
     def stream(self, **kwargs: Any) -> Generator[OpenAICallResponseChunk, None, None]:
         """Streams the response for a call using this `OpenAICall`.
 
         Args:
             **kwargs: Additional keyword arguments parameters to pass to the call. These
                 will override any existing arguments in `call_params`.
@@ -147,32 +145,30 @@
         Yields:
             A `OpenAICallResponseChunk` for each chunk of the response.
 
         Raises:
             OpenAIError: raises any OpenAI errors, see:
                 https://platform.openai.com/docs/guides/error-codes/api-errors
         """
-        kwargs, tool_types = self._setup(kwargs, OpenAITool)
+        kwargs, tool_types = self._setup_openai_kwargs(kwargs)
         client = OpenAI(api_key=self.api_key, base_url=self.base_url)
         if self.call_params.wrapper is not None:
             client = self.call_params.wrapper(client)
         messages = self._update_messages_if_json(self.messages(), tool_types)
         stream = client.chat.completions.create(
             messages=messages,
             stream=True,
             **kwargs,
         )
         for chunk in stream:
-            openai_call_response_chunk = OpenAICallResponseChunk(
-                chunk=chunk, tool_types=tool_types
+            yield OpenAICallResponseChunk(
+                chunk=chunk,
+                tool_types=tool_types,
+                response_format=self.call_params.response_format,
             )
-            openai_call_response_chunk.response_format = (
-                self.call_params.response_format
-            )
-            yield openai_call_response_chunk
 
     async def stream_async(
         self, **kwargs: Any
     ) -> AsyncGenerator[OpenAICallResponseChunk, None]:
         """Streams the response for an asynchronous call using this `OpenAICall`.
 
         Args:
@@ -182,32 +178,30 @@
         Yields:
             A `OpenAICallResponseChunk` for each chunk of the response.
 
         Raises:
             OpenAIError: raises any OpenAI errors, see:
                 https://platform.openai.com/docs/guides/error-codes/api-errors
         """
-        kwargs, tool_types = self._setup(kwargs, OpenAITool)
+        kwargs, tool_types = self._setup_openai_kwargs(kwargs)
         client = AsyncOpenAI(api_key=self.api_key, base_url=self.base_url)
         if self.call_params.wrapper_async is not None:
             client = self.call_params.wrapper_async(client)
         messages = self._update_messages_if_json(self.messages(), tool_types)
         stream = await client.chat.completions.create(
             messages=messages,
             stream=True,
             **kwargs,
         )
         async for chunk in stream:
-            openai_call_response_chunk = OpenAICallResponseChunk(
-                chunk=chunk, tool_types=tool_types
-            )
-            openai_call_response_chunk.response_format = (
-                self.call_params.response_format
+            yield OpenAICallResponseChunk(
+                chunk=chunk,
+                tool_types=tool_types,
+                response_format=self.call_params.response_format,
             )
-            yield openai_call_response_chunk
 
     ############################## PRIVATE METHODS ###################################
 
     def _setup_openai_kwargs(
         self,
         kwargs: dict[str, Any],
     ) -> tuple[
```

### Comparing `mirascope-0.8.4/mirascope/openai/extractors.py` & `mirascope-0.9.0/mirascope/openai/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/openai/tools.py` & `mirascope-0.9.0/mirascope/openai/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/openai/types.py` & `mirascope-0.9.0/mirascope/openai/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/wandb/wandb.py` & `mirascope-0.9.0/mirascope/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/mirascope/wandb/weave.py` & `mirascope-0.9.0/mirascope/wandb/weave.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.8.4/pyproject.toml` & `mirascope-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mirascope"
-version = "0.8.4"
+version = "0.9.0"
 description = "LLM toolkit for lightning-fast, high-quality development"
 license = "MIT"
 authors = [
     "William Bakst <william@mirascope.io>",
     "Brendan Kao <brendan@mirascope.io>",
 ]
 readme = "docs/README.md"
@@ -24,22 +24,31 @@
 
 # A list of optional dependencies that are required for certain features
 wandb = { version = "^0.16.4", optional = true }
 weave = { version = "^0.50.0", optional = true }
 google-generativeai = { version = "^0.4.0", optional = true }
 anthropic = { version = "^0.23.1", optional = true }
 mistralai = { version = "^0.1.6", optional = true }
+groq = { version = "^0.4.2", optional = true }
 
 [tool.poetry.extras]
 wandb = ["wandb"]
 weave = ["weave"]
 gemini = ["google-generativeai"]
 anthropic = ["anthropic"]
 mistral = ["mistralai"]
-all = ["wandb", "weave", "google-generativeai", "anthropic", "mistralai"]
+groq = ["groq"]
+all = [
+    "wandb",
+    "weave",
+    "google-generativeai",
+    "anthropic",
+    "mistralai",
+    "groq",
+]
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.6.1"
 pytest = "^7.4.0"
 ruff = "^0.1.5"
 pytest-asyncio = "^0.23.3"
 pytest-cov = "^4.1.0"
```

### Comparing `mirascope-0.8.4/PKG-INFO` & `mirascope-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirascope
-Version: 0.8.4
+Version: 0.9.0
 Summary: LLM toolkit for lightning-fast, high-quality development
 Home-page: https://github.com/Mirascope/mirascope
 License: MIT
 Author: William Bakst
 Author-email: william@mirascope.io
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -12,21 +12,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
 Provides-Extra: anthropic
 Provides-Extra: gemini
+Provides-Extra: groq
 Provides-Extra: mistral
 Provides-Extra: wandb
 Provides-Extra: weave
 Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: anthropic (>=0.23.1,<0.24.0) ; extra == "anthropic" or extra == "all"
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: google-generativeai (>=0.4.0,<0.5.0) ; extra == "gemini" or extra == "all"
+Requires-Dist: groq (>=0.4.2,<0.5.0) ; extra == "groq" or extra == "all"
 Requires-Dist: mistralai (>=0.1.6,<0.2.0) ; extra == "mistral" or extra == "all"
 Requires-Dist: openai (>=1.6.0,<2.0.0)
 Requires-Dist: pydantic (>=2.0.2,<3.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: wandb (>=0.16.4,<0.17.0) ; extra == "wandb" or extra == "all"
 Requires-Dist: weave (>=0.50.0,<0.51.0) ; extra == "weave" or extra == "all"
 Project-URL: Repository, https://github.com/Mirascope/mirascope
@@ -322,29 +324,34 @@
 def root(book_recommender: BookRecommender) -> Book:
     """Generates a book based on provided `genre`."""
     return book_recommender.extract()
 ```
 
 ## Roadmap
 
-- [x]  Extracting structured information using LLMs
+- [X]  Extracting structured information using LLMs
+- [ ]  RAG
+- [ ]  Agents
 - [ ]  Streaming extraction for tools (function calling)
 - [ ]  Additional template parsing for more complex messages
-    - [x]  Chat History
+    - [X]  Chat History
+    - [ ]  Better Tool Messages
     - [ ]  Additional Metadata
     - [ ]  Vision
-- [ ]  RAG
-- [ ]  Agents
 - [ ]  Support for more LLM providers:
-    - [X]  Anthropic Function Calling
-    - [ ]  Mistral
+    - [X]  Anthropic
+    - [X]  Gemini
+    - [X]  Mistral
+    - [X]  Groq
+    - [ ]  Cohere
     - [ ]  HuggingFace
 - [ ]  Integrations
-    - [x]  Weights & Biases
-    - [x]  LangChain / LangSmith
+    - [X]  Weights & Biases Trace
+    - [X]  Weave by Weights & Biases
+    - [X]  LangChain / LangSmith
     - [ ]  … tell us what you’d like integrated!
 - [ ]  Evaluating prompts and their quality by version
 
 ## Versioning
 
 Mirascope uses [Semantic Versioning](https://semver.org/).
```

