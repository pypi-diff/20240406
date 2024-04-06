# Comparing `tmp/ABSQL-0.5.0.tar.gz` & `tmp/ABSQL-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABSQL-0.5.0.tar", last modified: Fri Feb  9 23:57:55 2024, max compression
+gzip compressed data, was "ABSQL-0.5.1.tar", last modified: Sat Apr  6 01:04:15 2024, max compression
```

## Comparing `ABSQL-0.5.0.tar` & `ABSQL-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.916675 ABSQL-0.5.0/
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.915203 ABSQL-0.5.0/ABSQL.egg-info/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9773 2024-02-09 23:57:55.000000 ABSQL-0.5.0/ABSQL.egg-info/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)      740 2024-02-09 23:57:55.000000 ABSQL-0.5.0/ABSQL.egg-info/SOURCES.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-02-09 23:57:55.000000 ABSQL-0.5.0/ABSQL.egg-info/dependency_links.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       65 2024-02-09 23:57:55.000000 ABSQL-0.5.0/ABSQL.egg-info/requires.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-02-09 23:57:55.000000 ABSQL-0.5.0/ABSQL.egg-info/top_level.txt
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 ABSQL-0.5.0/LICENSE
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9773 2024-02-09 23:57:55.915910 ABSQL-0.5.0/PKG-INFO
--rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 ABSQL-0.5.0/README.md
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.906783 ABSQL-0.5.0/absql/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2023-05-12 18:29:12.000000 ABSQL-0.5.0/absql/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.907683 ABSQL-0.5.0/absql/files/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      740 2023-05-12 18:29:12.000000 ABSQL-0.5.0/absql/files/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 ABSQL-0.5.0/absql/files/loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2606 2024-02-09 23:11:51.000000 ABSQL-0.5.0/absql/files/parsers.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.908822 ABSQL-0.5.0/absql/functions/
--rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 ABSQL-0.5.0/absql/functions/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 ABSQL-0.5.0/absql/functions/db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 ABSQL-0.5.0/absql/functions/env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 ABSQL-0.5.0/absql/functions/time.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.909097 ABSQL-0.5.0/absql/render/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2970 2023-05-12 18:29:12.000000 ABSQL-0.5.0/absql/render/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.909364 ABSQL-0.5.0/absql/text/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 ABSQL-0.5.0/absql/text/__init__.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.909635 ABSQL-0.5.0/absql/utils/
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 ABSQL-0.5.0/absql/utils/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-02-09 23:57:55.916792 ABSQL-0.5.0/setup.cfg
--rw-r--r--   0 chriscardillo   (501) staff       (20)      826 2024-02-09 23:11:51.000000 ABSQL-0.5.0/setup.py
-drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-02-09 23:57:55.914660 ABSQL-0.5.0/tests/
--rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/__init__.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_copy.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_funcs_db.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_funcs_env.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_funcs_time.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_loader.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      909 2024-01-03 15:37:15.000000 ABSQL-0.5.0/tests/test_parse_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 ABSQL-0.5.0/tests/test_partial_kwargs.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 ABSQL-0.5.0/tests/test_render.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     3575 2024-02-09 23:11:51.000000 ABSQL-0.5.0/tests/test_render_file.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_render_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_set.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_text.py
--rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 ABSQL-0.5.0/tests/test_utils.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.045240 ABSQL-0.5.1/
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.044434 ABSQL-0.5.1/ABSQL.egg-info/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9773 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      778 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/SOURCES.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        1 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       65 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/requires.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       12 2024-04-06 01:04:15.000000 ABSQL-0.5.1/ABSQL.egg-info/top_level.txt
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1071 2023-05-12 18:29:12.000000 ABSQL-0.5.1/LICENSE
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9773 2024-04-06 01:04:15.044823 ABSQL-0.5.1/PKG-INFO
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     9165 2024-02-09 23:11:51.000000 ABSQL-0.5.1/README.md
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.037192 ABSQL-0.5.1/absql/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3157 2024-04-05 21:55:53.000000 ABSQL-0.5.1/absql/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.038014 ABSQL-0.5.1/absql/files/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      740 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/files/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2980 2024-01-03 15:38:53.000000 ABSQL-0.5.1/absql/files/loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2606 2024-02-09 23:11:51.000000 ABSQL-0.5.1/absql/files/parsers.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.039342 ABSQL-0.5.1/absql/functions/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      772 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/functions/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2331 2024-02-09 23:49:25.000000 ABSQL-0.5.1/absql/functions/db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      560 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/functions/env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      350 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/functions/time.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.039715 ABSQL-0.5.1/absql/render/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3068 2024-04-06 01:03:31.000000 ABSQL-0.5.1/absql/render/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.039999 ABSQL-0.5.1/absql/text/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1596 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/text/__init__.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.040247 ABSQL-0.5.1/absql/utils/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1218 2023-05-12 18:29:12.000000 ABSQL-0.5.1/absql/utils/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)       38 2024-04-06 01:04:15.045309 ABSQL-0.5.1/setup.cfg
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      826 2024-04-06 01:03:31.000000 ABSQL-0.5.1/setup.py
+drwxr-xr-x   0 chriscardillo   (501) staff       (20)        0 2024-04-06 01:04:15.044110 ABSQL-0.5.1/tests/
+-rw-r--r--   0 chriscardillo   (501) staff       (20)        0 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/__init__.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      814 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_copy.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2440 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_funcs_db.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      835 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_funcs_env.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      638 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_funcs_time.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      586 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_loader.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      909 2024-01-03 15:37:15.000000 ABSQL-0.5.1/tests/test_parse_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1235 2024-01-03 15:38:53.000000 ABSQL-0.5.1/tests/test_partial_kwargs.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2020 2024-01-03 15:37:15.000000 ABSQL-0.5.1/tests/test_render.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     3575 2024-02-09 23:11:51.000000 ABSQL-0.5.1/tests/test_render_file.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      641 2024-04-06 01:03:31.000000 ABSQL-0.5.1/tests/test_render_file_return_dict.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     2523 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_render_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      288 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_set.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)      729 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_text.py
+-rw-r--r--   0 chriscardillo   (501) staff       (20)     1401 2023-05-12 18:29:12.000000 ABSQL-0.5.1/tests/test_utils.py
```

### Comparing `ABSQL-0.5.0/ABSQL.egg-info/PKG-INFO` & `ABSQL-0.5.1/ABSQL.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.5.0
+Version: 0.5.1
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.5.0/ABSQL.egg-info/SOURCES.txt` & `ABSQL-0.5.1/ABSQL.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 tests/test_funcs_env.py
 tests/test_funcs_time.py
 tests/test_loader.py
 tests/test_parse_file.py
 tests/test_partial_kwargs.py
 tests/test_render.py
 tests/test_render_file.py
+tests/test_render_file_return_dict.py
 tests/test_render_text.py
 tests/test_set.py
 tests/test_text.py
 tests/test_utils.py
```

### Comparing `ABSQL-0.5.0/LICENSE` & `ABSQL-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/PKG-INFO` & `ABSQL-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABSQL
-Version: 0.5.0
+Version: 0.5.1
 Summary: A rendering engine for templated SQL
 Home-page: https://github.com/pipeline-tools/ABSQL
 Author: Chris Cardillo
 Author-email: cfcardillo23@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ABSQL-0.5.0/README.md` & `ABSQL-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/__init__.py` & `ABSQL-0.5.1/absql/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/files/__init__.py` & `ABSQL-0.5.1/absql/files/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/files/loader.py` & `ABSQL-0.5.1/absql/files/loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/files/parsers.py` & `ABSQL-0.5.1/absql/files/parsers.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/functions/__init__.py` & `ABSQL-0.5.1/absql/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/functions/db.py` & `ABSQL-0.5.1/absql/functions/db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/functions/env.py` & `ABSQL-0.5.1/absql/functions/env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/render/__init__.py` & `ABSQL-0.5.1/absql/render/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,27 +66,27 @@
     file_path,
     loader=None,
     replace_only=False,
     extra_constructors=None,
     file_context_from=None,
     pretty_encode=False,
     partial_kwargs=None,
+    return_dict=False,
     **extra_context,
 ):
     """
     Given a file path, render SQL with a combination of
     the vars in the file and any extras passed to extra_context.
     """
     if loader is None:
         loader = generate_loader(extra_constructors or [])
 
     file_contents = parse(file_path, loader=loader)
 
-    sql = file_contents["sql"]
-    file_contents.pop("sql")
+    sql = file_contents.pop("sql", "")
 
     if file_context_from:
         file_contents.update(file_contents.get(file_context_from, {}))
         file_contents.pop(file_context_from, {})
 
     rendered_context = render_context(extra_context, file_contents, partial_kwargs)
 
@@ -94,8 +94,12 @@
         text=sql,
         replace_only=replace_only,
         pretty_encode=pretty_encode,
         partial_kwargs=partial_kwargs,
         **rendered_context,
     )
 
+    if return_dict:
+        rendered_context["sql"] = rendered
+        return rendered_context
+
     return rendered
```

### Comparing `ABSQL-0.5.0/absql/text/__init__.py` & `ABSQL-0.5.1/absql/text/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/absql/utils/__init__.py` & `ABSQL-0.5.1/absql/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/setup.py` & `ABSQL-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ABSQL",
-    version="0.5.0",
+    version="0.5.1",
     author="Chris Cardillo",
     author_email="cfcardillo23@gmail.com",
     description="A rendering engine for templated SQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pipeline-tools/ABSQL",
     packages=setuptools.find_packages(),
```

### Comparing `ABSQL-0.5.0/tests/test_copy.py` & `ABSQL-0.5.1/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_funcs_db.py` & `ABSQL-0.5.1/tests/test_funcs_db.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_funcs_env.py` & `ABSQL-0.5.1/tests/test_funcs_env.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_funcs_time.py` & `ABSQL-0.5.1/tests/test_funcs_time.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_loader.py` & `ABSQL-0.5.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_parse_file.py` & `ABSQL-0.5.1/tests/test_parse_file.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_partial_kwargs.py` & `ABSQL-0.5.1/tests/test_partial_kwargs.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_render.py` & `ABSQL-0.5.1/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_render_file.py` & `ABSQL-0.5.1/tests/test_render_file.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_render_text.py` & `ABSQL-0.5.1/tests/test_render_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_text.py` & `ABSQL-0.5.1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `ABSQL-0.5.0/tests/test_utils.py` & `ABSQL-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

