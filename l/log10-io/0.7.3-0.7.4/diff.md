# Comparing `tmp/log10_io-0.7.3.tar.gz` & `tmp/log10_io-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.7.3.tar", max compression
+gzip compressed data, was "log10_io-0.7.4.tar", max compression
```

## Comparing `log10_io-0.7.3.tar` & `log10_io-0.7.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1083 2024-03-29 16:46:58.521744 log10_io-0.7.3/LICENSE
--rw-r--r--   0        0        0     8934 2024-03-29 16:46:58.521744 log10_io-0.7.3/README.md
--rw-r--r--   0        0        0        0 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/__init__.py
--rw-r--r--   0        0        0     1470 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/__main__.py
--rw-r--r--   0        0        0     9386 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/_httpx_utils.py
--rw-r--r--   0        0        0     9112 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/agents/camel.py
--rw-r--r--   0        0        0      722 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     6079 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/anthropic.py
--rw-r--r--   0        0        0     2578 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/bigquery.py
--rw-r--r--   0        0        0     9532 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/completions/completions.py
--rw-r--r--   0        0        0     2648 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/evals.py
--rw-r--r--   0        0        0     5399 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/feedback/_summary_feedback_utils.py
--rw-r--r--   0        0        0     4153 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/feedback/autofeedback.py
--rw-r--r--   0        0        0     8359 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/feedback/feedback.py
--rw-r--r--   0        0        0     4880 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/feedback/feedback_task.py
--rw-r--r--   0        0        0     9274 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/langchain.py
--rw-r--r--   0        0        0     7967 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/llm.py
--rw-r--r--   0        0        0    34415 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/load.py
--rw-r--r--   0        0        0     2886 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/mosaicml.py
--rw-r--r--   0        0        0     3217 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/openai.py
--rw-r--r--   0        0        0     5343 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/prompt_analyzer.py
--rw-r--r--   0        0        0     1020 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2654 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/together.py
--rw-r--r--   0        0        0     2101 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/tools.py
--rw-r--r--   0        0        0     1211 2024-03-29 16:46:58.525745 log10_io-0.7.3/log10/utils.py
--rw-r--r--   0        0        0     2087 2024-03-29 16:46:58.525745 log10_io-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    10234 1970-01-01 00:00:00.000000 log10_io-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-05 23:28:11.370088 log10_io-0.7.4/LICENSE
+-rw-r--r--   0        0        0     8934 2024-04-05 23:28:11.370088 log10_io-0.7.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/__init__.py
+-rw-r--r--   0        0        0     1470 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/__main__.py
+-rw-r--r--   0        0        0     9386 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/_httpx_utils.py
+-rw-r--r--   0        0        0     9112 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/agents/camel.py
+-rw-r--r--   0        0        0      722 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     6079 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/anthropic.py
+-rw-r--r--   0        0        0     2578 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/bigquery.py
+-rw-r--r--   0        0        0     9532 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/completions/completions.py
+-rw-r--r--   0        0        0     2648 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/evals.py
+-rw-r--r--   0        0        0     5399 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/feedback/_summary_feedback_utils.py
+-rw-r--r--   0        0        0     4153 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/feedback/autofeedback.py
+-rw-r--r--   0        0        0     8357 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/feedback/feedback.py
+-rw-r--r--   0        0        0     4880 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/feedback/feedback_task.py
+-rw-r--r--   0        0        0     9274 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/langchain.py
+-rw-r--r--   0        0        0     4296 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/litellm.py
+-rw-r--r--   0        0        0     7967 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/llm.py
+-rw-r--r--   0        0        0    35836 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/load.py
+-rw-r--r--   0        0        0     2886 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/mosaicml.py
+-rw-r--r--   0        0        0     3217 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/openai.py
+-rw-r--r--   0        0        0     5343 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/prompt_analyzer.py
+-rw-r--r--   0        0        0     1020 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2654 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/together.py
+-rw-r--r--   0        0        0     2101 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/tools.py
+-rw-r--r--   0        0        0     1211 2024-04-05 23:28:11.374088 log10_io-0.7.4/log10/utils.py
+-rw-r--r--   0        0        0     2180 2024-04-05 23:28:11.378088 log10_io-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0    10363 1970-01-01 00:00:00.000000 log10_io-0.7.4/PKG-INFO
```

### Comparing `log10_io-0.7.3/LICENSE` & `log10_io-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/README.md` & `log10_io-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/__main__.py` & `log10_io-0.7.4/log10/__main__.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/_httpx_utils.py` & `log10_io-0.7.4/log10/_httpx_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/agents/camel.py` & `log10_io-0.7.4/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/agents/scrape_summarizer.py` & `log10_io-0.7.4/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/anthropic.py` & `log10_io-0.7.4/log10/anthropic.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/bigquery.py` & `log10_io-0.7.4/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/completions/completions.py` & `log10_io-0.7.4/log10/completions/completions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/evals.py` & `log10_io-0.7.4/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/feedback/_summary_feedback_utils.py` & `log10_io-0.7.4/log10/feedback/_summary_feedback_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/feedback/autofeedback.py` & `log10_io-0.7.4/log10/feedback/autofeedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/feedback/feedback.py` & `log10_io-0.7.4/log10/feedback/feedback.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             "json_values": values,
             "completion_tags_selector": completion_tags_selector,
             "comment": comment,
         }
         res = self._post_request(self.feedback_create_url, json_payload)
         return res
 
-    def list(self, offset: int = 0, limit: int = 50, task_id: str = None) -> httpx.Response:
+    def list(self, offset: int = 0, limit: int = 50, task_id: str = "") -> httpx.Response:
         base_url = self._log10_config.url
         api_url = "/api/v1/feedback"
         url = f"{base_url}{api_url}?organization_id={self._log10_config.org_id}&offset={offset}&limit={limit}&task_id={task_id}"
 
         # GET feedback
         try:
             res = self._http_client.get(url=url)
```

### Comparing `log10_io-0.7.3/log10/feedback/feedback_task.py` & `log10_io-0.7.4/log10/feedback/feedback_task.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/langchain.py` & `log10_io-0.7.4/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/llm.py` & `log10_io-0.7.4/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/load.py` & `log10_io-0.7.4/log10/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,29 +279,38 @@
         self.final_result = ""  # Store the final result
         self.function_name = ""
         self.function_arguments = ""
         self.start_time = time.perf_counter()
         self.gpt_id = None
         self.model = None
         self.finish_reason = None
+        self.usage = None
 
     def __iter__(self):
         return self
 
     def __next__(self):
         try:
             chunk = next(self.response)
-            if chunk.choices[0].delta.content:
+            if hasattr(chunk.choices[0].delta, "content") and chunk.choices[0].delta.content is not None:
                 # Here you can intercept and modify content if needed
                 content = chunk.choices[0].delta.content
                 self.final_result += content  # Save the content
                 # Yield the original or modified content
 
                 self.model = chunk.model
                 self.gpt_id = chunk.id
+
+                # for mistral stream
+                if chunk.choices[0].finish_reason:
+                    self.finish_reason = chunk.choices[0].finish_reason
+
+                # for mistral stream
+                if getattr(chunk, "usage", None):
+                    self.usage = chunk.usage
             elif chunk.choices[0].delta.function_call:
                 arguments = chunk.choices[0].delta.function_call.arguments
                 self.function_arguments += arguments
                 if not self.function_name and chunk.choices[0].delta.function_call.name:
                     self.function_name = chunk.choices[0].delta.function_call.name
             else:
                 self.finish_reason = chunk.choices[0].finish_reason
@@ -338,14 +347,16 @@
                             "function_call": {
                                 "name": self.function_name,
                                 "arguments": self.function_arguments,
                             },
                         }
                     ],
                 }
+            if self.usage:
+                response["usage"] = self.usage.dict()
             self.partial_log_row["response"] = json.dumps(response)
             self.partial_log_row["duration"] = int((time.perf_counter() - self.start_time) * 1000)
 
             try:
                 res = post_request(self.completion_url + "/" + self.completionID, self.partial_log_row)
                 if res.status_code != 200:
                     logger.error(f"LOG10: failed to insert in log10: {self.partial_log_row} with error {res.text}")
@@ -508,17 +519,20 @@
             if kwargs_copy.get("generation_config"):
                 for key, value in kwargs_copy["generation_config"].to_dict().items():
                     if key == "max_output_tokens":
                         kwargs_copy["max_tokens"] = value
                     else:
                         kwargs_copy[key] = value
                 kwargs_copy.pop("generation_config")
+    elif "mistralai" in func.__module__:
+        log_row["kind"] = "chat"
     elif "openai" in func.__module__:
         kind = "chat" if "chat" in func.__module__ else "completion"
         log_row["kind"] = kind
+
     log_row["request"] = json.dumps(kwargs_copy)
 
     return log_row
 
 
 def intercepting_decorator(func):
     @functools.wraps(func)
@@ -632,18 +646,29 @@
                         log_row["status"] = "finished"
                         return StreamingResponseWrapper(
                             completion_url=completion_url,
                             completionID=completionID,
                             response=response,
                             partial_log_row=log_row,
                         )
-                    response = output
+                    response = output.copy()
 
                     if "choices" in response:
                         response = flatten_response(response)
+                elif "mistralai" in func.__module__:
+                    if "stream" in func.__qualname__:
+                        log_row["response"] = response
+                        log_row["status"] = "finished"
+                        return StreamingResponseWrapper(
+                            completion_url=completion_url,
+                            completionID=completionID,
+                            response=response,
+                            partial_log_row=log_row,
+                        )
+                    response = output.copy()
 
                 if hasattr(response, "model_dump_json"):
                     response = response.model_dump_json()
                 else:
                     response = json.dumps(response)
 
                 log_row["status"] = "finished"
@@ -685,15 +710,15 @@
 
 def set_sync_log_text(USE_ASYNC=True):
     return "async" if USE_ASYNC else "sync"
 
 
 def log10(module, DEBUG_=False, USE_ASYNC_=True):
     """Intercept and overload module for logging purposes
-    support both openai V0 and V1, and anthropic
+    support both openai V0 and V1, anthropic, vertexai, and mistralai
 
     Keyword arguments:
     module -- the module to be intercepted (e.g. openai)
     DEBUG_ -- whether to show log10 related debug statements via python logging (default False)
     USE_ASYNC_ -- whether to run in async mode (default True)
 
     Openai V0 example:
@@ -795,14 +820,21 @@
         method = getattr(attr, "create")
         setattr(attr, "create", intercepting_decorator(method))
 
         # anthropic Messages completion
         attr = module.resources.messages.Messages
         method = getattr(attr, "create")
         setattr(attr, "create", intercepting_decorator(method))
+    if module.__name__ == "mistralai":
+        attr = module.client.MistralClient
+        method = getattr(attr, "chat")
+        setattr(attr, "chat", intercepting_decorator(method))
+
+        method = getattr(attr, "chat_stream")
+        setattr(attr, "chat_stream", intercepting_decorator(method))
     elif module.__name__ == "openai":
         openai_version = parse(version("openai"))
         global OPENAI_V1
         OPENAI_V1 = openai_version >= parse("1.0.0")
 
         # support for sync completions
         if OPENAI_V1:
```

### Comparing `log10_io-0.7.3/log10/mosaicml.py` & `log10_io-0.7.4/log10/mosaicml.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/openai.py` & `log10_io-0.7.4/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/prompt_analyzer.py` & `log10_io-0.7.4/log10/prompt_analyzer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/schemas/bigquery.json` & `log10_io-0.7.4/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/together.py` & `log10_io-0.7.4/log10/together.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/tools.py` & `log10_io-0.7.4/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/log10/utils.py` & `log10_io-0.7.4/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.7.3/pyproject.toml` & `log10_io-0.7.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.7.3"
+version = "0.7.4"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -46,19 +46,22 @@
 wikipedia = "^1.4.0"
 faker = "^19.2.0"
 backoff = "^2.2.1"
 anthropic = "<1"
 mosaicml-cli = "^0.5.30"
 together = "^0.2.7"
 google-cloud-aiplatform = ">=1.44.0"
+mistralai = "^0.1.5"
 
 magentic = {version = ">=0.17.0", optional = true, markers = "python_version >= '3.10'"}
+litellm = {version = "^1.34.18", optional = true}
 
 [tool.poetry.extras]
 autofeedback_icl = ["magentic"]
+litellm = ["litellm"]
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
 lint.ignore = ["C901", "E501", "E741", "F402", "F823" ]
 lint.select = ["C", "E", "F", "I", "W"]
 line-length = 119
```

### Comparing `log10_io-0.7.3/PKG-INFO` & `log10_io-0.7.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.7.3
+Version: 0.7.4
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: autofeedback-icl
+Provides-Extra: litellm
 Requires-Dist: anthropic (<1)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
 Requires-Dist: faker (>=19.2.0,<20.0.0)
 Requires-Dist: google-cloud-aiplatform (>=1.44.0)
 Requires-Dist: google-cloud-bigquery (>=3.11.4,<4.0.0)
 Requires-Dist: google-search-results (>=2.4.2,<3.0.0)
 Requires-Dist: langchain (<0.2.0)
+Requires-Dist: litellm (>=1.34.18,<2.0.0) ; extra == "litellm"
 Requires-Dist: magentic (>=0.17.0) ; (python_version >= "3.10") and (extra == "autofeedback-icl")
+Requires-Dist: mistralai (>=0.1.5,<0.2.0)
 Requires-Dist: mosaicml-cli (>=0.5.30,<0.6.0)
 Requires-Dist: openai (<2)
 Requires-Dist: pexpect (>=4.8.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: together (>=0.2.7,<0.3.0)
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
```

