# Comparing `tmp/ABSQL-0.5.1.tar.gz` & `tmp/ABSQL-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABSQL-0.5.1.tar", last modified: Sat Apr  6 01:04:15 2024, max compression
+gzip compressed data, was "ABSQL-0.5.2.tar", last modified: Sat Apr  6 01:50:25 2024, max compression
```

## Comparing `ABSQL-0.5.1.tar` & `ABSQL-0.5.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.045240 ABSQL-0.5.1/
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.044434 ABSQL-0.5.1/ABSQL.egg-info/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9773 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/SOURCES.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/dependency_links.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       65 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/requires.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/top_level.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 ABSQL-0.5.1/LICENSE
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9773 2024-04-06 01:04:15.044823 ABSQL-0.5.1/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 ABSQL-0.5.1/README.md
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.037192 ABSQL-0.5.1/absql/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 ABSQL-0.5.1/absql/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.038014 ABSQL-0.5.1/absql/files/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      740 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/files/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 ABSQL-0.5.1/absql/files/loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2606 2024-02-09 23:11:51.000000 ABSQL-0.5.1/absql/files/parsers.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.039342 ABSQL-0.5.1/absql/functions/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/functions/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 ABSQL-0.5.1/absql/functions/db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/functions/env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/functions/time.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.039715 ABSQL-0.5.1/absql/render/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3068 2024-04-06 01:03:31.000000 ABSQL-0.5.1/absql/render/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.039999 ABSQL-0.5.1/absql/text/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/text/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.040247 ABSQL-0.5.1/absql/utils/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/utils/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-06 01:04:15.045309 ABSQL-0.5.1/setup.cfg
--rw-r--r--   0 chriscardillo   (501) staff       (20)      826 2024-04-06 01:03:31.000000 ABSQL-0.5.1/setup.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.044110 ABSQL-0.5.1/tests/
--rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_copy.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_funcs_db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_funcs_env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_funcs_time.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      909 2024-01-03 15:37:15.000000 ABSQL-0.5.1/tests/test_parse_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 ABSQL-0.5.1/tests/test_partial_kwargs.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 ABSQL-0.5.1/tests/test_render.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3575 2024-02-09 23:11:51.000000 ABSQL-0.5.1/tests/test_render_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      641 2024-04-06 01:03:31.000000 ABSQL-0.5.1/tests/test_render_file_return_dict.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_render_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_set.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_utils.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.503510 ABSQL-0.5.2/
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.501143 ABSQL-0.5.2/ABSQL.egg-info/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9773 2024-04-06 01:50:25.000000 ABSQL-0.5.2/ABSQL.egg-info/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-06 01:50:25.000000 ABSQL-0.5.2/ABSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-06 01:50:25.000000 ABSQL-0.5.2/ABSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       65 2024-04-06 01:50:25.000000 ABSQL-0.5.2/ABSQL.egg-info/requires.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-06 01:50:25.000000 ABSQL-0.5.2/ABSQL.egg-info/top_level.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 ABSQL-0.5.2/LICENSE
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9773 2024-04-06 01:50:25.502323 ABSQL-0.5.2/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 ABSQL-0.5.2/README.md
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.485534 ABSQL-0.5.2/absql/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 ABSQL-0.5.2/absql/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.487923 ABSQL-0.5.2/absql/files/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      792 2024-04-06 01:44:58.000000 ABSQL-0.5.2/absql/files/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 ABSQL-0.5.2/absql/files/loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2614 2024-04-06 01:48:02.000000 ABSQL-0.5.2/absql/files/parsers.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.489997 ABSQL-0.5.2/absql/functions/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 ABSQL-0.5.2/absql/functions/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 ABSQL-0.5.2/absql/functions/db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 ABSQL-0.5.2/absql/functions/env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 ABSQL-0.5.2/absql/functions/time.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.490847 ABSQL-0.5.2/absql/render/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3068 2024-04-06 01:03:31.000000 ABSQL-0.5.2/absql/render/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.491374 ABSQL-0.5.2/absql/text/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 ABSQL-0.5.2/absql/text/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.491895 ABSQL-0.5.2/absql/utils/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 ABSQL-0.5.2/absql/utils/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-06 01:50:25.503653 ABSQL-0.5.2/setup.cfg
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      826 2024-04-06 01:45:57.000000 ABSQL-0.5.2/setup.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:50:25.500418 ABSQL-0.5.2/tests/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_copy.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_funcs_db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_funcs_env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_funcs_time.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      909 2024-01-03 15:37:15.000000 ABSQL-0.5.2/tests/test_parse_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 ABSQL-0.5.2/tests/test_partial_kwargs.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 ABSQL-0.5.2/tests/test_render.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3575 2024-02-09 23:11:51.000000 ABSQL-0.5.2/tests/test_render_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      641 2024-04-06 01:03:31.000000 ABSQL-0.5.2/tests/test_render_file_return_dict.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_render_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_set.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 ABSQL-0.5.2/tests/test_utils.py
```

### Comparing `ABSQL-0.5.1/ABSQL.egg-info/PKG-INFO` & `ABSQL-0.5.2/ABSQL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.5.1
+Version: 0.5.2
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.5.1/ABSQL.egg-info/SOURCES.txt` & `ABSQL-0.5.2/ABSQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/LICENSE` & `ABSQL-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/PKG-INFO` & `ABSQL-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.5.1
+Version: 0.5.2
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.5.1/README.md` & `ABSQL-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/absql/__init__.py` & `ABSQL-0.5.2/absql/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/absql/files/__init__.py` & `ABSQL-0.5.2/absql/files/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from absql.utils import get_function_arg_names
 from absql.files.loader import generate_loader
 from absql.files.parsers import parse_generic, parse_sql
 
 default_parsers = {
     ".yml": parse_generic,
     ".yaml": parse_generic,
+    ".js": parse_generic,
+    ".py": parse_generic,
     ".sql": parse_sql,
 }
 
 accepted_file_types = tuple(default_parsers.keys())
 
 
 def parse(file_path, parse_dict=default_parsers, loader=None):
```

### Comparing `ABSQL-0.5.1/absql/files/loader.py` & `ABSQL-0.5.2/absql/files/loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/absql/files/parsers.py` & `ABSQL-0.5.2/absql/files/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             content = content.strip("\n")
         elif text.startswith("{"):
             tmp_header = "/*ABSQLQSBA*/ "
             text = tmp_header + text
             metadata = {}
             content = yaml.load(text, Loader=loader)
             content = content.replace(tmp_header, "")
-        elif text.startswith("/*") and file_path.endswith(".sql"):
+        elif text.startswith("/*") and file_path.endswith((".sql", "js")):
             # Retrieve the first matched set of text within a block comment
             # (i.e. /* ... */).
             metadata = (
                 re.compile(r"^\/\*([\S\s]*?)\*\/$", re.MULTILINE).match(text).group(1)
             )
             # Text after the first block-comment end is considered the content of the
             # SQL file. This will handle block comments within the contents as well.
```

### Comparing `ABSQL-0.5.1/absql/functions/__init__.py` & `ABSQL-0.5.2/absql/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/absql/functions/db.py` & `ABSQL-0.5.2/absql/functions/db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/absql/functions/env.py` & `ABSQL-0.5.2/absql/functions/env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/absql/render/__init__.py` & `ABSQL-0.5.2/absql/render/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/absql/text/__init__.py` & `ABSQL-0.5.2/absql/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/absql/utils/__init__.py` & `ABSQL-0.5.2/absql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/setup.py` & `ABSQL-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ABSQL",
-    version="0.5.1",
+    version="0.5.2",
     author="Chris Cardillo",
     author_email="cfcardillo23@gmail.com",
     description="A rendering engine for templated SQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pipeline-tools/ABSQL",
     packages=setuptools.find_packages(),
```

### Comparing `ABSQL-0.5.1/tests/test_copy.py` & `ABSQL-0.5.2/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_funcs_db.py` & `ABSQL-0.5.2/tests/test_funcs_db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_funcs_env.py` & `ABSQL-0.5.2/tests/test_funcs_env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_funcs_time.py` & `ABSQL-0.5.2/tests/test_funcs_time.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_loader.py` & `ABSQL-0.5.2/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_parse_file.py` & `ABSQL-0.5.2/tests/test_parse_file.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_partial_kwargs.py` & `ABSQL-0.5.2/tests/test_partial_kwargs.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_render.py` & `ABSQL-0.5.2/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_render_file.py` & `ABSQL-0.5.2/tests/test_render_file.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_render_file_return_dict.py` & `ABSQL-0.5.2/tests/test_render_file_return_dict.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_render_text.py` & `ABSQL-0.5.2/tests/test_render_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_text.py` & `ABSQL-0.5.2/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.1/tests/test_utils.py` & `ABSQL-0.5.2/tests/test_utils.py`

 * *Files identical despite different names*

