# Comparing `tmp/xraygpt-0.1.1.dev0.tar.gz` & `tmp/xraygpt-0.1.1.dev1.tar.gz`

## Comparing `xraygpt-0.1.1.dev0.tar` & `xraygpt-0.1.1.dev1.tar`

### file list

```diff
@@ -1,11 +1,16 @@
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/Makefile
--rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/update_version.sh
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/.github/workflows/release.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/xraygpt/__about__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/xraygpt/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/xraygpt/about.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/.gitignore
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/LICENSE
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/README.md
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/pyproject.toml
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/Makefile
+-rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/update_version.sh
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/.github/workflows/release.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/__about__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/__main__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/flow.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/llm.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/ner.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/reader.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/xraygpt/splitter.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/LICENSE
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/README.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 xraygpt-0.1.1.dev1/PKG-INFO
```

### Comparing `xraygpt-0.1.1.dev0/update_version.sh` & `xraygpt-0.1.1.dev1/update_version.sh`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev0/.github/workflows/release.yml` & `xraygpt-0.1.1.dev1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev0/.gitignore` & `xraygpt-0.1.1.dev1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+/workdir
 .DS_Store
 *.swp
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `xraygpt-0.1.1.dev0/LICENSE` & `xraygpt-0.1.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `xraygpt-0.1.1.dev0/pyproject.toml` & `xraygpt-0.1.1.dev1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -22,18 +22,33 @@
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
 dependencies = [
+  "langchain",
+  "langchain_openai",
+  "loguru",
+  "ebooklib",
+  "BeautifulSoup4",
 ]
 
 [project.optional-dependencies]
+azure = [
+    "azure-core",
+    "azure-ai-textanalytics",
+]
+
+all = [
+    "xraygpt[azure]",
+]
+
 dev = [
+    "xraygpt[all]",
     "hatch",
     "build",
     "isort",
     "black",
     "mypy",
     "q",
 ]
```

### Comparing `xraygpt-0.1.1.dev0/PKG-INFO` & `xraygpt-0.1.1.dev1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,50 @@
 Metadata-Version: 2.3
 Name: xraygpt
-Version: 0.1.1.dev0
+Version: 0.1.1.dev1
 Summary: GPT to generate X-ray
 Project-URL: homepage, https://github.com/iaalm/xraygpt
 Project-URL: repository, https://github.com/iaalm/xraygpt
 Project-URL: documentation, https://github.com/iaalm/xraygpt
 Author-email: iaalm <iaalmsimon@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
+Requires-Dist: beautifulsoup4
+Requires-Dist: ebooklib
+Requires-Dist: langchain
+Requires-Dist: langchain-openai
+Requires-Dist: loguru
+Provides-Extra: all
+Requires-Dist: xraygpt[azure]; extra == 'all'
+Provides-Extra: azure
+Requires-Dist: azure-ai-textanalytics; extra == 'azure'
+Requires-Dist: azure-core; extra == 'azure'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: q; extra == 'dev'
+Requires-Dist: xraygpt[all]; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# xraygpt
+# 🔬📖 X-ray GPT
 
-## Dev Setup
+Generate kindle-like x-ray for e-books with LLM
+
+## 🚀 Usage
+
+## 🧑‍💻 Dev Setup
 ```shell
 pip install -e '.[dev]'
 ```
 
-### Static analysis
+### 🎩 Static analysis
 ```shell
 make format
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

