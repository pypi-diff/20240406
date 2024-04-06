# Comparing `tmp/ipython_openai-0.0.3.tar.gz` & `tmp/ipython_openai-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipython_openai-0.0.3.tar", last modified: Sat Apr  6 00:37:48 2024, max compression
+gzip compressed data, was "ipython_openai-0.0.4.tar", last modified: Sat Apr  6 01:30:31 2024, max compression
```

## Comparing `ipython_openai-0.0.3.tar` & `ipython_openai-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:37:48.187293 ipython_openai-0.0.3/
--rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 ipython_openai-0.0.3/LICENSE
--rw-r--r--   0 jordan     (501) staff       (20)     2151 2024-04-06 00:37:48.187186 ipython_openai-0.0.3/PKG-INFO
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:37:48.186380 ipython_openai-0.0.3/ipython_openai/
--rw-r--r--   0 jordan     (501) staff       (20)      116 2024-04-05 20:25:04.000000 ipython_openai-0.0.3/ipython_openai/__init__.py
--rw-r--r--   0 jordan     (501) staff       (20)     3860 2024-04-05 22:04:38.000000 ipython_openai-0.0.3/ipython_openai/gpt.py
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 00:37:48.187050 ipython_openai-0.0.3/ipython_openai.egg-info/
--rw-r--r--   0 jordan     (501) staff       (20)     2151 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/PKG-INFO
--rw-r--r--   0 jordan     (501) staff       (20)      295 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/SOURCES.txt
--rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/dependency_links.txt
--rw-r--r--   0 jordan     (501) staff       (20)       77 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/entry_points.txt
--rw-r--r--   0 jordan     (501) staff       (20)       51 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/requires.txt
--rw-r--r--   0 jordan     (501) staff       (20)       15 2024-04-06 00:37:48.000000 ipython_openai-0.0.3/ipython_openai.egg-info/top_level.txt
--rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-06 00:37:48.187338 ipython_openai-0.0.3/setup.cfg
--rw-r--r--   0 jordan     (501) staff       (20)      930 2024-04-06 00:34:47.000000 ipython_openai-0.0.3/setup.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 01:30:31.333882 ipython_openai-0.0.4/
+-rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 ipython_openai-0.0.4/LICENSE
+-rw-r--r--   0 jordan     (501) staff       (20)     2361 2024-04-06 01:30:31.333770 ipython_openai-0.0.4/PKG-INFO
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 01:30:31.332874 ipython_openai-0.0.4/ipython_openai/
+-rw-r--r--   0 jordan     (501) staff       (20)      116 2024-04-06 01:22:22.000000 ipython_openai-0.0.4/ipython_openai/__init__.py
+-rw-r--r--   0 jordan     (501) staff       (20)     3985 2024-04-06 01:28:46.000000 ipython_openai-0.0.4/ipython_openai/gpt.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 01:30:31.333620 ipython_openai-0.0.4/ipython_openai.egg-info/
+-rw-r--r--   0 jordan     (501) staff       (20)     2361 2024-04-06 01:30:31.000000 ipython_openai-0.0.4/ipython_openai.egg-info/PKG-INFO
+-rw-r--r--   0 jordan     (501) staff       (20)      295 2024-04-06 01:30:31.000000 ipython_openai-0.0.4/ipython_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-06 01:30:31.000000 ipython_openai-0.0.4/ipython_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       77 2024-04-06 01:30:31.000000 ipython_openai-0.0.4/ipython_openai.egg-info/entry_points.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       51 2024-04-06 01:30:31.000000 ipython_openai-0.0.4/ipython_openai.egg-info/requires.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       15 2024-04-06 01:30:31.000000 ipython_openai-0.0.4/ipython_openai.egg-info/top_level.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-06 01:30:31.333922 ipython_openai-0.0.4/setup.cfg
+-rw-r--r--   0 jordan     (501) staff       (20)      930 2024-04-06 01:28:58.000000 ipython_openai-0.0.4/setup.py
```

### Comparing `ipython_openai-0.0.3/LICENSE` & `ipython_openai-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipython_openai-0.0.3/PKG-INFO` & `ipython_openai-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython_openai
-Version: 0.0.3
+Version: 0.0.4
 Summary: An IPython extension for interacting with OpenAI's models
 Home-page: https://github.com/dustmason/ipython_openai
 Author: Jordan Sitkin
 Author-email: jordan@fiftyfootfoghorn.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -29,19 +29,24 @@
 Then, you can either load the extension during an ipython session with `%load_ext ipython_openai` or add the following
 to your ipython config.
 
 ```
 c.InteractiveShellApp.extensions = ['ipython_openai']
 ```
 
+## Configuration
+
+Your OpenAI API key should be available in the `OPENAI_API_KEY` env var. You can configure the model used by adding an
+entry to your ipython config: `c.GPT.model_name = 'gpt-4-turbo-preview'`.
+
 ## Usage
 
 This extension adds two new "magic" functions
 
-### `gen`
+## `gen`
 
 ```
 In [1]: gen a 5 line greeter function with randomness
 import random
 def greet():
     names = ["Alice", "Bob", "Charlie", "Diana", "Edward"]
     greeting = ["Hello", "Hi", "Hey", "Greetings", "What's up"]
@@ -49,15 +54,15 @@
 
 Run it? (y/n) y
 
 In [2]: greet()
 Hello, Bob!
 ```
 
-### `ask`
+## `ask`
 
 ```
 In [3]: ask what happened
 When the `greet()` function was called, the following occurred:
 1. The function selected a random name from the list `names`, which contains five different names: "Alice", "Bob", "Charlie", "Diana", and "Edward".
 2. It also selected a random greeting from the list `greeting`, which includes five different greetings: "Hello", "Hi", "Hey", "Greetings", and "What's up".
 3. It combined the selected greeting and name with a formatted string to create a message.
```

### Comparing `ipython_openai-0.0.3/ipython_openai/gpt.py` & `ipython_openai-0.0.4/ipython_openai/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 from prompt_toolkit import print_formatted_text
 from prompt_toolkit.formatted_text import PygmentsTokens
 from pygments.lexers.markup import MarkdownLexer
 from pygments.lexers.python import PythonLexer
 from pygments import lex
 
 from prompt_toolkit.shortcuts import confirm
+from traitlets import Unicode
 
 
 @magics_class
 class GPT(Magics):
+    model_name = Unicode("gpt-4-turbo-preview", config=True, help="OpenAI model name")
 
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self._samples: dict[int, str] = {}
 
     def _sample(self, line, system_message):
         history = self._history_lines()
         client = openai.OpenAI()
         response = client.chat.completions.create(
-            model="gpt-4-turbo-preview",
+            model=self.model_name,
             messages=[
                 system_message,
                 {"role": "user", "content": '\n'.join(history)},
                 {"role": "user", "content": line},
             ],
             max_tokens=2000,
             stream=True,
```

### Comparing `ipython_openai-0.0.3/ipython_openai.egg-info/PKG-INFO` & `ipython_openai-0.0.4/ipython_openai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipython-openai
-Version: 0.0.3
+Version: 0.0.4
 Summary: An IPython extension for interacting with OpenAI's models
 Home-page: https://github.com/dustmason/ipython_openai
 Author: Jordan Sitkin
 Author-email: jordan@fiftyfootfoghorn.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -29,19 +29,24 @@
 Then, you can either load the extension during an ipython session with `%load_ext ipython_openai` or add the following
 to your ipython config.
 
 ```
 c.InteractiveShellApp.extensions = ['ipython_openai']
 ```
 
+## Configuration
+
+Your OpenAI API key should be available in the `OPENAI_API_KEY` env var. You can configure the model used by adding an
+entry to your ipython config: `c.GPT.model_name = 'gpt-4-turbo-preview'`.
+
 ## Usage
 
 This extension adds two new "magic" functions
 
-### `gen`
+## `gen`
 
 ```
 In [1]: gen a 5 line greeter function with randomness
 import random
 def greet():
     names = ["Alice", "Bob", "Charlie", "Diana", "Edward"]
     greeting = ["Hello", "Hi", "Hey", "Greetings", "What's up"]
@@ -49,15 +54,15 @@
 
 Run it? (y/n) y
 
 In [2]: greet()
 Hello, Bob!
 ```
 
-### `ask`
+## `ask`
 
 ```
 In [3]: ask what happened
 When the `greet()` function was called, the following occurred:
 1. The function selected a random name from the list `names`, which contains five different names: "Alice", "Bob", "Charlie", "Diana", and "Edward".
 2. It also selected a random greeting from the list `greeting`, which includes five different greetings: "Hello", "Hi", "Hey", "Greetings", and "What's up".
 3. It combined the selected greeting and name with a formatted string to create a message.
```

### Comparing `ipython_openai-0.0.3/setup.py` & `ipython_openai-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipython_openai",
-    version="0.0.3",
+    version="0.0.4",
     author="Jordan Sitkin",
     author_email="jordan@fiftyfootfoghorn.com",
     description="An IPython extension for interacting with OpenAI's models",
     long_description=open('readme.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dustmason/ipython_openai",
     packages=find_packages(),
```

