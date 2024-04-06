# Comparing `tmp/scalesafe-0.0.2.tar.gz` & `tmp/scalesafe-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalesafe-0.0.2.tar", last modified: Sun Mar 24 20:21:39 2024, max compression
+gzip compressed data, was "scalesafe-0.0.3.tar", last modified: Sat Apr  6 14:54:44 2024, max compression
```

## Comparing `scalesafe-0.0.2.tar` & `scalesafe-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 20:21:39.691164 scalesafe-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-24 20:21:35.000000 scalesafe-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-24 20:21:35.000000 scalesafe-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-24 20:21:39.691164 scalesafe-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-24 20:21:35.000000 scalesafe-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-24 20:21:35.000000 scalesafe-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 20:21:39.691164 scalesafe-0.0.2/scalesafe/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 20:21:35.000000 scalesafe-0.0.2/scalesafe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 20:21:35.000000 scalesafe-0.0.2/scalesafe/benchmarking.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 20:21:35.000000 scalesafe-0.0.2/scalesafe/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-03-24 20:21:35.000000 scalesafe-0.0.2/scalesafe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-03-24 20:21:35.000000 scalesafe-0.0.2/scalesafe/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 20:21:35.000000 scalesafe-0.0.2/scalesafe/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-24 20:21:35.000000 scalesafe-0.0.2/scalesafe/onprem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-24 20:21:35.000000 scalesafe-0.0.2/scalesafe/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 20:21:39.691164 scalesafe-0.0.2/scalesafe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-24 20:21:39.000000 scalesafe-0.0.2/scalesafe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-24 20:21:39.000000 scalesafe-0.0.2/scalesafe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 20:21:39.000000 scalesafe-0.0.2/scalesafe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-24 20:21:39.000000 scalesafe-0.0.2/scalesafe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-24 20:21:39.000000 scalesafe-0.0.2/scalesafe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 20:21:39.691164 scalesafe-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-24 20:21:35.000000 scalesafe-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 20:21:39.691164 scalesafe-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-24 20:21:35.000000 scalesafe-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-24 20:21:35.000000 scalesafe-0.0.2/tests/example_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-24 20:21:35.000000 scalesafe-0.0.2/tests/test_generic_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:54:44.889133 scalesafe-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 14:54:41.000000 scalesafe-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-06 14:54:41.000000 scalesafe-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-06 14:54:44.889133 scalesafe-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-06 14:54:41.000000 scalesafe-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 14:54:41.000000 scalesafe-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:54:44.889133 scalesafe-0.0.3/scalesafe/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:54:41.000000 scalesafe-0.0.3/scalesafe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-06 14:54:41.000000 scalesafe-0.0.3/scalesafe/benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:54:41.000000 scalesafe-0.0.3/scalesafe/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-06 14:54:41.000000 scalesafe-0.0.3/scalesafe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-06 14:54:41.000000 scalesafe-0.0.3/scalesafe/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 14:54:41.000000 scalesafe-0.0.3/scalesafe/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-06 14:54:41.000000 scalesafe-0.0.3/scalesafe/onprem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-06 14:54:41.000000 scalesafe-0.0.3/scalesafe/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:54:44.889133 scalesafe-0.0.3/scalesafe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-06 14:54:44.000000 scalesafe-0.0.3/scalesafe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-06 14:54:44.000000 scalesafe-0.0.3/scalesafe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:54:44.000000 scalesafe-0.0.3/scalesafe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-06 14:54:44.000000 scalesafe-0.0.3/scalesafe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 14:54:44.000000 scalesafe-0.0.3/scalesafe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 14:54:44.889133 scalesafe-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-06 14:54:41.000000 scalesafe-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:54:44.889133 scalesafe-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-06 14:54:41.000000 scalesafe-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-06 14:54:41.000000 scalesafe-0.0.3/tests/example_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-06 14:54:41.000000 scalesafe-0.0.3/tests/test_generic_monitor.py
```

### Comparing `scalesafe-0.0.2/LICENSE` & `scalesafe-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scalesafe-0.0.2/PKG-INFO` & `scalesafe-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalesafe
-Version: 0.0.2
+Version: 0.0.3
 Summary: ScaleSafe Monitoring Engine: Toolkit for integrating monitoring into AI systems for compliance and safety.
 Home-page: https://scalesafe.ai
 Author: Tobin South
 Author-email: tsouth@mit.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `scalesafe-0.0.2/README.md` & `scalesafe-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 
 To integrate with your app, choose the appropriate monitoring class and include it with your AI system / model usage. 
 
 ```bash
 pip install scalesafe
 ```
 
-### OpenAI Chat Example
+#### API Keys
+For anything here to connect to the server, you need to set your API key. You can find your model-specific secret at [app.scalesafe.ai/models/<model>/api-keys](app.scalesafe.ai/models/<model>/api-keys). You can pass them to any function with `api_key=` or set them as an environment variable `SCALESAFE_API_KEY`. The key will look something like `sk-72cb69c4af4d406c854d135b66b67f-iy6liAQuToYDBIA1h44bfTq7Rgj1`. All monitoring, benchmarking, screening, and human-in-the-loop controls are unique to the model and its use case.
+
+### Monitoring OpenAI Chat Example
 When a synchronous AI model is being used, you just need to monitor the input and output of the model. This can be done with the `OpenAIChatMonitor` class.
 ```python
 from scalesafe.openai import OpenAIChatMonitor
 from openai import OpenAI
 
 client = OpenAI()
 monitor = OpenAIChatMonitor() # We create a monitor instance
@@ -41,28 +44,41 @@
 try:
     monitor.monitor(response, user_inputs, screen_inputs=True, screen_outputs=True)
 except (UnsafeInputError, BannedOutputError) as e:
     print(f"Bad model usage. Error: {e}")
 ```
 
 ### Check Compliance Status
-If want to check if the model is still compliant with the requirements (which update overtime as regulation chnages), you can use the `status` method.
+If want to check if the model is still compliant with the requirements (which update overtime as regulation changes), you can use the `status` method.
 ```python
 from scalesafe.exceptions import OutOfComplianceError, HumanReviewNeededException
 try:
     monitor.status()
 except OutOfComplianceError as e:
     print(f"Model is out of compliance. Error: {e}")
 ```
 
-### Human in the loop
+### Complete Required Benchmarks
+Some applications require that you complete certain benchmarks to ensure compliance. 
+```python
+from scalesafe.benchmarking import Benchmarker
+dataset = Benchmarker('nyEmploymentScreening') # Example bias screening for employment AI in New York
+
+for item in dataset:
+    print(item)  # Process the batch here
+    result = True if np.random.random() > 0.5 else False # Do some AI
+    dataset.answer(result, item['id'])  # We add our responses to the buffer
 
+dataset.post_answers() # We send them to our audit team for analysis
+```
 
+<!-- ### Human in the loop -->
 
 
+## Other examples
 
 ### For OpenAI Assistants
 This can be a little more complicated, as we're no longer working synchronously. We still need to monitor all the usage of the model (including start and end time). The simplest way to format this is to use the `OpenAIAssistantMonitor` class.
 ```python
 from scalesafe.openai import OpenAIAssistantMonitor
 from openai import OpenAI
```

### Comparing `scalesafe-0.0.2/scalesafe/exceptions.py` & `scalesafe-0.0.3/scalesafe/exceptions.py`

 * *Files identical despite different names*

### Comparing `scalesafe-0.0.2/scalesafe/generic.py` & `scalesafe-0.0.3/scalesafe/generic.py`

 * *Files identical despite different names*

### Comparing `scalesafe-0.0.2/scalesafe/openai.py` & `scalesafe-0.0.3/scalesafe/openai.py`

 * *Files identical despite different names*

### Comparing `scalesafe-0.0.2/scalesafe.egg-info/PKG-INFO` & `scalesafe-0.0.3/scalesafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalesafe
-Version: 0.0.2
+Version: 0.0.3
 Summary: ScaleSafe Monitoring Engine: Toolkit for integrating monitoring into AI systems for compliance and safety.
 Home-page: https://scalesafe.ai
 Author: Tobin South
 Author-email: tsouth@mit.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `scalesafe-0.0.2/setup.py` & `scalesafe-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     install_requires = f.read().splitlines()
 
 setup(
     name='scalesafe',
-    version='0.0.2',  # Semantic Versioning (https://semver.org/)
+    version='0.0.3',  # Semantic Versioning (https://semver.org/)
     description='ScaleSafe Monitoring Engine: Toolkit for integrating monitoring into AI systems for compliance and safety.',
     long_description="""
         ScaleSafe is an open-source toolkit designed to integrate monitoring into AI systems, 
         supporting compliance with the EU AI Act, New York Bill 144, and other regulations. 
         It offers functionalities for logging AI usage, screening responses, handling human-in-the-loop control, 
         and conducting risk and compliance audits.
     """,
```

### Comparing `scalesafe-0.0.2/tests/example_usage.py` & `scalesafe-0.0.3/tests/example_usage.py`

 * *Files identical despite different names*

### Comparing `scalesafe-0.0.2/tests/test_generic_monitor.py` & `scalesafe-0.0.3/tests/test_generic_monitor.py`

 * *Files identical despite different names*

