# Comparing `tmp/shell_gpt-1.4.0.tar.gz` & `tmp/shell_gpt-1.4.1.tar.gz`

## Comparing `shell_gpt-1.4.0.tar` & `shell_gpt-1.4.1.tar`

### file list

```diff
@@ -1,41 +1,32 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/LICENSE
--rw-r--r--   0        0        0    25787 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/pyproject.toml
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/__version__.py
--rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/app.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/cache.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/config.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/function.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/integration.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/printer.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/role.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/handlers/__init__.py
--rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/handlers/chat_handler.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/handlers/default_handler.py
--rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/handlers/handler.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/handlers/repl_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/llm_functions/__init__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/llm_functions/init_functions.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/llm_functions/common/execute_shell.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/sgpt/llm_functions/mac/apple_script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/_integration.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/conftest.py
--rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/test_code.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/test_default.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/test_roles.py
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/test_shell.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/utils.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/LICENSE
--rw-r--r--   0        0        0    25787 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    27993 2020-02-02 00:00:00.000000 shell_gpt-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/__version__.py
+-rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/app.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/cache.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/config.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/function.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/integration.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/printer.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/role.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/__init__.py
+-rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/chat_handler.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/default_handler.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/handler.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/repl_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/llm_functions/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/llm_functions/init_functions.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/llm_functions/common/execute_shell.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/llm_functions/mac/apple_script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/_integration.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/test_code.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/test_default.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/test_roles.py
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/test_shell.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/utils.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/LICENSE
+-rw-r--r--   0        0        0    25954 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/README.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    28160 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/PKG-INFO
```

### Comparing `shell_gpt-1.4.0/LICENSE` & `shell_gpt-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/README.md` & `shell_gpt-1.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -470,7 +470,9 @@
 sgpt --chat rainbow "translate your last answer in french"
 ```
 
 You also can use the provided `Dockerfile` to build your own image:
 ```shell
 docker build -t sgpt .
 ```
+
+Additional documentation: [Azure integration](https://github.com/TheR1D/shell_gpt/wiki/Azure), [Ollama integration](https://github.com/TheR1D/shell_gpt/wiki/Ollama).
```

### Comparing `shell_gpt-1.4.0/pyproject.toml` & `shell_gpt-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/app.py` & `shell_gpt-1.4.1/sgpt/app.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/cache.py` & `shell_gpt-1.4.1/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/config.py` & `shell_gpt-1.4.1/sgpt/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                 string_config += f"{key}={value}\n"
             file.write(string_config)
 
     def _read(self) -> None:
         with open(self.config_path, "r", encoding="utf-8") as file:
             for line in file:
                 if line.strip() and not line.startswith("#"):
-                    key, value = line.strip().split("=")
+                    key, value = line.strip().split("=", 1)
                     self[key] = value
 
     def get(self, key: str) -> str:  # type: ignore
         # Prioritize environment variables over config file.
         value = os.getenv(key) or super().get(key)
         if not value:
             raise UsageError(f"Missing config key: {key}")
```

### Comparing `shell_gpt-1.4.0/sgpt/function.py` & `shell_gpt-1.4.1/sgpt/function.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/integration.py` & `shell_gpt-1.4.1/sgpt/integration.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/printer.py` & `shell_gpt-1.4.1/sgpt/printer.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/role.py` & `shell_gpt-1.4.1/sgpt/role.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/utils.py` & `shell_gpt-1.4.1/sgpt/utils.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/handlers/chat_handler.py` & `shell_gpt-1.4.1/sgpt/handlers/chat_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         """
 
         def wrapper(*args: Any, **kwargs: Any) -> Generator[str, None, None]:
             chat_id = kwargs.pop("chat_id", None)
             if not kwargs.get("messages"):
                 return
             if not chat_id:
-                yield from func(*args, **kwargs, caching=False)
+                yield from func(*args, **kwargs)
                 return
             previous_messages = self._read(chat_id)
             for message in kwargs["messages"]:
                 previous_messages.append(message)
             kwargs["messages"] = previous_messages
             response_text = ""
             for word in func(*args, **kwargs):
```

### Comparing `shell_gpt-1.4.0/sgpt/handlers/default_handler.py` & `shell_gpt-1.4.1/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/handlers/handler.py` & `shell_gpt-1.4.1/sgpt/handlers/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..cache import Cache
 from ..config import cfg
 from ..function import get_function
 from ..printer import MarkdownPrinter, Printer, TextPrinter
 from ..role import DefaultRoles, SystemRole
 
-completion: Callable[..., Any] = lambda *args, **kwargs: None
+completion: Callable[..., Any] = lambda *args, **kwargs: Generator[Any, None, None]
 base_url = cfg.get("API_BASE_URL")
 use_litellm = cfg.get("USE_LITELLM") == "true"
 additional_kwargs = {
     "timeout": int(cfg.get("REQUEST_TIMEOUT")),
     "api_key": cfg.get("OPENAI_API_KEY"),
     "base_url": None if base_url == "default" else base_url,
 }
@@ -92,41 +92,51 @@
         name = arguments = ""
         is_shell_role = self.role.name == DefaultRoles.SHELL.value
         is_code_role = self.role.name == DefaultRoles.CODE.value
         is_dsc_shell_role = self.role.name == DefaultRoles.DESCRIBE_SHELL.value
         if is_shell_role or is_code_role or is_dsc_shell_role:
             functions = None
 
-        for chunk in completion(
+        response = completion(
             model=model,
             temperature=temperature,
             top_p=top_p,
             messages=messages,
             functions=functions,
             stream=True,
             **additional_kwargs,
-        ):
-            delta = chunk.choices[0].delta
-            # LiteLLM uses dict instead of Pydantic object like OpenAI does.
-            function_call = (
-                delta.get("function_call") if use_litellm else delta.function_call
-            )
-            if function_call:
-                if function_call.name:
-                    name = function_call.name
-                if function_call.arguments:
-                    arguments += function_call.arguments
-            if chunk.choices[0].finish_reason == "function_call":
-                yield from self.handle_function_call(messages, name, arguments)
-                yield from self.get_completion(
-                    model, temperature, top_p, messages, functions, caching=False
-                )
-                return
+        )
 
-            yield delta.content or ""
+        try:
+            for chunk in response:
+                delta = chunk.choices[0].delta
+                # LiteLLM uses dict instead of Pydantic object like OpenAI does.
+                function_call = (
+                    delta.get("function_call") if use_litellm else delta.function_call
+                )
+                if function_call:
+                    if function_call.name:
+                        name = function_call.name
+                    if function_call.arguments:
+                        arguments += function_call.arguments
+                if chunk.choices[0].finish_reason == "function_call":
+                    yield from self.handle_function_call(messages, name, arguments)
+                    yield from self.get_completion(
+                        model=model,
+                        temperature=temperature,
+                        top_p=top_p,
+                        messages=messages,
+                        functions=functions,
+                        caching=False,
+                    )
+                    return
+
+                yield delta.content or ""
+        except KeyboardInterrupt:
+            response.close()
 
     def handle(
         self,
         prompt: str,
         model: str,
         temperature: float,
         top_p: float,
```

### Comparing `shell_gpt-1.4.0/sgpt/handlers/repl_handler.py` & `shell_gpt-1.4.1/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/llm_functions/init_functions.py` & `shell_gpt-1.4.1/sgpt/llm_functions/init_functions.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/llm_functions/common/execute_shell.py` & `shell_gpt-1.4.1/sgpt/llm_functions/common/execute_shell.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/sgpt/llm_functions/mac/apple_script.py` & `shell_gpt-1.4.1/sgpt/llm_functions/mac/apple_script.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/tests/_integration.py` & `shell_gpt-1.4.1/tests/_integration.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/tests/test_code.py` & `shell_gpt-1.4.1/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/tests/test_default.py` & `shell_gpt-1.4.1/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/tests/test_roles.py` & `shell_gpt-1.4.1/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/tests/test_shell.py` & `shell_gpt-1.4.1/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/tests/utils.py` & `shell_gpt-1.4.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.0/PKG-INFO` & `shell_gpt-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: shell_gpt
-Version: 1.4.0
+Version: 1.4.1
 Summary: A command-line productivity tool powered by large language models, will help you accomplish your tasks faster and more efficiently.
 Project-URL: homepage, https://github.com/ther1d/shell_gpt
 Project-URL: repository, https://github.com/ther1d/shell_gpt
 Project-URL: documentation, https://github.com/TheR1D/shell_gpt/blob/main/README.md
 Author-email: Farkhod Sadykov <farkhod@sadykov.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -518,7 +518,9 @@
 sgpt --chat rainbow "translate your last answer in french"
 ```
 
 You also can use the provided `Dockerfile` to build your own image:
 ```shell
 docker build -t sgpt .
 ```
+
+Additional documentation: [Azure integration](https://github.com/TheR1D/shell_gpt/wiki/Azure), [Ollama integration](https://github.com/TheR1D/shell_gpt/wiki/Ollama).
```

