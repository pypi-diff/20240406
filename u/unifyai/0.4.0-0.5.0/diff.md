# Comparing `tmp/unifyai-0.4.0.tar.gz` & `tmp/unifyai-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.4.0.tar", max compression
+gzip compressed data, was "unifyai-0.5.0.tar", max compression
```

## Comparing `unifyai-0.4.0.tar` & `unifyai-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.4.0/LICENSE
--rw-r--r--   0        0        0     5465 2024-04-03 10:55:32.016364 unifyai-0.4.0/README.md
--rw-r--r--   0        0        0      998 2024-04-03 11:20:47.800342 unifyai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-02 01:55:16.869353 unifyai-0.4.0/unifyai/__init__.py
--rw-r--r--   0        0        0    10479 2024-04-03 11:19:06.804344 unifyai-0.4.0/unifyai/clients.py
--rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.4.0/unifyai/exceptions.py
--rw-r--r--   0        0        0     4100 2024-04-02 01:55:16.873353 unifyai-0.4.0/unifyai/tests.py
--rw-r--r--   0        0        0     6106 1970-01-01 00:00:00.000000 unifyai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5585 2024-04-06 07:19:00.771524 unifyai-0.5.0/README.md
+-rw-r--r--   0        0        0     1019 2024-04-06 07:18:44.483524 unifyai-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-02 01:55:16.869353 unifyai-0.5.0/unifyai/__init__.py
+-rw-r--r--   0        0        0    13325 2024-04-06 07:18:44.483524 unifyai-0.5.0/unifyai/clients.py
+-rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.5.0/unifyai/exceptions.py
+-rw-r--r--   0        0        0     3820 2024-04-06 07:18:44.483524 unifyai-0.5.0/unifyai/tests.py
+-rw-r--r--   0        0        0     6268 1970-01-01 00:00:00.000000 unifyai-0.5.0/PKG-INFO
```

### Comparing `unifyai-0.4.0/LICENSE` & `unifyai-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.4.0/README.md` & `unifyai-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,24 +21,30 @@
 ## Basic Usage
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@anyscale"
 )
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale")
+response = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
 ```
 
 Here, `response` is a string containing the model's output.
 
-You can influence the model's persona using the `system_prompt` argument in the `.generate` function.
+You can influence the model's persona using the `system_prompt` argument in the `.generate` function:
 
 ```python
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", system_prompt="You should always talk in rhymes", model="llama-2-13b-chat", provider="anyscale")
+response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", system_prompt="You should always talk in rhymes")
+```
+
+If you want change the model, you can do so by updating the `.model` attribute of the client:
+```python
+client.model = "mistral-7b-instruct-v0.1@deepinfra"
 ```
 
 ### Supported Models
 The list of supported models and providers is available in [the platform](https://unify.ai/hub).
 
 ### API Key
 You can get an API Key from [the Unify console](https://console.unify.ai/)
@@ -56,15 +62,15 @@
 
  ```python
  messages=[
     {"role": "user", "content": "Who won the world series in 2020?"},
     {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
     {"role": "user", "content": "Where was it played?"}
 ]
-res = unify.generate(messages=messages, model="llama-2-7b-chat", provider="anyscale")
+res = unify.generate(messages=messages)
  ```
 
 
 ## Asynchronous Usage
 For optimal performance in handling multiple user requests simultaneously, such as in a chatbot application, processing them asynchronously is recommended.
 To use the AsyncUnify client, simply import `AsyncUnify` instead
  of `Unify` and use `await` with the `.generate` function.
@@ -72,18 +78,19 @@
  ```python
 from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@anyscale"
 )
 
 async def main():
-    responses = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale")
+    responses = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?")
 
 asyncio.run(main())
 ```
 
 Functionality wise, the Async and Sync clients are identical.
 
 ## Streaming Responses
@@ -91,33 +98,35 @@
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@anyscale"
 )
-stream = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale", stream=True)
+stream = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
 for chunk in stream:
     print(chunk, end="")
 ```
 
 It works in exactly the same way with Async clients.
 
  ```python
 from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@anyscale"
 )
 
 async def main():
-    async_stream = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale", stream=True)
+    async_stream = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?")
     async for chunk in async_stream:
         print(chunk, end="")
 
 asyncio.run(main())
 ```
 
 ## Get Current Credit Balance
@@ -131,11 +140,18 @@
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@lowest-input-cost"
 )
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="lowest-input-cost")
+response = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
 ```
+You can see the provider chosen by printing the `.provider` attribute of the client:
+
+```python
+print(unify.provider)
+```
+
 Dynamic routing works with both Synchronous and Asynchronous clients. For more information on Dynamic Routing, check our [documentation](https://unify.ai/docs/hub/concepts/runtime_routing.html#dynamic-routing).
```

### Comparing `unifyai-0.4.0/pyproject.toml` & `unifyai-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tool.poetry]
 name = "unifyai"
-version = "0.4.0"
+version = "0.5.0"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
 repository = "https://github.com/unifyai/unify-llm-python"
 
 [tool.poetry.dependencies]
 python = "^3.9"
+requests = "^2.31.0"
 openai = "^1.12.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "~4.0.1"
 mypy = "^1.1.1"
 isort = "^5.11.4"
 pre-commit = "^3.0.1"
```

### Comparing `unifyai-0.4.0/unifyai/clients.py` & `unifyai-0.5.0/unifyai/clients.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import AsyncGenerator, Dict, Generator, List, Optional, Union
+from typing import AsyncGenerator, Dict, Generator, List, Optional, Tuple, Union
 
 import openai
 import requests
 from unifyai.exceptions import BadRequestError, UnifyError, status_error_map
 
 
 def _validate_api_key(api_key: Optional[str]) -> str:
@@ -12,58 +12,106 @@
     if api_key is None:
         raise KeyError(
             "UNIFY_KEY is missing. Please make sure it is set correctly!",
         )
     return api_key
 
 
+def _validate_model_name(value: str) -> Tuple[str, str]:
+    error_message = "model string must use OpenAI API format: <uploaded_by>/<model_name>@<provider_name>"  # noqa: E501
+
+    if not isinstance(value, str):
+        raise UnifyError(error_message)
+
+    try:
+        model_name, provider_name = value.split("/")[-1].split("@")
+    except ValueError:
+        raise UnifyError(error_message)
+
+    if not model_name or not provider_name:
+        raise UnifyError(error_message)
+    return (model_name, provider_name)
+
+
 class Unify:
     """Class for interacting with the Unify API."""
 
     def __init__(
         self,
         api_key: Optional[str] = None,
+        model: str = "llama-2-7b-chat@anyscale",
     ) -> None:  # noqa: DAR101, DAR401
         """Initialize the Unify client.
 
         Args:
             api_key (str, optional): API key for accessing the Unify API.
                 If None, it attempts to retrieve the API key from the
                 environment variable UNIFY_KEY.
                 Defaults to None.
 
+            model (str): Model name in OpenAI API format:
+                <uploaded_by>/<model_name>@<provider_name>
+                Defaults to llama-2-7b-chat@anyscale.
         Raises:
             UnifyError: If the API key is missing.
         """
-        self.api_key = _validate_api_key(api_key)
+        self._api_key = _validate_api_key(api_key)
         try:
             self.client = openai.OpenAI(
                 base_url="https://api.unify.ai/v0/",
-                api_key=self.api_key,
+                api_key=self._api_key,
             )
         except openai.OpenAIError as e:
             raise UnifyError(f"Failed to initialize Unify client: {str(e)}")
 
+        self._model, self._provider = _validate_model_name(model)  # noqa:WPS414
+
+    @property
+    def model(self) -> str:
+        """
+        Get the model name along with the provider.  # noqa: DAR201.
+
+        Returns:
+            str: The model name along with the provider, separated by '@'.
+        """
+        return "@".join([self._model, self._provider])
+
+    @model.setter
+    def model(self, value: str) -> None:
+        """
+        Set the model name and provider.  # noqa: DAR101.
+
+        Args:
+            value (str): The model name along with the provider, separated by '@'.
+        """
+        self._model, self._provider = _validate_model_name(value)  # noqa:WPS414
+
+    @property
+    def provider(self) -> str:
+        """
+        Get the provider name.  # noqa :DAR201.
+
+        Returns:
+            str: The provider name.
+        """
+        return self._provider
+
     def generate(  # noqa: WPS234, WPS211
         self,
         messages: Union[str, List[Dict[str, str]]],
         system_prompt: Optional[str] = None,
-        model: str = "llama-2-13b-chat",
-        provider: str = "anyscale",
         stream: bool = False,
     ) -> Union[Generator[str, None, None], str]:  # noqa: DAR101, DAR201
         """Generate content using the Unify API.
 
         Args:
             messages (Union[str, List[Dict[str, str]]]): A single prompt as a
             string or a dictionary containing the conversation history.
             system_prompt (Optinal[str]): An optional string containing the
             system prompt.
-            model (str): The name of the model. Defaults to "llama-2-13b-chat".
-            provider (str): The provider of the model. Defaults to "anyscale".
             stream (bool): If True, generates content as a stream.
             If False, generates content as a single response.
             Defaults to False.
 
         Returns:
             Union[Generator[str, None, None], str]: If stream is True,
              returns a generator yielding chunks of content.
@@ -78,16 +126,16 @@
 
         if isinstance(messages, str):
             contents.append({"role": "user", "content": messages})
         else:
             contents.extend(messages)
 
         if stream:
-            return self._generate_stream(contents, model, provider)
-        return self._generate_non_stream(contents, model, provider)
+            return self._generate_stream(contents, self._model, self._provider)
+        return self._generate_non_stream(contents, self._model, self._provider)
 
     def get_credit_balance(self) -> Optional[int]:
         # noqa: DAR201, DAR401
         """
         Get the remaining credits left on your account.
 
         Returns:
@@ -96,15 +144,15 @@
         Raises:
             BadRequestError: If there was an HTTP error.
             ValueError: If there was an error parsing the JSON response.
         """
         url = "https://api.unify.ai/v0/get_credits"
         headers = {
             "accept": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
+            "Authorization": f"Bearer {self._api_key}",
         }
         try:
             response = requests.get(url, headers=headers, timeout=10)
             response.raise_for_status()
             return response.json()["credits"]
         except requests.RequestException as e:
             raise BadRequestError("There was an error with the request.") from e
@@ -121,14 +169,15 @@
             chat_completion = self.client.chat.completions.create(
                 model="@".join([model, provider]),
                 messages=messages,  # type: ignore[arg-type]
                 stream=True,
             )
             for chunk in chat_completion:
                 content = chunk.choices[0].delta.content  # type: ignore[union-attr]
+                self._provider = chunk.model.split("@")[-1]  # type: ignore[union-attr]
                 if content is not None:
                     yield content
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
     def _generate_non_stream(
         self,
@@ -138,46 +187,87 @@
     ) -> str:
         try:
             chat_completion = self.client.chat.completions.create(
                 model="@".join([model, provider]),
                 messages=messages,  # type: ignore[arg-type]
                 stream=False,
             )
+            self._provider = chat_completion.model.split(  # type: ignore[union-attr]
+                "@",
+            )[-1]
+
             return chat_completion.choices[0].message.content.strip(" ")  # type: ignore # noqa: E501, WPS219
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
 
 class AsyncUnify:
     """Class for interacting asynchronously with the Unify API."""
 
     def __init__(
         self,
         api_key: Optional[str] = None,
+        model: str = "llama-2-7b-chat@anyscale",
     ) -> None:  # noqa:DAR101, DAR401
         """Initialize the AsyncUnify client.
 
         Args:
             api_key (str, optional): API key for accessing the Unify API.
             If None, it attempts to retrieve the API key from
             the environment variable UNIFY_KEY.
             Defaults to None.
 
+            model (str): Model name in OpenAI API format:
+                <uploaded_by>/<model_name>@<provider_name>
+                Defaults to llama-2-7b-chat@anyscale.
+
         Raises:
             UnifyError: If the API key is missing.
         """
-        self.api_key = _validate_api_key(api_key)
+        self._api_key = _validate_api_key(api_key)
         try:
             self.client = openai.AsyncOpenAI(
                 base_url="https://api.unify.ai/v0/",
-                api_key=self.api_key,
+                api_key=self._api_key,
             )
         except openai.APIStatusError as e:
             raise UnifyError(f"Failed to initialize Unify client: {str(e)}")
 
+        self._model, self._provider = _validate_model_name(model)  # noqa: WPS414
+
+    @property
+    def model(self) -> str:
+        """
+        Get the model name along with the provider. # noqa: DAR201.
+
+        Returns:
+            str: The model name along with the provider, separated by '@'.
+        """
+        return "@".join([self._model, self._provider])
+
+    @model.setter
+    def model(self, value: str) -> None:
+        """
+        Set the model name and provider.  # noqa: DAR101.
+
+        Args:
+            value (str): The model name along with the provider, separated by '@'.
+        """
+        self._model, self._provider = _validate_model_name(value)  # noqa: WPS414
+
+    @property
+    def provider(self) -> str:
+        """
+        Get the provider name. # noqa: DAR201.
+
+        Returns:
+            str: The provider name.
+        """
+        return self._provider
+
     def get_credit_balance(self) -> Optional[int]:
         # noqa: DAR201, DAR401
         """
         Get the remaining credits left on your account.
 
         Returns:
             int or None: The remaining credits on the account
@@ -186,31 +276,29 @@
         Raises:
             BadRequestError: If there was an HTTP error.
             ValueError: If there was an error parsing the JSON response.
         """
         url = "https://api.unify.ai/v0/get_credits"
         headers = {
             "accept": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
+            "Authorization": f"Bearer {self._api_key}",
         }
         try:
             response = requests.get(url, headers=headers, timeout=10)
             response.raise_for_status()
             return response.json()["credits"]
         except requests.RequestException as e:
             raise BadRequestError("There was an error with the request.") from e
         except (KeyError, ValueError) as e:
             raise ValueError("Error parsing JSON response.") from e
 
     async def generate(  # noqa: WPS234, WPS211
         self,
         messages: Union[str, List[Dict[str, str]]],
         system_prompt: Optional[str] = None,
-        model: str = "llama-2-13b-chat",
-        provider: str = "anyscale",
         stream: bool = False,
     ) -> Union[AsyncGenerator[str, None], str]:  # noqa: DAR101, DAR201
         """Generate content asynchronously using the Unify API.
 
         Args:
             messages (Union[str, List[Dict[str, str]]]): A single prompt as a
             string or a dictionary containing the conversation history.
@@ -236,16 +324,16 @@
 
         if isinstance(messages, str):
             contents.append({"role": "user", "content": messages})
         else:
             contents.extend(messages)
 
         if stream:
-            return self._generate_stream(contents, model, provider)
-        return await self._generate_non_stream(contents, model, provider)
+            return self._generate_stream(contents, self._model, self._provider)
+        return await self._generate_non_stream(contents, self._model, self._provider)
 
     async def _generate_stream(
         self,
         messages: List[Dict[str, str]],
         model: str,
         provider: str,
     ) -> AsyncGenerator[str, None]:
@@ -253,14 +341,15 @@
             async with self.client as async_client:
                 async_stream = await async_client.chat.completions.create(
                     model="@".join([model, provider]),
                     messages=messages,  # type: ignore[arg-type]
                     stream=True,
                 )
                 async for chunk in async_stream:  # type: ignore[union-attr]
+                    self._provider = chunk.model.split("@")[-1]
                     yield chunk.choices[0].delta.content or ""
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
     async def _generate_non_stream(
         self,
         messages: List[Dict[str, str]],
@@ -270,10 +359,11 @@
         try:
             async with self.client as async_client:
                 async_response = await async_client.chat.completions.create(
                     model="@".join([model, provider]),
                     messages=messages,  # type: ignore[arg-type]
                     stream=False,
                 )
+            self._provider = async_response.model.split("@")[-1]  # type: ignore
             return async_response.choices[0].message.content.strip(" ")  # type: ignore # noqa: E501, WPS219
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
```

### Comparing `unifyai-0.4.0/unifyai/exceptions.py` & `unifyai-0.5.0/unifyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.4.0/unifyai/tests.py` & `unifyai-0.5.0/unifyai/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import unittest
 from types import AsyncGeneratorType, GeneratorType
 from unittest.mock import MagicMock, patch
 
 from unifyai.clients import AsyncUnify, Unify
-from unifyai.exceptions import AuthenticationError, InternalServerError
+from unifyai.exceptions import AuthenticationError, UnifyError
 
 
 class TestUnify(unittest.TestCase):
     def setUp(self) -> None:
         # Set up a valid API key for testing
         self.valid_api_key = os.environ.get("UNIFY_KEY")
 
@@ -21,19 +21,17 @@
     @patch("os.environ.get", return_value=None)
     def test_missing_api_key_raises_key_error(self, mock_get: MagicMock) -> None:
         # Initializing Unify without providing API key should raise KeyError
         with self.assertRaises(KeyError):
             Unify()
 
     def test_incorrect_model_name_raises_internal_server_error(self) -> None:
-        # Instantiate Unify with a valid API key
-        unify = Unify(self.valid_api_key)
-        # Provide incorrect model name to generate function
-        with self.assertRaises(InternalServerError):
-            unify.generate(messages="hello", model="llama-chat")
+        # Provide incorrect model name
+        with self.assertRaises(UnifyError):
+            Unify(api_key=self.valid_api_key, model="llama-chat")
 
     def test_generate_returns_string_when_stream_false(self) -> None:
         # Instantiate Unify with a valid API key
         unify = Unify(api_key=self.valid_api_key)
         # Call generate with stream=False
         result = unify.generate("hello", stream=False)
         # Assert that the result is a string
@@ -64,19 +62,17 @@
         # Initializing AsyncUnify without providing
         # API key should raise KeyError
         with self.assertRaises(KeyError):
             async_unify = AsyncUnify()
             await async_unify.generate("hello")
 
     async def test_incorrect_model_name_raises_internal_server_error(self) -> None:
-        # Instantiate AsyncUnify with a valid API key
-        async_unify = AsyncUnify(api_key=self.valid_api_key)
-        # Provide incorrect model name to generate function
-        with self.assertRaises(InternalServerError):
-            await async_unify.generate(messages="hello", model="llama-chat")
+        # Provide incorrect model name
+        with self.assertRaises(UnifyError):
+            AsyncUnify(api_key=self.valid_api_key, model="llama-chat")
 
     async def test_generate_returns_string_when_stream_false(self) -> None:
         # Instantiate AsyncUnify with a valid API key
         async_unify = AsyncUnify(api_key=self.valid_api_key)
         # Call generate with stream=False
         result = await async_unify.generate("hello", stream=False)
         # Assert that the result is a string
```

### Comparing `unifyai-0.4.0/PKG-INFO` & `unifyai-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python package for interacting with the Unify API
 Home-page: https://github.com/unifyai/unify-llm-python
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: openai (>=1.12.0,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/unifyai/unify-llm-python
 Description-Content-Type: text/markdown
 
 # Unify Python API Library
 The Unify Python Package provides access to the [Unify](https://unify.ai) REST API, allowing you to query Large Language Models (LLMs)
 from any Python 3.7.1+ application.
 It includes Synchronous and Asynchronous clients with Streaming responses support.
@@ -38,24 +39,30 @@
 ## Basic Usage
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@anyscale"
 )
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale")
+response = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
 ```
 
 Here, `response` is a string containing the model's output.
 
-You can influence the model's persona using the `system_prompt` argument in the `.generate` function.
+You can influence the model's persona using the `system_prompt` argument in the `.generate` function:
 
 ```python
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", system_prompt="You should always talk in rhymes", model="llama-2-13b-chat", provider="anyscale")
+response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", system_prompt="You should always talk in rhymes")
+```
+
+If you want change the model, you can do so by updating the `.model` attribute of the client:
+```python
+client.model = "mistral-7b-instruct-v0.1@deepinfra"
 ```
 
 ### Supported Models
 The list of supported models and providers is available in [the platform](https://unify.ai/hub).
 
 ### API Key
 You can get an API Key from [the Unify console](https://console.unify.ai/)
@@ -73,15 +80,15 @@
 
  ```python
  messages=[
     {"role": "user", "content": "Who won the world series in 2020?"},
     {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
     {"role": "user", "content": "Where was it played?"}
 ]
-res = unify.generate(messages=messages, model="llama-2-7b-chat", provider="anyscale")
+res = unify.generate(messages=messages)
  ```
 
 
 ## Asynchronous Usage
 For optimal performance in handling multiple user requests simultaneously, such as in a chatbot application, processing them asynchronously is recommended.
 To use the AsyncUnify client, simply import `AsyncUnify` instead
  of `Unify` and use `await` with the `.generate` function.
@@ -89,18 +96,19 @@
  ```python
 from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@anyscale"
 )
 
 async def main():
-    responses = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale")
+    responses = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?")
 
 asyncio.run(main())
 ```
 
 Functionality wise, the Async and Sync clients are identical.
 
 ## Streaming Responses
@@ -108,33 +116,35 @@
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@anyscale"
 )
-stream = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale", stream=True)
+stream = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
 for chunk in stream:
     print(chunk, end="")
 ```
 
 It works in exactly the same way with Async clients.
 
  ```python
 from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@anyscale"
 )
 
 async def main():
-    async_stream = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale", stream=True)
+    async_stream = await async_unify.generate(messages="Hello Llama! Who was Isaac Newton?")
     async for chunk in async_stream:
         print(chunk, end="")
 
 asyncio.run(main())
 ```
 
 ## Get Current Credit Balance
@@ -148,12 +158,19 @@
 
 ```python
 import os
 from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
+    model="llama-2-13b-chat@lowest-input-cost"
 )
-response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="lowest-input-cost")
+response = unify.generate(messages="Hello Llama! Who was Isaac Newton?")
 ```
+You can see the provider chosen by printing the `.provider` attribute of the client:
+
+```python
+print(unify.provider)
+```
+
 Dynamic routing works with both Synchronous and Asynchronous clients. For more information on Dynamic Routing, check our [documentation](https://unify.ai/docs/hub/concepts/runtime_routing.html#dynamic-routing).
```

