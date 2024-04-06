# Comparing `tmp/GABRIEL-ratings-0.1.0.tar.gz` & `tmp/GABRIEL-ratings-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GABRIEL-ratings-0.1.0.tar", last modified: Fri Mar 22 14:15:15 2024, max compression
+gzip compressed data, was "dist/GABRIEL-ratings-0.1.3.tar", last modified: Sat Apr  6 20:09:52 2024, max compression
```

## Comparing `GABRIEL-ratings-0.1.0.tar` & `GABRIEL-ratings-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-03-22 14:15:15.365959 GABRIEL-ratings-0.1.0/
-drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-03-22 14:15:15.364723 GABRIEL-ratings-0.1.0/GABRIEL/
-drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-03-22 14:15:15.365018 GABRIEL-ratings-0.1.0/GABRIEL/Prompts/
--rw-r--r--   0 elliottmokski   (501) staff       (20)        0 2024-03-22 12:02:02.000000 GABRIEL-ratings-0.1.0/GABRIEL/Prompts/__init__.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)        0 2024-03-22 10:50:50.000000 GABRIEL-ratings-0.1.0/GABRIEL/__init__.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     4773 2024-03-22 12:33:14.000000 GABRIEL-ratings-0.1.0/GABRIEL/combined_assistant.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     2244 2024-03-22 13:16:33.000000 GABRIEL-ratings-0.1.0/GABRIEL/decorators.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     4208 2024-03-22 11:45:40.000000 GABRIEL-ratings-0.1.0/GABRIEL/foundational_functions.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     5206 2024-03-22 13:16:45.000000 GABRIEL-ratings-0.1.0/GABRIEL/openai_api_calls.py
--rw-r--r--   0 elliottmokski   (501) staff       (20)     1116 2024-03-22 13:16:51.000000 GABRIEL-ratings-0.1.0/GABRIEL/prompt_wrapping.py
-drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-03-22 14:15:15.365645 GABRIEL-ratings-0.1.0/GABRIEL_ratings.egg-info/
--rw-r--r--   0 elliottmokski   (501) staff       (20)      814 2024-03-22 14:15:15.000000 GABRIEL-ratings-0.1.0/GABRIEL_ratings.egg-info/PKG-INFO
--rw-r--r--   0 elliottmokski   (501) staff       (20)      413 2024-03-22 14:15:15.000000 GABRIEL-ratings-0.1.0/GABRIEL_ratings.egg-info/SOURCES.txt
--rw-r--r--   0 elliottmokski   (501) staff       (20)        1 2024-03-22 14:15:15.000000 GABRIEL-ratings-0.1.0/GABRIEL_ratings.egg-info/dependency_links.txt
--rw-r--r--   0 elliottmokski   (501) staff       (20)       57 2024-03-22 14:15:15.000000 GABRIEL-ratings-0.1.0/GABRIEL_ratings.egg-info/requires.txt
--rw-r--r--   0 elliottmokski   (501) staff       (20)        8 2024-03-22 14:15:15.000000 GABRIEL-ratings-0.1.0/GABRIEL_ratings.egg-info/top_level.txt
--rw-r--r--   0 elliottmokski   (501) staff       (20)       41 2024-03-22 11:53:15.000000 GABRIEL-ratings-0.1.0/MANIFEST.in
--rw-r--r--   0 elliottmokski   (501) staff       (20)      814 2024-03-22 14:15:15.365812 GABRIEL-ratings-0.1.0/PKG-INFO
--rw-r--r--   0 elliottmokski   (501) staff       (20)      235 2024-03-22 11:08:08.000000 GABRIEL-ratings-0.1.0/README.md
--rw-r--r--   0 elliottmokski   (501) staff       (20)       38 2024-03-22 14:15:15.366003 GABRIEL-ratings-0.1.0/setup.cfg
--rw-r--r--   0 elliottmokski   (501) staff       (20)      891 2024-03-22 14:11:18.000000 GABRIEL-ratings-0.1.0/setup.py
+drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-06 20:09:52.250261 GABRIEL-ratings-0.1.3/
+drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-06 20:09:52.248212 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     7037 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/PKG-INFO
+-rw-r--r--   0 elliottmokski   (501) staff       (20)      434 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/SOURCES.txt
+-rw-r--r--   0 elliottmokski   (501) staff       (20)        1 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/dependency_links.txt
+-rw-r--r--   0 elliottmokski   (501) staff       (20)       70 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/requires.txt
+-rw-r--r--   0 elliottmokski   (501) staff       (20)        8 2024-04-06 20:09:52.000000 GABRIEL-ratings-0.1.3/GABRIEL_ratings.egg-info/top_level.txt
+-rw-r--r--   0 elliottmokski   (501) staff       (20)       41 2024-03-22 11:53:15.000000 GABRIEL-ratings-0.1.3/MANIFEST.in
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     7037 2024-04-06 20:09:52.250113 GABRIEL-ratings-0.1.3/PKG-INFO
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     5858 2024-04-06 20:09:14.000000 GABRIEL-ratings-0.1.3/README.md
+drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-06 20:09:52.249711 GABRIEL-ratings-0.1.3/gabriel/
+drwxr-xr-x   0 elliottmokski   (501) staff       (20)        0 2024-04-06 20:09:52.249942 GABRIEL-ratings-0.1.3/gabriel/Prompts/
+-rw-r--r--   0 elliottmokski   (501) staff       (20)        0 2024-03-22 12:02:02.000000 GABRIEL-ratings-0.1.3/gabriel/Prompts/__init__.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)        0 2024-03-22 10:50:50.000000 GABRIEL-ratings-0.1.3/gabriel/__init__.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     7894 2024-04-06 20:06:07.000000 GABRIEL-ratings-0.1.3/gabriel/archangel.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     6899 2024-04-06 19:56:15.000000 GABRIEL-ratings-0.1.3/gabriel/combined_assistant.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     2292 2024-04-06 19:55:40.000000 GABRIEL-ratings-0.1.3/gabriel/decorators.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     7178 2024-04-06 19:51:15.000000 GABRIEL-ratings-0.1.3/gabriel/foundational_functions.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     5206 2024-04-06 19:57:30.000000 GABRIEL-ratings-0.1.3/gabriel/openai_api_calls.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)     1049 2024-04-06 19:51:29.000000 GABRIEL-ratings-0.1.3/gabriel/prompt_wrapping.py
+-rw-r--r--   0 elliottmokski   (501) staff       (20)       38 2024-04-06 20:09:52.250308 GABRIEL-ratings-0.1.3/setup.cfg
+-rw-r--r--   0 elliottmokski   (501) staff       (20)      915 2024-04-06 20:03:15.000000 GABRIEL-ratings-0.1.3/setup.py
```

### Comparing `GABRIEL-ratings-0.1.0/GABRIEL/combined_assistant.py` & `GABRIEL-ratings-0.1.3/gabriel/combined_assistant.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from GABRIEL.foundational_functions import *
+from gabriel.foundational_functions import *
 import json
 import pandas as pd
 import numpy as np
 
 class CombinedAssistant:
     def __init__(self, api_key, drive_folder = None, model='gpt-3.5-turbo-0125'):
         self.drive_folder = drive_folder
@@ -81,8 +81,52 @@
                         passage_data[attribute] = rating_value
 
                     dfs.append(passage_data)
             except:
                 pass
         output_df = pd.DataFrame(dfs)
         print(output_df)
+        return output_df
+    
+    def rate_single_text(self, text, attribute_dict, entity_category, attribute_category, temperature,use_classification, format, classification_clarification, 
+                                project_probs, truncate, model, seed, api_key, truncate_len, timeout):
+        
+        if use_classification:
+            rating_function = generate_simple_classification
+            attribute_param = 'classification category'
+        else:
+            rating_function = generate_full_ratings
+            attribute_param = 'attribute'
+
+        if truncate: 
+            try:
+                text = ' '.join(text.split()[:truncate_len])
+            except:
+                pass
+        
+        dfs = list()
+        # descriptions = list(attribute_dict.values())
+        attributes = list(attribute_dict.keys())
+        try:
+            raw_ratings = rating_function(attribute_dict=attribute_dict,attributes = attributes,
+                                                passage = text, entity_category= entity_category, 
+                                                attribute_category=attribute_category,format = format,
+                                                temperature = temperature, model = model, seed = seed, 
+                                                api_key = api_key, timeout = timeout)
+            
+            if format == 'json':
+                ratings = json.loads(raw_ratings)
+                output_df = pd.DataFrame.from_dict(ratings, orient = 'index').T
+                output_df['Text'] = text
+                output_df = output_df.set_index('Text').reset_index()
+                 # passage_data = {'Text': text}
+                # for rating in ratings:
+                #     attribute = rating[attribute_param]
+                #     rating_value = rating['rating']
+                #     if project_probs:
+                #         rating_value = float(rating_value) / 100
+                #         rating_value = 1 / (1 + np.exp(-24 * (rating_value - 0.5)))
+                #     passage_data[attribute] = rating_value
+
+        except:
+            output_df = None
         return output_df
```

### Comparing `GABRIEL-ratings-0.1.0/GABRIEL/decorators.py` & `GABRIEL-ratings-0.1.3/gabriel/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 import time 
 import os
 
 class APIError(Exception):
     pass
 
-from GABRIEL import foundational_functions
+from gabriel import foundational_functions
 
 # Determine the path to the 'Prompts' folder dynamically
 package_dir = os.path.dirname(os.path.abspath(foundational_functions.__file__))
 templates_dir = os.path.join(package_dir, 'Prompts')
 
 env = Environment(
     loader=FileSystemLoader(templates_dir),
@@ -24,14 +24,15 @@
         def wrapper(*args, **kwargs):
             # Extract additional context for the template from kwargs
             context = kwargs.pop('template_context', {})
             
             # Load and render the template
             template = env.get_template(f"{template_name}.j2")
             prompt = template.render(**context)
+            # print("Rendered Prompt:", prompt)
             
             # Execute the wrapped function with the rendered prompt and any remaining kwargs
             return func(prompt, *args, **kwargs)
         return wrapper
     return decorator
 
 def retry_on_api_error(max_retries, delay=45):
```

### Comparing `GABRIEL-ratings-0.1.0/GABRIEL/openai_api_calls.py` & `GABRIEL-ratings-0.1.3/gabriel/openai_api_calls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 import openai
 import queue
 import threading
 import time
 from jinja2 import Environment, FileSystemLoader, select_autoescape
-from GABRIEL import foundational_functions
+from gabriel import foundational_functions
 
 import os
 
 # Determine the path to the 'Prompts' folder dynamically
 package_dir = os.path.dirname(os.path.abspath(foundational_functions.__file__))
 templates_dir = os.path.join(package_dir, 'Prompts')
 env = Environment(
@@ -77,15 +77,15 @@
 class ChatAssistant:
     def __init__(self, model, api_key):
         self.model = model
         self.client = openai.OpenAI(api_key = api_key)
 
     @retry_on_api_error(max_retries=3)
     def generate_response(self, prompt, system_instruction, external_messages=None, timeout=100, 
-                          temperature=0.9, max_tokens=1500, desired_response_format='text', seed = None):
+                          temperature=0.9, max_tokens=2000, desired_response_format='text', seed = None):
         response_queue = queue.Queue()
 
         def target():
             nonlocal response_queue, external_messages
 
             # Compose messages for the API call
             messages = [{"role": "system", "content": system_instruction}]
```

### Comparing `GABRIEL-ratings-0.1.0/GABRIEL/prompt_wrapping.py` & `GABRIEL-ratings-0.1.3/gabriel/prompt_wrapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import functools
 from jinja2 import Environment, FileSystemLoader, select_autoescape
-
-# Assuming your Jinja2 templates are in the 'templates' directory
-from GABRIEL import foundational_functions
+from gabriel import foundational_functions
 import os
 
 # Determine the path to the 'Prompts' folder dynamically
 package_dir = os.path.dirname(os.path.abspath(foundational_functions.__file__))
 templates_dir = os.path.join(package_dir, 'Prompts')
 
 env = Environment(
```

### Comparing `GABRIEL-ratings-0.1.0/setup.py` & `GABRIEL-ratings-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GABRIEL-ratings', 
-    version='0.1.0',  
+    version='0.1.3',  
     author='Hemanth Asirvatham and Elliott Mokski',  
     author_email='elliottpmokski@gmail.com',  
     description='THE GABRIEL library for numerical analysis of texts in the social sciences.', 
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/elliottmokski/GABRIEL-distribution',  
     packages=find_packages(),
     include_package_data=True,
     package_data={
-        'GABRIEL': ['Prompts/*.j2'],
+        'gabriel': ['Prompts/*.j2'],
     },
     install_requires=[
         'numpy>=1.18.0',
         'pandas>=1.0.0',
         'openai>=1.0.0',
-        'Jinja2>=2.11.0'
+        'Jinja2>=2.11.0',
+        'tqdm>=4.42.0'
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)'],
     python_requires='>=3.6'
 )
```

