# Comparing `tmp/athina_logger-1.1.0.tar.gz` & `tmp/athina_logger-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athina_logger-1.1.0.tar", max compression
+gzip compressed data, was "athina_logger-1.2.0.tar", max compression
```

## Comparing `athina_logger-1.1.0.tar` & `athina_logger-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     6103 2024-03-20 17:09:51.913295 athina_logger-1.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.913405 athina_logger-1.1.0/athina_logger/__init__.py
--rw-r--r--   0        0        0      244 2024-03-20 17:09:51.913523 athina_logger-1.1.0/athina_logger/api_key.py
--rw-r--r--   0        0        0      579 2024-03-20 17:09:51.913654 athina_logger-1.1.0/athina_logger/athina_meta.py
--rw-r--r--   0        0        0      346 2024-03-26 18:25:24.303825 athina_logger-1.1.0/athina_logger/constants.py
--rw-r--r--   0        0        0      210 2024-03-20 17:09:51.913916 athina_logger-1.1.0/athina_logger/exception/custom_exception.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914025 athina_logger-1.1.0/athina_logger/feedback/__init__.py
--rw-r--r--   0        0        0     1127 2024-03-20 17:09:51.914195 athina_logger-1.1.0/athina_logger/feedback/user_feedback.py
--rw-r--r--   0        0        0     4081 2024-03-20 17:09:51.914318 athina_logger-1.1.0/athina_logger/inference_logger.py
--rw-r--r--   0        0        0    14226 2024-03-20 17:11:17.685407 athina_logger-1.1.0/athina_logger/langchain_handler.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914553 athina_logger-1.1.0/athina_logger/log_stream_inference/__init__.py
--rw-r--r--   0        0        0     4471 2024-03-20 17:09:51.914716 athina_logger-1.1.0/athina_logger/log_stream_inference/log_stream_inference.py
--rw-r--r--   0        0        0     7377 2024-03-20 17:09:51.914858 athina_logger-1.1.0/athina_logger/log_stream_inference/openai_chat_completion_stream.py
--rw-r--r--   0        0        0     6703 2024-03-20 17:09:51.914999 athina_logger-1.1.0/athina_logger/log_stream_inference/openai_completion_stream.py
--rw-r--r--   0        0        0    10539 2024-03-26 17:19:28.304716 athina_logger-1.1.0/athina_logger/openai_wrapper.py
--rw-r--r--   0        0        0     1883 2024-03-26 17:48:02.077627 athina_logger-1.1.0/athina_logger/request_helper.py
--rw-r--r--   0        0        0        0 2024-03-26 17:19:28.304911 athina_logger-1.1.0/athina_logger/tracing/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 17:19:28.305006 athina_logger-1.1.0/athina_logger/tracing/callback/__init__.py
--rw-r--r--   0        0        0    20259 2024-03-26 18:24:37.156796 athina_logger-1.1.0/athina_logger/tracing/callback/langchain.py
--rw-r--r--   0        0        0      755 2024-03-26 17:19:28.305239 athina_logger-1.1.0/athina_logger/tracing/models.py
--rw-r--r--   0        0        0    13693 2024-03-26 17:19:28.305359 athina_logger-1.1.0/athina_logger/tracing/span.py
--rw-r--r--   0        0        0     6759 2024-03-26 17:19:28.305462 athina_logger-1.1.0/athina_logger/tracing/trace.py
--rw-r--r--   0        0        0      260 2024-03-26 17:19:28.305535 athina_logger-1.1.0/athina_logger/tracing/util.py
--rw-r--r--   0        0        0        0 2024-03-20 17:09:51.915369 athina_logger-1.1.0/athina_logger/util/__init__.py
--rw-r--r--   0        0        0    10414 2024-03-20 17:11:17.685568 athina_logger-1.1.0/athina_logger/util/extract_model.py
--rw-r--r--   0        0        0     3259 2024-03-20 17:09:51.915502 athina_logger-1.1.0/athina_logger/util/token_count_helper.py
--rw-r--r--   0        0        0      465 2024-03-26 18:26:33.756230 athina_logger-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 athina_logger-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6103 2024-03-20 17:09:51.913295 athina_logger-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.913405 athina_logger-1.2.0/athina_logger/__init__.py
+-rw-r--r--   0        0        0      244 2024-03-20 17:09:51.913523 athina_logger-1.2.0/athina_logger/api_key.py
+-rw-r--r--   0        0        0      626 2024-04-06 02:19:19.299377 athina_logger-1.2.0/athina_logger/athina_meta.py
+-rw-r--r--   0        0        0      346 2024-04-06 02:20:32.526115 athina_logger-1.2.0/athina_logger/constants.py
+-rw-r--r--   0        0        0      210 2024-03-20 17:09:51.913916 athina_logger-1.2.0/athina_logger/exception/custom_exception.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914025 athina_logger-1.2.0/athina_logger/feedback/__init__.py
+-rw-r--r--   0        0        0     1127 2024-03-20 17:09:51.914195 athina_logger-1.2.0/athina_logger/feedback/user_feedback.py
+-rw-r--r--   0        0        0     4235 2024-04-06 02:19:19.299809 athina_logger-1.2.0/athina_logger/inference_logger.py
+-rw-r--r--   0        0        0    14226 2024-04-02 05:37:10.002663 athina_logger-1.2.0/athina_logger/langchain_handler.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.914553 athina_logger-1.2.0/athina_logger/log_stream_inference/__init__.py
+-rw-r--r--   0        0        0     4943 2024-04-06 02:19:19.299987 athina_logger-1.2.0/athina_logger/log_stream_inference/log_stream_inference.py
+-rw-r--r--   0        0        0     7678 2024-04-06 02:19:19.300143 athina_logger-1.2.0/athina_logger/log_stream_inference/openai_chat_completion_stream.py
+-rw-r--r--   0        0        0     7004 2024-04-06 02:19:19.300276 athina_logger-1.2.0/athina_logger/log_stream_inference/openai_completion_stream.py
+-rw-r--r--   0        0        0    10771 2024-04-06 02:19:19.300668 athina_logger-1.2.0/athina_logger/openai_wrapper.py
+-rw-r--r--   0        0        0     1883 2024-03-31 23:05:11.799630 athina_logger-1.2.0/athina_logger/request_helper.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:30:00.376453 athina_logger-1.2.0/athina_logger/tracing/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 22:30:00.406928 athina_logger-1.2.0/athina_logger/tracing/callback/__init__.py
+-rw-r--r--   0        0        0    20259 2024-03-31 23:08:32.644755 athina_logger-1.2.0/athina_logger/tracing/callback/langchain.py
+-rw-r--r--   0        0        0      755 2024-03-31 22:30:00.403809 athina_logger-1.2.0/athina_logger/tracing/models.py
+-rw-r--r--   0        0        0    14103 2024-04-06 02:19:19.300937 athina_logger-1.2.0/athina_logger/tracing/span.py
+-rw-r--r--   0        0        0     6864 2024-04-06 02:19:19.301218 athina_logger-1.2.0/athina_logger/tracing/trace.py
+-rw-r--r--   0        0        0      260 2024-03-31 22:30:00.379971 athina_logger-1.2.0/athina_logger/tracing/util.py
+-rw-r--r--   0        0        0        0 2024-03-20 17:09:51.915369 athina_logger-1.2.0/athina_logger/util/__init__.py
+-rw-r--r--   0        0        0    10414 2024-03-31 22:30:00.357924 athina_logger-1.2.0/athina_logger/util/extract_model.py
+-rw-r--r--   0        0        0     3259 2024-03-20 17:09:51.915502 athina_logger-1.2.0/athina_logger/util/token_count_helper.py
+-rw-r--r--   0        0        0      465 2024-04-06 02:19:46.556941 athina_logger-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6725 1970-01-01 00:00:00.000000 athina_logger-1.2.0/PKG-INFO
```

### Comparing `athina_logger-1.1.0/README.md` & `athina_logger-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `athina_logger-1.1.0/athina_logger/athina_meta.py` & `athina_logger-1.2.0/athina_logger/athina_meta.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,7 +12,8 @@
     user_query: Optional[dict] = None
     environment: Optional[dict] = None
     external_reference_id: Optional[dict] = None
     customer_id: Optional[str] = None
     customer_user_id: Optional[str] = None
     response_time: Optional[int] = None
     custom_attributes: Optional[dict] = None
+    custom_eval_metrics: Optional[dict] = None
```

### Comparing `athina_logger-1.1.0/athina_logger/feedback/user_feedback.py` & `athina_logger-1.2.0/athina_logger/feedback/user_feedback.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.1.0/athina_logger/inference_logger.py` & `athina_logger-1.2.0/athina_logger/inference_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,26 @@
         prompt_tokens: Optional[int] = None,
         completion_tokens: Optional[int] = None,
         total_tokens: Optional[int] = None,
         response_time: Optional[int] = None,
         context: Optional[Dict] = None,
         expected_response: Optional[str] = None,
         custom_attributes: Optional[Dict] = None,
+        custom_eval_metrics: Optional[Dict] = None,
         cost: Optional[float] = None,
     ) -> None:
         try:
-            args = (prompt, response, prompt_slug, language_model_id, environment, functions, function_call_response, tools, tool_calls, external_reference_id, customer_id, customer_user_id, session_id, user_query, prompt_tokens, completion_tokens, total_tokens, response_time, context, expected_response, custom_attributes, cost)
+            args = (prompt, response, prompt_slug, language_model_id, environment, functions, function_call_response, tools, tool_calls, external_reference_id, customer_id, customer_user_id, session_id, user_query, prompt_tokens, completion_tokens, total_tokens, response_time, context, expected_response, custom_attributes, cost, custom_eval_metrics)
             threading.Thread(target=lambda: asyncio.run(InferenceLogger._log_inference_asynchronously(*args))).start()
         except Exception as e:
             print("Error in logging inference to Athina: ", str(e))
 
     @staticmethod
     async def _log_inference_asynchronously(
-        prompt, response, prompt_slug, language_model_id, environment, functions, function_call_response, tools, tool_calls, external_reference_id, customer_id, customer_user_id, session_id, user_query, prompt_tokens, completion_tokens, total_tokens, response_time, context, expected_response, custom_attributes, cost
+        prompt, response, prompt_slug, language_model_id, environment, functions, function_call_response, tools, tool_calls, external_reference_id, customer_id, customer_user_id, session_id, user_query, prompt_tokens, completion_tokens, total_tokens, response_time, context, expected_response, custom_attributes, cost, custom_eval_metrics
     ) -> None:
         """
         logs the llm inference to athina
         """
         try:
             payload = {
                 'prompt': prompt,
@@ -65,14 +66,15 @@
                 'user_query': str(user_query) if user_query is not None else None,
                 'external_reference_id': str(external_reference_id) if external_reference_id is not None else None,
                 'prompt_tokens': prompt_tokens,
                 'completion_tokens': completion_tokens,
                 'total_tokens': total_tokens,
                 'expected_response': expected_response,
                 'custom_attributes': custom_attributes,
+                'custom_eval_metrics': custom_eval_metrics,
                 'cost': cost,
             }
             # Remove None fields from the payload
             payload = {k: v for k, v in payload.items() if v is not None}
             RequestHelper.make_post_request(endpoint=f'{API_BASE_URL}/api/v1/log/inference', payload=payload, headers={
                 'athina-api-key': InferenceLogger.get_api_key(),
             })
```

### Comparing `athina_logger-1.1.0/athina_logger/langchain_handler.py` & `athina_logger-1.2.0/athina_logger/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.1.0/athina_logger/log_stream_inference/log_stream_inference.py` & `athina_logger-1.2.0/athina_logger/log_stream_inference/log_stream_inference.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,38 +13,42 @@
                  context: Optional[Dict] = None,
                  environment: Optional[str] = 'production',
                  customer_id: Optional[str] = None,
                  customer_user_id: Optional[str] = None,
                  session_id: Optional[str] = None,
                  user_query: Optional[str] = None,
                  external_reference_id: Optional[str] = None,
-                 custom_attributes: Optional[Dict] = None):
+                 custom_attributes: Optional[Dict] = None,
+                 custom_eval_metrics: Optional[Dict] = None
+                ):
         """
         constructor for log stream inference
         :param prompt_slug: str - The slug of the prompt used for the inference.
         :param response_time: Optional[int] - The response time in milliseconds. Defaults to None.
         :param context: Optional[Dict] - A dictionary containing additional context information. Defaults to None.
         :param environment: Optional[str] - The environment in which the inference occurred. Defaults to production.
         :param customer_id: Optional[str] - The customer's unique identifier. Defaults to None.
         :param customer_user_id: Optional[str] - The customer's user identifier. Defaults to None.
         :param session_id: Optional[str] - The session identifier. Defaults to None.
         :param user_query: Optional[str] - The user's query or input. Defaults to None.
         :param external_reference_id: Optional[str] - The external reference id. Defaults to None.
         :param custom_attributes: Optional[Dict] - A dictionary containing custom attributes. Defaults to None.
+        :param custom_eval_metrics: Optional[Dict] - A dictionary containing custom evaluation metrics. Defaults to None.
         """
         self._prompt_slug = prompt_slug
         self._response_time = response_time
         self._context = context
         self._environment = environment
         self._customer_id = customer_id
         self._customer_user_id = customer_user_id
         self._session_id = session_id
         self._user_query = user_query
         self._external_reference_id = external_reference_id
         self._custom_attributes = custom_attributes
+        self._custom_eval_metrics = custom_eval_metrics
 
     @property
     def prompt_slug(self):
         return self._prompt_slug
 
     @prompt_slug.setter
     def prompt_slug(self, value):
@@ -117,14 +121,22 @@
     @property
     def custom_attributes(self):
         return self._custom_attributes
 
     @custom_attributes.setter
     def custom_attributes(self, value):
         self._custom_attributes = value
+    
+    @property
+    def custom_eval_metrics(self):
+        return self._custom_eval_metrics
+    
+    @custom_eval_metrics.setter
+    def custom_eval_metrics(self, value):
+        self._custom_eval_metrics = value
 
     @abstractmethod
     def collect_stream_inference(self, response):
         """
         collects the inference from the log stream
         """
         pass
```

### Comparing `athina_logger-1.1.0/athina_logger/log_stream_inference/openai_chat_completion_stream.py` & `athina_logger-1.2.0/athina_logger/log_stream_inference/openai_completion_stream.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,116 +1,106 @@
 from typing import List, Optional, Dict, Any
-import tiktoken
 from ..constants import LOG_INFERENCE_URL
 from .log_stream_inference import LogStreamInference
 from ..api_key import AthinaApiKey
 from ..request_helper import RequestHelper
-from ..util.token_count_helper import get_prompt_tokens_openai_chat_completion, get_completion_tokens_openai_chat_completion
+from ..util.token_count_helper import get_token_usage_openai_completion
 
 
-class LogOpenAiChatCompletionStreamInference(LogStreamInference, AthinaApiKey):
+class LogOpenAiCompletionStreamInference(LogStreamInference, AthinaApiKey):
     def __init__(self,
                  prompt_slug: str,
-                 prompt: List[Dict[str, Any]],
+                 prompt: str,
                  language_model_id: str,
                  response_time: Optional[int] = None,
                  context: Optional[Dict] = None,
                  environment: Optional[str] = 'production',
                  customer_id: Optional[str] = None,
                  customer_user_id: Optional[str] = None,
                  session_id: Optional[str] = None,
                  user_query: Optional[str] = None,
                  external_reference_id: Optional[str] = None,
-                 custom_attributes: Optional[Dict] = None):
+                 custom_attributes: Optional[Dict] = None,
+                 custom_eval_metrics: Optional[Dict] = None):
         """
         constructor for log stream inference
         :param prompt_slug: str - The slug of the prompt used for the inference.
-        :param prompt: List[Dict[str, Any]] - The messages used for the inference.
+        :param prompt: str - The prompt used for the inference.
         :param language_model_id: str - The model used for the inference.
         :param response_time: Optional[int] - The response time in milliseconds. Defaults to None.
         :param context: Optional[Dict] - A dictionary containing additional context information. Defaults to None.
         :param environment: Optional[str] - The environment in which the inference occurred. Defaults to production.
         :param customer_id: Optional[str] - The customer's unique identifier. Defaults to None.
         :param customer_user_id: Optional[str] - The customer's user identifier. Defaults to None.
         :param session_id: Optional[str] - The session identifier. Defaults to None.
         :param user_query: Optional[str] - The user's query or input. Defaults to None.
         :param external_reference_id: Optional[str] - The external reference id. Defaults to None.
         :param custom_attributes: Optional[Dict] - A dictionary containing custom attributes. Defaults to None.
+        :param custom_eval_metrics: Optional[Dict] - A dictionary containing custom evaluation metrics. Defaults to None.
         """
         super().__init__(
             prompt_slug=prompt_slug,
             response_time=response_time,
             context=context,
             environment=environment,
             customer_id=customer_id,
             customer_user_id=customer_user_id,
             session_id=session_id,
             user_query=user_query,
             external_reference_id=external_reference_id,
-            custom_attributes=custom_attributes)
+            custom_attributes=custom_attributes,
+            custom_eval_metrics=custom_eval_metrics)
         self.prompt = prompt
         self.language_model_id = language_model_id
         self.response = ''
 
     def _get_text_from_stream_chunk(self, stream_chunk):
         """
         gets the text from the stream chunk
         """
         try:
             text = ''
-            choices = stream_chunk.get('choices', []) 
-            if choices and len(choices) > 0 and 'delta' in choices[0]:
-                delta = choices[0].get('delta', {})
-                if 'content' in delta and delta['content'] is not None:
-                    text = delta.get('content', '')
+            choices = stream_chunk.get('choices', [])
+            if choices and len(choices) > 0 and 'text' in choices[0]:
+                text = choices[0].get('text', {})
 
             return text
         except Exception as e:
             raise e
 
     def collect_stream_inference(self, response):
         """
         collects the inference from the log stream
         """
         try:
             for stream_chunk in response:
-                if isinstance(stream_chunk, dict):
-                    self.response += self._get_text_from_stream_chunk(
-                        stream_chunk)
-                else:
-                    self.response += self._get_text_from_stream_chunk(
-                        stream_chunk.model_dump())
+                self.response += self._get_text_from_stream_chunk(
+                    stream_chunk)
         except Exception as e:
             raise e
 
     def collect_stream_inference_by_chunk(self, stream_chunk):
         """
         collects the inference from the log stream of openai chat completion chunk by chunk
         """
         try:
-            if isinstance(stream_chunk, dict):
-                self.response += self._get_text_from_stream_chunk(
-                    stream_chunk)
-            else:
-                self.response += self._get_text_from_stream_chunk(
-                    stream_chunk.model_dump())
+            self.response += self._get_text_from_stream_chunk(
+                stream_chunk)
         except Exception as e:
             raise e
 
     def log_stream_inference(self):
         """
         logs the stream inference to the athina api server
         """
         try:
             prompt_tokens = self._get_prompt_tokens(
                 prompt=self.prompt, language_model_id=self.language_model_id)
-
             completion_tokens = self._get_completion_tokens(
                 response=self.response, language_model_id=self.language_model_id)
-
             if prompt_tokens is not None and completion_tokens is not None:
                 total_tokens = prompt_tokens + completion_tokens
             else:
                 total_tokens = None
             payload = {
                 'prompt_slug': self.prompt_slug,
                 'prompt': self.prompt,
@@ -124,37 +114,38 @@
                 'session_id': str(self.session_id) if self.session_id is not None else None,
                 'user_query': str(self.user_query) if self.user_query is not None else None,
                 'external_reference_id': str(self.external_reference_id) if self.external_reference_id is not None else None,
                 'prompt_tokens': prompt_tokens,
                 'completion_tokens': completion_tokens,
                 'total_tokens': total_tokens,
                 'custom_attributes': self.custom_attributes,
+                'custom_eval_metrics': self.custom_eval_metrics,
             }
             # Remove None fields from the payload
             payload = {k: v for k, v in payload.items() if v is not None}
             RequestHelper.make_post_request(endpoint=LOG_INFERENCE_URL, payload=payload, headers={
-                'athina-api-key': LogOpenAiChatCompletionStreamInference.get_api_key(),
+                'athina-api-key': LogOpenAiCompletionStreamInference.get_api_key(),
             })
         except Exception as e:
             raise e
 
-    def _get_prompt_tokens(self, prompt: List[Dict[str, Any]], language_model_id: str):
+    def _get_prompt_tokens(self, prompt: str, language_model_id: str):
         """
         gets the prompt tokens given the prompt for the openai chat model completion
         """
         try:
-            tokens = get_prompt_tokens_openai_chat_completion(
-                prompt=prompt, language_model_id=language_model_id)
+            tokens = get_token_usage_openai_completion(
+                text=prompt, language_model_id=language_model_id)
             return tokens
         except Exception as e:
             return None
 
     def _get_completion_tokens(self, response: str, language_model_id: str):
         """
         gets the completion tokens given the prompt response from the openai chat model completion
         """
         try:
-            tokens = get_completion_tokens_openai_chat_completion(
-                response=response, language_model_id=language_model_id)
+            tokens = get_token_usage_openai_completion(
+                text=response, language_model_id=language_model_id)
             return tokens
         except Exception as e:
             return None
```

### Comparing `athina_logger-1.1.0/athina_logger/log_stream_inference/openai_completion_stream.py` & `athina_logger-1.2.0/athina_logger/log_stream_inference/openai_chat_completion_stream.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,103 +1,119 @@
 from typing import List, Optional, Dict, Any
+import tiktoken
 from ..constants import LOG_INFERENCE_URL
 from .log_stream_inference import LogStreamInference
 from ..api_key import AthinaApiKey
 from ..request_helper import RequestHelper
-from ..util.token_count_helper import get_token_usage_openai_completion
+from ..util.token_count_helper import get_prompt_tokens_openai_chat_completion, get_completion_tokens_openai_chat_completion
 
 
-class LogOpenAiCompletionStreamInference(LogStreamInference, AthinaApiKey):
+class LogOpenAiChatCompletionStreamInference(LogStreamInference, AthinaApiKey):
     def __init__(self,
                  prompt_slug: str,
-                 prompt: str,
+                 prompt: List[Dict[str, Any]],
                  language_model_id: str,
                  response_time: Optional[int] = None,
                  context: Optional[Dict] = None,
                  environment: Optional[str] = 'production',
                  customer_id: Optional[str] = None,
                  customer_user_id: Optional[str] = None,
                  session_id: Optional[str] = None,
                  user_query: Optional[str] = None,
                  external_reference_id: Optional[str] = None,
-                 custom_attributes: Optional[Dict] = None):
+                 custom_attributes: Optional[Dict] = None,
+                 custom_eval_metrics: Optional[Dict] = None):
         """
         constructor for log stream inference
         :param prompt_slug: str - The slug of the prompt used for the inference.
-        :param prompt: str - The prompt used for the inference.
+        :param prompt: List[Dict[str, Any]] - The messages used for the inference.
         :param language_model_id: str - The model used for the inference.
         :param response_time: Optional[int] - The response time in milliseconds. Defaults to None.
         :param context: Optional[Dict] - A dictionary containing additional context information. Defaults to None.
         :param environment: Optional[str] - The environment in which the inference occurred. Defaults to production.
         :param customer_id: Optional[str] - The customer's unique identifier. Defaults to None.
         :param customer_user_id: Optional[str] - The customer's user identifier. Defaults to None.
         :param session_id: Optional[str] - The session identifier. Defaults to None.
         :param user_query: Optional[str] - The user's query or input. Defaults to None.
         :param external_reference_id: Optional[str] - The external reference id. Defaults to None.
         :param custom_attributes: Optional[Dict] - A dictionary containing custom attributes. Defaults to None.
+        :param custom_eval_metrics: Optional[Dict] - A dictionary containing custom evaluation metrics. Defaults to None.
         """
         super().__init__(
             prompt_slug=prompt_slug,
             response_time=response_time,
             context=context,
             environment=environment,
             customer_id=customer_id,
             customer_user_id=customer_user_id,
             session_id=session_id,
             user_query=user_query,
             external_reference_id=external_reference_id,
-            custom_attributes=custom_attributes)
+            custom_attributes=custom_attributes,
+            custom_eval_metrics=custom_eval_metrics)
         self.prompt = prompt
         self.language_model_id = language_model_id
         self.response = ''
 
     def _get_text_from_stream_chunk(self, stream_chunk):
         """
         gets the text from the stream chunk
         """
         try:
             text = ''
-            choices = stream_chunk.get('choices', [])
-            if choices and len(choices) > 0 and 'text' in choices[0]:
-                text = choices[0].get('text', {})
+            choices = stream_chunk.get('choices', []) 
+            if choices and len(choices) > 0 and 'delta' in choices[0]:
+                delta = choices[0].get('delta', {})
+                if 'content' in delta and delta['content'] is not None:
+                    text = delta.get('content', '')
 
             return text
         except Exception as e:
             raise e
 
     def collect_stream_inference(self, response):
         """
         collects the inference from the log stream
         """
         try:
             for stream_chunk in response:
-                self.response += self._get_text_from_stream_chunk(
-                    stream_chunk)
+                if isinstance(stream_chunk, dict):
+                    self.response += self._get_text_from_stream_chunk(
+                        stream_chunk)
+                else:
+                    self.response += self._get_text_from_stream_chunk(
+                        stream_chunk.model_dump())
         except Exception as e:
             raise e
 
     def collect_stream_inference_by_chunk(self, stream_chunk):
         """
         collects the inference from the log stream of openai chat completion chunk by chunk
         """
         try:
-            self.response += self._get_text_from_stream_chunk(
-                stream_chunk)
+            if isinstance(stream_chunk, dict):
+                self.response += self._get_text_from_stream_chunk(
+                    stream_chunk)
+            else:
+                self.response += self._get_text_from_stream_chunk(
+                    stream_chunk.model_dump())
         except Exception as e:
             raise e
 
     def log_stream_inference(self):
         """
         logs the stream inference to the athina api server
         """
         try:
             prompt_tokens = self._get_prompt_tokens(
                 prompt=self.prompt, language_model_id=self.language_model_id)
+
             completion_tokens = self._get_completion_tokens(
                 response=self.response, language_model_id=self.language_model_id)
+
             if prompt_tokens is not None and completion_tokens is not None:
                 total_tokens = prompt_tokens + completion_tokens
             else:
                 total_tokens = None
             payload = {
                 'prompt_slug': self.prompt_slug,
                 'prompt': self.prompt,
@@ -111,37 +127,38 @@
                 'session_id': str(self.session_id) if self.session_id is not None else None,
                 'user_query': str(self.user_query) if self.user_query is not None else None,
                 'external_reference_id': str(self.external_reference_id) if self.external_reference_id is not None else None,
                 'prompt_tokens': prompt_tokens,
                 'completion_tokens': completion_tokens,
                 'total_tokens': total_tokens,
                 'custom_attributes': self.custom_attributes,
+                'custom_eval_metrics': self.custom_eval_metrics,
             }
             # Remove None fields from the payload
             payload = {k: v for k, v in payload.items() if v is not None}
             RequestHelper.make_post_request(endpoint=LOG_INFERENCE_URL, payload=payload, headers={
-                'athina-api-key': LogOpenAiCompletionStreamInference.get_api_key(),
+                'athina-api-key': LogOpenAiChatCompletionStreamInference.get_api_key(),
             })
         except Exception as e:
             raise e
 
-    def _get_prompt_tokens(self, prompt: str, language_model_id: str):
+    def _get_prompt_tokens(self, prompt: List[Dict[str, Any]], language_model_id: str):
         """
         gets the prompt tokens given the prompt for the openai chat model completion
         """
         try:
-            tokens = get_token_usage_openai_completion(
-                text=prompt, language_model_id=language_model_id)
+            tokens = get_prompt_tokens_openai_chat_completion(
+                prompt=prompt, language_model_id=language_model_id)
             return tokens
         except Exception as e:
             return None
 
     def _get_completion_tokens(self, response: str, language_model_id: str):
         """
         gets the completion tokens given the prompt response from the openai chat model completion
         """
         try:
-            tokens = get_token_usage_openai_completion(
-                text=response, language_model_id=language_model_id)
+            tokens = get_completion_tokens_openai_chat_completion(
+                response=response, language_model_id=language_model_id)
             return tokens
         except Exception as e:
             return None
```

### Comparing `athina_logger-1.1.0/athina_logger/openai_wrapper.py` & `athina_logger-1.2.0/athina_logger/openai_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,26 +25,28 @@
         customer_user_id = None
         response_time_ms = None
         session_id = None
         user_query = None
         environment = "production"
         external_reference_id = None
         custom_attributes = None
+        custom_eval_metrics = None
 
         if athina_meta:
             prompt_slug = athina_meta.prompt_slug
             context = athina_meta.context
             response_time_ms = athina_meta.response_time
             customer_id = athina_meta.customer_id
             customer_user_id = athina_meta.customer_user_id
             session_id = athina_meta.session_id
             user_query = athina_meta.user_query
             environment = athina_meta.environment or "production"
             external_reference_id = athina_meta.external_reference_id
             custom_attributes = athina_meta.custom_attributes
+            custom_eval_metrics = athina_meta.custom_eval_metrics
 
         InferenceLogger.log_inference(
             prompt_slug=prompt_slug,
             prompt=args["messages"],
             language_model_id=args["model"],
             response=result,
             context=context,
@@ -52,14 +54,15 @@
             customer_id=customer_id,
             customer_user_id=customer_user_id,
             session_id=session_id,
             user_query=user_query,
             environment=environment,
             external_reference_id=external_reference_id,
             custom_attributes=custom_attributes,
+            custom_eval_metrics=custom_eval_metrics,
         )
     except Exception as e:
         print("Exception while logging to Athina: ", e)
         traceback.print_exc()
 
 
 class OpenAiMiddleware:
@@ -188,14 +191,15 @@
                 'session_id': str(self._athina_meta.session_id) if self._athina_meta.session_id is not None else None,
                 'user_query': str(self._athina_meta.user_query) if self._athina_meta.user_query is not None else None,
                 'external_reference_id': str(self._athina_meta.external_reference_id) if self._athina_meta.external_reference_id is not None else None,
                 'prompt_tokens': prompt_tokens,
                 'completion_tokens': completion_tokens,
                 'total_tokens': total_tokens,
                 'custom_attributes': self._athina_meta.custom_attributes,
+                'custom_eval_metrics': self._athina_meta.custom_eval_metrics,
             }
             # Remove None fields from the payload
             payload = {k: v for k, v in payload.items() if v is not None}
             InferenceLogger.log_inference(**payload)
         except Exception as e:
             raise e
```

### Comparing `athina_logger-1.1.0/athina_logger/request_helper.py` & `athina_logger-1.2.0/athina_logger/request_helper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.1.0/athina_logger/tracing/callback/langchain.py` & `athina_logger-1.2.0/athina_logger/tracing/callback/langchain.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.1.0/athina_logger/tracing/models.py` & `athina_logger-1.2.0/athina_logger/tracing/models.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.1.0/athina_logger/tracing/span.py` & `athina_logger-1.2.0/athina_logger/tracing/span.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         completion_tokens: Optional[int] = None,
         total_tokens: Optional[int] = None,
         response_time: Optional[int] = None,
         context: Optional[Dict] = None,
         expected_response: Optional[str] = None,
         custom_attributes: Optional[Dict] = None,
         cost: Optional[float] = None,
+        custom_eval_metrics: Optional[Dict] = None,
     ):
         span = Generation(
             name=name,
             start_time=start_time,
             end_time=end_time,
             span_type=span_type,
             status=status,
@@ -142,14 +143,15 @@
             completion_tokens=completion_tokens,
             total_tokens=total_tokens,
             response_time=response_time,
             context=context,
             expected_response=expected_response,
             custom_attributes=custom_attributes,
             cost=cost,
+            custom_eval_metrics=custom_eval_metrics,
         )
         self._children.append(span)
         return span
     
     def update(
         self,
         end_time: Optional[datetime.datetime] = None,
@@ -212,14 +214,15 @@
         completion_tokens: Optional[int] = None,
         total_tokens: Optional[int] = None,
         response_time: Optional[int] = None,
         context: Optional[Dict] = None,
         expected_response: Optional[str] = None,
         custom_attributes: Optional[Dict] = None,
         cost: Optional[float] = None,
+        custom_eval_metrics: Optional[Dict] = None,
     ):
         if attributes is None:
             attributes = {}
         additional_attributes = {
             "prompt": prompt,
             "response": response,
             "prompt_slug": prompt_slug,
@@ -238,14 +241,15 @@
             "completion_tokens": completion_tokens,
             "total_tokens": total_tokens,
             "response_time": response_time,
             "context": context,
             "expected_response": expected_response,
             "custom_attributes": custom_attributes,
             "cost": cost,
+            "custom_eval_metrics": custom_eval_metrics,
         }
         # Update 'attributes' only with non-None values from 'additional_attributes'
         for key, value in additional_attributes.items():
             if value is not None:
                 attributes[key] = value
         super().__init__(
             name=name,
@@ -285,14 +289,15 @@
         completion_tokens: Optional[int] = None,
         total_tokens: Optional[int] = None,
         response_time: Optional[int] = None,
         context: Optional[Dict] = None,
         expected_response: Optional[str] = None,
         custom_attributes: Optional[Dict] = None,
         cost: Optional[float] = None,
+        custom_eval_metrics: Optional[Dict] = None,
     ):
         if self._span.attributes is None:
             self._span.attributes = {}
         attributes = {
             "prompt": prompt if prompt is not None else self._span.attributes.get("prompt"),
             "response": response if response is not None else self._span.attributes.get("response"),
             "prompt_slug": prompt_slug if prompt_slug is not None else self._span.attributes.get("prompt_slug"),
@@ -311,14 +316,15 @@
             "completion_tokens": completion_tokens if completion_tokens is not None else self._span.attributes.get("completion_tokens"),
             "total_tokens": total_tokens if total_tokens is not None else self._span.attributes.get("total_tokens"),
             "response_time": response_time if response_time is not None else self._span.attributes.get("response_time"),
             "context": context if context is not None else self._span.attributes.get("context"),
             "expected_response": expected_response if expected_response is not None else self._span.attributes.get("expected_response"),
             "custom_attributes": custom_attributes if custom_attributes is not None else self._span.attributes.get("custom_attributes"),
             "cost": cost if cost is not None else self._span.attributes.get("cost"),
+            "custom_eval_metrics": custom_eval_metrics if custom_eval_metrics is not None else self._span.attributes.get("custom_eval_metrics"),
         }
         super().update(
             end_time=end_time,
             status=status,
             input=input,
             output=output,
             duration=duration,
```

### Comparing `athina_logger-1.1.0/athina_logger/tracing/trace.py` & `athina_logger-1.2.0/athina_logger/tracing/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
         completion_tokens: Optional[int] = None,
         total_tokens: Optional[int] = None,
         response_time: Optional[int] = None,
         context: Optional[Dict] = None,
         expected_response: Optional[str] = None,
         custom_attributes: Optional[Dict] = None,
         cost: Optional[float] = None,
+        custom_eval_metrics: Optional[Dict] = None,
     ) -> Generation:
         span = Generation(
             name=name,
             start_time=(start_time or datetime.datetime.utcnow()),
             end_time=end_time,
             span_type=span_type,
             status=status,
@@ -137,14 +138,15 @@
             completion_tokens=completion_tokens,
             total_tokens=total_tokens,
             response_time=response_time,
             context=context,
             expected_response=expected_response,
             custom_attributes=custom_attributes,
             cost=cost,
+            custom_eval_metrics=custom_eval_metrics,
         )
         self._spans.append(span)
         return span
     
     def to_dict(self):
         trace_dict = self._trace.model_dump()
         trace_dict["spans"] = [span.to_dict() for span in self._spans]
```

### Comparing `athina_logger-1.1.0/athina_logger/util/extract_model.py` & `athina_logger-1.2.0/athina_logger/util/extract_model.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.1.0/athina_logger/util/token_count_helper.py` & `athina_logger-1.2.0/athina_logger/util/token_count_helper.py`

 * *Files identical despite different names*

### Comparing `athina_logger-1.1.0/PKG-INFO` & `athina_logger-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athina-logger
-Version: 1.1.0
+Version: 1.2.0
 Summary: 
 Author: Akshat Gupta
 Author-email: akshat@athina.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

