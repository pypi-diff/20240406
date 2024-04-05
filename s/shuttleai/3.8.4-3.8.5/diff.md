# Comparing `tmp/shuttleai-3.8.4.tar.gz` & `tmp/shuttleai-3.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.8.4.tar", last modified: Fri Apr  5 20:22:18 2024, max compression
+gzip compressed data, was "shuttleai-3.8.5.tar", last modified: Fri Apr  5 22:38:02 2024, max compression
```

## Comparing `shuttleai-3.8.4.tar` & `shuttleai-3.8.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.384580 shuttleai-3.8.4/
--rw-rw-rw-   0        0        0     4109 2024-04-05 20:22:18.382582 shuttleai-3.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 20:22:18.384580 shuttleai-3.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1321 2024-04-05 20:21:42.000000 shuttleai-3.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.314577 shuttleai-3.8.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.322581 shuttleai-3.8.4/src/shuttleai/
--rw-rw-rw-   0        0        0      576 2024-04-05 20:21:58.000000 shuttleai-3.8.4/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.4/src/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.373581 shuttleai-3.8.4/src/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.4/src/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17420 2024-04-05 20:22:01.000000 shuttleai-3.8.4/src/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0    15283 2024-04-05 20:22:03.000000 shuttleai-3.8.4/src/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.4/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.377581 shuttleai-3.8.4/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.4/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.8.4/src/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:22:18.379581 shuttleai-3.8.4/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4109 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 20:22:18.000000 shuttleai-3.8.4/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.888396 shuttleai-3.8.5/
+-rw-rw-rw-   0        0        0     4084 2024-04-05 22:38:02.885383 shuttleai-3.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 22:38:02.888396 shuttleai-3.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2024-04-05 22:37:34.000000 shuttleai-3.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.800159 shuttleai-3.8.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.806681 shuttleai-3.8.5/src/shuttleai/
+-rw-rw-rw-   0        0        0      576 2024-04-05 22:37:41.000000 shuttleai-3.8.5/src/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:54:56.000000 shuttleai-3.8.5/src/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.877868 shuttleai-3.8.5/src/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-03 19:49:40.000000 shuttleai-3.8.5/src/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17322 2024-04-05 22:37:02.000000 shuttleai-3.8.5/src/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0    15233 2024-04-05 22:36:13.000000 shuttleai-3.8.5/src/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8.5/src/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.880866 shuttleai-3.8.5/src/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8.5/src/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     4108 2024-04-05 22:32:01.000000 shuttleai-3.8.5/src/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:38:02.882865 shuttleai-3.8.5/src/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4084 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-05 22:38:02.000000 shuttleai-3.8.5/src/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.8.4/PKG-INFO` & `shuttleai-3.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.4
+Version: 3.8.5
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: httpx
 Requires-Dist: orjson
-Requires-Dist: pydantic
 Provides-Extra: cli
 Requires-Dist: asyncclick; extra == "cli"
 Requires-Dist: pystyle; extra == "cli"
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
```

### Comparing `shuttleai-3.8.4/README.md` & `shuttleai-3.8.5/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.4/setup.py` & `shuttleai-3.8.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,19 @@
     packages=find_packages("src"),
     package_dir={"": "src"},
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=[
         'aiohttp',
         'httpx',
-        'orjson',
-        'pydantic'
+        'orjson'
     ],
     extras_require={
         'cli': ['asyncclick', 'pystyle']
     },
     keywords=['shuttleai', 'ai', 'gpt', 'claude', 'api', 'free', 'chatgpt', 'gpt-4'],
     url='https://github.com/shuttleai/shuttleai-python',
     entry_points={
```

### Comparing `shuttleai-3.8.4/src/shuttleai/__init__.py` & `shuttleai-3.8.5/src/shuttleai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .client import ShuttleAsyncClient, ShuttleClient
 
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.8.4"
+__version__ = "3.8.5"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
```

### Comparing `shuttleai-3.8.4/src/shuttleai/cli.py` & `shuttleai-3.8.5/src/shuttleai/cli.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.4/src/shuttleai/client/_async.py` & `shuttleai-3.8.5/src/shuttleai/client/_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -280,30 +280,30 @@
             response = await self._make_request(
                 "POST", "chat/completions", data, headers={"Authorization": f"Bearer {self.api_key}"}, stream=stream
             )
             if stream:
                 async def streamer():
                     async for chunk in response:
                         try:
-                            yield ChatChunk.model_validate(chunk)
+                            yield ChatChunk.from_dict(chunk)
                         except:
                             try:
-                                yield ShuttleError.model_validate(chunk)
+                                yield ShuttleError(**chunk)
                             except:
                                 try:
                                     yield chunk
                                 except:
                                     pass
                 return streamer()
             else:
                 try:
-                    return Chat.model_validate(response)
+                    return Chat.from_dict(response)
                 except:
                     try:
-                        return ShuttleError.model_validate(response)
+                        return ShuttleError(**response)
                     except:
                         return response
 
         except aiohttp.ClientError as e:
             log.error(f"Failed to get chat completions: {e}")
             raise
 
@@ -330,18 +330,18 @@
         """
         try:
             data = {"model": model, "prompt": prompt, "n": n}
             response = await self._make_request(
                 "POST", "images/generations", data, headers={"Authorization": f"Bearer {self.api_key}"}
             )
             try:
-                return Image.model_validate(response)
+                return Image.from_dict(response)
             except:
                 try:
-                    return ShuttleError.model_validate(response)
+                    return ShuttleError(**response)
                 except:
                     return response
         except aiohttp.ClientError as e:
             log.error(f"Failed to generate images: {e}")
             raise
 
     async def audio_generations(
@@ -367,18 +367,18 @@
         """
         try:
             data = {"model": model, "input": input, "voice": voice}
             response = await self._make_request(
                 "POST", "audio/generations", data, headers={"Authorization": f"Bearer {self.api_key}"}
             )
             try:
-                return Audio.model_validate(response)
+                return Audio.from_dict(response)
             except:
                 try:
-                    return ShuttleError.model_validate(response)
+                    return ShuttleError(**response)
                 except:
                     return response
         except aiohttp.ClientError as e:
             log.error(f"Failed to generate audio: {e}")
             raise
 
     async def audio_transcriptions(
@@ -457,16 +457,16 @@
         try:
             input = [input] if isinstance(input, str) else input
             data = {"model": model, "input": input, "encoding_format": "float"}
             response = await self._make_request(
                 "POST", "embeddings", data, headers={"Authorization": f"Bearer {self.api_key}"}
             )
             try:
-                return Embedding.model_validate(response)
+                return Embedding(**response)
             except:
                 try:
-                    return ShuttleError.model_validate(response)
+                    return ShuttleError(**response)
                 except:
                     return response
         except aiohttp.ClientError as e:
             log.error(f"Failed to generate embeddings: {e}")
             raise
```

### Comparing `shuttleai-3.8.4/src/shuttleai/client/_sync.py` & `shuttleai-3.8.5/src/shuttleai/client/_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
         Raises:
             httpx.HTTPError: If the API request failed.
         """
         try:
             params = {"endpoints": endpoint,
                       **({"format": "free"} if free else {"format": "premium"} if premium else {})}
-            return Models.model_validate(self._make_request("GET", "models", params=params))
+            return Models.from_dict(self._make_request("GET", "models", params=params))
         except httpx.HTTPError as e:
             log.error(f"Failed to retrieve models: {e}")
             raise
 
     def chat_completion(
         self,
         model: str,
@@ -213,30 +213,31 @@
             response = self._make_request(
                 "POST", "chat/completions", data, stream=stream
             )
             if stream:
                 def streamer():
                     for chunk in response:
                         try:
-                            yield ChatChunk.model_validate(chunk)
-                        except:
+                            yield ChatChunk.from_dict(chunk)
+                        except Exception as e:
+                            print(e)
                             try:
-                                yield ShuttleError.model_validate(chunk)
+                                yield ShuttleError(**chunk)
                             except:
                                 try:
                                     yield chunk
                                 except:
                                     pass
                 return streamer()
             else:
                 try:
-                    return Chat.model_validate(response)
+                    return Chat.from_dict(response)
                 except:
                     try:
-                        return ShuttleError.model_validate(response)
+                        return ShuttleError(**response)
                     except:
                         return response
 
         except httpx.HTTPError as e:
             log.error(f"Failed to get chat completions: {e}")
             raise
 
@@ -263,18 +264,18 @@
         """
         try:
             data = {"model": model, "prompt": prompt, "n": n}
             response = self._make_request(
                 "POST", "images/generations", data, headers={"Authorization": f"Bearer {self.api_key}"}
             )
             try:
-                return Image.model_validate(response)
+                return Image.from_dict(response)
             except:
                 try:
-                    return ShuttleError.model_validate(response)
+                    return ShuttleError(**response)
                 except:
                     return response
         except httpx.HTTPError as e:
             log.error(f"Failed to generate images: {e}")
             raise
 
     def audio_generations(
@@ -300,18 +301,18 @@
         """
         try:
             data = {"model": model, "input": input, "voice": voice}
             response = self._make_request(
                 "POST", "audio/generations", data, headers={"Authorization": f"Bearer {self.api_key}"}
             )
             try:
-                return Audio.model_validate(response)
+                return Audio.from_dict(response)
             except:
                 try:
-                    return ShuttleError.model_validate(response)
+                    return ShuttleError(**response)
                 except:
                     return response
         except httpx.HTTPError as e:
             log.error(f"Failed to generate audio: {e}")
             raise
 
     def audio_transcriptions(
@@ -390,16 +391,16 @@
         try:
             input = [input] if isinstance(input, str) else input
             data = {"model": model, "input": input, "encoding_format": "float"}
             response = self._make_request(
                 "POST", "embeddings", data, headers={"Authorization": f"Bearer {self.api_key}"}
             )
             try:
-                return Embedding.model_validate(response)
+                return Embedding(**response)
             except:
                 try:
-                    return ShuttleError.model_validate(response)
+                    return ShuttleError(**response)
                 except:
                     return response
         except httpx.HTTPError as e:
             log.error(f"Failed to generate embeddings: {e}")
             raise
```

### Comparing `shuttleai-3.8.4/src/shuttleai/log.py` & `shuttleai-3.8.5/src/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.8.4/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.8.5/src/shuttleai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.8.4
+Version: 3.8.5
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: httpx
 Requires-Dist: orjson
-Requires-Dist: pydantic
 Provides-Extra: cli
 Requires-Dist: asyncclick; extra == "cli"
 Requires-Dist: pystyle; extra == "cli"
 
 # The official Python library for the ShuttleAI API
 Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
```

