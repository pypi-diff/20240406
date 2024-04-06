# Comparing `tmp/myllm-4.7.8.tar.gz` & `tmp/myllm-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myllm-4.7.8.tar", max compression
+gzip compressed data, was "myllm-4.8.0.tar", max compression
```

## Comparing `myllm-4.7.8.tar` & `myllm-4.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-05 06:29:58.261690 myllm-4.7.8/LICENSE
--rw-r--r--   0        0        0     3014 2024-04-05 06:29:58.261690 myllm-4.7.8/README.md
--rw-r--r--   0        0        0       95 2024-04-05 06:30:39.357566 myllm-4.7.8/myllm/__init__.py
--rw-r--r--   0        0        0      772 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/config.py
--rw-r--r--   0        0        0     3094 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/default_settings.toml
--rw-r--r--   0        0        0     7189 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/main.py
--rw-r--r--   0        0        0      117 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/__init__.py
--rw-r--r--   0        0        0     4643 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/client.py
--rw-r--r--   0        0        0     1996 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/g4f.py
--rw-r--r--   0        0        0     2212 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/gemini.py
--rw-r--r--   0        0        0     2078 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/openai.py
--rw-r--r--   0        0        0     2322 2024-04-05 06:29:58.265689 myllm-4.7.8/myllm/provider/petals.py
--rw-r--r--   0        0        0     3926 2024-04-05 06:30:39.357566 myllm-4.7.8/pyproject.toml
--rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 myllm-4.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-06 07:37:08.382699 myllm-4.8.0/LICENSE
+-rw-r--r--   0        0        0     3014 2024-04-06 07:37:08.382699 myllm-4.8.0/README.md
+-rw-r--r--   0        0        0       95 2024-04-06 07:37:48.243262 myllm-4.8.0/myllm/__init__.py
+-rw-r--r--   0        0        0      772 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/config.py
+-rw-r--r--   0        0        0     3094 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/default_settings.toml
+-rw-r--r--   0        0        0      131 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/__init__.py
+-rw-r--r--   0        0        0     4643 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/client.py
+-rw-r--r--   0        0        0     1986 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/g4f.py
+-rw-r--r--   0        0        0     2193 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/not_working/gemini.py
+-rw-r--r--   0        0        0     2308 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/not_working/petals.py
+-rw-r--r--   0        0        0     2068 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/handler/openai.py
+-rw-r--r--   0        0        0     7197 2024-04-06 07:37:08.386699 myllm-4.8.0/myllm/main.py
+-rw-r--r--   0        0        0     3928 2024-04-06 07:37:48.239262 myllm-4.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 myllm-4.8.0/PKG-INFO
```

### Comparing `myllm-4.7.8/LICENSE` & `myllm-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `myllm-4.7.8/README.md` & `myllm-4.8.0/README.md`

 * *Files identical despite different names*

### Comparing `myllm-4.7.8/myllm/config.py` & `myllm-4.8.0/myllm/config.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.8/myllm/default_settings.toml` & `myllm-4.8.0/myllm/default_settings.toml`

 * *Files identical despite different names*

### Comparing `myllm-4.7.8/myllm/main.py` & `myllm-4.8.0/myllm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 
         Returns:
             A client object based on the specified protocol or None if the
             library is not supported.
 
         """
         library = kwargs.get("llm_library") or kwargs.get("library")
-        client_class = self.client_classes.get(f"{library.upper()}LLM")
+        client_class = self.client_classes.get(f"{library.capitalize()}Handler")
 
         if client_class is None:
             logger.error(f"library {library} not supported")
             return None
 
         return client_class(**kwargs)
 
@@ -147,15 +147,15 @@
         names of the classes and the values are the corresponding
         class objects.
 
         Returns:
             dict: A dictionary containing all the client classes
             from the `myllm.provider` module.
         """
-        provider_module = importlib.import_module("myllm.provider")
+        provider_module = importlib.import_module("myllm.handler")
         return {
             name: cls
             for name, cls in provider_module.__dict__.items()
             if isinstance(cls, type)
         }
 
     async def get_info(self):
```

### Comparing `myllm-4.7.8/myllm/provider/client.py` & `myllm-4.8.0/myllm/handler/client.py`

 * *Files identical despite different names*

### Comparing `myllm-4.7.8/myllm/provider/g4f.py` & `myllm-4.8.0/myllm/handler/g4f.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
 import importlib
 from time import sleep
 
 from loguru import logger
 
-from myllm.provider.client import AIClient
+from .client import AIClient
 
 
-class G4FLLM(AIClient):
+class G4fHandler(AIClient):
     """
     MyLLM class for G4F
 
     """
 
     def __init__(self, **kwargs):
         """
```

### Comparing `myllm-4.7.8/myllm/provider/gemini.py` & `myllm-4.8.0/myllm/handler/not_working/gemini.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 # """
 
 # from time import sleep
 
 # import google.generativeai as genai
 # from loguru import logger
 
-# from myllm.provider.client import AIClient
+# from .client import AIClient
 
 
-# class GeminiLLM(AIClient):
+# class GeminiHandler(AIClient):
 #     """
 #     MyLLM class for Bard
 
 #     """
 
 #     def __init__(self, **kwargs):
 #         """
 #         Initializes the object with the given keyword arguments.
-#         
+#
 
 #         Args:
 #             **kwargs: Variable length keyword arguments.
 
 #         Returns:
 #             None
 #         """
```

### Comparing `myllm-4.7.8/myllm/provider/openai.py` & `myllm-4.8.0/myllm/handler/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 """
 from time import sleep
 
 from loguru import logger
 from openai import OpenAI
 
-from myllm.provider.client import AIClient
+from .client import AIClient
 
 
-class OPENAILLM(AIClient):
+class OpenaiHandler(AIClient):
     """
     MyLLM class for OpenAI and LocalAI
 
     """
 
     def __init__(self, **kwargs):
         """
```

### Comparing `myllm-4.7.8/myllm/provider/petals.py` & `myllm-4.8.0/myllm/handler/not_working/petals.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # from time import sleep
 
 # from loguru import logger
 # from petals import AutoDistributedModelForCausalLM
 # from transformers import AutoTokenizer
 
-# from myllm.provider.client import AIClient
+# from .client import AIClient
 
 
 # class PetalsLLM(AIClient):
 #     """
 #     MyLLM class for Petals
 
 #     """
```

### Comparing `myllm-4.7.8/pyproject.toml` & `myllm-4.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MyLLM"
-version = "4.7.8"
+version = "4.8.0"
 description = "A python package to interact with llm model supported by g4f and langchain."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["chatgpt","llm","ai","llama","ai", "g4f", "freegpt"]
 packages = [
     {include = "myllm"}
@@ -23,15 +23,15 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = ">=0.95.2"
 uvicorn = ">=0.22.0"
 dynaconf = ">=3.2.0"
 loguru = ">=0.6.0"
 httpx = ">=0.24.1"
-g4f = "0.2.7.2"
+g4f = "0.2.8.0"
 js2py = "^0.74"
 PyExecJS2="1.6.1"
 curl_cffi = "0.6.2"
 Brotli = "1.1.0"
 openai = "1.16.2"
 # petals = "2.2.0.post1"
 # transformers = "4.32"
@@ -164,27 +164,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `myllm-4.7.8/PKG-INFO` & `myllm-4.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyLLM
-Version: 4.7.8
+Version: 4.8.0
 Summary: A python package to interact with llm model supported by g4f and langchain.
 License: MIT
 Keywords: chatgpt,llm,ai,llama,ai,g4f,freegpt
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Brotli (==1.1.0)
 Requires-Dist: PyExecJS2 (==1.6.1)
 Requires-Dist: curl_cffi (==0.6.2)
 Requires-Dist: dynaconf (>=3.2.0)
 Requires-Dist: fastapi (>=0.95.2)
-Requires-Dist: g4f (==0.2.7.2)
+Requires-Dist: g4f (==0.2.8.0)
 Requires-Dist: httpx (>=0.24.1)
 Requires-Dist: js2py (>=0.74,<0.75)
 Requires-Dist: loguru (>=0.6.0)
 Requires-Dist: openai (==1.16.2)
 Requires-Dist: uvicorn (>=0.22.0)
 Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/dev/CHANGELOG.rst
 Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: MyLLM Version: 4.7.8 Summary: A python package to
+Metadata-Version: 2.1 Name: MyLLM Version: 4.8.0 Summary: A python package to
 interact with llm model supported by g4f and langchain. License: MIT Keywords:
 chatgpt,llm,ai,llama,ai,g4f,freegpt Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: Brotli (==1.1.0) Requires-Dist:
 PyExecJS2 (==1.6.1) Requires-Dist: curl_cffi (==0.6.2) Requires-Dist: dynaconf
-(>=3.2.0) Requires-Dist: fastapi (>=0.95.2) Requires-Dist: g4f (==0.2.7.2)
+(>=3.2.0) Requires-Dist: fastapi (>=0.95.2) Requires-Dist: g4f (==0.2.8.0)
 Requires-Dist: httpx (>=0.24.1) Requires-Dist: js2py (>=0.74,<0.75) Requires-
 Dist: loguru (>=0.6.0) Requires-Dist: openai (==1.16.2) Requires-Dist: uvicorn
 (>=0.22.0) Project-URL: Changelog, https://github.com/mraniki/MyLLM/blob/dev/
 CHANGELOG.rst Project-URL: Issues, https://github.com/mraniki/MyLLM/issues
 Project-URL: Support, https://github.com/mraniki/MyLLM/discussions Description-
 Content-Type: text/markdown
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_W_i_k_i_-
```

