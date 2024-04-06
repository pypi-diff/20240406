# Comparing `tmp/xraygpt-0.1.1.dev1.tar.gz` & `tmp/xraygpt-0.1.1.dev2.tar.gz`

## Comparing `xraygpt-0.1.1.dev1.tar` & `xraygpt-0.1.1.dev2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/Makefile
--rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/update_version.sh
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/.github/workflows/release.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/__about__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/__main__.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/flow.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/llm.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/ner.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/reader.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/splitter.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/.gitignore
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/LICENSE
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/README.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/pyproject.toml
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/PKG-INFO
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/Makefile
+-rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/update_version.sh
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/.github/workflows/release.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/xraygpt/__about__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/xraygpt/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/xraygpt/__main__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/xraygpt/flow.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/xraygpt/llm.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/xraygpt/ner.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/xraygpt/reader.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/xraygpt/splitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/.gitignore
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/LICENSE
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/README.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev2/PKG-INFO
```

### Comparing `xraygpt-0.1.1.dev1/update_version.sh` & `xraygpt-0.1.1.dev2/update_version.sh`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev1/.github/workflows/release.yml` & `xraygpt-0.1.1.dev2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev1/xraygpt/llm.py` & `xraygpt-0.1.1.dev2/xraygpt/llm.py`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev1/xraygpt/ner.py` & `xraygpt-0.1.1.dev2/xraygpt/ner.py`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev1/xraygpt/reader.py` & `xraygpt-0.1.1.dev2/xraygpt/reader.py`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev1/.gitignore` & `xraygpt-0.1.1.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev1/LICENSE` & `xraygpt-0.1.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev1/pyproject.toml` & `xraygpt-0.1.1.dev2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xraygpt"
-description = "GPT to generate X-ray"
+description = "Generate kindle-like x-ray for e-books with LLM"
 authors = [
     {name = "iaalm", email= "iaalmsimon@gmail.com"}
 ]
-license = {text = "MIT"}
+license = {text = "BSD-3"}
 readme = "README.md"
 requires-python = ">=3.9"
 dynamic = [
     "version",
 ]
 
 keywords = [
```

### Comparing `xraygpt-0.1.1.dev1/PKG-INFO` & `xraygpt-0.1.1.dev2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: xraygpt
-Version: 0.1.1.dev1
-Summary: GPT to generate X-ray
+Version: 0.1.1.dev2
+Summary: Generate kindle-like x-ray for e-books with LLM
 Project-URL: homepage, https://github.com/iaalm/xraygpt
 Project-URL: repository, https://github.com/iaalm/xraygpt
 Project-URL: documentation, https://github.com/iaalm/xraygpt
 Author-email: iaalm <iaalmsimon@gmail.com>
-License: MIT
+License: BSD-3
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Requires-Dist: beautifulsoup4
```

