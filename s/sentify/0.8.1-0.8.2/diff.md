# Comparing `tmp/sentify-0.8.1.tar.gz` & `tmp/sentify-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentify-0.8.1.tar", last modified: Thu Apr  4 03:06:00 2024, max compression
+gzip compressed data, was "sentify-0.8.2.tar", last modified: Sat Apr  6 00:57:44 2024, max compression
```

## Comparing `sentify-0.8.1.tar` & `sentify-0.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:06:00.143067 sentify-0.8.1/
--rw-r--r--   0 tarau      (503) staff       (20)     1067 2024-01-01 22:59:06.000000 sentify-0.8.1/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     1310 2024-04-04 03:06:00.142837 sentify-0.8.1/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)      994 2024-01-14 04:32:35.000000 sentify-0.8.1/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:06:00.140773 sentify-0.8.1/sentify/
--rw-r--r--   0 tarau      (503) staff       (20)       58 2024-04-04 01:12:07.000000 sentify-0.8.1/sentify/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)      443 2024-01-01 20:36:11.000000 sentify-0.8.1/sentify/config.py
--rw-r--r--   0 tarau      (503) staff       (20)     6152 2024-04-04 01:30:03.000000 sentify-0.8.1/sentify/main.py
--rw-r--r--   0 tarau      (503) staff       (20)       51 2024-03-10 22:07:38.000000 sentify-0.8.1/sentify/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1529 2024-03-16 22:04:34.000000 sentify-0.8.1/sentify/segmenter.py
--rw-r--r--   0 tarau      (503) staff       (20)     2049 2024-03-16 19:18:26.000000 sentify-0.8.1/sentify/tools.py
--rw-r--r--   0 tarau      (503) staff       (20)     1649 2024-01-01 22:00:27.000000 sentify-0.8.1/sentify/wikifetch.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:06:00.142495 sentify-0.8.1/sentify.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     1310 2024-04-04 03:06:00.000000 sentify-0.8.1/sentify.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)      348 2024-04-04 03:06:00.000000 sentify-0.8.1/sentify.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:06:00.000000 sentify-0.8.1/sentify.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:06:00.000000 sentify-0.8.1/sentify.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       50 2024-04-04 03:06:00.000000 sentify-0.8.1/sentify.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2024-04-04 03:06:00.000000 sentify-0.8.1/sentify.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-04 03:06:00.143162 sentify-0.8.1/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      844 2024-01-01 23:42:49.000000 sentify-0.8.1/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-06 00:57:44.433274 sentify-0.8.2/
+-rw-r--r--   0 tarau      (503) staff       (20)     1067 2024-01-01 22:59:06.000000 sentify-0.8.2/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     1310 2024-04-06 00:57:44.432973 sentify-0.8.2/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)      994 2024-01-14 04:32:35.000000 sentify-0.8.2/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-06 00:57:44.430702 sentify-0.8.2/sentify/
+-rw-r--r--   0 tarau      (503) staff       (20)       58 2024-04-05 20:04:47.000000 sentify-0.8.2/sentify/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)      443 2024-01-01 20:36:11.000000 sentify-0.8.2/sentify/config.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6214 2024-04-05 20:03:53.000000 sentify-0.8.2/sentify/main.py
+-rw-r--r--   0 tarau      (503) staff       (20)       51 2024-03-10 22:07:38.000000 sentify-0.8.2/sentify/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1529 2024-03-16 22:04:34.000000 sentify-0.8.2/sentify/segmenter.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2049 2024-03-16 19:18:26.000000 sentify-0.8.2/sentify/tools.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1649 2024-01-01 22:00:27.000000 sentify-0.8.2/sentify/wikifetch.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-06 00:57:44.432551 sentify-0.8.2/sentify.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     1310 2024-04-06 00:57:44.000000 sentify-0.8.2/sentify.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)      348 2024-04-06 00:57:44.000000 sentify-0.8.2/sentify.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-06 00:57:44.000000 sentify-0.8.2/sentify.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-06 00:57:44.000000 sentify-0.8.2/sentify.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       50 2024-04-06 00:57:44.000000 sentify-0.8.2/sentify.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2024-04-06 00:57:44.000000 sentify-0.8.2/sentify.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-06 00:57:44.433379 sentify-0.8.2/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      844 2024-01-01 23:42:49.000000 sentify-0.8.2/setup.py
```

### Comparing `sentify-0.8.1/LICENSE` & `sentify-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentify-0.8.1/PKG-INFO` & `sentify-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentify
-Version: 0.8.1
+Version: 0.8.2
 Summary: Converter from urls,pdfs,wikipages to clean text document one sentence per line.
 Home-page: https://github.com/ptarau/sentify.git
 Author: Paul Tarau
 Author-email: ptarau@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sentify-0.8.1/README.md` & `sentify-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `sentify-0.8.1/sentify/main.py` & `sentify-0.8.2/sentify/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,23 +124,26 @@
 def pdf2text(pdf_or_stream, minline=4, trace=1):
     """
     pdf to txt conversion with external tool - if availble
     (on Mac, install pdftotext as part of "poppler tools")
     otherwise, we use pdfminer
     """
 
-    if exists_file('/usr/bin/pdftotext') or exists_file('/opt/local/bin/pdftotext'):
+    if ((exists_file('/usr/bin/pdftotext')
+        or exists_file('/opt/local/bin/pdftotext'))
+        or exists_file('/opt/homebrew/bin//pdftotext')):
+
         if trace: print('!!! ENTER pdf2text')
         try:
             txt = "__temp__.txt"
             pdf = "__temp__.pdf"
             if not isinstance(pdf_or_stream, str):
-                bytes = pdf_or_stream.read()
+                bs = pdf_or_stream.read()
                 with open(pdf, 'wb') as g:
-                    g.write(bytes)
+                    g.write(bs)
             else:
                 pdf = pdf_or_stream
 
             subprocess.run(["pdftotext", "-q", pdf, txt])
 
             if exists_file(pdf): remove_file(pdf)
             text = file2text(txt)
```

### Comparing `sentify-0.8.1/sentify/segmenter.py` & `sentify-0.8.2/sentify/segmenter.py`

 * *Files identical despite different names*

### Comparing `sentify-0.8.1/sentify/tools.py` & `sentify-0.8.2/sentify/tools.py`

 * *Files identical despite different names*

### Comparing `sentify-0.8.1/sentify/wikifetch.py` & `sentify-0.8.2/sentify/wikifetch.py`

 * *Files identical despite different names*

### Comparing `sentify-0.8.1/sentify.egg-info/PKG-INFO` & `sentify-0.8.2/sentify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentify
-Version: 0.8.1
+Version: 0.8.2
 Summary: Converter from urls,pdfs,wikipages to clean text document one sentence per line.
 Home-page: https://github.com/ptarau/sentify.git
 Author: Paul Tarau
 Author-email: ptarau@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sentify-0.8.1/setup.py` & `sentify-0.8.2/setup.py`

 * *Files identical despite different names*

