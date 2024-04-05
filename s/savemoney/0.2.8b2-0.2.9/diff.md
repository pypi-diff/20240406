# Comparing `tmp/savemoney-0.2.8b2.tar.gz` & `tmp/savemoney-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "savemoney-0.2.8b2.tar", last modified: Fri Jan 12 18:58:31 2024, max compression
+gzip compressed data, was "savemoney-0.2.9.tar", last modified: Sun Jan 14 05:35:04 2024, max compression
```

## Comparing `savemoney-0.2.8b2.tar` & `savemoney-0.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.234029 savemoney-0.2.8b2/
--rw-r--r--   0 masaaki    (502) staff       (20)     1427 2023-04-14 22:34:31.000000 savemoney-0.2.8b2/LICENSE
--rw-r--r--   0 masaaki    (502) staff       (20)      174 2023-12-23 01:19:12.000000 savemoney-0.2.8b2/MANIFEST.in
--rw-r--r--   0 masaaki    (502) staff       (20)    10023 2024-01-12 18:58:31.233056 savemoney-0.2.8b2/PKG-INFO
--rw-r--r--   0 masaaki    (502) staff       (20)     8732 2024-01-11 07:01:26.000000 savemoney-0.2.8b2/README.md
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.204635 savemoney-0.2.8b2/savemoney/
--rw-r--r--   0 masaaki    (502) staff       (20)      651 2024-01-12 18:46:37.000000 savemoney-0.2.8b2/savemoney/__about__.py
--rw-r--r--   0 masaaki    (502) staff       (20)      525 2024-01-11 07:06:14.000000 savemoney-0.2.8b2/savemoney/__init__.py
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.207901 savemoney-0.2.8b2/savemoney/ca2bam/
--rw-r--r--   0 masaaki    (502) staff       (20)       47 2024-01-11 07:21:22.000000 savemoney-0.2.8b2/savemoney/ca2bam/__init__.py
--rw-r--r--   0 masaaki    (502) staff       (20)      555 2024-01-11 07:21:28.000000 savemoney-0.2.8b2/savemoney/ca2bam/__main__.py
--rw-r--r--   0 masaaki    (502) staff       (20)      469 2024-01-11 07:20:52.000000 savemoney-0.2.8b2/savemoney/ca2bam/ca2bam.py
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.211774 savemoney-0.2.8b2/savemoney/modules/
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.212919 savemoney-0.2.8b2/savemoney/modules/NanoporeStats_PDF/
--rw-r--r--   0 masaaki    (502) staff       (20)     3773 2023-12-08 17:08:11.000000 savemoney-0.2.8b2/savemoney/modules/NanoporeStats_PDF/NanoporeStats_pdf_0.2.0.csv
--rw-r--r--   0 masaaki    (502) staff       (20)       24 2023-12-23 04:28:47.000000 savemoney-0.2.8b2/savemoney/modules/__init__.py
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.224086 savemoney-0.2.8b2/savemoney/modules/cython_functions/
--rw-r--r--   0 masaaki    (502) staff       (20)       24 2023-12-23 03:48:46.000000 savemoney-0.2.8b2/savemoney/modules/cython_functions/__init__.py
--rw-r--r--   0 masaaki    (502) staff       (20)  1211920 2024-01-12 18:58:31.000000 savemoney-0.2.8b2/savemoney/modules/cython_functions/alignment_functions.cpp
--rw-r--r--   0 masaaki    (502) staff       (20)    17174 2023-12-29 00:18:06.000000 savemoney-0.2.8b2/savemoney/modules/cython_functions/alignment_functions.pyx
--rwxrwxrwx   0 masaaki    (502) staff       (20)      508 2023-12-04 00:54:53.000000 savemoney-0.2.8b2/savemoney/modules/cython_functions/alignment_functions_setup.py
--rw-r--r--   0 masaaki    (502) staff       (20)   132221 2024-01-12 17:31:47.000000 savemoney-0.2.8b2/savemoney/modules/msa.py
--rw-r--r--   0 masaaki    (502) staff       (20)    19513 2024-01-11 22:17:30.000000 savemoney-0.2.8b2/savemoney/modules/my_classes.py
--rw-r--r--   0 masaaki    (502) staff       (20)    48492 2024-01-08 23:24:04.000000 savemoney-0.2.8b2/savemoney/modules/ref_query_alignment.py
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.226522 savemoney-0.2.8b2/savemoney/post_analysis/
--rw-r--r--   0 masaaki    (502) staff       (20)       89 2023-12-22 02:58:55.000000 savemoney-0.2.8b2/savemoney/post_analysis/__init__.py
--rw-r--r--   0 masaaki    (502) staff       (20)      953 2023-12-26 03:26:44.000000 savemoney-0.2.8b2/savemoney/post_analysis/__main__.py
--rw-r--r--   0 masaaki    (502) staff       (20)     2658 2024-01-12 18:50:45.000000 savemoney-0.2.8b2/savemoney/post_analysis/post_analysis.py
--rw-r--r--   0 masaaki    (502) staff       (20)    14626 2024-01-11 06:50:33.000000 savemoney-0.2.8b2/savemoney/post_analysis/post_analysis_core.py
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.229023 savemoney-0.2.8b2/savemoney/pre_survey/
--rw-r--r--   0 masaaki    (502) staff       (20)       83 2023-12-22 02:59:54.000000 savemoney-0.2.8b2/savemoney/pre_survey/__init__.py
--rw-r--r--   0 masaaki    (502) staff       (20)      959 2023-12-26 03:26:39.000000 savemoney-0.2.8b2/savemoney/pre_survey/__main__.py
--rw-r--r--   0 masaaki    (502) staff       (20)     2375 2024-01-11 22:46:59.000000 savemoney-0.2.8b2/savemoney/pre_survey/pre_survey.py
--rw-r--r--   0 masaaki    (502) staff       (20)    68060 2024-01-12 01:20:57.000000 savemoney-0.2.8b2/savemoney/pre_survey/pre_survey_core.py
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.231300 savemoney-0.2.8b2/savemoney/show_consensus/
--rw-r--r--   0 masaaki    (502) staff       (20)       56 2024-01-11 07:20:11.000000 savemoney-0.2.8b2/savemoney/show_consensus/__init__.py
--rw-r--r--   0 masaaki    (502) staff       (20)      881 2024-01-11 07:17:52.000000 savemoney-0.2.8b2/savemoney/show_consensus/__main__.py
--rw-r--r--   0 masaaki    (502) staff       (20)      371 2024-01-11 07:16:53.000000 savemoney-0.2.8b2/savemoney/show_consensus/show_consensus.py
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.232456 savemoney-0.2.8b2/savemoney.egg-info/
--rw-r--r--   0 masaaki    (502) staff       (20)    10023 2024-01-12 18:58:31.000000 savemoney-0.2.8b2/savemoney.egg-info/PKG-INFO
--rw-r--r--   0 masaaki    (502) staff       (20)     1193 2024-01-12 18:58:31.000000 savemoney-0.2.8b2/savemoney.egg-info/SOURCES.txt
--rw-r--r--   0 masaaki    (502) staff       (20)        1 2024-01-12 18:58:31.000000 savemoney-0.2.8b2/savemoney.egg-info/dependency_links.txt
--rw-r--r--   0 masaaki    (502) staff       (20)      198 2024-01-12 18:58:31.000000 savemoney-0.2.8b2/savemoney.egg-info/requires.txt
--rw-r--r--   0 masaaki    (502) staff       (20)       10 2024-01-12 18:58:31.000000 savemoney-0.2.8b2/savemoney.egg-info/top_level.txt
--rw-r--r--   0 masaaki    (502) staff       (20)       38 2024-01-12 18:58:31.234132 savemoney-0.2.8b2/setup.cfg
--rw-r--r--   0 masaaki    (502) staff       (20)     4485 2024-01-12 18:44:39.000000 savemoney-0.2.8b2/setup.py
-drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-12 18:58:31.231779 savemoney-0.2.8b2/test/
--rw-r--r--   0 masaaki    (502) staff       (20)     1493 2024-01-09 20:48:39.000000 savemoney-0.2.8b2/test/test_local_all.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.977815 savemoney-0.2.9/
+-rw-r--r--   0 masaaki    (502) staff       (20)     1427 2023-04-14 22:34:31.000000 savemoney-0.2.9/LICENSE
+-rw-r--r--   0 masaaki    (502) staff       (20)      174 2023-12-23 01:19:12.000000 savemoney-0.2.9/MANIFEST.in
+-rw-r--r--   0 masaaki    (502) staff       (20)     9991 2024-01-14 05:35:04.977222 savemoney-0.2.9/PKG-INFO
+-rw-r--r--   0 masaaki    (502) staff       (20)     8732 2024-01-11 07:01:26.000000 savemoney-0.2.9/README.md
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.962758 savemoney-0.2.9/savemoney/
+-rw-r--r--   0 masaaki    (502) staff       (20)      651 2024-01-13 06:26:12.000000 savemoney-0.2.9/savemoney/__about__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)      525 2024-01-11 07:06:14.000000 savemoney-0.2.9/savemoney/__init__.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.964407 savemoney-0.2.9/savemoney/ca2bam/
+-rw-r--r--   0 masaaki    (502) staff       (20)       47 2024-01-11 07:21:22.000000 savemoney-0.2.9/savemoney/ca2bam/__init__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)      555 2024-01-11 07:21:28.000000 savemoney-0.2.9/savemoney/ca2bam/__main__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)      469 2024-01-11 07:20:52.000000 savemoney-0.2.9/savemoney/ca2bam/ca2bam.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.968131 savemoney-0.2.9/savemoney/modules/
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.969427 savemoney-0.2.9/savemoney/modules/NanoporeStats_PDF/
+-rw-r--r--   0 masaaki    (502) staff       (20)     3773 2023-12-08 17:08:11.000000 savemoney-0.2.9/savemoney/modules/NanoporeStats_PDF/NanoporeStats_pdf_0.2.0.csv
+-rw-r--r--   0 masaaki    (502) staff       (20)       24 2023-12-23 04:28:47.000000 savemoney-0.2.9/savemoney/modules/__init__.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.972741 savemoney-0.2.9/savemoney/modules/cython_functions/
+-rw-r--r--   0 masaaki    (502) staff       (20)       24 2023-12-23 03:48:46.000000 savemoney-0.2.9/savemoney/modules/cython_functions/__init__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)  1342757 2024-01-14 05:35:04.000000 savemoney-0.2.9/savemoney/modules/cython_functions/alignment_functions.cpp
+-rw-r--r--   0 masaaki    (502) staff       (20)    19737 2024-01-14 04:46:29.000000 savemoney-0.2.9/savemoney/modules/cython_functions/alignment_functions.pyx
+-rwxrwxrwx   0 masaaki    (502) staff       (20)      508 2023-12-04 00:54:53.000000 savemoney-0.2.9/savemoney/modules/cython_functions/alignment_functions_setup.py
+-rw-r--r--   0 masaaki    (502) staff       (20)   134646 2024-01-13 06:14:22.000000 savemoney-0.2.9/savemoney/modules/msa.py
+-rw-r--r--   0 masaaki    (502) staff       (20)    19513 2024-01-11 22:17:30.000000 savemoney-0.2.9/savemoney/modules/my_classes.py
+-rw-r--r--   0 masaaki    (502) staff       (20)    48500 2024-01-12 22:57:15.000000 savemoney-0.2.9/savemoney/modules/ref_query_alignment.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.974058 savemoney-0.2.9/savemoney/post_analysis/
+-rw-r--r--   0 masaaki    (502) staff       (20)       89 2023-12-22 02:58:55.000000 savemoney-0.2.9/savemoney/post_analysis/__init__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)      953 2023-12-26 03:26:44.000000 savemoney-0.2.9/savemoney/post_analysis/__main__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)     2658 2024-01-12 18:50:45.000000 savemoney-0.2.9/savemoney/post_analysis/post_analysis.py
+-rw-r--r--   0 masaaki    (502) staff       (20)    14562 2024-01-12 23:22:35.000000 savemoney-0.2.9/savemoney/post_analysis/post_analysis_core.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.975221 savemoney-0.2.9/savemoney/pre_survey/
+-rw-r--r--   0 masaaki    (502) staff       (20)       83 2023-12-22 02:59:54.000000 savemoney-0.2.9/savemoney/pre_survey/__init__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)      959 2023-12-26 03:26:39.000000 savemoney-0.2.9/savemoney/pre_survey/__main__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)     2375 2024-01-11 22:46:59.000000 savemoney-0.2.9/savemoney/pre_survey/pre_survey.py
+-rw-r--r--   0 masaaki    (502) staff       (20)    68060 2024-01-12 01:20:57.000000 savemoney-0.2.9/savemoney/pre_survey/pre_survey_core.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.976140 savemoney-0.2.9/savemoney/show_consensus/
+-rw-r--r--   0 masaaki    (502) staff       (20)       56 2024-01-11 07:20:11.000000 savemoney-0.2.9/savemoney/show_consensus/__init__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)      881 2024-01-11 07:17:52.000000 savemoney-0.2.9/savemoney/show_consensus/__main__.py
+-rw-r--r--   0 masaaki    (502) staff       (20)      371 2024-01-11 07:16:53.000000 savemoney-0.2.9/savemoney/show_consensus/show_consensus.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.963805 savemoney-0.2.9/savemoney.egg-info/
+-rw-r--r--   0 masaaki    (502) staff       (20)     9991 2024-01-14 05:35:04.000000 savemoney-0.2.9/savemoney.egg-info/PKG-INFO
+-rw-r--r--   0 masaaki    (502) staff       (20)     1193 2024-01-14 05:35:04.000000 savemoney-0.2.9/savemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 masaaki    (502) staff       (20)        1 2024-01-14 05:35:04.000000 savemoney-0.2.9/savemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 masaaki    (502) staff       (20)      183 2024-01-14 05:35:04.000000 savemoney-0.2.9/savemoney.egg-info/requires.txt
+-rw-r--r--   0 masaaki    (502) staff       (20)       10 2024-01-14 05:35:04.000000 savemoney-0.2.9/savemoney.egg-info/top_level.txt
+-rw-r--r--   0 masaaki    (502) staff       (20)       38 2024-01-14 05:35:04.977928 savemoney-0.2.9/setup.cfg
+-rw-r--r--   0 masaaki    (502) staff       (20)     4484 2024-01-14 05:34:49.000000 savemoney-0.2.9/setup.py
+drwxr-xr-x   0 masaaki    (502) staff       (20)        0 2024-01-14 05:35:04.976462 savemoney-0.2.9/test/
+-rw-r--r--   0 masaaki    (502) staff       (20)     1630 2024-01-13 06:32:58.000000 savemoney-0.2.9/test/test_local_all.py
```

### Comparing `savemoney-0.2.8b2/LICENSE` & `savemoney-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/PKG-INFO` & `savemoney-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savemoney
-Version: 0.2.8b2
+Version: 0.2.9
 Summary: Simple Algorithm for Very Efficient Multiplexing of Oxford Nanopore Experiments for You!
 Home-page: https://github.com/MasaakiU/MultiplexNanopore
 Author: Masaaki Uematsu
 Author-email: mu84@cornell.edu
 Maintainer: Masaaki Uematsu
 Maintainer-email: mu84@cornell.edu
 License: CC BY-NC-SA 4.0
@@ -15,26 +15,25 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas>=2.1.4
+Requires-Dist: pandas>=1.5.3
 Requires-Dist: parasail>=1.3.4
-Requires-Dist: Pillow>=10.2.0
+Requires-Dist: Pillow>=9.4.0
 Requires-Dist: PuLP>=2.7.0
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: snapgene_reader>=0.1.20
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: biopython>=1.83
 Requires-Dist: Cython>=3.0.7
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: numpy>=1.26.2
-Requires-Dist: pysam>=0.22.0
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: numpy>=1.23.5
 Requires-Dist: pyspoa>=0.2.1
 
 <p align="center"><img src="https://github.com/MasaakiU/MultiplexNanopore/raw/master/resources/logo/SAVEMONEY_logo_with_letter.png"/></p>
 
 *Simple Algorithm for Very Efficient Multiplexing of Oxford Nanopore Experiments for You!*
 
 # Overview
```

### Comparing `savemoney-0.2.8b2/README.md` & `savemoney-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/__about__.py` & `savemoney-0.2.9/savemoney/__about__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 __copyright__    = 'Copyright (C) 2023 Masaaki Uematsu'
-__version__      = 'ver_0.2.8'
+__version__      = 'ver_0.2.9'
 __license__      = 'CC BY-NC-SA 4.0'
 __author__       = 'Masaaki Uematsu'
 __email__        = 'mu84@cornell.edu'
 __url__          = 'https://github.com/MasaakiU/MultiplexNanopore'
 __appname__ = "SAVEMONEY"
 __comment__ = "written by MU"
 __description__ = "Simple Algorithm for Very Efficient Multiplexing of Oxford Nanopore Experiments for You!"
```

### Comparing `savemoney-0.2.8b2/savemoney/__init__.py` & `savemoney-0.2.9/savemoney/__init__.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/ca2bam/__main__.py` & `savemoney-0.2.9/savemoney/ca2bam/__main__.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/modules/NanoporeStats_PDF/NanoporeStats_pdf_0.2.0.csv` & `savemoney-0.2.9/savemoney/modules/NanoporeStats_PDF/NanoporeStats_pdf_0.2.0.csv`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/modules/cython_functions/alignment_functions.cpp` & `savemoney-0.2.9/savemoney/modules/cython_functions/alignment_functions.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.7 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O3"
@@ -37,18 +37,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_7" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x030007F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -598,22 +598,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info;
+        PyObject *version_info; // borrowed
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11;
+        minor_version = 11; // we don't yet need to distinguish between versions > 11
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -663,15 +663,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -1214,16 +1214,31 @@
 #define __PYX_HAVE_API__savemoney__modules__cython_functions__alignment_functions
 /* Early includes */
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
+#include <utility>
+
+    #if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+    // move should be defined for these versions of MSVC, but __cplusplus isn't set usefully
+    #include <type_traits>
+
+    namespace cython_std {
+    template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
+    template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
+    }
+
+    #endif
+    
+#include <map>
 #include <string.h>
 #include <string>
+#include <algorithm>
 #include "pythread.h"
 #include <stdlib.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
@@ -1364,15 +1379,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else
+  #else  // Py < 3.12
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1630,40 +1645,112 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "savemoney/modules/cython_functions/alignment_functions.pyx":43
- * # cythonize -3 -a -i alignment_functions.pyx
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":44
+ * 
  * from libcpp.vector cimport vector #cppvector
  * ctypedef long long LL   # unsigned             # <<<<<<<<<<<<<<
  * ctypedef vector[LL] vec
  * cpdef k_mer_offset_analysis_2(
  */
 typedef PY_LONG_LONG __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL;
+
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":69
+ * from libcpp.string cimport string
+ * from libcpp.algorithm cimport copy
+ * ctypedef long double LD             # <<<<<<<<<<<<<<
+ * ctypedef vector[char] char_vec
+ * ctypedef vector[LD] LD_vec
+ */
+typedef long double __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD;
 /* #### Code section: complex_type_declarations ### */
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
+struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "savemoney/modules/cython_functions/alignment_functions.pyx":44
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":45
  * from libcpp.vector cimport vector #cppvector
  * ctypedef long long LL   # unsigned
  * ctypedef vector[LL] vec             # <<<<<<<<<<<<<<
  * cpdef k_mer_offset_analysis_2(
  *         LL[:] ref_seq_v_repeated,
  */
 typedef std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL>  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec;
 
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":70
+ * from libcpp.algorithm cimport copy
+ * ctypedef long double LD
+ * ctypedef vector[char] char_vec             # <<<<<<<<<<<<<<
+ * ctypedef vector[LD] LD_vec
+ * ctypedef c_map[char, LD] chr_LD_map
+ */
+typedef std::vector<char>  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec;
+
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":71
+ * ctypedef long double LD
+ * ctypedef vector[char] char_vec
+ * ctypedef vector[LD] LD_vec             # <<<<<<<<<<<<<<
+ * ctypedef c_map[char, LD] chr_LD_map
+ * ctypedef c_map[string, LD] str_LD_map
+ */
+typedef std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec;
+
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":72
+ * ctypedef vector[char] char_vec
+ * ctypedef vector[LD] LD_vec
+ * ctypedef c_map[char, LD] chr_LD_map             # <<<<<<<<<<<<<<
+ * ctypedef c_map[string, LD] str_LD_map
+ * ctypedef c_map[string, LD_vec] str_LD_vec_map
+ */
+typedef std::map<char,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_chr_LD_map;
+
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":73
+ * ctypedef vector[LD] LD_vec
+ * ctypedef c_map[char, LD] chr_LD_map
+ * ctypedef c_map[string, LD] str_LD_map             # <<<<<<<<<<<<<<
+ * ctypedef c_map[string, LD_vec] str_LD_vec_map
+ * 
+ */
+typedef std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_map;
+
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":74
+ * ctypedef c_map[char, LD] chr_LD_map
+ * ctypedef c_map[string, LD] str_LD_map
+ * ctypedef c_map[string, LD_vec] str_LD_vec_map             # <<<<<<<<<<<<<<
+ * 
+ * cdef class SequenceBasecallQscorePDF:
+ */
+typedef std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec>  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_vec_map;
+
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":76
+ * ctypedef c_map[string, LD_vec] str_LD_vec_map
+ * 
+ * cdef class SequenceBasecallQscorePDF:             # <<<<<<<<<<<<<<
+ *     # default
+ *     cdef str_LD_map P_base_calling_given_true_refseq_dict
+ */
+struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF {
+  PyObject_HEAD
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_map P_base_calling_given_true_refseq_dict;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_vec_map pdf_core;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec bases;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL N_bases;
+  std::string key;
+};
+
+
 /* "View.MemoryView":114
  * @cython.collection_type("sequence")
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
@@ -1926,14 +2013,113 @@
 
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* IterFinish.proto */
+static CYTHON_INLINE int __Pyx_IterFinish(void);
+
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+#endif
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
+#else
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif
+#endif
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
+#endif
+
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
+
+/* PyObjectCallNoArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
+
+/* RaiseNeedMoreValuesToUnpack.proto */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
+
+/* RaiseTooManyValuesToUnpack.proto */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
+
+/* UnpackItemEndCheck.proto */
+static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected);
+
+/* RaiseNoneIterError.proto */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
+
+/* UnpackTupleError.proto */
+static void __Pyx_UnpackTupleError(PyObject *, Py_ssize_t index);
+
+/* UnpackTuple2.proto */
+#define __Pyx_unpack_tuple2(tuple, value1, value2, is_tuple, has_known_size, decref_tuple)\
+    (likely(is_tuple || PyTuple_Check(tuple)) ?\
+        (likely(has_known_size || PyTuple_GET_SIZE(tuple) == 2) ?\
+            __Pyx_unpack_tuple2_exact(tuple, value1, value2, decref_tuple) :\
+            (__Pyx_UnpackTupleError(tuple, 2), -1)) :\
+        __Pyx_unpack_tuple2_generic(tuple, value1, value2, has_known_size, decref_tuple))
+static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+    PyObject* tuple, PyObject** value1, PyObject** value2, int decref_tuple);
+static int __Pyx_unpack_tuple2_generic(
+    PyObject* tuple, PyObject** value1, PyObject** value2, int has_known_size, int decref_tuple);
+
+/* dict_iter.proto */
+static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
+                                                   Py_ssize_t* p_orig_length, int* p_is_dict);
+static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
+                                              PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
+
 /* TupleAndListFromArray.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
 static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
 #endif
 
 /* IncludeStringH.proto */
@@ -1953,16 +2139,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
-    #define __Pyx_Arg_XDECREF_VARARGS(arg)
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -1970,17 +2156,16 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
-                                                   to have the same reference counting */
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2012,65 +2197,14 @@
     ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* PyFunctionFastCall.proto */
-#if CYTHON_FAST_PYCALL
-#if !CYTHON_VECTORCALL
-#define __Pyx_PyFunction_FastCall(func, args, nargs)\
-    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
-#endif
-#define __Pyx_BUILD_ASSERT_EXPR(cond)\
-    (sizeof(char [1 - 2*!(cond)]) - 1)
-#ifndef Py_MEMBER_SIZE
-#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
-#endif
-#if !CYTHON_VECTORCALL
-#if PY_VERSION_HEX >= 0x03080000
-  #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-  #define __Pxy_PyFrame_Initialize_Offsets()
-  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
-#else
-  static size_t __pyx_pyframe_localsplus_offset = 0;
-  #include "frameobject.h"
-  #define __Pxy_PyFrame_Initialize_Offsets()\
-    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
-     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
-  #define __Pyx_PyFrame_GetLocalsplus(frame)\
-    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif
-#endif
-#endif
-
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
-/* PyObjectCallMethO.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
-#endif
-
-/* PyObjectFastCall.proto */
-#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
-static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
-
 /* RaiseUnexpectedTypeError.proto */
 static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
 
 /* GCCDiagnostics.proto */
 #if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
@@ -2141,17 +2275,14 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* PyObjectCallOneArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
-
 /* ObjectGetItem.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject *__Pyx_PyObject_GetItem(PyObject *obj, PyObject *key);
 #else
 #define __Pyx_PyObject_GetItem(obj, key)  PyObject_GetItem(obj, key)
 #endif
 
@@ -2242,23 +2373,14 @@
     return -1;
   }
 #else
   #define __Pyx_init_assertions_enabled()  (0)
   #define __pyx_assertions_enabled()  (!Py_OptimizeFlag)
 #endif
 
-/* RaiseTooManyValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
-
-/* RaiseNeedMoreValuesToUnpack.proto */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
-
-/* RaiseNoneIterError.proto */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
-
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
@@ -2400,47 +2522,38 @@
 #include <structmember.h>
 
 /* FixUpExtensionType.proto */
 #if CYTHON_USE_TYPE_SPECS
 static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* PyObjectCallNoArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
-
-/* PyObjectCallMethod0.proto */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
-
 /* ValidateBasesTuple.proto */
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
 static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
 #endif
 
 /* PyType_Ready.proto */
 CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
 
+/* SetupReduce.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_setup_reduce(PyObject* type_obj);
+#endif
+
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyTypeObject* typeptr , void* vtable);
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyTypeObject *type);
 
 /* MergeVTables.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_MergeVtables(PyTypeObject *type);
 #endif
 
-/* SetupReduce.proto */
-#if !CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_setup_reduce(PyObject* type_obj);
-#endif
-
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
@@ -2523,15 +2636,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -2632,14 +2745,17 @@
 static int __pyx_memviewslice_is_contig(const __Pyx_memviewslice mvs, char order, int ndim);
 
 /* OverlappingSlices.proto */
 static int __pyx_slices_overlap(__Pyx_memviewslice *slice1,
                                 __Pyx_memviewslice *slice2,
                                 int ndim, size_t itemsize);
 
+/* None.proto */
+#include <new>
+
 /* IsLittleEndian.proto */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
 
 /* BufferFormatCheck.proto */
 static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
 static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
                               __Pyx_BufFmt_StackElem* stack,
@@ -2735,38 +2851,35 @@
 #define __PYX_XCLEAR_MEMVIEW(slice, have_gil) __Pyx_XCLEAR_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XCLEAR_MEMVIEW(__Pyx_memviewslice *, int, int);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *);
 
+/* CIntFromPy.proto */
+static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
-/* None.proto */
-#include <new>
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
-
 /* FormatTypeName.proto */
 #if CYTHON_COMPILING_IN_LIMITED_API
 typedef PyObject *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%U"
 static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
 #define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
 #else
@@ -2795,31 +2908,46 @@
 static PyObject *__pyx_memoryview__get_base(struct __pyx_memoryview_obj *__pyx_v_self); /* proto*/
 static PyObject *__pyx_memoryviewslice_convert_item_to_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp); /* proto*/
 static PyObject *__pyx_memoryviewslice_assign_item_from_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp, PyObject *__pyx_v_value); /* proto*/
 static PyObject *__pyx_memoryviewslice__get_base(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto*/
 
 /* Module declarations from "libcpp.vector" */
 
+/* Module declarations from "libcpp.utility" */
+
+/* Module declarations from "libcpp.map" */
+
 /* Module declarations from "libc.string" */
 
 /* Module declarations from "libcpp.string" */
 
+/* Module declarations from "libcpp" */
+
+/* Module declarations from "libcpp.algorithm" */
+
 /* Module declarations from "savemoney.modules.cython_functions.alignment_functions" */
 static PyObject *__pyx_collections_abc_Sequence = 0;
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
 static PyObject *__pyx_f_9savemoney_7modules_16cython_functions_19alignment_functions_k_mer_offset_analysis_2(__Pyx_memviewslice, __Pyx_memviewslice, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9savemoney_7modules_16cython_functions_19alignment_functions_my_special_dp_cython(std::string, std::string, std::string, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL, int __pyx_skip_dispatch); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
+static std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(PyObject *); /*proto*/
+static std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(PyObject *); /*proto*/
+static std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec>  __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec(PyObject *); /*proto*/
+static std::vector<char>  __pyx_convert_vector_from_py_char(PyObject *); /*proto*/
+static std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL>  __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(PyObject *); /*proto*/
+static std::map<char,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(PyObject *); /*proto*/
 static PyObject *__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL>  const &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  const &); /*proto*/
 static PyObject *__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec(std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec>  const &); /*proto*/
 static int __pyx_array_allocate_buffer(struct __pyx_array_obj *); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
 static int assert_direct_dimensions(Py_ssize_t *, int); /*proto*/
@@ -2857,115 +2985,132 @@
 #define __Pyx_MODULE_NAME "savemoney.modules.cython_functions.alignment_functions"
 extern int __pyx_module_is_main_savemoney__modules__cython_functions__alignment_functions;
 int __pyx_module_is_main_savemoney__modules__cython_functions__alignment_functions = 0;
 
 /* Implementation of "savemoney.modules.cython_functions.alignment_functions" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_range;
+static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_AssertionError;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin___import__;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_enumerate;
-static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_Ellipsis;
 static PyObject *__pyx_builtin_id;
 static PyObject *__pyx_builtin_IndexError;
 /* #### Code section: string_decls ### */
 static const char __pyx_k_[] = ": ";
+static const char __pyx_k_B[] = "B";
 static const char __pyx_k_O[] = "O";
 static const char __pyx_k_c[] = "c";
 static const char __pyx_k__2[] = ".";
 static const char __pyx_k__3[] = "*";
 static const char __pyx_k__6[] = "'";
 static const char __pyx_k__7[] = ")";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
-static const char __pyx_k__24[] = "?";
+static const char __pyx_k__30[] = "?";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_got[] = " (got ";
+static const char __pyx_k_idx[] = "idx";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_sys[] = "sys";
+static const char __pyx_k_val[] = "val";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
+static const char __pyx_k_self[] = "self";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_N_ref[] = "N_ref";
+static const char __pyx_k_bases[] = "bases";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_count[] = "count";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_index[] = "index";
+static const char __pyx_k_items[] = "items";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "__name__";
+static const char __pyx_k_p_list[] = "p_list";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_ref_seq[] = "ref_seq";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
+static const char __pyx_k_P_N_dict[] = "P_N_dict";
 static const char __pyx_k_Sequence[] = "Sequence";
+static const char __pyx_k_base_idx[] = "base_idx";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
+static const char __pyx_k_pdf_core[] = "pdf_core";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_register[] = "register";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_isenabled[] = "isenabled";
+static const char __pyx_k_iteritems[] = "iteritems";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
+static const char __pyx_k_bunshi_P_N[] = "bunshi_P_N";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
+static const char __pyx_k_query_list[] = "query_list";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_bunshi_list[] = "bunshi_list";
 static const char __pyx_k_collections[] = "collections";
 static const char __pyx_k_match_score[] = "match_score";
 static const char __pyx_k_query_seq_1[] = "query_seq_1";
 static const char __pyx_k_query_seq_2[] = "query_seq_2";
 static const char __pyx_k_query_seq_v[] = "query_seq_v";
+static const char __pyx_k_N_query_list[] = "N_query_list";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
+static const char __pyx_k_q_score_list[] = "q_score_list";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_version_info[] = "version_info";
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_AssertionError[] = "AssertionError";
 static const char __pyx_k_mismatch_score[] = "mismatch_score";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
 static const char __pyx_k_len_query_seq_v[] = "len_query_seq_v";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_bunbo_bunshi_sum[] = "bunbo_bunshi_sum";
 static const char __pyx_k_gap_open_penalty[] = "gap_open_penalty";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_gap_extend_penalty[] = "gap_extend_penalty";
 static const char __pyx_k_ref_seq_v_repeated[] = "ref_seq_v_repeated";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
@@ -2975,14 +3120,16 @@
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_Cannot_index_with_type[] = "Cannot index with type '";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_k_mer_offset_analysis_2[] = "k_mer_offset_analysis_2";
 static const char __pyx_k_Dimension_d_is_not_direct[] = "Dimension %d is not direct";
+static const char __pyx_k_SequenceBasecallQscorePDF[] = "SequenceBasecallQscorePDF";
+static const char __pyx_k_calc_consensus_error_rate[] = "calc_consensus_error_rate";
 static const char __pyx_k_Index_out_of_bounds_axis_d[] = "Index out of bounds (axis %d)";
 static const char __pyx_k_Step_may_not_be_zero_axis_d[] = "Step may not be zero (axis %d)";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_All_dimensions_preceding_dimensi[] = "All dimensions preceding dimension %d must be indexed and not sliced";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
@@ -2991,14 +3138,18 @@
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Cannot_transpose_memoryview_with[] = "Cannot transpose memoryview with indirect dimensions";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
 static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got ";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis ";
+static const char __pyx_k_P_base_calling_given_true_refseq[] = "P_base_calling_given_true_refseq_dict";
+static const char __pyx_k_SequenceBasecallQscorePDF___redu[] = "SequenceBasecallQscorePDF.__reduce_cython__";
+static const char __pyx_k_SequenceBasecallQscorePDF___sets[] = "SequenceBasecallQscorePDF.__setstate_cython__";
+static const char __pyx_k_SequenceBasecallQscorePDF_calc_c[] = "SequenceBasecallQscorePDF.calc_consensus_error_rate";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension ";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_savemoney_modules_cython_functio[] = "savemoney/modules/cython_functions/alignment_functions.pyx";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 static const char __pyx_k_savemoney_modules_cython_functio_2[] = "savemoney.modules.cython_functions.alignment_functions";
 /* #### Code section: decls ### */
@@ -3040,15 +3191,20 @@
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_k_mer_offset_analysis_2(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_ref_seq_v_repeated, __Pyx_memviewslice __pyx_v_query_seq_v, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_N_ref, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_len_query_seq_v); /* proto */
+static int __pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF___cinit__(struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *__pyx_v_self, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_map __pyx_v_P_base_calling_given_true_refseq_dict, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_vec_map __pyx_v_pdf_core, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec __pyx_v_bases); /* proto */
+static PyObject *__pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_2calc_consensus_error_rate(struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *__pyx_v_self, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec __pyx_v_query_list, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec __pyx_v_q_score_list, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_chr_LD_map __pyx_v_P_N_dict); /* proto */
+static PyObject *__pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_2my_special_dp_cython(CYTHON_UNUSED PyObject *__pyx_self, std::string __pyx_v_query_seq_1, std::string __pyx_v_query_seq_2, std::string __pyx_v_ref_seq, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_gap_open_penalty, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_gap_extend_penalty, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_match_score, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_mismatch_score); /* proto */
+static PyObject *__pyx_tp_new_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -3079,27 +3235,38 @@
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
   #endif
   #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  PyObject *__pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF;
   PyObject *__pyx_type___pyx_array;
   PyObject *__pyx_type___pyx_MemviewEnum;
   PyObject *__pyx_type___pyx_memoryview;
   PyObject *__pyx_type___pyx_memoryviewslice;
   #endif
+  PyTypeObject *__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF;
   PyTypeObject *__pyx_array_type;
   PyTypeObject *__pyx_MemviewEnum_type;
   PyTypeObject *__pyx_memoryview_type;
   PyTypeObject *__pyx_memoryviewslice_type;
   PyObject *__pyx_kp_u_;
   PyObject *__pyx_n_s_ASCII;
   PyObject *__pyx_kp_s_All_dimensions_preceding_dimensi;
   PyObject *__pyx_n_s_AssertionError;
+  PyObject *__pyx_n_s_B;
   PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
   PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
   PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
   PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
   PyObject *__pyx_kp_u_Cannot_index_with_type;
   PyObject *__pyx_kp_s_Cannot_transpose_memoryview_with;
   PyObject *__pyx_kp_s_Dimension_d_is_not_direct;
@@ -3110,36 +3277,49 @@
   PyObject *__pyx_kp_s_Index_out_of_bounds_axis_d;
   PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
   PyObject *__pyx_kp_u_Invalid_mode_expected_c_or_fortr;
   PyObject *__pyx_kp_u_Invalid_shape_in_axis;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
   PyObject *__pyx_kp_s_MemoryView_of_r_object;
+  PyObject *__pyx_n_s_N_query_list;
   PyObject *__pyx_n_s_N_ref;
   PyObject *__pyx_n_b_O;
   PyObject *__pyx_kp_u_Out_of_bounds_on_buffer_access_a;
+  PyObject *__pyx_n_s_P_N_dict;
+  PyObject *__pyx_n_s_P_base_calling_given_true_refseq;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_Sequence;
+  PyObject *__pyx_n_s_SequenceBasecallQscorePDF;
+  PyObject *__pyx_n_s_SequenceBasecallQscorePDF___redu;
+  PyObject *__pyx_n_s_SequenceBasecallQscorePDF___sets;
+  PyObject *__pyx_n_s_SequenceBasecallQscorePDF_calc_c;
   PyObject *__pyx_kp_s_Step_may_not_be_zero_axis_d;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_View_MemoryView;
   PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_n_s__24;
   PyObject *__pyx_n_s__3;
+  PyObject *__pyx_n_s__30;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_s_abc;
   PyObject *__pyx_n_s_allocate_buffer;
   PyObject *__pyx_kp_u_and;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_base;
+  PyObject *__pyx_n_s_base_idx;
+  PyObject *__pyx_n_s_bases;
+  PyObject *__pyx_n_s_bunbo_bunshi_sum;
+  PyObject *__pyx_n_s_bunshi_P_N;
+  PyObject *__pyx_n_s_bunshi_list;
   PyObject *__pyx_n_s_c;
   PyObject *__pyx_n_u_c;
+  PyObject *__pyx_n_s_calc_consensus_error_rate;
   PyObject *__pyx_n_s_class;
   PyObject *__pyx_n_s_class_getitem;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_collections;
   PyObject *__pyx_kp_s_collections_abc;
   PyObject *__pyx_kp_s_contiguous_and_direct;
   PyObject *__pyx_kp_s_contiguous_and_indirect;
@@ -3158,56 +3338,64 @@
   PyObject *__pyx_n_s_gap_extend_penalty;
   PyObject *__pyx_n_s_gap_open_penalty;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_kp_u_got;
   PyObject *__pyx_kp_u_got_differing_extents_in_dimensi;
   PyObject *__pyx_n_s_id;
+  PyObject *__pyx_n_s_idx;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_index;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
+  PyObject *__pyx_n_s_items;
   PyObject *__pyx_n_s_itemsize;
   PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
+  PyObject *__pyx_n_s_iteritems;
   PyObject *__pyx_n_s_k_mer_offset_analysis_2;
   PyObject *__pyx_n_s_len_query_seq_v;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_match_score;
   PyObject *__pyx_n_s_memview;
   PyObject *__pyx_n_s_mismatch_score;
   PyObject *__pyx_n_s_mode;
   PyObject *__pyx_n_s_my_special_dp_cython;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_name_2;
   PyObject *__pyx_n_s_ndim;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
   PyObject *__pyx_n_s_obj;
+  PyObject *__pyx_n_s_p_list;
   PyObject *__pyx_n_s_pack;
+  PyObject *__pyx_n_s_pdf_core;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_Enum;
   PyObject *__pyx_n_s_pyx_vtable;
+  PyObject *__pyx_n_s_q_score_list;
+  PyObject *__pyx_n_s_query_list;
   PyObject *__pyx_n_s_query_seq_1;
   PyObject *__pyx_n_s_query_seq_2;
   PyObject *__pyx_n_s_query_seq_v;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_ref_seq;
   PyObject *__pyx_n_s_ref_seq_v_repeated;
   PyObject *__pyx_n_s_register;
   PyObject *__pyx_kp_s_savemoney_modules_cython_functio;
   PyObject *__pyx_n_s_savemoney_modules_cython_functio_2;
+  PyObject *__pyx_n_s_self;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shape;
   PyObject *__pyx_n_s_size;
   PyObject *__pyx_n_s_spec;
   PyObject *__pyx_n_s_start;
   PyObject *__pyx_n_s_step;
@@ -3219,14 +3407,15 @@
   PyObject *__pyx_n_s_struct;
   PyObject *__pyx_n_s_sys;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_kp_s_unable_to_allocate_array_data;
   PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
   PyObject *__pyx_n_s_unpack;
   PyObject *__pyx_n_s_update;
+  PyObject *__pyx_n_s_val;
   PyObject *__pyx_n_s_version_info;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_3;
   PyObject *__pyx_int_112105877;
   PyObject *__pyx_int_136983863;
   PyObject *__pyx_int_184977713;
@@ -3242,17 +3431,23 @@
   PyObject *__pyx_tuple__14;
   PyObject *__pyx_tuple__15;
   PyObject *__pyx_tuple__16;
   PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__18;
   PyObject *__pyx_tuple__20;
   PyObject *__pyx_tuple__22;
+  PyObject *__pyx_tuple__24;
+  PyObject *__pyx_tuple__26;
+  PyObject *__pyx_tuple__28;
   PyObject *__pyx_codeobj__19;
   PyObject *__pyx_codeobj__21;
   PyObject *__pyx_codeobj__23;
+  PyObject *__pyx_codeobj__25;
+  PyObject *__pyx_codeobj__27;
+  PyObject *__pyx_codeobj__29;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -3287,26 +3482,29 @@
   Py_CLEAR(clear_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
   #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF);
+  Py_CLEAR(clear_module_state->__pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF);
   Py_CLEAR(clear_module_state->__pyx_array_type);
   Py_CLEAR(clear_module_state->__pyx_type___pyx_array);
   Py_CLEAR(clear_module_state->__pyx_MemviewEnum_type);
   Py_CLEAR(clear_module_state->__pyx_type___pyx_MemviewEnum);
   Py_CLEAR(clear_module_state->__pyx_memoryview_type);
   Py_CLEAR(clear_module_state->__pyx_type___pyx_memoryview);
   Py_CLEAR(clear_module_state->__pyx_memoryviewslice_type);
   Py_CLEAR(clear_module_state->__pyx_type___pyx_memoryviewslice);
   Py_CLEAR(clear_module_state->__pyx_kp_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_ASCII);
   Py_CLEAR(clear_module_state->__pyx_kp_s_All_dimensions_preceding_dimensi);
   Py_CLEAR(clear_module_state->__pyx_n_s_AssertionError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_B);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Buffer_view_does_not_expose_stri);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Can_only_create_a_buffer_that_is);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Cannot_assign_to_read_only_memor);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Cannot_create_writable_memory_vi);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Cannot_index_with_type);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Cannot_transpose_memoryview_with);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Dimension_d_is_not_direct);
@@ -3317,36 +3515,49 @@
   Py_CLEAR(clear_module_state->__pyx_kp_s_Index_out_of_bounds_axis_d);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Indirect_dimensions_not_supporte);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_mode_expected_c_or_fortr);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_shape_in_axis);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_MemoryView_of_r_at_0x_x);
   Py_CLEAR(clear_module_state->__pyx_kp_s_MemoryView_of_r_object);
+  Py_CLEAR(clear_module_state->__pyx_n_s_N_query_list);
   Py_CLEAR(clear_module_state->__pyx_n_s_N_ref);
   Py_CLEAR(clear_module_state->__pyx_n_b_O);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Out_of_bounds_on_buffer_access_a);
+  Py_CLEAR(clear_module_state->__pyx_n_s_P_N_dict);
+  Py_CLEAR(clear_module_state->__pyx_n_s_P_base_calling_given_true_refseq);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Sequence);
+  Py_CLEAR(clear_module_state->__pyx_n_s_SequenceBasecallQscorePDF);
+  Py_CLEAR(clear_module_state->__pyx_n_s_SequenceBasecallQscorePDF___redu);
+  Py_CLEAR(clear_module_state->__pyx_n_s_SequenceBasecallQscorePDF___sets);
+  Py_CLEAR(clear_module_state->__pyx_n_s_SequenceBasecallQscorePDF_calc_c);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_View_MemoryView);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_n_s__24);
   Py_CLEAR(clear_module_state->__pyx_n_s__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s__30);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_abc);
   Py_CLEAR(clear_module_state->__pyx_n_s_allocate_buffer);
   Py_CLEAR(clear_module_state->__pyx_kp_u_and);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_base);
+  Py_CLEAR(clear_module_state->__pyx_n_s_base_idx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bases);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bunbo_bunshi_sum);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bunshi_P_N);
+  Py_CLEAR(clear_module_state->__pyx_n_s_bunshi_list);
   Py_CLEAR(clear_module_state->__pyx_n_s_c);
   Py_CLEAR(clear_module_state->__pyx_n_u_c);
+  Py_CLEAR(clear_module_state->__pyx_n_s_calc_consensus_error_rate);
   Py_CLEAR(clear_module_state->__pyx_n_s_class);
   Py_CLEAR(clear_module_state->__pyx_n_s_class_getitem);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_collections);
   Py_CLEAR(clear_module_state->__pyx_kp_s_collections_abc);
   Py_CLEAR(clear_module_state->__pyx_kp_s_contiguous_and_direct);
   Py_CLEAR(clear_module_state->__pyx_kp_s_contiguous_and_indirect);
@@ -3365,56 +3576,64 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_gap_extend_penalty);
   Py_CLEAR(clear_module_state->__pyx_n_s_gap_open_penalty);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_kp_u_got);
   Py_CLEAR(clear_module_state->__pyx_kp_u_got_differing_extents_in_dimensi);
   Py_CLEAR(clear_module_state->__pyx_n_s_id);
+  Py_CLEAR(clear_module_state->__pyx_n_s_idx);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
+  Py_CLEAR(clear_module_state->__pyx_n_s_items);
   Py_CLEAR(clear_module_state->__pyx_n_s_itemsize);
   Py_CLEAR(clear_module_state->__pyx_kp_s_itemsize_0_for_cython_array);
+  Py_CLEAR(clear_module_state->__pyx_n_s_iteritems);
   Py_CLEAR(clear_module_state->__pyx_n_s_k_mer_offset_analysis_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_len_query_seq_v);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_match_score);
   Py_CLEAR(clear_module_state->__pyx_n_s_memview);
   Py_CLEAR(clear_module_state->__pyx_n_s_mismatch_score);
   Py_CLEAR(clear_module_state->__pyx_n_s_mode);
   Py_CLEAR(clear_module_state->__pyx_n_s_my_special_dp_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_ndim);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj);
+  Py_CLEAR(clear_module_state->__pyx_n_s_p_list);
   Py_CLEAR(clear_module_state->__pyx_n_s_pack);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pdf_core);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_Enum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_q_score_list);
+  Py_CLEAR(clear_module_state->__pyx_n_s_query_list);
   Py_CLEAR(clear_module_state->__pyx_n_s_query_seq_1);
   Py_CLEAR(clear_module_state->__pyx_n_s_query_seq_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_query_seq_v);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_ref_seq);
   Py_CLEAR(clear_module_state->__pyx_n_s_ref_seq_v_repeated);
   Py_CLEAR(clear_module_state->__pyx_n_s_register);
   Py_CLEAR(clear_module_state->__pyx_kp_s_savemoney_modules_cython_functio);
   Py_CLEAR(clear_module_state->__pyx_n_s_savemoney_modules_cython_functio_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shape);
   Py_CLEAR(clear_module_state->__pyx_n_s_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_spec);
   Py_CLEAR(clear_module_state->__pyx_n_s_start);
   Py_CLEAR(clear_module_state->__pyx_n_s_step);
@@ -3426,14 +3645,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_struct);
   Py_CLEAR(clear_module_state->__pyx_n_s_sys);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_kp_s_unable_to_allocate_array_data);
   Py_CLEAR(clear_module_state->__pyx_kp_s_unable_to_allocate_shape_and_str);
   Py_CLEAR(clear_module_state->__pyx_n_s_unpack);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
+  Py_CLEAR(clear_module_state->__pyx_n_s_val);
   Py_CLEAR(clear_module_state->__pyx_n_s_version_info);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_3);
   Py_CLEAR(clear_module_state->__pyx_int_112105877);
   Py_CLEAR(clear_module_state->__pyx_int_136983863);
   Py_CLEAR(clear_module_state->__pyx_int_184977713);
@@ -3449,17 +3669,23 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__14);
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
   Py_CLEAR(clear_module_state->__pyx_tuple__16);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
   Py_CLEAR(clear_module_state->__pyx_tuple__20);
   Py_CLEAR(clear_module_state->__pyx_tuple__22);
+  Py_CLEAR(clear_module_state->__pyx_tuple__24);
+  Py_CLEAR(clear_module_state->__pyx_tuple__26);
+  Py_CLEAR(clear_module_state->__pyx_tuple__28);
   Py_CLEAR(clear_module_state->__pyx_codeobj__19);
   Py_CLEAR(clear_module_state->__pyx_codeobj__21);
   Py_CLEAR(clear_module_state->__pyx_codeobj__23);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__29);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3472,26 +3698,29 @@
   Py_VISIT(traverse_module_state->__pyx_empty_unicode);
   #ifdef __Pyx_CyFunction_USED
   Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
   #endif
   #ifdef __Pyx_FusedFunction_USED
   Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
   #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF);
+  Py_VISIT(traverse_module_state->__pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF);
   Py_VISIT(traverse_module_state->__pyx_array_type);
   Py_VISIT(traverse_module_state->__pyx_type___pyx_array);
   Py_VISIT(traverse_module_state->__pyx_MemviewEnum_type);
   Py_VISIT(traverse_module_state->__pyx_type___pyx_MemviewEnum);
   Py_VISIT(traverse_module_state->__pyx_memoryview_type);
   Py_VISIT(traverse_module_state->__pyx_type___pyx_memoryview);
   Py_VISIT(traverse_module_state->__pyx_memoryviewslice_type);
   Py_VISIT(traverse_module_state->__pyx_type___pyx_memoryviewslice);
   Py_VISIT(traverse_module_state->__pyx_kp_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_ASCII);
   Py_VISIT(traverse_module_state->__pyx_kp_s_All_dimensions_preceding_dimensi);
   Py_VISIT(traverse_module_state->__pyx_n_s_AssertionError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_B);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Buffer_view_does_not_expose_stri);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Can_only_create_a_buffer_that_is);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Cannot_assign_to_read_only_memor);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Cannot_create_writable_memory_vi);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Cannot_index_with_type);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Cannot_transpose_memoryview_with);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Dimension_d_is_not_direct);
@@ -3502,36 +3731,49 @@
   Py_VISIT(traverse_module_state->__pyx_kp_s_Index_out_of_bounds_axis_d);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Indirect_dimensions_not_supporte);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_mode_expected_c_or_fortr);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_shape_in_axis);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_MemoryView_of_r_at_0x_x);
   Py_VISIT(traverse_module_state->__pyx_kp_s_MemoryView_of_r_object);
+  Py_VISIT(traverse_module_state->__pyx_n_s_N_query_list);
   Py_VISIT(traverse_module_state->__pyx_n_s_N_ref);
   Py_VISIT(traverse_module_state->__pyx_n_b_O);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Out_of_bounds_on_buffer_access_a);
+  Py_VISIT(traverse_module_state->__pyx_n_s_P_N_dict);
+  Py_VISIT(traverse_module_state->__pyx_n_s_P_base_calling_given_true_refseq);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Sequence);
+  Py_VISIT(traverse_module_state->__pyx_n_s_SequenceBasecallQscorePDF);
+  Py_VISIT(traverse_module_state->__pyx_n_s_SequenceBasecallQscorePDF___redu);
+  Py_VISIT(traverse_module_state->__pyx_n_s_SequenceBasecallQscorePDF___sets);
+  Py_VISIT(traverse_module_state->__pyx_n_s_SequenceBasecallQscorePDF_calc_c);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_View_MemoryView);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_n_s__24);
   Py_VISIT(traverse_module_state->__pyx_n_s__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s__30);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_abc);
   Py_VISIT(traverse_module_state->__pyx_n_s_allocate_buffer);
   Py_VISIT(traverse_module_state->__pyx_kp_u_and);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_base);
+  Py_VISIT(traverse_module_state->__pyx_n_s_base_idx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bases);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bunbo_bunshi_sum);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bunshi_P_N);
+  Py_VISIT(traverse_module_state->__pyx_n_s_bunshi_list);
   Py_VISIT(traverse_module_state->__pyx_n_s_c);
   Py_VISIT(traverse_module_state->__pyx_n_u_c);
+  Py_VISIT(traverse_module_state->__pyx_n_s_calc_consensus_error_rate);
   Py_VISIT(traverse_module_state->__pyx_n_s_class);
   Py_VISIT(traverse_module_state->__pyx_n_s_class_getitem);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_collections);
   Py_VISIT(traverse_module_state->__pyx_kp_s_collections_abc);
   Py_VISIT(traverse_module_state->__pyx_kp_s_contiguous_and_direct);
   Py_VISIT(traverse_module_state->__pyx_kp_s_contiguous_and_indirect);
@@ -3550,56 +3792,64 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_gap_extend_penalty);
   Py_VISIT(traverse_module_state->__pyx_n_s_gap_open_penalty);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_kp_u_got);
   Py_VISIT(traverse_module_state->__pyx_kp_u_got_differing_extents_in_dimensi);
   Py_VISIT(traverse_module_state->__pyx_n_s_id);
+  Py_VISIT(traverse_module_state->__pyx_n_s_idx);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
+  Py_VISIT(traverse_module_state->__pyx_n_s_items);
   Py_VISIT(traverse_module_state->__pyx_n_s_itemsize);
   Py_VISIT(traverse_module_state->__pyx_kp_s_itemsize_0_for_cython_array);
+  Py_VISIT(traverse_module_state->__pyx_n_s_iteritems);
   Py_VISIT(traverse_module_state->__pyx_n_s_k_mer_offset_analysis_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_len_query_seq_v);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_match_score);
   Py_VISIT(traverse_module_state->__pyx_n_s_memview);
   Py_VISIT(traverse_module_state->__pyx_n_s_mismatch_score);
   Py_VISIT(traverse_module_state->__pyx_n_s_mode);
   Py_VISIT(traverse_module_state->__pyx_n_s_my_special_dp_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_ndim);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj);
+  Py_VISIT(traverse_module_state->__pyx_n_s_p_list);
   Py_VISIT(traverse_module_state->__pyx_n_s_pack);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pdf_core);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_Enum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_q_score_list);
+  Py_VISIT(traverse_module_state->__pyx_n_s_query_list);
   Py_VISIT(traverse_module_state->__pyx_n_s_query_seq_1);
   Py_VISIT(traverse_module_state->__pyx_n_s_query_seq_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_query_seq_v);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_ref_seq);
   Py_VISIT(traverse_module_state->__pyx_n_s_ref_seq_v_repeated);
   Py_VISIT(traverse_module_state->__pyx_n_s_register);
   Py_VISIT(traverse_module_state->__pyx_kp_s_savemoney_modules_cython_functio);
   Py_VISIT(traverse_module_state->__pyx_n_s_savemoney_modules_cython_functio_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shape);
   Py_VISIT(traverse_module_state->__pyx_n_s_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_spec);
   Py_VISIT(traverse_module_state->__pyx_n_s_start);
   Py_VISIT(traverse_module_state->__pyx_n_s_step);
@@ -3611,14 +3861,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_struct);
   Py_VISIT(traverse_module_state->__pyx_n_s_sys);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_kp_s_unable_to_allocate_array_data);
   Py_VISIT(traverse_module_state->__pyx_kp_s_unable_to_allocate_shape_and_str);
   Py_VISIT(traverse_module_state->__pyx_n_s_unpack);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
+  Py_VISIT(traverse_module_state->__pyx_n_s_val);
   Py_VISIT(traverse_module_state->__pyx_n_s_version_info);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_3);
   Py_VISIT(traverse_module_state->__pyx_int_112105877);
   Py_VISIT(traverse_module_state->__pyx_int_136983863);
   Py_VISIT(traverse_module_state->__pyx_int_184977713);
@@ -3634,17 +3885,23 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__14);
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
   Py_VISIT(traverse_module_state->__pyx_tuple__16);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
   Py_VISIT(traverse_module_state->__pyx_tuple__20);
   Py_VISIT(traverse_module_state->__pyx_tuple__22);
+  Py_VISIT(traverse_module_state->__pyx_tuple__24);
+  Py_VISIT(traverse_module_state->__pyx_tuple__26);
+  Py_VISIT(traverse_module_state->__pyx_tuple__28);
   Py_VISIT(traverse_module_state->__pyx_codeobj__19);
   Py_VISIT(traverse_module_state->__pyx_codeobj__21);
   Py_VISIT(traverse_module_state->__pyx_codeobj__23);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__29);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -3672,27 +3929,38 @@
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
 #endif
 #if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#define __pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF __pyx_mstate_global->__pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF
 #define __pyx_type___pyx_array __pyx_mstate_global->__pyx_type___pyx_array
 #define __pyx_type___pyx_MemviewEnum __pyx_mstate_global->__pyx_type___pyx_MemviewEnum
 #define __pyx_type___pyx_memoryview __pyx_mstate_global->__pyx_type___pyx_memoryview
 #define __pyx_type___pyx_memoryviewslice __pyx_mstate_global->__pyx_type___pyx_memoryviewslice
 #endif
+#define __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF __pyx_mstate_global->__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF
 #define __pyx_array_type __pyx_mstate_global->__pyx_array_type
 #define __pyx_MemviewEnum_type __pyx_mstate_global->__pyx_MemviewEnum_type
 #define __pyx_memoryview_type __pyx_mstate_global->__pyx_memoryview_type
 #define __pyx_memoryviewslice_type __pyx_mstate_global->__pyx_memoryviewslice_type
 #define __pyx_kp_u_ __pyx_mstate_global->__pyx_kp_u_
 #define __pyx_n_s_ASCII __pyx_mstate_global->__pyx_n_s_ASCII
 #define __pyx_kp_s_All_dimensions_preceding_dimensi __pyx_mstate_global->__pyx_kp_s_All_dimensions_preceding_dimensi
 #define __pyx_n_s_AssertionError __pyx_mstate_global->__pyx_n_s_AssertionError
+#define __pyx_n_s_B __pyx_mstate_global->__pyx_n_s_B
 #define __pyx_kp_s_Buffer_view_does_not_expose_stri __pyx_mstate_global->__pyx_kp_s_Buffer_view_does_not_expose_stri
 #define __pyx_kp_s_Can_only_create_a_buffer_that_is __pyx_mstate_global->__pyx_kp_s_Can_only_create_a_buffer_that_is
 #define __pyx_kp_s_Cannot_assign_to_read_only_memor __pyx_mstate_global->__pyx_kp_s_Cannot_assign_to_read_only_memor
 #define __pyx_kp_s_Cannot_create_writable_memory_vi __pyx_mstate_global->__pyx_kp_s_Cannot_create_writable_memory_vi
 #define __pyx_kp_u_Cannot_index_with_type __pyx_mstate_global->__pyx_kp_u_Cannot_index_with_type
 #define __pyx_kp_s_Cannot_transpose_memoryview_with __pyx_mstate_global->__pyx_kp_s_Cannot_transpose_memoryview_with
 #define __pyx_kp_s_Dimension_d_is_not_direct __pyx_mstate_global->__pyx_kp_s_Dimension_d_is_not_direct
@@ -3703,36 +3971,49 @@
 #define __pyx_kp_s_Index_out_of_bounds_axis_d __pyx_mstate_global->__pyx_kp_s_Index_out_of_bounds_axis_d
 #define __pyx_kp_s_Indirect_dimensions_not_supporte __pyx_mstate_global->__pyx_kp_s_Indirect_dimensions_not_supporte
 #define __pyx_kp_u_Invalid_mode_expected_c_or_fortr __pyx_mstate_global->__pyx_kp_u_Invalid_mode_expected_c_or_fortr
 #define __pyx_kp_u_Invalid_shape_in_axis __pyx_mstate_global->__pyx_kp_u_Invalid_shape_in_axis
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_kp_s_MemoryView_of_r_at_0x_x __pyx_mstate_global->__pyx_kp_s_MemoryView_of_r_at_0x_x
 #define __pyx_kp_s_MemoryView_of_r_object __pyx_mstate_global->__pyx_kp_s_MemoryView_of_r_object
+#define __pyx_n_s_N_query_list __pyx_mstate_global->__pyx_n_s_N_query_list
 #define __pyx_n_s_N_ref __pyx_mstate_global->__pyx_n_s_N_ref
 #define __pyx_n_b_O __pyx_mstate_global->__pyx_n_b_O
 #define __pyx_kp_u_Out_of_bounds_on_buffer_access_a __pyx_mstate_global->__pyx_kp_u_Out_of_bounds_on_buffer_access_a
+#define __pyx_n_s_P_N_dict __pyx_mstate_global->__pyx_n_s_P_N_dict
+#define __pyx_n_s_P_base_calling_given_true_refseq __pyx_mstate_global->__pyx_n_s_P_base_calling_given_true_refseq
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_Sequence __pyx_mstate_global->__pyx_n_s_Sequence
+#define __pyx_n_s_SequenceBasecallQscorePDF __pyx_mstate_global->__pyx_n_s_SequenceBasecallQscorePDF
+#define __pyx_n_s_SequenceBasecallQscorePDF___redu __pyx_mstate_global->__pyx_n_s_SequenceBasecallQscorePDF___redu
+#define __pyx_n_s_SequenceBasecallQscorePDF___sets __pyx_mstate_global->__pyx_n_s_SequenceBasecallQscorePDF___sets
+#define __pyx_n_s_SequenceBasecallQscorePDF_calc_c __pyx_mstate_global->__pyx_n_s_SequenceBasecallQscorePDF_calc_c
 #define __pyx_kp_s_Step_may_not_be_zero_axis_d __pyx_mstate_global->__pyx_kp_s_Step_may_not_be_zero_axis_d
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_kp_s_Unable_to_convert_item_to_object __pyx_mstate_global->__pyx_kp_s_Unable_to_convert_item_to_object
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_View_MemoryView __pyx_mstate_global->__pyx_n_s_View_MemoryView
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_n_s__24 __pyx_mstate_global->__pyx_n_s__24
 #define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
+#define __pyx_n_s__30 __pyx_mstate_global->__pyx_n_s__30
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_s_abc __pyx_mstate_global->__pyx_n_s_abc
 #define __pyx_n_s_allocate_buffer __pyx_mstate_global->__pyx_n_s_allocate_buffer
 #define __pyx_kp_u_and __pyx_mstate_global->__pyx_kp_u_and
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_base __pyx_mstate_global->__pyx_n_s_base
+#define __pyx_n_s_base_idx __pyx_mstate_global->__pyx_n_s_base_idx
+#define __pyx_n_s_bases __pyx_mstate_global->__pyx_n_s_bases
+#define __pyx_n_s_bunbo_bunshi_sum __pyx_mstate_global->__pyx_n_s_bunbo_bunshi_sum
+#define __pyx_n_s_bunshi_P_N __pyx_mstate_global->__pyx_n_s_bunshi_P_N
+#define __pyx_n_s_bunshi_list __pyx_mstate_global->__pyx_n_s_bunshi_list
 #define __pyx_n_s_c __pyx_mstate_global->__pyx_n_s_c
 #define __pyx_n_u_c __pyx_mstate_global->__pyx_n_u_c
+#define __pyx_n_s_calc_consensus_error_rate __pyx_mstate_global->__pyx_n_s_calc_consensus_error_rate
 #define __pyx_n_s_class __pyx_mstate_global->__pyx_n_s_class
 #define __pyx_n_s_class_getitem __pyx_mstate_global->__pyx_n_s_class_getitem
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_collections __pyx_mstate_global->__pyx_n_s_collections
 #define __pyx_kp_s_collections_abc __pyx_mstate_global->__pyx_kp_s_collections_abc
 #define __pyx_kp_s_contiguous_and_direct __pyx_mstate_global->__pyx_kp_s_contiguous_and_direct
 #define __pyx_kp_s_contiguous_and_indirect __pyx_mstate_global->__pyx_kp_s_contiguous_and_indirect
@@ -3751,56 +4032,64 @@
 #define __pyx_n_s_gap_extend_penalty __pyx_mstate_global->__pyx_n_s_gap_extend_penalty
 #define __pyx_n_s_gap_open_penalty __pyx_mstate_global->__pyx_n_s_gap_open_penalty
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_kp_u_got __pyx_mstate_global->__pyx_kp_u_got
 #define __pyx_kp_u_got_differing_extents_in_dimensi __pyx_mstate_global->__pyx_kp_u_got_differing_extents_in_dimensi
 #define __pyx_n_s_id __pyx_mstate_global->__pyx_n_s_id
+#define __pyx_n_s_idx __pyx_mstate_global->__pyx_n_s_idx
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
+#define __pyx_n_s_items __pyx_mstate_global->__pyx_n_s_items
 #define __pyx_n_s_itemsize __pyx_mstate_global->__pyx_n_s_itemsize
 #define __pyx_kp_s_itemsize_0_for_cython_array __pyx_mstate_global->__pyx_kp_s_itemsize_0_for_cython_array
+#define __pyx_n_s_iteritems __pyx_mstate_global->__pyx_n_s_iteritems
 #define __pyx_n_s_k_mer_offset_analysis_2 __pyx_mstate_global->__pyx_n_s_k_mer_offset_analysis_2
 #define __pyx_n_s_len_query_seq_v __pyx_mstate_global->__pyx_n_s_len_query_seq_v
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_match_score __pyx_mstate_global->__pyx_n_s_match_score
 #define __pyx_n_s_memview __pyx_mstate_global->__pyx_n_s_memview
 #define __pyx_n_s_mismatch_score __pyx_mstate_global->__pyx_n_s_mismatch_score
 #define __pyx_n_s_mode __pyx_mstate_global->__pyx_n_s_mode
 #define __pyx_n_s_my_special_dp_cython __pyx_mstate_global->__pyx_n_s_my_special_dp_cython
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
 #define __pyx_n_s_ndim __pyx_mstate_global->__pyx_n_s_ndim
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
 #define __pyx_n_s_obj __pyx_mstate_global->__pyx_n_s_obj
+#define __pyx_n_s_p_list __pyx_mstate_global->__pyx_n_s_p_list
 #define __pyx_n_s_pack __pyx_mstate_global->__pyx_n_s_pack
+#define __pyx_n_s_pdf_core __pyx_mstate_global->__pyx_n_s_pdf_core
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_Enum __pyx_mstate_global->__pyx_n_s_pyx_unpickle_Enum
 #define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
+#define __pyx_n_s_q_score_list __pyx_mstate_global->__pyx_n_s_q_score_list
+#define __pyx_n_s_query_list __pyx_mstate_global->__pyx_n_s_query_list
 #define __pyx_n_s_query_seq_1 __pyx_mstate_global->__pyx_n_s_query_seq_1
 #define __pyx_n_s_query_seq_2 __pyx_mstate_global->__pyx_n_s_query_seq_2
 #define __pyx_n_s_query_seq_v __pyx_mstate_global->__pyx_n_s_query_seq_v
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_ref_seq __pyx_mstate_global->__pyx_n_s_ref_seq
 #define __pyx_n_s_ref_seq_v_repeated __pyx_mstate_global->__pyx_n_s_ref_seq_v_repeated
 #define __pyx_n_s_register __pyx_mstate_global->__pyx_n_s_register
 #define __pyx_kp_s_savemoney_modules_cython_functio __pyx_mstate_global->__pyx_kp_s_savemoney_modules_cython_functio
 #define __pyx_n_s_savemoney_modules_cython_functio_2 __pyx_mstate_global->__pyx_n_s_savemoney_modules_cython_functio_2
+#define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shape __pyx_mstate_global->__pyx_n_s_shape
 #define __pyx_n_s_size __pyx_mstate_global->__pyx_n_s_size
 #define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
 #define __pyx_n_s_start __pyx_mstate_global->__pyx_n_s_start
 #define __pyx_n_s_step __pyx_mstate_global->__pyx_n_s_step
@@ -3812,14 +4101,15 @@
 #define __pyx_n_s_struct __pyx_mstate_global->__pyx_n_s_struct
 #define __pyx_n_s_sys __pyx_mstate_global->__pyx_n_s_sys
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_kp_s_unable_to_allocate_array_data __pyx_mstate_global->__pyx_kp_s_unable_to_allocate_array_data
 #define __pyx_kp_s_unable_to_allocate_shape_and_str __pyx_mstate_global->__pyx_kp_s_unable_to_allocate_shape_and_str
 #define __pyx_n_s_unpack __pyx_mstate_global->__pyx_n_s_unpack
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
+#define __pyx_n_s_val __pyx_mstate_global->__pyx_n_s_val
 #define __pyx_n_s_version_info __pyx_mstate_global->__pyx_n_s_version_info
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_3 __pyx_mstate_global->__pyx_int_3
 #define __pyx_int_112105877 __pyx_mstate_global->__pyx_int_112105877
 #define __pyx_int_136983863 __pyx_mstate_global->__pyx_int_136983863
 #define __pyx_int_184977713 __pyx_mstate_global->__pyx_int_184977713
@@ -3835,17 +4125,23 @@
 #define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
 #define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
 #define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
+#define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
+#define __pyx_tuple__26 __pyx_mstate_global->__pyx_tuple__26
+#define __pyx_tuple__28 __pyx_mstate_global->__pyx_tuple__28
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
+#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
+#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
+#define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 /* #### Code section: module_code ### */
 
 /* "string.from_py":13
  * 
  * @cname("__pyx_convert_string_from_py_std__in_string")
  * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t length = 0
@@ -3909,14 +4205,993 @@
   __pyx_L1_error:;
   __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   return __pyx_r;
 }
 
+/* "map.from_py":207
+ * 
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ */
+
+static std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(PyObject *__pyx_v_o) {
+  std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_v_m;
+  PyObject *__pyx_v_key = NULL;
+  PyObject *__pyx_v_value = NULL;
+  std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  std::string __pyx_t_9;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD __pyx_t_10;
+  std::pair<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD", 1);
+
+  /* "map.from_py":209
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:             # <<<<<<<<<<<<<<
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ */
+  __pyx_t_1 = (PY_MAJOR_VERSION < 3);
+  if (__pyx_t_1) {
+
+    /* "map.from_py":210
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ *         for key, value in o.iteritems():             # <<<<<<<<<<<<<<
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     else:
+ */
+    __pyx_t_3 = 0;
+    if (unlikely(__pyx_v_o == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "iteritems");
+      __PYX_ERR(1, 210, __pyx_L1_error)
+    }
+    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_o, 0, __pyx_n_s_iteritems, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_2);
+    __pyx_t_2 = __pyx_t_6;
+    __pyx_t_6 = 0;
+    while (1) {
+      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
+      if (unlikely(__pyx_t_8 == 0)) break;
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 210, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
+      __pyx_t_6 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_7);
+      __pyx_t_7 = 0;
+
+      /* "map.from_py":211
+ *     if PY_MAJOR_VERSION < 3:
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
+ *     else:
+ *         for key, value in o.items():
+ */
+      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 211, __pyx_L1_error)
+      __pyx_t_10 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_10 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(1, 211, __pyx_L1_error)
+      try {
+        __pyx_t_11 = std::pair<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD> (((std::string)__pyx_t_9), ((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)__pyx_t_10));
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 211, __pyx_L1_error)
+      }
+      try {
+        __pyx_v_m.insert(__pyx_t_11);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 211, __pyx_L1_error)
+      }
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "map.from_py":209
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:             # <<<<<<<<<<<<<<
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ */
+    goto __pyx_L3;
+  }
+
+  /* "map.from_py":213
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     else:
+ *         for key, value in o.items():             # <<<<<<<<<<<<<<
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     return m
+ */
+  /*else*/ {
+    __pyx_t_4 = 0;
+    if (unlikely(__pyx_v_o == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
+      __PYX_ERR(1, 213, __pyx_L1_error)
+    }
+    __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_o, 0, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_5)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_2);
+    __pyx_t_2 = __pyx_t_7;
+    __pyx_t_7 = 0;
+    while (1) {
+      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_3, &__pyx_t_4, &__pyx_t_7, &__pyx_t_6, NULL, __pyx_t_5);
+      if (unlikely(__pyx_t_8 == 0)) break;
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 213, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_7);
+      __pyx_t_7 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_6);
+      __pyx_t_6 = 0;
+
+      /* "map.from_py":214
+ *     else:
+ *         for key, value in o.items():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
+ *     return m
+ * 
+ */
+      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 214, __pyx_L1_error)
+      __pyx_t_10 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_10 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(1, 214, __pyx_L1_error)
+      try {
+        __pyx_t_11 = std::pair<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD> (((std::string)__pyx_t_9), ((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)__pyx_t_10));
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 214, __pyx_L1_error)
+      }
+      try {
+        __pyx_v_m.insert(__pyx_t_11);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 214, __pyx_L1_error)
+      }
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_L3:;
+
+  /* "map.from_py":215
+ *         for key, value in o.items():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     return m             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_m;
+  goto __pyx_L0;
+
+  /* "map.from_py":207
+ * 
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_key);
+  __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef vector[X] __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+static std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(PyObject *__pyx_v_o) {
+  std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD", 1);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_v_item); if (unlikely((__pyx_t_5 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef vector[X] __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "map.from_py":207
+ * 
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ */
+
+static std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec>  __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec(PyObject *__pyx_v_o) {
+  std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec>  __pyx_v_m;
+  PyObject *__pyx_v_key = NULL;
+  PyObject *__pyx_v_value = NULL;
+  std::map<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  std::string __pyx_t_9;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec __pyx_t_10;
+  std::pair<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec>  __pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec", 1);
+
+  /* "map.from_py":209
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec(object o) except *:
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:             # <<<<<<<<<<<<<<
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ */
+  __pyx_t_1 = (PY_MAJOR_VERSION < 3);
+  if (__pyx_t_1) {
+
+    /* "map.from_py":210
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ *         for key, value in o.iteritems():             # <<<<<<<<<<<<<<
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     else:
+ */
+    __pyx_t_3 = 0;
+    if (unlikely(__pyx_v_o == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "iteritems");
+      __PYX_ERR(1, 210, __pyx_L1_error)
+    }
+    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_o, 0, __pyx_n_s_iteritems, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_2);
+    __pyx_t_2 = __pyx_t_6;
+    __pyx_t_6 = 0;
+    while (1) {
+      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
+      if (unlikely(__pyx_t_8 == 0)) break;
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 210, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
+      __pyx_t_6 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_7);
+      __pyx_t_7 = 0;
+
+      /* "map.from_py":211
+ *     if PY_MAJOR_VERSION < 3:
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
+ *     else:
+ *         for key, value in o.items():
+ */
+      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 211, __pyx_L1_error)
+      __pyx_t_10 = __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(__pyx_v_value); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 211, __pyx_L1_error)
+      try {
+        __pyx_t_11 = std::pair<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec> (((std::string)__pyx_t_9), ((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec)__pyx_t_10));
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 211, __pyx_L1_error)
+      }
+      try {
+        __pyx_v_m.insert(__pyx_t_11);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 211, __pyx_L1_error)
+      }
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "map.from_py":209
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec(object o) except *:
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:             # <<<<<<<<<<<<<<
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ */
+    goto __pyx_L3;
+  }
+
+  /* "map.from_py":213
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     else:
+ *         for key, value in o.items():             # <<<<<<<<<<<<<<
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     return m
+ */
+  /*else*/ {
+    __pyx_t_4 = 0;
+    if (unlikely(__pyx_v_o == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
+      __PYX_ERR(1, 213, __pyx_L1_error)
+    }
+    __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_o, 0, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_5)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_2);
+    __pyx_t_2 = __pyx_t_7;
+    __pyx_t_7 = 0;
+    while (1) {
+      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_3, &__pyx_t_4, &__pyx_t_7, &__pyx_t_6, NULL, __pyx_t_5);
+      if (unlikely(__pyx_t_8 == 0)) break;
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 213, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_7);
+      __pyx_t_7 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_6);
+      __pyx_t_6 = 0;
+
+      /* "map.from_py":214
+ *     else:
+ *         for key, value in o.items():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
+ *     return m
+ * 
+ */
+      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_v_key); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 214, __pyx_L1_error)
+      __pyx_t_10 = __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(__pyx_v_value); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 214, __pyx_L1_error)
+      try {
+        __pyx_t_11 = std::pair<std::string,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec> (((std::string)__pyx_t_9), ((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec)__pyx_t_10));
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 214, __pyx_L1_error)
+      }
+      try {
+        __pyx_v_m.insert(__pyx_t_11);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 214, __pyx_L1_error)
+      }
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_L3:;
+
+  /* "map.from_py":215
+ *         for key, value in o.items():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     return m             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_m;
+  goto __pyx_L0;
+
+  /* "map.from_py":207
+ * 
+ * @cname("__pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec")
+ * cdef map[X,Y] __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_key);
+  __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_char")
+ * cdef vector[X] __pyx_convert_vector_from_py_char(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+static std::vector<char>  __pyx_convert_vector_from_py_char(PyObject *__pyx_v_o) {
+  std::vector<char>  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<char>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  char __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_char", 1);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_char(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __Pyx_PyInt_As_char(__pyx_v_item); if (unlikely((__pyx_t_5 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((char)__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_char(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_char")
+ * cdef vector[X] __pyx_convert_vector_from_py_char(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_char", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL>  __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(PyObject *__pyx_v_o) {
+  std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL>  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL", 1);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1);
+    __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+          #endif
+          if (__pyx_t_2 >= __pyx_temp) break;
+        }
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_item); if (unlikely((__pyx_t_5 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL)__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL")
+ * cdef vector[X] __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "map.from_py":207
+ * 
+ * @cname("__pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef map[X,Y] __pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ */
+
+static std::map<char,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(PyObject *__pyx_v_o) {
+  std::map<char,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_v_m;
+  PyObject *__pyx_v_key = NULL;
+  PyObject *__pyx_v_value = NULL;
+  std::map<char,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  char __pyx_t_9;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD __pyx_t_10;
+  std::pair<char,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  __pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD", 1);
+
+  /* "map.from_py":209
+ * cdef map[X,Y] __pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:             # <<<<<<<<<<<<<<
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ */
+  __pyx_t_1 = (PY_MAJOR_VERSION < 3);
+  if (__pyx_t_1) {
+
+    /* "map.from_py":210
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ *         for key, value in o.iteritems():             # <<<<<<<<<<<<<<
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     else:
+ */
+    __pyx_t_3 = 0;
+    if (unlikely(__pyx_v_o == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "iteritems");
+      __PYX_ERR(1, 210, __pyx_L1_error)
+    }
+    __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_o, 0, __pyx_n_s_iteritems, (&__pyx_t_4), (&__pyx_t_5)); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_2);
+    __pyx_t_2 = __pyx_t_6;
+    __pyx_t_6 = 0;
+    while (1) {
+      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_4, &__pyx_t_3, &__pyx_t_6, &__pyx_t_7, NULL, __pyx_t_5);
+      if (unlikely(__pyx_t_8 == 0)) break;
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 210, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_6);
+      __pyx_t_6 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_7);
+      __pyx_t_7 = 0;
+
+      /* "map.from_py":211
+ *     if PY_MAJOR_VERSION < 3:
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
+ *     else:
+ *         for key, value in o.items():
+ */
+      __pyx_t_9 = __Pyx_PyInt_As_char(__pyx_v_key); if (unlikely((__pyx_t_9 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 211, __pyx_L1_error)
+      __pyx_t_10 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_10 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(1, 211, __pyx_L1_error)
+      try {
+        __pyx_t_11 = std::pair<char,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD> (((char)__pyx_t_9), ((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)__pyx_t_10));
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 211, __pyx_L1_error)
+      }
+      try {
+        __pyx_v_m.insert(__pyx_t_11);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 211, __pyx_L1_error)
+      }
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "map.from_py":209
+ * cdef map[X,Y] __pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:             # <<<<<<<<<<<<<<
+ *         for key, value in o.iteritems():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ */
+    goto __pyx_L3;
+  }
+
+  /* "map.from_py":213
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     else:
+ *         for key, value in o.items():             # <<<<<<<<<<<<<<
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     return m
+ */
+  /*else*/ {
+    __pyx_t_4 = 0;
+    if (unlikely(__pyx_v_o == Py_None)) {
+      PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
+      __PYX_ERR(1, 213, __pyx_L1_error)
+    }
+    __pyx_t_7 = __Pyx_dict_iterator(__pyx_v_o, 0, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_5)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_2);
+    __pyx_t_2 = __pyx_t_7;
+    __pyx_t_7 = 0;
+    while (1) {
+      __pyx_t_8 = __Pyx_dict_iter_next(__pyx_t_2, __pyx_t_3, &__pyx_t_4, &__pyx_t_7, &__pyx_t_6, NULL, __pyx_t_5);
+      if (unlikely(__pyx_t_8 == 0)) break;
+      if (unlikely(__pyx_t_8 == -1)) __PYX_ERR(1, 213, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_XDECREF_SET(__pyx_v_key, __pyx_t_7);
+      __pyx_t_7 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_value, __pyx_t_6);
+      __pyx_t_6 = 0;
+
+      /* "map.from_py":214
+ *     else:
+ *         for key, value in o.items():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))             # <<<<<<<<<<<<<<
+ *     return m
+ * 
+ */
+      __pyx_t_9 = __Pyx_PyInt_As_char(__pyx_v_key); if (unlikely((__pyx_t_9 == (char)-1) && PyErr_Occurred())) __PYX_ERR(1, 214, __pyx_L1_error)
+      __pyx_t_10 = __pyx_PyFloat_AsDouble(__pyx_v_value); if (unlikely((__pyx_t_10 == (long double)-1) && PyErr_Occurred())) __PYX_ERR(1, 214, __pyx_L1_error)
+      try {
+        __pyx_t_11 = std::pair<char,__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD> (((char)__pyx_t_9), ((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)__pyx_t_10));
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 214, __pyx_L1_error)
+      }
+      try {
+        __pyx_v_m.insert(__pyx_t_11);
+      } catch(...) {
+        __Pyx_CppExn2PyErr();
+        __PYX_ERR(1, 214, __pyx_L1_error)
+      }
+    }
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+  __pyx_L3:;
+
+  /* "map.from_py":215
+ *         for key, value in o.items():
+ *             m.insert(pair[X,Y](<X>key, <Y>value))
+ *     return m             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_m;
+  goto __pyx_L0;
+
+  /* "map.from_py":207
+ * 
+ * @cname("__pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef map[X,Y] __pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef map[X,Y] m
+ *     if PY_MAJOR_VERSION < 3:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_AddTraceback("map.from_py.__pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_key);
+  __Pyx_XDECREF(__pyx_v_value);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "vector.to_py":66
  * 
  * @cname("__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL")
  * cdef object __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(const vector[X]& v):             # <<<<<<<<<<<<<<
  *     if v.size() > <size_t> PY_SSIZE_T_MAX:
  *         raise MemoryError()
  */
@@ -4058,14 +5333,155 @@
   __Pyx_XDECREF(__pyx_v_o);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+static PyObject *__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD>  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD", 1);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef object __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef object __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD")
+ * cdef object __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 static PyObject *__pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec(std::vector<__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec>  const &__pyx_v_v) {
   Py_ssize_t __pyx_v_v_size_signed;
   PyObject *__pyx_v_o = NULL;
   Py_ssize_t __pyx_v_i;
   PyObject *__pyx_v_item = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -17825,15 +19241,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "savemoney/modules/cython_functions/alignment_functions.pyx":45
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":46
  * ctypedef long long LL   # unsigned
  * ctypedef vector[LL] vec
  * cpdef k_mer_offset_analysis_2(             # <<<<<<<<<<<<<<
  *         LL[:] ref_seq_v_repeated,
  *         LL[:] query_seq_v,
  */
 
@@ -17862,131 +19278,131 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("k_mer_offset_analysis_2", 1);
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":55
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":56
  *     cdef LL s
  *     cdef vec result_array
  *     result_array.reserve(N_ref)             # <<<<<<<<<<<<<<
  *     s = 0
  *     for k in range(N_ref):    # k
  */
   try {
     __pyx_v_result_array.reserve(__pyx_v_N_ref);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 55, __pyx_L1_error)
+    __PYX_ERR(0, 56, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":56
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":57
  *     cdef vec result_array
  *     result_array.reserve(N_ref)
  *     s = 0             # <<<<<<<<<<<<<<
  *     for k in range(N_ref):    # k
  *         for i in range(len_query_seq_v):
  */
   __pyx_v_s = 0;
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":57
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":58
  *     result_array.reserve(N_ref)
  *     s = 0
  *     for k in range(N_ref):    # k             # <<<<<<<<<<<<<<
  *         for i in range(len_query_seq_v):
  *             if ref_seq_v_repeated[k + i] == query_seq_v[i]:
  */
   __pyx_t_1 = __pyx_v_N_ref;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_k = __pyx_t_3;
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":58
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":59
  *     s = 0
  *     for k in range(N_ref):    # k
  *         for i in range(len_query_seq_v):             # <<<<<<<<<<<<<<
  *             if ref_seq_v_repeated[k + i] == query_seq_v[i]:
  *                 s += 1
  */
     __pyx_t_4 = __pyx_v_len_query_seq_v;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":59
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":60
  *     for k in range(N_ref):    # k
  *         for i in range(len_query_seq_v):
  *             if ref_seq_v_repeated[k + i] == query_seq_v[i]:             # <<<<<<<<<<<<<<
  *                 s += 1
  *         result_array.push_back(s)
  */
       __pyx_t_7 = (__pyx_v_k + __pyx_v_i);
       __pyx_t_8 = __pyx_v_i;
       __pyx_t_9 = ((*((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL *) ( /* dim=0 */ (__pyx_v_ref_seq_v_repeated.data + __pyx_t_7 * __pyx_v_ref_seq_v_repeated.strides[0]) ))) == (*((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL *) ( /* dim=0 */ (__pyx_v_query_seq_v.data + __pyx_t_8 * __pyx_v_query_seq_v.strides[0]) ))));
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":60
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":61
  *         for i in range(len_query_seq_v):
  *             if ref_seq_v_repeated[k + i] == query_seq_v[i]:
  *                 s += 1             # <<<<<<<<<<<<<<
  *         result_array.push_back(s)
  *         s = 0
  */
         __pyx_v_s = (__pyx_v_s + 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":59
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":60
  *     for k in range(N_ref):    # k
  *         for i in range(len_query_seq_v):
  *             if ref_seq_v_repeated[k + i] == query_seq_v[i]:             # <<<<<<<<<<<<<<
  *                 s += 1
  *         result_array.push_back(s)
  */
       }
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":61
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":62
  *             if ref_seq_v_repeated[k + i] == query_seq_v[i]:
  *                 s += 1
  *         result_array.push_back(s)             # <<<<<<<<<<<<<<
  *         s = 0
  *     return result_array
  */
     try {
       __pyx_v_result_array.push_back(__pyx_v_s);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 61, __pyx_L1_error)
+      __PYX_ERR(0, 62, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":62
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":63
  *                 s += 1
  *         result_array.push_back(s)
  *         s = 0             # <<<<<<<<<<<<<<
  *     return result_array
  * 
  */
     __pyx_v_s = 0;
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":63
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":64
  *         result_array.push_back(s)
  *         s = 0
  *     return result_array             # <<<<<<<<<<<<<<
  * 
- * from libcpp.string cimport string
+ * from libcpp.map cimport map as c_map
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_10 = __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(__pyx_v_result_array); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_10 = __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(__pyx_v_result_array); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_r = __pyx_t_10;
   __pyx_t_10 = 0;
   goto __pyx_L0;
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":45
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":46
  * ctypedef long long LL   # unsigned
  * ctypedef vector[LL] vec
  * cpdef k_mer_offset_analysis_2(             # <<<<<<<<<<<<<<
  *         LL[:] ref_seq_v_repeated,
  *         LL[:] query_seq_v,
  */
 
@@ -18060,67 +19476,67 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ref_seq_v_repeated)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_query_seq_v)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("k_mer_offset_analysis_2", 1, 4, 4, 1); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("k_mer_offset_analysis_2", 1, 4, 4, 1); __PYX_ERR(0, 46, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_N_ref)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("k_mer_offset_analysis_2", 1, 4, 4, 2); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("k_mer_offset_analysis_2", 1, 4, 4, 2); __PYX_ERR(0, 46, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_len_query_seq_v)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("k_mer_offset_analysis_2", 1, 4, 4, 3); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("k_mer_offset_analysis_2", 1, 4, 4, 3); __PYX_ERR(0, 46, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "k_mer_offset_analysis_2") < 0)) __PYX_ERR(0, 45, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "k_mer_offset_analysis_2") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_ref_seq_v_repeated = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_ref_seq_v_repeated.memview)) __PYX_ERR(0, 46, __pyx_L3_error)
-    __pyx_v_query_seq_v = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_query_seq_v.memview)) __PYX_ERR(0, 47, __pyx_L3_error)
-    __pyx_v_N_ref = __Pyx_PyInt_As_PY_LONG_LONG(values[2]); if (unlikely((__pyx_v_N_ref == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 48, __pyx_L3_error)
-    __pyx_v_len_query_seq_v = __Pyx_PyInt_As_PY_LONG_LONG(values[3]); if (unlikely((__pyx_v_len_query_seq_v == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_ref_seq_v_repeated = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_ref_seq_v_repeated.memview)) __PYX_ERR(0, 47, __pyx_L3_error)
+    __pyx_v_query_seq_v = __Pyx_PyObject_to_MemoryviewSlice_ds_nn___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_query_seq_v.memview)) __PYX_ERR(0, 48, __pyx_L3_error)
+    __pyx_v_N_ref = __Pyx_PyInt_As_PY_LONG_LONG(values[2]); if (unlikely((__pyx_v_N_ref == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
+    __pyx_v_len_query_seq_v = __Pyx_PyInt_As_PY_LONG_LONG(values[3]); if (unlikely((__pyx_v_len_query_seq_v == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("k_mer_offset_analysis_2", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 45, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("k_mer_offset_analysis_2", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 46, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -18152,17 +19568,17 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("k_mer_offset_analysis_2", 1);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_ref_seq_v_repeated.memview)) { __Pyx_RaiseUnboundLocalError("ref_seq_v_repeated"); __PYX_ERR(0, 45, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_query_seq_v.memview)) { __Pyx_RaiseUnboundLocalError("query_seq_v"); __PYX_ERR(0, 45, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_f_9savemoney_7modules_16cython_functions_19alignment_functions_k_mer_offset_analysis_2(__pyx_v_ref_seq_v_repeated, __pyx_v_query_seq_v, __pyx_v_N_ref, __pyx_v_len_query_seq_v, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (unlikely(!__pyx_v_ref_seq_v_repeated.memview)) { __Pyx_RaiseUnboundLocalError("ref_seq_v_repeated"); __PYX_ERR(0, 46, __pyx_L1_error) }
+  if (unlikely(!__pyx_v_query_seq_v.memview)) { __Pyx_RaiseUnboundLocalError("query_seq_v"); __PYX_ERR(0, 46, __pyx_L1_error) }
+  __pyx_t_1 = __pyx_f_9savemoney_7modules_16cython_functions_19alignment_functions_k_mer_offset_analysis_2(__pyx_v_ref_seq_v_repeated, __pyx_v_query_seq_v, __pyx_v_N_ref, __pyx_v_len_query_seq_v, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -18171,17 +19587,896 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "savemoney/modules/cython_functions/alignment_functions.pyx":66
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":84
+ *     # additional
+ *     cdef string key
+ *     def __cinit__(self, str_LD_map P_base_calling_given_true_refseq_dict, str_LD_vec_map pdf_core, char_vec bases):             # <<<<<<<<<<<<<<
+ *         self.P_base_calling_given_true_refseq_dict = P_base_calling_given_true_refseq_dict
+ *         self.pdf_core = pdf_core
+ */
+
+/* Python wrapper */
+static int __pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_map __pyx_v_P_base_calling_given_true_refseq_dict;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_vec_map __pyx_v_pdf_core;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec __pyx_v_bases;
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[3] = {0,0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_P_base_calling_given_true_refseq,&__pyx_n_s_pdf_core,&__pyx_n_s_bases,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_P_base_calling_given_true_refseq)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pdf_core)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 1); __PYX_ERR(0, 84, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_bases)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[2]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, 2); __PYX_ERR(0, 84, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 84, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 3)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
+      values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
+      values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
+    }
+    __pyx_v_P_base_calling_given_true_refseq_dict = __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+    __pyx_v_pdf_core = __pyx_convert_map_from_py_std_3a__3a_string__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+    __pyx_v_bases = __pyx_convert_vector_from_py_char(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 84, __pyx_L3_error)
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 84, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("savemoney.modules.cython_functions.alignment_functions.SequenceBasecallQscorePDF.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return -1;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF___cinit__(((struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *)__pyx_v_self), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_P_base_calling_given_true_refseq_dict), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_pdf_core), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_bases));
+
+  /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static int __pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF___cinit__(struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *__pyx_v_self, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_map __pyx_v_P_base_calling_given_true_refseq_dict, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_vec_map __pyx_v_pdf_core, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec __pyx_v_bases) {
+  int __pyx_r;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":85
+ *     cdef string key
+ *     def __cinit__(self, str_LD_map P_base_calling_given_true_refseq_dict, str_LD_vec_map pdf_core, char_vec bases):
+ *         self.P_base_calling_given_true_refseq_dict = P_base_calling_given_true_refseq_dict             # <<<<<<<<<<<<<<
+ *         self.pdf_core = pdf_core
+ *         self.key.resize(3)
+ */
+  __pyx_v_self->P_base_calling_given_true_refseq_dict = __pyx_v_P_base_calling_given_true_refseq_dict;
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":86
+ *     def __cinit__(self, str_LD_map P_base_calling_given_true_refseq_dict, str_LD_vec_map pdf_core, char_vec bases):
+ *         self.P_base_calling_given_true_refseq_dict = P_base_calling_given_true_refseq_dict
+ *         self.pdf_core = pdf_core             # <<<<<<<<<<<<<<
+ *         self.key.resize(3)
+ *         self.key[1] = b"_"
+ */
+  __pyx_v_self->pdf_core = __pyx_v_pdf_core;
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":87
+ *         self.P_base_calling_given_true_refseq_dict = P_base_calling_given_true_refseq_dict
+ *         self.pdf_core = pdf_core
+ *         self.key.resize(3)             # <<<<<<<<<<<<<<
+ *         self.key[1] = b"_"
+ *         self.bases = bases
+ */
+  try {
+    __pyx_v_self->key.resize(3);
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(0, 87, __pyx_L1_error)
+  }
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":88
+ *         self.pdf_core = pdf_core
+ *         self.key.resize(3)
+ *         self.key[1] = b"_"             # <<<<<<<<<<<<<<
+ *         self.bases = bases
+ *         self.N_bases = self.bases.size()
+ */
+  (__pyx_v_self->key[1]) = '_';
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":89
+ *         self.key.resize(3)
+ *         self.key[1] = b"_"
+ *         self.bases = bases             # <<<<<<<<<<<<<<
+ *         self.N_bases = self.bases.size()
+ * 
+ */
+  __pyx_v_self->bases = __pyx_v_bases;
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":90
+ *         self.key[1] = b"_"
+ *         self.bases = bases
+ *         self.N_bases = self.bases.size()             # <<<<<<<<<<<<<<
+ * 
+ *     def calc_consensus_error_rate(self, char_vec query_list, vec q_score_list, chr_LD_map P_N_dict):
+ */
+  __pyx_v_self->N_bases = __pyx_v_self->bases.size();
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":84
+ *     # additional
+ *     cdef string key
+ *     def __cinit__(self, str_LD_map P_base_calling_given_true_refseq_dict, str_LD_vec_map pdf_core, char_vec bases):             # <<<<<<<<<<<<<<
+ *         self.P_base_calling_given_true_refseq_dict = P_base_calling_given_true_refseq_dict
+ *         self.pdf_core = pdf_core
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("savemoney.modules.cython_functions.alignment_functions.SequenceBasecallQscorePDF.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":92
+ *         self.N_bases = self.bases.size()
+ * 
+ *     def calc_consensus_error_rate(self, char_vec query_list, vec q_score_list, chr_LD_map P_N_dict):             # <<<<<<<<<<<<<<
+ *         cdef LL N_query_list
+ *         cdef LL base_idx
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_3calc_consensus_error_rate(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_2calc_consensus_error_rate, "SequenceBasecallQscorePDF.calc_consensus_error_rate(self, char_vec query_list, vec q_score_list, chr_LD_map P_N_dict)");
+static PyMethodDef __pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_3calc_consensus_error_rate = {"calc_consensus_error_rate", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_3calc_consensus_error_rate, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_2calc_consensus_error_rate};
+static PyObject *__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_3calc_consensus_error_rate(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec __pyx_v_query_list;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec __pyx_v_q_score_list;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_chr_LD_map __pyx_v_P_N_dict;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[3] = {0,0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("calc_consensus_error_rate (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_query_list,&__pyx_n_s_q_score_list,&__pyx_n_s_P_N_dict,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_query_list)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 92, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_q_score_list)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 92, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("calc_consensus_error_rate", 1, 3, 3, 1); __PYX_ERR(0, 92, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_P_N_dict)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 92, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("calc_consensus_error_rate", 1, 3, 3, 2); __PYX_ERR(0, 92, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "calc_consensus_error_rate") < 0)) __PYX_ERR(0, 92, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 3)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+    }
+    __pyx_v_query_list = __pyx_convert_vector_from_py_char(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 92, __pyx_L3_error)
+    __pyx_v_q_score_list = __pyx_convert_vector_from_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 92, __pyx_L3_error)
+    __pyx_v_P_N_dict = __pyx_convert_map_from_py_char__and___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 92, __pyx_L3_error)
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("calc_consensus_error_rate", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 92, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("savemoney.modules.cython_functions.alignment_functions.SequenceBasecallQscorePDF.calc_consensus_error_rate", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_2calc_consensus_error_rate(((struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *)__pyx_v_self), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_query_list), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_q_score_list), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_P_N_dict));
+
+  /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_2calc_consensus_error_rate(struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *__pyx_v_self, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec __pyx_v_query_list, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec __pyx_v_q_score_list, __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_chr_LD_map __pyx_v_P_N_dict) {
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_N_query_list;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_base_idx;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_v_idx;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec __pyx_v_bunshi_list;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD __pyx_v_bunshi_P_N;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD __pyx_v_bunbo_bunshi_sum;
+  char __pyx_v_base;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD __pyx_v_val;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD_vec __pyx_v_p_list;
+  char __pyx_v_B;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_t_1;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_t_2;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_t_3;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_t_4;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_t_5;
+  __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LL __pyx_t_6;
+  int __pyx_t_7;
+  std::vector<char> ::iterator __pyx_t_8;
+  char __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("calc_consensus_error_rate", 1);
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":103
+ *         cdef LD_vec p_list
+ * 
+ *         N_query_list = query_list.size()             # <<<<<<<<<<<<<<
+ * 
+ *         for base_idx in range(self.N_bases):
+ */
+  __pyx_v_N_query_list = __pyx_v_query_list.size();
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":105
+ *         N_query_list = query_list.size()
+ * 
+ *         for base_idx in range(self.N_bases):             # <<<<<<<<<<<<<<
+ *             #
+ *             B = self.bases[base_idx]
+ */
+  __pyx_t_1 = __pyx_v_self->N_bases;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_base_idx = __pyx_t_3;
+
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":107
+ *         for base_idx in range(self.N_bases):
+ *             #
+ *             B = self.bases[base_idx]             # <<<<<<<<<<<<<<
+ *             self.key[0] = B
+ *             bunshi_list.clear()
+ */
+    __pyx_v_B = (__pyx_v_self->bases[__pyx_v_base_idx]);
+
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":108
+ *             #
+ *             B = self.bases[base_idx]
+ *             self.key[0] = B             # <<<<<<<<<<<<<<
+ *             bunshi_list.clear()
+ * 
+ */
+    (__pyx_v_self->key[0]) = __pyx_v_B;
+
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":109
+ *             B = self.bases[base_idx]
+ *             self.key[0] = B
+ *             bunshi_list.clear()             # <<<<<<<<<<<<<<
+ * 
+ *             for idx in range(N_query_list):
+ */
+    __pyx_v_bunshi_list.clear();
+
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":111
+ *             bunshi_list.clear()
+ * 
+ *             for idx in range(N_query_list):             # <<<<<<<<<<<<<<
+ *                 self.key[2] = query_list[idx]
+ *                 if q_score_list[idx] >= 0:
+ */
+    __pyx_t_4 = __pyx_v_N_query_list;
+    __pyx_t_5 = __pyx_t_4;
+    for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
+      __pyx_v_idx = __pyx_t_6;
+
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":112
+ * 
+ *             for idx in range(N_query_list):
+ *                 self.key[2] = query_list[idx]             # <<<<<<<<<<<<<<
+ *                 if q_score_list[idx] >= 0:
+ *                     bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]])
+ */
+      (__pyx_v_self->key[2]) = (__pyx_v_query_list[__pyx_v_idx]);
+
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":113
+ *             for idx in range(N_query_list):
+ *                 self.key[2] = query_list[idx]
+ *                 if q_score_list[idx] >= 0:             # <<<<<<<<<<<<<<
+ *                     bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]])
+ *                 else:
+ */
+      __pyx_t_7 = ((__pyx_v_q_score_list[__pyx_v_idx]) >= 0);
+      if (__pyx_t_7) {
+
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":114
+ *                 self.key[2] = query_list[idx]
+ *                 if q_score_list[idx] >= 0:
+ *                     bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]])             # <<<<<<<<<<<<<<
+ *                 else:
+ *                     bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key])
+ */
+        try {
+          __pyx_v_bunshi_list.push_back(((__pyx_v_self->P_base_calling_given_true_refseq_dict[__pyx_v_self->key]) * ((__pyx_v_self->pdf_core[__pyx_v_self->key])[(__pyx_v_q_score_list[__pyx_v_idx])])));
+        } catch(...) {
+          __Pyx_CppExn2PyErr();
+          __PYX_ERR(0, 114, __pyx_L1_error)
+        }
+
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":113
+ *             for idx in range(N_query_list):
+ *                 self.key[2] = query_list[idx]
+ *                 if q_score_list[idx] >= 0:             # <<<<<<<<<<<<<<
+ *                     bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]])
+ *                 else:
+ */
+        goto __pyx_L7;
+      }
+
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":116
+ *                     bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]])
+ *                 else:
+ *                     bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key])             # <<<<<<<<<<<<<<
+ *             bunshi_P_N = P_N_dict[B]
+ * 
+ */
+      /*else*/ {
+        try {
+          __pyx_v_bunshi_list.push_back((__pyx_v_self->P_base_calling_given_true_refseq_dict[__pyx_v_self->key]));
+        } catch(...) {
+          __Pyx_CppExn2PyErr();
+          __PYX_ERR(0, 116, __pyx_L1_error)
+        }
+      }
+      __pyx_L7:;
+    }
+
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":117
+ *                 else:
+ *                     bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key])
+ *             bunshi_P_N = P_N_dict[B]             # <<<<<<<<<<<<<<
+ * 
+ *             # inside sum
+ */
+    __pyx_v_bunshi_P_N = (__pyx_v_P_N_dict[__pyx_v_B]);
+
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":120
+ * 
+ *             # inside sum
+ *             bunbo_bunshi_sum = 0             # <<<<<<<<<<<<<<
+ *             for base in self.bases:
+ *                 self.key[0] = base
+ */
+    __pyx_v_bunbo_bunshi_sum = 0.0;
+
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":121
+ *             # inside sum
+ *             bunbo_bunshi_sum = 0
+ *             for base in self.bases:             # <<<<<<<<<<<<<<
+ *                 self.key[0] = base
+ *                 val = P_N_dict[base] / bunshi_P_N
+ */
+    __pyx_t_8 = __pyx_v_self->bases.begin();
+    for (;;) {
+      if (!(__pyx_t_8 != __pyx_v_self->bases.end())) break;
+      __pyx_t_9 = *__pyx_t_8;
+      ++__pyx_t_8;
+      __pyx_v_base = __pyx_t_9;
+
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":122
+ *             bunbo_bunshi_sum = 0
+ *             for base in self.bases:
+ *                 self.key[0] = base             # <<<<<<<<<<<<<<
+ *                 val = P_N_dict[base] / bunshi_P_N
+ *                 for idx in range(N_query_list):
+ */
+      (__pyx_v_self->key[0]) = __pyx_v_base;
+
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":123
+ *             for base in self.bases:
+ *                 self.key[0] = base
+ *                 val = P_N_dict[base] / bunshi_P_N             # <<<<<<<<<<<<<<
+ *                 for idx in range(N_query_list):
+ *                     self.key[2] = query_list[idx]
+ */
+      __pyx_v_val = (((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)(__pyx_v_P_N_dict[__pyx_v_base])) / __pyx_v_bunshi_P_N);
+
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":124
+ *                 self.key[0] = base
+ *                 val = P_N_dict[base] / bunshi_P_N
+ *                 for idx in range(N_query_list):             # <<<<<<<<<<<<<<
+ *                     self.key[2] = query_list[idx]
+ *                     if q_score_list[idx] >= 0:
+ */
+      __pyx_t_4 = __pyx_v_N_query_list;
+      __pyx_t_5 = __pyx_t_4;
+      for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
+        __pyx_v_idx = __pyx_t_6;
+
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":125
+ *                 val = P_N_dict[base] / bunshi_P_N
+ *                 for idx in range(N_query_list):
+ *                     self.key[2] = query_list[idx]             # <<<<<<<<<<<<<<
+ *                     if q_score_list[idx] >= 0:
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]]) / bunshi_list[idx]
+ */
+        (__pyx_v_self->key[2]) = (__pyx_v_query_list[__pyx_v_idx]);
+
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":126
+ *                 for idx in range(N_query_list):
+ *                     self.key[2] = query_list[idx]
+ *                     if q_score_list[idx] >= 0:             # <<<<<<<<<<<<<<
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]]) / bunshi_list[idx]
+ *                     else:
+ */
+        __pyx_t_7 = ((__pyx_v_q_score_list[__pyx_v_idx]) >= 0);
+        if (__pyx_t_7) {
+
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":127
+ *                     self.key[2] = query_list[idx]
+ *                     if q_score_list[idx] >= 0:
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]]) / bunshi_list[idx]             # <<<<<<<<<<<<<<
+ *                     else:
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key]) / bunshi_list[idx]
+ */
+          __pyx_v_val = (__pyx_v_val * (((__pyx_v_self->P_base_calling_given_true_refseq_dict[__pyx_v_self->key]) * ((__pyx_v_self->pdf_core[__pyx_v_self->key])[(__pyx_v_q_score_list[__pyx_v_idx])])) / ((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)(__pyx_v_bunshi_list[__pyx_v_idx]))));
+
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":126
+ *                 for idx in range(N_query_list):
+ *                     self.key[2] = query_list[idx]
+ *                     if q_score_list[idx] >= 0:             # <<<<<<<<<<<<<<
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]]) / bunshi_list[idx]
+ *                     else:
+ */
+          goto __pyx_L12;
+        }
+
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":129
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]]) / bunshi_list[idx]
+ *                     else:
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key]) / bunshi_list[idx]             # <<<<<<<<<<<<<<
+ *                 bunbo_bunshi_sum += val
+ *             p_list.push_back(1 - 1 / bunbo_bunshi_sum)
+ */
+        /*else*/ {
+          __pyx_v_val = (__pyx_v_val * (((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)(__pyx_v_self->P_base_calling_given_true_refseq_dict[__pyx_v_self->key])) / ((__pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD)(__pyx_v_bunshi_list[__pyx_v_idx]))));
+        }
+        __pyx_L12:;
+      }
+
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":130
+ *                     else:
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key]) / bunshi_list[idx]
+ *                 bunbo_bunshi_sum += val             # <<<<<<<<<<<<<<
+ *             p_list.push_back(1 - 1 / bunbo_bunshi_sum)
+ *         return p_list
+ */
+      __pyx_v_bunbo_bunshi_sum = (__pyx_v_bunbo_bunshi_sum + __pyx_v_val);
+
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":121
+ *             # inside sum
+ *             bunbo_bunshi_sum = 0
+ *             for base in self.bases:             # <<<<<<<<<<<<<<
+ *                 self.key[0] = base
+ *                 val = P_N_dict[base] / bunshi_P_N
+ */
+    }
+
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":131
+ *                         val *= (self.P_base_calling_given_true_refseq_dict[self.key]) / bunshi_list[idx]
+ *                 bunbo_bunshi_sum += val
+ *             p_list.push_back(1 - 1 / bunbo_bunshi_sum)             # <<<<<<<<<<<<<<
+ *         return p_list
+ * 
+ */
+    try {
+      __pyx_v_p_list.push_back((1.0 - (1.0 / __pyx_v_bunbo_bunshi_sum)));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(0, 131, __pyx_L1_error)
+    }
+  }
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":132
+ *                 bunbo_bunshi_sum += val
+ *             p_list.push_back(1 - 1 / bunbo_bunshi_sum)
+ *         return p_list             # <<<<<<<<<<<<<<
+ * 
+ * cpdef my_special_dp_cython(
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_10 = __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_LD(__pyx_v_p_list); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+  __pyx_r = __pyx_t_10;
+  __pyx_t_10 = 0;
+  goto __pyx_L0;
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":92
+ *         self.N_bases = self.bases.size()
+ * 
+ *     def calc_consensus_error_rate(self, char_vec query_list, vec q_score_list, chr_LD_map P_N_dict):             # <<<<<<<<<<<<<<
+ *         cdef LL N_query_list
+ *         cdef LL base_idx
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_AddTraceback("savemoney.modules.cython_functions.alignment_functions.SequenceBasecallQscorePDF.calc_consensus_error_rate", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_5__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_4__reduce_cython__, "SequenceBasecallQscorePDF.__reduce_cython__(self)");
+static PyMethodDef __pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_5__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_4__reduce_cython__};
+static PyObject *__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_5__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
+  __pyx_r = __pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_4__reduce_cython__(((struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_4__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
+
+  /* "(tree fragment)":2
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
+  __PYX_ERR(1, 2, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("savemoney.modules.cython_functions.alignment_functions.SequenceBasecallQscorePDF.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_7__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_6__setstate_cython__, "SequenceBasecallQscorePDF.__setstate_cython__(self, __pyx_state)");
+static PyMethodDef __pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_7__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_6__setstate_cython__};
+static PyObject *__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_7__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v___pyx_state = values[0];
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_AddTraceback("savemoney.modules.cython_functions.alignment_functions.SequenceBasecallQscorePDF.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_6__setstate_cython__(((struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *)__pyx_v_self), __pyx_v___pyx_state);
+
+  /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_6__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
+
+  /* "(tree fragment)":4
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
+ */
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
+  __PYX_ERR(1, 4, __pyx_L1_error)
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("savemoney.modules.cython_functions.alignment_functions.SequenceBasecallQscorePDF.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "savemoney/modules/cython_functions/alignment_functions.pyx":134
+ *         return p_list
  * 
- * from libcpp.string cimport string
  * cpdef my_special_dp_cython(             # <<<<<<<<<<<<<<
  *         string query_seq_1,
  *         string query_seq_2,
  */
 
 static PyObject *__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_3my_special_dp_cython(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
@@ -18223,436 +20518,436 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("my_special_dp_cython", 1);
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":78
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":146
  *     cdef size_t N_query_seq_1
  *     cdef size_t N_query_seq_2
  *     N_ref_seq = ref_seq.size()             # <<<<<<<<<<<<<<
  *     N_query_seq_1 = query_seq_1.size()
  *     N_query_seq_2 = query_seq_2.size()
  */
   __pyx_v_N_ref_seq = __pyx_v_ref_seq.size();
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":79
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":147
  *     cdef size_t N_query_seq_2
  *     N_ref_seq = ref_seq.size()
  *     N_query_seq_1 = query_seq_1.size()             # <<<<<<<<<<<<<<
  *     N_query_seq_2 = query_seq_2.size()
  *     assert N_ref_seq > N_query_seq_1 + N_query_seq_2
  */
   __pyx_v_N_query_seq_1 = __pyx_v_query_seq_1.size();
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":80
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":148
  *     N_ref_seq = ref_seq.size()
  *     N_query_seq_1 = query_seq_1.size()
  *     N_query_seq_2 = query_seq_2.size()             # <<<<<<<<<<<<<<
  *     assert N_ref_seq > N_query_seq_1 + N_query_seq_2
  * 
  */
   __pyx_v_N_query_seq_2 = __pyx_v_query_seq_2.size();
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":81
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":149
  *     N_query_seq_1 = query_seq_1.size()
  *     N_query_seq_2 = query_seq_2.size()
  *     assert N_ref_seq > N_query_seq_1 + N_query_seq_2             # <<<<<<<<<<<<<<
  * 
  *     ################
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_1 = (__pyx_v_N_ref_seq > (__pyx_v_N_query_seq_1 + __pyx_v_N_query_seq_2));
     if (unlikely(!__pyx_t_1)) {
       __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-      __PYX_ERR(0, 81, __pyx_L1_error)
+      __PYX_ERR(0, 149, __pyx_L1_error)
     }
   }
   #else
-  if ((1)); else __PYX_ERR(0, 81, __pyx_L1_error)
+  if ((1)); else __PYX_ERR(0, 149, __pyx_L1_error)
   #endif
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":120
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":188
  *     cdef LL deletion_score
  *     cdef LL modifier
  *     dp_row.reserve(N_ref_seq + 1)             # <<<<<<<<<<<<<<
  *     dp_row.push_back(0)
  *     dp.reserve(N_query_seq_1 + N_query_seq_2 + 1)
  */
   try {
     __pyx_v_dp_row.reserve((__pyx_v_N_ref_seq + 1));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 120, __pyx_L1_error)
+    __PYX_ERR(0, 188, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":121
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":189
  *     cdef LL modifier
  *     dp_row.reserve(N_ref_seq + 1)
  *     dp_row.push_back(0)             # <<<<<<<<<<<<<<
  *     dp.reserve(N_query_seq_1 + N_query_seq_2 + 1)
  *     trace_row.reserve(N_ref_seq + 1)
  */
   try {
     __pyx_v_dp_row.push_back(0);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 121, __pyx_L1_error)
+    __PYX_ERR(0, 189, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":122
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":190
  *     dp_row.reserve(N_ref_seq + 1)
  *     dp_row.push_back(0)
  *     dp.reserve(N_query_seq_1 + N_query_seq_2 + 1)             # <<<<<<<<<<<<<<
  *     trace_row.reserve(N_ref_seq + 1)
  *     trace_row.push_back(42)     # origin
  */
   try {
     __pyx_v_dp.reserve(((__pyx_v_N_query_seq_1 + __pyx_v_N_query_seq_2) + 1));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 122, __pyx_L1_error)
+    __PYX_ERR(0, 190, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":123
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":191
  *     dp_row.push_back(0)
  *     dp.reserve(N_query_seq_1 + N_query_seq_2 + 1)
  *     trace_row.reserve(N_ref_seq + 1)             # <<<<<<<<<<<<<<
  *     trace_row.push_back(42)     # origin
  *     trace.reserve(N_query_seq_1 + N_query_seq_2 + 1)
  */
   try {
     __pyx_v_trace_row.reserve((__pyx_v_N_ref_seq + 1));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 123, __pyx_L1_error)
+    __PYX_ERR(0, 191, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":124
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":192
  *     dp.reserve(N_query_seq_1 + N_query_seq_2 + 1)
  *     trace_row.reserve(N_ref_seq + 1)
  *     trace_row.push_back(42)     # origin             # <<<<<<<<<<<<<<
  *     trace.reserve(N_query_seq_1 + N_query_seq_2 + 1)
  *     #####################
  */
   try {
     __pyx_v_trace_row.push_back(42);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 124, __pyx_L1_error)
+    __PYX_ERR(0, 192, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":125
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":193
  *     trace_row.reserve(N_ref_seq + 1)
  *     trace_row.push_back(42)     # origin
  *     trace.reserve(N_query_seq_1 + N_query_seq_2 + 1)             # <<<<<<<<<<<<<<
  *     #####################
  *     # DP of query_seq_1 #
  */
   try {
     __pyx_v_trace.reserve(((__pyx_v_N_query_seq_1 + __pyx_v_N_query_seq_2) + 1));
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 125, __pyx_L1_error)
+    __PYX_ERR(0, 193, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":129
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":197
  *     # DP of query_seq_1 #
  *     #####################
  *     if N_query_seq_1 > 0:             # <<<<<<<<<<<<<<
  *         ###############
  *         # query_seq_1 #
  */
   __pyx_t_1 = (__pyx_v_N_query_seq_1 > 0);
   if (__pyx_t_1) {
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":134
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":202
  *         ###############
  *         #
  *         dp_row.push_back(-gap_open_penalty)             # <<<<<<<<<<<<<<
  *         trace_row.push_back(68)
  *         for j in range(1, N_ref_seq):
  */
     try {
       __pyx_v_dp_row.push_back((-__pyx_v_gap_open_penalty));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 134, __pyx_L1_error)
+      __PYX_ERR(0, 202, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":135
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":203
  *         #
  *         dp_row.push_back(-gap_open_penalty)
  *         trace_row.push_back(68)             # <<<<<<<<<<<<<<
  *         for j in range(1, N_ref_seq):
  *             dp_row.push_back(dp_row[j] - gap_extend_penalty)
  */
     try {
       __pyx_v_trace_row.push_back(68);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 135, __pyx_L1_error)
+      __PYX_ERR(0, 203, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":136
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":204
  *         dp_row.push_back(-gap_open_penalty)
  *         trace_row.push_back(68)
  *         for j in range(1, N_ref_seq):             # <<<<<<<<<<<<<<
  *             dp_row.push_back(dp_row[j] - gap_extend_penalty)
  *             trace_row.push_back(68) #  deletion
  */
     __pyx_t_2 = __pyx_v_N_ref_seq;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 1; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_j = __pyx_t_4;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":137
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":205
  *         trace_row.push_back(68)
  *         for j in range(1, N_ref_seq):
  *             dp_row.push_back(dp_row[j] - gap_extend_penalty)             # <<<<<<<<<<<<<<
  *             trace_row.push_back(68) #  deletion
  *         dp.push_back(dp_row)
  */
       try {
         __pyx_v_dp_row.push_back(((__pyx_v_dp_row[__pyx_v_j]) - __pyx_v_gap_extend_penalty));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 137, __pyx_L1_error)
+        __PYX_ERR(0, 205, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":138
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":206
  *         for j in range(1, N_ref_seq):
  *             dp_row.push_back(dp_row[j] - gap_extend_penalty)
  *             trace_row.push_back(68) #  deletion             # <<<<<<<<<<<<<<
  *         dp.push_back(dp_row)
  *         trace.push_back(trace_row)
  */
       try {
         __pyx_v_trace_row.push_back(68);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 138, __pyx_L1_error)
+        __PYX_ERR(0, 206, __pyx_L1_error)
       }
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":139
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":207
  *             dp_row.push_back(dp_row[j] - gap_extend_penalty)
  *             trace_row.push_back(68) #  deletion
  *         dp.push_back(dp_row)             # <<<<<<<<<<<<<<
  *         trace.push_back(trace_row)
  *         #
  */
     try {
       __pyx_v_dp.push_back(__pyx_v_dp_row);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 139, __pyx_L1_error)
+      __PYX_ERR(0, 207, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":140
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":208
  *             trace_row.push_back(68) #  deletion
  *         dp.push_back(dp_row)
  *         trace.push_back(trace_row)             # <<<<<<<<<<<<<<
  *         #
  *         for i in range(N_query_seq_1 - 1):
  */
     try {
       __pyx_v_trace.push_back(__pyx_v_trace_row);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 140, __pyx_L1_error)
+      __PYX_ERR(0, 208, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":142
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":210
  *         trace.push_back(trace_row)
  *         #
  *         for i in range(N_query_seq_1 - 1):             # <<<<<<<<<<<<<<
  *             q = query_seq_1[i]
  *             #
  */
     __pyx_t_2 = (__pyx_v_N_query_seq_1 - 1);
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":143
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":211
  *         #
  *         for i in range(N_query_seq_1 - 1):
  *             q = query_seq_1[i]             # <<<<<<<<<<<<<<
  *             #
  *             dp_row.clear()
  */
       __pyx_v_q = (__pyx_v_query_seq_1[__pyx_v_i]);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":145
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":213
  *             q = query_seq_1[i]
  *             #
  *             dp_row.clear()             # <<<<<<<<<<<<<<
  *             if i == 0:
  *                 dp_row.push_back(dp[i][0] - gap_open_penalty)
  */
       __pyx_v_dp_row.clear();
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":146
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":214
  *             #
  *             dp_row.clear()
  *             if i == 0:             # <<<<<<<<<<<<<<
  *                 dp_row.push_back(dp[i][0] - gap_open_penalty)
  *             else:
  */
       __pyx_t_1 = (__pyx_v_i == 0);
       if (__pyx_t_1) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":147
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":215
  *             dp_row.clear()
  *             if i == 0:
  *                 dp_row.push_back(dp[i][0] - gap_open_penalty)             # <<<<<<<<<<<<<<
  *             else:
  *                 dp_row.push_back(dp[i][0] - gap_extend_penalty)
  */
         try {
           __pyx_v_dp_row.push_back((((__pyx_v_dp[__pyx_v_i])[0]) - __pyx_v_gap_open_penalty));
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 147, __pyx_L1_error)
+          __PYX_ERR(0, 215, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":146
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":214
  *             #
  *             dp_row.clear()
  *             if i == 0:             # <<<<<<<<<<<<<<
  *                 dp_row.push_back(dp[i][0] - gap_open_penalty)
  *             else:
  */
         goto __pyx_L8;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":149
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":217
  *                 dp_row.push_back(dp[i][0] - gap_open_penalty)
  *             else:
  *                 dp_row.push_back(dp[i][0] - gap_extend_penalty)             # <<<<<<<<<<<<<<
  *             trace_row.clear()
  *             trace_row.push_back(73)     #  insertion
  */
       /*else*/ {
         try {
           __pyx_v_dp_row.push_back((((__pyx_v_dp[__pyx_v_i])[0]) - __pyx_v_gap_extend_penalty));
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 149, __pyx_L1_error)
+          __PYX_ERR(0, 217, __pyx_L1_error)
         }
       }
       __pyx_L8:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":150
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":218
  *             else:
  *                 dp_row.push_back(dp[i][0] - gap_extend_penalty)
  *             trace_row.clear()             # <<<<<<<<<<<<<<
  *             trace_row.push_back(73)     #  insertion
  *             #
  */
       __pyx_v_trace_row.clear();
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":151
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":219
  *                 dp_row.push_back(dp[i][0] - gap_extend_penalty)
  *             trace_row.clear()
  *             trace_row.push_back(73)     #  insertion             # <<<<<<<<<<<<<<
  *             #
  *             for j in range(N_ref_seq):
  */
       try {
         __pyx_v_trace_row.push_back(73);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 151, __pyx_L1_error)
+        __PYX_ERR(0, 219, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":153
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":221
  *             trace_row.push_back(73)     #  insertion
  *             #
  *             for j in range(N_ref_seq):             # <<<<<<<<<<<<<<
  *                 r = ref_seq[j]
  *                 # aligned_score
  */
       __pyx_t_5 = __pyx_v_N_ref_seq;
       __pyx_t_6 = __pyx_t_5;
       for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
         __pyx_v_j = __pyx_t_7;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":154
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":222
  *             #
  *             for j in range(N_ref_seq):
  *                 r = ref_seq[j]             # <<<<<<<<<<<<<<
  *                 # aligned_score
  *                 if q == r:
  */
         __pyx_v_r = (__pyx_v_ref_seq[__pyx_v_j]);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":156
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":224
  *                 r = ref_seq[j]
  *                 # aligned_score
  *                 if q == r:             # <<<<<<<<<<<<<<
  *                     aligned_score = dp[i][j] + match_score
  *                     modifier = 0
  */
         __pyx_t_1 = (__pyx_v_q == __pyx_v_r);
         if (__pyx_t_1) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":157
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":225
  *                 # aligned_score
  *                 if q == r:
  *                     aligned_score = dp[i][j] + match_score             # <<<<<<<<<<<<<<
  *                     modifier = 0
  *                 else:
  */
           __pyx_v_aligned_score = (((__pyx_v_dp[__pyx_v_i])[__pyx_v_j]) + __pyx_v_match_score);
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":158
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":226
  *                 if q == r:
  *                     aligned_score = dp[i][j] + match_score
  *                     modifier = 0             # <<<<<<<<<<<<<<
  *                 else:
  *                     aligned_score = dp[i][j] + mismatch_score
  */
           __pyx_v_modifier = 0;
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":156
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":224
  *                 r = ref_seq[j]
  *                 # aligned_score
  *                 if q == r:             # <<<<<<<<<<<<<<
  *                     aligned_score = dp[i][j] + match_score
  *                     modifier = 0
  */
           goto __pyx_L11;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":160
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":228
  *                     modifier = 0
  *                 else:
  *                     aligned_score = dp[i][j] + mismatch_score             # <<<<<<<<<<<<<<
  *                     modifier = 27
  *                 # insertion_score   #  insertion
  */
         /*else*/ {
           __pyx_v_aligned_score = (((__pyx_v_dp[__pyx_v_i])[__pyx_v_j]) + __pyx_v_mismatch_score);
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":161
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":229
  *                 else:
  *                     aligned_score = dp[i][j] + mismatch_score
  *                     modifier = 27             # <<<<<<<<<<<<<<
  *                 # insertion_score   #  insertion
  *                 if trace[i][j+1] in (73, 141, 134, 202, 161, 229):
  */
           __pyx_v_modifier = 27;
         }
         __pyx_L11:;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":163
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":231
  *                     modifier = 27
  *                 # insertion_score   #  insertion
  *                 if trace[i][j+1] in (73, 141, 134, 202, 161, 229):             # <<<<<<<<<<<<<<
  *                     insertion_score = dp[i][j+1] - gap_extend_penalty
  *                 else:
  */
         __pyx_t_8 = ((__pyx_v_trace[__pyx_v_i])[(__pyx_v_j + 1)]);
@@ -18688,46 +20983,46 @@
         }
         __pyx_t_9 = (__pyx_t_8 == 0xE5);
         __pyx_t_1 = __pyx_t_9;
         __pyx_L13_bool_binop_done:;
         __pyx_t_9 = __pyx_t_1;
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":164
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":232
  *                 # insertion_score   #  insertion
  *                 if trace[i][j+1] in (73, 141, 134, 202, 161, 229):
  *                     insertion_score = dp[i][j+1] - gap_extend_penalty             # <<<<<<<<<<<<<<
  *                 else:
  *                     insertion_score = dp[i][j+1] - gap_open_penalty
  */
           __pyx_v_insertion_score = (((__pyx_v_dp[__pyx_v_i])[(__pyx_v_j + 1)]) - __pyx_v_gap_extend_penalty);
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":163
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":231
  *                     modifier = 27
  *                 # insertion_score   #  insertion
  *                 if trace[i][j+1] in (73, 141, 134, 202, 161, 229):             # <<<<<<<<<<<<<<
  *                     insertion_score = dp[i][j+1] - gap_extend_penalty
  *                 else:
  */
           goto __pyx_L12;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":166
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":234
  *                     insertion_score = dp[i][j+1] - gap_extend_penalty
  *                 else:
  *                     insertion_score = dp[i][j+1] - gap_open_penalty             # <<<<<<<<<<<<<<
  *                 # deletion_score   #  deletion
  *                 if trace_row[j] in (68, 141, 129, 202, 156, 229):
  */
         /*else*/ {
           __pyx_v_insertion_score = (((__pyx_v_dp[__pyx_v_i])[(__pyx_v_j + 1)]) - __pyx_v_gap_open_penalty);
         }
         __pyx_L12:;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":168
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":236
  *                     insertion_score = dp[i][j+1] - gap_open_penalty
  *                 # deletion_score   #  deletion
  *                 if trace_row[j] in (68, 141, 129, 202, 156, 229):             # <<<<<<<<<<<<<<
  *                     deletion_score = dp_row[j] - gap_extend_penalty
  *                 else:
  */
         __pyx_t_8 = (__pyx_v_trace_row[__pyx_v_j]);
@@ -18763,644 +21058,644 @@
         }
         __pyx_t_1 = (__pyx_t_8 == 0xE5);
         __pyx_t_9 = __pyx_t_1;
         __pyx_L20_bool_binop_done:;
         __pyx_t_1 = __pyx_t_9;
         if (__pyx_t_1) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":169
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":237
  *                 # deletion_score   #  deletion
  *                 if trace_row[j] in (68, 141, 129, 202, 156, 229):
  *                     deletion_score = dp_row[j] - gap_extend_penalty             # <<<<<<<<<<<<<<
  *                 else:
  *                     deletion_score = dp_row[j] - gap_open_penalty
  */
           __pyx_v_deletion_score = ((__pyx_v_dp_row[__pyx_v_j]) - __pyx_v_gap_extend_penalty);
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":168
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":236
  *                     insertion_score = dp[i][j+1] - gap_open_penalty
  *                 # deletion_score   #  deletion
  *                 if trace_row[j] in (68, 141, 129, 202, 156, 229):             # <<<<<<<<<<<<<<
  *                     deletion_score = dp_row[j] - gap_extend_penalty
  *                 else:
  */
           goto __pyx_L19;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":171
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":239
  *                     deletion_score = dp_row[j] - gap_extend_penalty
  *                 else:
  *                     deletion_score = dp_row[j] - gap_open_penalty             # <<<<<<<<<<<<<<
  *                 # set dp and trace
  *                 if aligned_score > deletion_score:
  */
         /*else*/ {
           __pyx_v_deletion_score = ((__pyx_v_dp_row[__pyx_v_j]) - __pyx_v_gap_open_penalty);
         }
         __pyx_L19:;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":173
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":241
  *                     deletion_score = dp_row[j] - gap_open_penalty
  *                 # set dp and trace
  *                 if aligned_score > deletion_score:             # <<<<<<<<<<<<<<
  *                     if aligned_score > insertion_score:     # = or X
  *                         dp_row.push_back(aligned_score)
  */
         __pyx_t_1 = (__pyx_v_aligned_score > __pyx_v_deletion_score);
         if (__pyx_t_1) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":174
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":242
  *                 # set dp and trace
  *                 if aligned_score > deletion_score:
  *                     if aligned_score > insertion_score:     # = or X             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(aligned_score)
  *                         trace_row.push_back(61 + modifier)
  */
           __pyx_t_1 = (__pyx_v_aligned_score > __pyx_v_insertion_score);
           if (__pyx_t_1) {
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":175
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":243
  *                 if aligned_score > deletion_score:
  *                     if aligned_score > insertion_score:     # = or X
  *                         dp_row.push_back(aligned_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(61 + modifier)
  *                     elif aligned_score < insertion_score:   # I
  */
             try {
               __pyx_v_dp_row.push_back(__pyx_v_aligned_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 175, __pyx_L1_error)
+              __PYX_ERR(0, 243, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":176
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":244
  *                     if aligned_score > insertion_score:     # = or X
  *                         dp_row.push_back(aligned_score)
  *                         trace_row.push_back(61 + modifier)             # <<<<<<<<<<<<<<
  *                     elif aligned_score < insertion_score:   # I
  *                         dp_row.push_back(insertion_score)
  */
             try {
               __pyx_v_trace_row.push_back((61 + __pyx_v_modifier));
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 176, __pyx_L1_error)
+              __PYX_ERR(0, 244, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":174
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":242
  *                 # set dp and trace
  *                 if aligned_score > deletion_score:
  *                     if aligned_score > insertion_score:     # = or X             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(aligned_score)
  *                         trace_row.push_back(61 + modifier)
  */
             goto __pyx_L27;
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":177
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":245
  *                         dp_row.push_back(aligned_score)
  *                         trace_row.push_back(61 + modifier)
  *                     elif aligned_score < insertion_score:   # I             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  */
           __pyx_t_1 = (__pyx_v_aligned_score < __pyx_v_insertion_score);
           if (__pyx_t_1) {
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":178
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":246
  *                         trace_row.push_back(61 + modifier)
  *                     elif aligned_score < insertion_score:   # I
  *                         dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(73)
  *                     else:                                   # I= or IX
  */
             try {
               __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 178, __pyx_L1_error)
+              __PYX_ERR(0, 246, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":179
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":247
  *                     elif aligned_score < insertion_score:   # I
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                     else:                                   # I= or IX
  *                         dp_row.push_back(insertion_score)
  */
             try {
               __pyx_v_trace_row.push_back(73);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 179, __pyx_L1_error)
+              __PYX_ERR(0, 247, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":177
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":245
  *                         dp_row.push_back(aligned_score)
  *                         trace_row.push_back(61 + modifier)
  *                     elif aligned_score < insertion_score:   # I             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  */
             goto __pyx_L27;
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":181
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":249
  *                         trace_row.push_back(73)
  *                     else:                                   # I= or IX
  *                         dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(134 + modifier)
  *                 elif aligned_score < deletion_score:
  */
           /*else*/ {
             try {
               __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 181, __pyx_L1_error)
+              __PYX_ERR(0, 249, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":182
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":250
  *                     else:                                   # I= or IX
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(134 + modifier)             # <<<<<<<<<<<<<<
  *                 elif aligned_score < deletion_score:
  *                     if insertion_score > deletion_score:    # I
  */
             try {
               __pyx_v_trace_row.push_back((0x86 + __pyx_v_modifier));
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 182, __pyx_L1_error)
+              __PYX_ERR(0, 250, __pyx_L1_error)
             }
           }
           __pyx_L27:;
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":173
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":241
  *                     deletion_score = dp_row[j] - gap_open_penalty
  *                 # set dp and trace
  *                 if aligned_score > deletion_score:             # <<<<<<<<<<<<<<
  *                     if aligned_score > insertion_score:     # = or X
  *                         dp_row.push_back(aligned_score)
  */
           goto __pyx_L26;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":183
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":251
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(134 + modifier)
  *                 elif aligned_score < deletion_score:             # <<<<<<<<<<<<<<
  *                     if insertion_score > deletion_score:    # I
  *                         dp_row.push_back(insertion_score)
  */
         __pyx_t_1 = (__pyx_v_aligned_score < __pyx_v_deletion_score);
         if (__pyx_t_1) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":184
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":252
  *                         trace_row.push_back(134 + modifier)
  *                 elif aligned_score < deletion_score:
  *                     if insertion_score > deletion_score:    # I             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  */
           __pyx_t_1 = (__pyx_v_insertion_score > __pyx_v_deletion_score);
           if (__pyx_t_1) {
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":185
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":253
  *                 elif aligned_score < deletion_score:
  *                     if insertion_score > deletion_score:    # I
  *                         dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(73)
  *                     elif insertion_score < deletion_score:  # D
  */
             try {
               __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 185, __pyx_L1_error)
+              __PYX_ERR(0, 253, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":186
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":254
  *                     if insertion_score > deletion_score:    # I
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                     elif insertion_score < deletion_score:  # D
  *                         dp_row.push_back(deletion_score)
  */
             try {
               __pyx_v_trace_row.push_back(73);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 186, __pyx_L1_error)
+              __PYX_ERR(0, 254, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":184
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":252
  *                         trace_row.push_back(134 + modifier)
  *                 elif aligned_score < deletion_score:
  *                     if insertion_score > deletion_score:    # I             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  */
             goto __pyx_L28;
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":187
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":255
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  *                     elif insertion_score < deletion_score:  # D             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(68)
  */
           __pyx_t_1 = (__pyx_v_insertion_score < __pyx_v_deletion_score);
           if (__pyx_t_1) {
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":188
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":256
  *                         trace_row.push_back(73)
  *                     elif insertion_score < deletion_score:  # D
  *                         dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(68)
  *                     else:                                   # ID
  */
             try {
               __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 188, __pyx_L1_error)
+              __PYX_ERR(0, 256, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":189
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":257
  *                     elif insertion_score < deletion_score:  # D
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(68)             # <<<<<<<<<<<<<<
  *                     else:                                   # ID
  *                         dp_row.push_back(deletion_score)
  */
             try {
               __pyx_v_trace_row.push_back(68);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 189, __pyx_L1_error)
+              __PYX_ERR(0, 257, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":187
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":255
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  *                     elif insertion_score < deletion_score:  # D             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(68)
  */
             goto __pyx_L28;
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":191
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":259
  *                         trace_row.push_back(68)
  *                     else:                                   # ID
  *                         dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(141)
  *                 else:
  */
           /*else*/ {
             try {
               __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 191, __pyx_L1_error)
+              __PYX_ERR(0, 259, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":192
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":260
  *                     else:                                   # ID
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(141)             # <<<<<<<<<<<<<<
  *                 else:
  *                     if aligned_score < insertion_score:     # I
  */
             try {
               __pyx_v_trace_row.push_back(0x8D);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 192, __pyx_L1_error)
+              __PYX_ERR(0, 260, __pyx_L1_error)
             }
           }
           __pyx_L28:;
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":183
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":251
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(134 + modifier)
  *                 elif aligned_score < deletion_score:             # <<<<<<<<<<<<<<
  *                     if insertion_score > deletion_score:    # I
  *                         dp_row.push_back(insertion_score)
  */
           goto __pyx_L26;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":194
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":262
  *                         trace_row.push_back(141)
  *                 else:
  *                     if aligned_score < insertion_score:     # I             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  */
         /*else*/ {
           __pyx_t_1 = (__pyx_v_aligned_score < __pyx_v_insertion_score);
           if (__pyx_t_1) {
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":195
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":263
  *                 else:
  *                     if aligned_score < insertion_score:     # I
  *                         dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(73)
  *                     elif aligned_score > insertion_score:   # D= or DX
  */
             try {
               __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 195, __pyx_L1_error)
+              __PYX_ERR(0, 263, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":196
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":264
  *                     if aligned_score < insertion_score:     # I
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                     elif aligned_score > insertion_score:   # D= or DX
  *                         dp_row.push_back(deletion_score)
  */
             try {
               __pyx_v_trace_row.push_back(73);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 196, __pyx_L1_error)
+              __PYX_ERR(0, 264, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":194
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":262
  *                         trace_row.push_back(141)
  *                 else:
  *                     if aligned_score < insertion_score:     # I             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  */
             goto __pyx_L29;
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":197
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":265
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  *                     elif aligned_score > insertion_score:   # D= or DX             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(129 + modifier)
  */
           __pyx_t_1 = (__pyx_v_aligned_score > __pyx_v_insertion_score);
           if (__pyx_t_1) {
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":198
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":266
  *                         trace_row.push_back(73)
  *                     elif aligned_score > insertion_score:   # D= or DX
  *                         dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(129 + modifier)
  *                     else:                                   # ID= or IDX
  */
             try {
               __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 198, __pyx_L1_error)
+              __PYX_ERR(0, 266, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":199
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":267
  *                     elif aligned_score > insertion_score:   # D= or DX
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(129 + modifier)             # <<<<<<<<<<<<<<
  *                     else:                                   # ID= or IDX
  *                         dp_row.push_back(deletion_score)
  */
             try {
               __pyx_v_trace_row.push_back((0x81 + __pyx_v_modifier));
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 199, __pyx_L1_error)
+              __PYX_ERR(0, 267, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":197
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":265
  *                         dp_row.push_back(insertion_score)
  *                         trace_row.push_back(73)
  *                     elif aligned_score > insertion_score:   # D= or DX             # <<<<<<<<<<<<<<
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(129 + modifier)
  */
             goto __pyx_L29;
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":201
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":269
  *                         trace_row.push_back(129 + modifier)
  *                     else:                                   # ID= or IDX
  *                         dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                         trace_row.push_back(202 + modifier)
  *             dp.push_back(dp_row)
  */
           /*else*/ {
             try {
               __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 201, __pyx_L1_error)
+              __PYX_ERR(0, 269, __pyx_L1_error)
             }
 
-            /* "savemoney/modules/cython_functions/alignment_functions.pyx":202
+            /* "savemoney/modules/cython_functions/alignment_functions.pyx":270
  *                     else:                                   # ID= or IDX
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(202 + modifier)             # <<<<<<<<<<<<<<
  *             dp.push_back(dp_row)
  *             trace.push_back(trace_row)
  */
             try {
               __pyx_v_trace_row.push_back((0xCA + __pyx_v_modifier));
             } catch(...) {
               __Pyx_CppExn2PyErr();
-              __PYX_ERR(0, 202, __pyx_L1_error)
+              __PYX_ERR(0, 270, __pyx_L1_error)
             }
           }
           __pyx_L29:;
         }
         __pyx_L26:;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":203
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":271
  *                         dp_row.push_back(deletion_score)
  *                         trace_row.push_back(202 + modifier)
  *             dp.push_back(dp_row)             # <<<<<<<<<<<<<<
  *             trace.push_back(trace_row)
  *         ###########
  */
       try {
         __pyx_v_dp.push_back(__pyx_v_dp_row);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 203, __pyx_L1_error)
+        __PYX_ERR(0, 271, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":204
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":272
  *                         trace_row.push_back(202 + modifier)
  *             dp.push_back(dp_row)
  *             trace.push_back(trace_row)             # <<<<<<<<<<<<<<
  *         ###########
  *         # query #
  */
       try {
         __pyx_v_trace.push_back(__pyx_v_trace_row);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 204, __pyx_L1_error)
+        __PYX_ERR(0, 272, __pyx_L1_error)
       }
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":208
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":276
  *         # query #
  *         ###########
  *         i = N_query_seq_1 - 1             # <<<<<<<<<<<<<<
  *         q = query_seq_1[N_query_seq_1 - 1]
  *         #
  */
     __pyx_v_i = (__pyx_v_N_query_seq_1 - 1);
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":209
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":277
  *         ###########
  *         i = N_query_seq_1 - 1
  *         q = query_seq_1[N_query_seq_1 - 1]             # <<<<<<<<<<<<<<
  *         #
  *         dp_row.clear()
  */
     __pyx_v_q = (__pyx_v_query_seq_1[(__pyx_v_N_query_seq_1 - 1)]);
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":211
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":279
  *         q = query_seq_1[N_query_seq_1 - 1]
  *         #
  *         dp_row.clear()             # <<<<<<<<<<<<<<
  *         dp_row.push_back(dp[i][0] - gap_extend_penalty)
  *         trace_row.clear()
  */
     __pyx_v_dp_row.clear();
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":212
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":280
  *         #
  *         dp_row.clear()
  *         dp_row.push_back(dp[i][0] - gap_extend_penalty)             # <<<<<<<<<<<<<<
  *         trace_row.clear()
  *         trace_row.push_back(73)     #  insertion
  */
     try {
       __pyx_v_dp_row.push_back((((__pyx_v_dp[__pyx_v_i])[0]) - __pyx_v_gap_extend_penalty));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 212, __pyx_L1_error)
+      __PYX_ERR(0, 280, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":213
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":281
  *         dp_row.clear()
  *         dp_row.push_back(dp[i][0] - gap_extend_penalty)
  *         trace_row.clear()             # <<<<<<<<<<<<<<
  *         trace_row.push_back(73)     #  insertion
  *         #
  */
     __pyx_v_trace_row.clear();
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":214
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":282
  *         dp_row.push_back(dp[i][0] - gap_extend_penalty)
  *         trace_row.clear()
  *         trace_row.push_back(73)     #  insertion             # <<<<<<<<<<<<<<
  *         #
  *         for j in range(N_ref_seq):
  */
     try {
       __pyx_v_trace_row.push_back(73);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 214, __pyx_L1_error)
+      __PYX_ERR(0, 282, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":216
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":284
  *         trace_row.push_back(73)     #  insertion
  *         #
  *         for j in range(N_ref_seq):             # <<<<<<<<<<<<<<
  *             r = ref_seq[j]
  *             # aligned_score
  */
     __pyx_t_2 = __pyx_v_N_ref_seq;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_j = __pyx_t_4;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":217
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":285
  *         #
  *         for j in range(N_ref_seq):
  *             r = ref_seq[j]             # <<<<<<<<<<<<<<
  *             # aligned_score
  *             if q == r:
  */
       __pyx_v_r = (__pyx_v_ref_seq[__pyx_v_j]);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":219
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":287
  *             r = ref_seq[j]
  *             # aligned_score
  *             if q == r:             # <<<<<<<<<<<<<<
  *                 aligned_score = dp[i][j] + match_score
  *                 modifier = 0
  */
       __pyx_t_1 = (__pyx_v_q == __pyx_v_r);
       if (__pyx_t_1) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":220
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":288
  *             # aligned_score
  *             if q == r:
  *                 aligned_score = dp[i][j] + match_score             # <<<<<<<<<<<<<<
  *                 modifier = 0
  *             else:
  */
         __pyx_v_aligned_score = (((__pyx_v_dp[__pyx_v_i])[__pyx_v_j]) + __pyx_v_match_score);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":221
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":289
  *             if q == r:
  *                 aligned_score = dp[i][j] + match_score
  *                 modifier = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 aligned_score = dp[i][j] + mismatch_score
  */
         __pyx_v_modifier = 0;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":219
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":287
  *             r = ref_seq[j]
  *             # aligned_score
  *             if q == r:             # <<<<<<<<<<<<<<
  *                 aligned_score = dp[i][j] + match_score
  *                 modifier = 0
  */
         goto __pyx_L32;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":223
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":291
  *                 modifier = 0
  *             else:
  *                 aligned_score = dp[i][j] + mismatch_score             # <<<<<<<<<<<<<<
  *                 modifier = 27
  *             # insertion_score   #  insertion
  */
       /*else*/ {
         __pyx_v_aligned_score = (((__pyx_v_dp[__pyx_v_i])[__pyx_v_j]) + __pyx_v_mismatch_score);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":224
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":292
  *             else:
  *                 aligned_score = dp[i][j] + mismatch_score
  *                 modifier = 27             # <<<<<<<<<<<<<<
  *             # insertion_score   #  insertion
  *             if trace[i][j+1] in (73, 141, 134, 202, 161, 229):
  */
         __pyx_v_modifier = 27;
       }
       __pyx_L32:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":226
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":294
  *                 modifier = 27
  *             # insertion_score   #  insertion
  *             if trace[i][j+1] in (73, 141, 134, 202, 161, 229):             # <<<<<<<<<<<<<<
  *                 insertion_score = dp[i][j+1] - gap_extend_penalty
  *             else:
  */
       __pyx_t_8 = ((__pyx_v_trace[__pyx_v_i])[(__pyx_v_j + 1)]);
@@ -19436,783 +21731,783 @@
       }
       __pyx_t_9 = (__pyx_t_8 == 0xE5);
       __pyx_t_1 = __pyx_t_9;
       __pyx_L34_bool_binop_done:;
       __pyx_t_9 = __pyx_t_1;
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":227
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":295
  *             # insertion_score   #  insertion
  *             if trace[i][j+1] in (73, 141, 134, 202, 161, 229):
  *                 insertion_score = dp[i][j+1] - gap_extend_penalty             # <<<<<<<<<<<<<<
  *             else:
  *                 insertion_score = dp[i][j+1] - gap_open_penalty
  */
         __pyx_v_insertion_score = (((__pyx_v_dp[__pyx_v_i])[(__pyx_v_j + 1)]) - __pyx_v_gap_extend_penalty);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":226
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":294
  *                 modifier = 27
  *             # insertion_score   #  insertion
  *             if trace[i][j+1] in (73, 141, 134, 202, 161, 229):             # <<<<<<<<<<<<<<
  *                 insertion_score = dp[i][j+1] - gap_extend_penalty
  *             else:
  */
         goto __pyx_L33;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":229
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":297
  *                 insertion_score = dp[i][j+1] - gap_extend_penalty
  *             else:
  *                 insertion_score = dp[i][j+1] - gap_open_penalty             # <<<<<<<<<<<<<<
  *             # deletion_score   #  deletion
  *             deletion_score = dp_row[j]      # special deletion: no penalty
  */
       /*else*/ {
         __pyx_v_insertion_score = (((__pyx_v_dp[__pyx_v_i])[(__pyx_v_j + 1)]) - __pyx_v_gap_open_penalty);
       }
       __pyx_L33:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":231
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":299
  *                 insertion_score = dp[i][j+1] - gap_open_penalty
  *             # deletion_score   #  deletion
  *             deletion_score = dp_row[j]      # special deletion: no penalty             # <<<<<<<<<<<<<<
  *             # set dp and trace
  *             if aligned_score > deletion_score:
  */
       __pyx_v_deletion_score = (__pyx_v_dp_row[__pyx_v_j]);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":233
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":301
  *             deletion_score = dp_row[j]      # special deletion: no penalty
  *             # set dp and trace
  *             if aligned_score > deletion_score:             # <<<<<<<<<<<<<<
  *                 if aligned_score > insertion_score:     # = or X
  *                     dp_row.push_back(aligned_score)
  */
       __pyx_t_9 = (__pyx_v_aligned_score > __pyx_v_deletion_score);
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":234
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":302
  *             # set dp and trace
  *             if aligned_score > deletion_score:
  *                 if aligned_score > insertion_score:     # = or X             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)
  */
         __pyx_t_9 = (__pyx_v_aligned_score > __pyx_v_insertion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":235
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":303
  *             if aligned_score > deletion_score:
  *                 if aligned_score > insertion_score:     # = or X
  *                     dp_row.push_back(aligned_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(61 + modifier)
  *                 elif aligned_score < insertion_score:   # I
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_aligned_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 235, __pyx_L1_error)
+            __PYX_ERR(0, 303, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":236
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":304
  *                 if aligned_score > insertion_score:     # = or X
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)             # <<<<<<<<<<<<<<
  *                 elif aligned_score < insertion_score:   # I
  *                     dp_row.push_back(insertion_score)
  */
           try {
             __pyx_v_trace_row.push_back((61 + __pyx_v_modifier));
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 236, __pyx_L1_error)
+            __PYX_ERR(0, 304, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":234
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":302
  *             # set dp and trace
  *             if aligned_score > deletion_score:
  *                 if aligned_score > insertion_score:     # = or X             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)
  */
           goto __pyx_L41;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":237
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":305
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)
  *                 elif aligned_score < insertion_score:   # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
         __pyx_t_9 = (__pyx_v_aligned_score < __pyx_v_insertion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":238
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":306
  *                     trace_row.push_back(61 + modifier)
  *                 elif aligned_score < insertion_score:   # I
  *                     dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(73)
  *                 else:                                   # I= or IX
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 238, __pyx_L1_error)
+            __PYX_ERR(0, 306, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":239
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":307
  *                 elif aligned_score < insertion_score:   # I
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                 else:                                   # I= or IX
  *                     dp_row.push_back(insertion_score)
  */
           try {
             __pyx_v_trace_row.push_back(73);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 239, __pyx_L1_error)
+            __PYX_ERR(0, 307, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":237
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":305
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)
  *                 elif aligned_score < insertion_score:   # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
           goto __pyx_L41;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":241
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":309
  *                     trace_row.push_back(73)
  *                 else:                                   # I= or IX
  *                     dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:
  */
         /*else*/ {
           try {
             __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 241, __pyx_L1_error)
+            __PYX_ERR(0, 309, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":242
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":310
  *                 else:                                   # I= or IX
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(134 + modifier)             # <<<<<<<<<<<<<<
  *             elif aligned_score < deletion_score:
  *                 if insertion_score > deletion_score:    # I
  */
           try {
             __pyx_v_trace_row.push_back((0x86 + __pyx_v_modifier));
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 242, __pyx_L1_error)
+            __PYX_ERR(0, 310, __pyx_L1_error)
           }
         }
         __pyx_L41:;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":233
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":301
  *             deletion_score = dp_row[j]      # special deletion: no penalty
  *             # set dp and trace
  *             if aligned_score > deletion_score:             # <<<<<<<<<<<<<<
  *                 if aligned_score > insertion_score:     # = or X
  *                     dp_row.push_back(aligned_score)
  */
         goto __pyx_L40;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":243
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":311
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:             # <<<<<<<<<<<<<<
  *                 if insertion_score > deletion_score:    # I
  *                     dp_row.push_back(insertion_score)
  */
       __pyx_t_9 = (__pyx_v_aligned_score < __pyx_v_deletion_score);
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":244
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":312
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:
  *                 if insertion_score > deletion_score:    # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
         __pyx_t_9 = (__pyx_v_insertion_score > __pyx_v_deletion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":245
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":313
  *             elif aligned_score < deletion_score:
  *                 if insertion_score > deletion_score:    # I
  *                     dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(73)
  *                 elif insertion_score < deletion_score:  # H #  deletion
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 245, __pyx_L1_error)
+            __PYX_ERR(0, 313, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":246
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":314
  *                 if insertion_score > deletion_score:    # I
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                 elif insertion_score < deletion_score:  # H #  deletion
  *                     dp_row.push_back(deletion_score)
  */
           try {
             __pyx_v_trace_row.push_back(73);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 246, __pyx_L1_error)
+            __PYX_ERR(0, 314, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":244
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":312
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:
  *                 if insertion_score > deletion_score:    # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
           goto __pyx_L42;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":247
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":315
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  *                 elif insertion_score < deletion_score:  # H #  deletion             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(72)
  */
         __pyx_t_9 = (__pyx_v_insertion_score < __pyx_v_deletion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":248
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":316
  *                     trace_row.push_back(73)
  *                 elif insertion_score < deletion_score:  # H #  deletion
  *                     dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(72)
  *                 else:                                   # IH
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 248, __pyx_L1_error)
+            __PYX_ERR(0, 316, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":249
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":317
  *                 elif insertion_score < deletion_score:  # H #  deletion
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(72)             # <<<<<<<<<<<<<<
  *                 else:                                   # IH
  *                     dp_row.push_back(deletion_score)
  */
           try {
             __pyx_v_trace_row.push_back(72);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 249, __pyx_L1_error)
+            __PYX_ERR(0, 317, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":247
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":315
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  *                 elif insertion_score < deletion_score:  # H #  deletion             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(72)
  */
           goto __pyx_L42;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":251
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":319
  *                     trace_row.push_back(72)
  *                 else:                                   # IH
  *                     dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(145)
  *             else:
  */
         /*else*/ {
           try {
             __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 251, __pyx_L1_error)
+            __PYX_ERR(0, 319, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":252
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":320
  *                 else:                                   # IH
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(145)             # <<<<<<<<<<<<<<
  *             else:
  *                 if aligned_score < insertion_score:     # I
  */
           try {
             __pyx_v_trace_row.push_back(0x91);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 252, __pyx_L1_error)
+            __PYX_ERR(0, 320, __pyx_L1_error)
           }
         }
         __pyx_L42:;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":243
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":311
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:             # <<<<<<<<<<<<<<
  *                 if insertion_score > deletion_score:    # I
  *                     dp_row.push_back(insertion_score)
  */
         goto __pyx_L40;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":254
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":322
  *                     trace_row.push_back(145)
  *             else:
  *                 if aligned_score < insertion_score:     # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
       /*else*/ {
         __pyx_t_9 = (__pyx_v_aligned_score < __pyx_v_insertion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":255
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":323
  *             else:
  *                 if aligned_score < insertion_score:     # I
  *                     dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(73)
  *                 elif aligned_score > insertion_score:   # H= or HX
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 255, __pyx_L1_error)
+            __PYX_ERR(0, 323, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":256
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":324
  *                 if aligned_score < insertion_score:     # I
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                 elif aligned_score > insertion_score:   # H= or HX
  *                     dp_row.push_back(deletion_score)
  */
           try {
             __pyx_v_trace_row.push_back(73);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 256, __pyx_L1_error)
+            __PYX_ERR(0, 324, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":254
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":322
  *                     trace_row.push_back(145)
  *             else:
  *                 if aligned_score < insertion_score:     # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
           goto __pyx_L43;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":257
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":325
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  *                 elif aligned_score > insertion_score:   # H= or HX             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(133 + modifier)
  */
         __pyx_t_9 = (__pyx_v_aligned_score > __pyx_v_insertion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":258
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":326
  *                     trace_row.push_back(73)
  *                 elif aligned_score > insertion_score:   # H= or HX
  *                     dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(133 + modifier)
  *                 else:                                   # IH= or IHX
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 258, __pyx_L1_error)
+            __PYX_ERR(0, 326, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":259
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":327
  *                 elif aligned_score > insertion_score:   # H= or HX
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(133 + modifier)             # <<<<<<<<<<<<<<
  *                 else:                                   # IH= or IHX
  *                     dp_row.push_back(deletion_score)
  */
           try {
             __pyx_v_trace_row.push_back((0x85 + __pyx_v_modifier));
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 259, __pyx_L1_error)
+            __PYX_ERR(0, 327, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":257
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":325
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  *                 elif aligned_score > insertion_score:   # H= or HX             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(133 + modifier)
  */
           goto __pyx_L43;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":261
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":329
  *                     trace_row.push_back(133 + modifier)
  *                 else:                                   # IH= or IHX
  *                     dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(206 + modifier)
  *         dp.push_back(dp_row)
  */
         /*else*/ {
           try {
             __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 261, __pyx_L1_error)
+            __PYX_ERR(0, 329, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":262
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":330
  *                 else:                                   # IH= or IHX
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(206 + modifier)             # <<<<<<<<<<<<<<
  *         dp.push_back(dp_row)
  *         trace.push_back(trace_row)
  */
           try {
             __pyx_v_trace_row.push_back((0xCE + __pyx_v_modifier));
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 262, __pyx_L1_error)
+            __PYX_ERR(0, 330, __pyx_L1_error)
           }
         }
         __pyx_L43:;
       }
       __pyx_L40:;
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":263
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":331
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(206 + modifier)
  *         dp.push_back(dp_row)             # <<<<<<<<<<<<<<
  *         trace.push_back(trace_row)
  *     else:
  */
     try {
       __pyx_v_dp.push_back(__pyx_v_dp_row);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 263, __pyx_L1_error)
+      __PYX_ERR(0, 331, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":264
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":332
  *                     trace_row.push_back(206 + modifier)
  *         dp.push_back(dp_row)
  *         trace.push_back(trace_row)             # <<<<<<<<<<<<<<
  *     else:
  *         #
  */
     try {
       __pyx_v_trace.push_back(__pyx_v_trace_row);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 264, __pyx_L1_error)
+      __PYX_ERR(0, 332, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":129
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":197
  *     # DP of query_seq_1 #
  *     #####################
  *     if N_query_seq_1 > 0:             # <<<<<<<<<<<<<<
  *         ###############
  *         # query_seq_1 #
  */
     goto __pyx_L3;
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":267
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":335
  *     else:
  *         #
  *         for j in range(N_ref_seq):             # <<<<<<<<<<<<<<
  *             dp_row.push_back(0)
  *             trace_row.push_back(72)
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_N_ref_seq;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_j = __pyx_t_4;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":268
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":336
  *         #
  *         for j in range(N_ref_seq):
  *             dp_row.push_back(0)             # <<<<<<<<<<<<<<
  *             trace_row.push_back(72)
  *         dp.push_back(dp_row)
  */
       try {
         __pyx_v_dp_row.push_back(0);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 268, __pyx_L1_error)
+        __PYX_ERR(0, 336, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":269
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":337
  *         for j in range(N_ref_seq):
  *             dp_row.push_back(0)
  *             trace_row.push_back(72)             # <<<<<<<<<<<<<<
  *         dp.push_back(dp_row)
  *         trace.push_back(trace_row)
  */
       try {
         __pyx_v_trace_row.push_back(72);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 269, __pyx_L1_error)
+        __PYX_ERR(0, 337, __pyx_L1_error)
       }
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":270
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":338
  *             dp_row.push_back(0)
  *             trace_row.push_back(72)
  *         dp.push_back(dp_row)             # <<<<<<<<<<<<<<
  *         trace.push_back(trace_row)
  *     #####################
  */
     try {
       __pyx_v_dp.push_back(__pyx_v_dp_row);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 270, __pyx_L1_error)
+      __PYX_ERR(0, 338, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":271
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":339
  *             trace_row.push_back(72)
  *         dp.push_back(dp_row)
  *         trace.push_back(trace_row)             # <<<<<<<<<<<<<<
  *     #####################
  *     # DP of query_seq_2 #
  */
     try {
       __pyx_v_trace.push_back(__pyx_v_trace_row);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 271, __pyx_L1_error)
+      __PYX_ERR(0, 339, __pyx_L1_error)
     }
   }
   __pyx_L3:;
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":275
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":343
  *     # DP of query_seq_2 #
  *     #####################
  *     for i in range(N_query_seq_2):             # <<<<<<<<<<<<<<
  *         q = query_seq_2[i]
  *         i += N_query_seq_1
  */
   __pyx_t_2 = __pyx_v_N_query_seq_2;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":276
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":344
  *     #####################
  *     for i in range(N_query_seq_2):
  *         q = query_seq_2[i]             # <<<<<<<<<<<<<<
  *         i += N_query_seq_1
  *         #
  */
     __pyx_v_q = (__pyx_v_query_seq_2[__pyx_v_i]);
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":277
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":345
  *     for i in range(N_query_seq_2):
  *         q = query_seq_2[i]
  *         i += N_query_seq_1             # <<<<<<<<<<<<<<
  *         #
  *         dp_row.clear()
  */
     __pyx_v_i = (__pyx_v_i + __pyx_v_N_query_seq_1);
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":279
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":347
  *         i += N_query_seq_1
  *         #
  *         dp_row.clear()             # <<<<<<<<<<<<<<
  *         if i == 0:
  *             dp_row.push_back(dp[i][0] - gap_open_penalty)
  */
     __pyx_v_dp_row.clear();
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":280
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":348
  *         #
  *         dp_row.clear()
  *         if i == 0:             # <<<<<<<<<<<<<<
  *             dp_row.push_back(dp[i][0] - gap_open_penalty)
  *         else:
  */
     __pyx_t_9 = (__pyx_v_i == 0);
     if (__pyx_t_9) {
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":281
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":349
  *         dp_row.clear()
  *         if i == 0:
  *             dp_row.push_back(dp[i][0] - gap_open_penalty)             # <<<<<<<<<<<<<<
  *         else:
  *             dp_row.push_back(dp[i][0] - gap_extend_penalty)
  */
       try {
         __pyx_v_dp_row.push_back((((__pyx_v_dp[__pyx_v_i])[0]) - __pyx_v_gap_open_penalty));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 281, __pyx_L1_error)
+        __PYX_ERR(0, 349, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":280
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":348
  *         #
  *         dp_row.clear()
  *         if i == 0:             # <<<<<<<<<<<<<<
  *             dp_row.push_back(dp[i][0] - gap_open_penalty)
  *         else:
  */
       goto __pyx_L48;
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":283
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":351
  *             dp_row.push_back(dp[i][0] - gap_open_penalty)
  *         else:
  *             dp_row.push_back(dp[i][0] - gap_extend_penalty)             # <<<<<<<<<<<<<<
  *         trace_row.clear()
  *         trace_row.push_back(73)     #  insertion
  */
     /*else*/ {
       try {
         __pyx_v_dp_row.push_back((((__pyx_v_dp[__pyx_v_i])[0]) - __pyx_v_gap_extend_penalty));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 283, __pyx_L1_error)
+        __PYX_ERR(0, 351, __pyx_L1_error)
       }
     }
     __pyx_L48:;
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":284
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":352
  *         else:
  *             dp_row.push_back(dp[i][0] - gap_extend_penalty)
  *         trace_row.clear()             # <<<<<<<<<<<<<<
  *         trace_row.push_back(73)     #  insertion
  *         #
  */
     __pyx_v_trace_row.clear();
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":285
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":353
  *             dp_row.push_back(dp[i][0] - gap_extend_penalty)
  *         trace_row.clear()
  *         trace_row.push_back(73)     #  insertion             # <<<<<<<<<<<<<<
  *         #
  *         for j in range(N_ref_seq):
  */
     try {
       __pyx_v_trace_row.push_back(73);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 285, __pyx_L1_error)
+      __PYX_ERR(0, 353, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":287
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":355
  *         trace_row.push_back(73)     #  insertion
  *         #
  *         for j in range(N_ref_seq):             # <<<<<<<<<<<<<<
  *             r = ref_seq[j]
  *             # aligned_score
  */
     __pyx_t_5 = __pyx_v_N_ref_seq;
     __pyx_t_6 = __pyx_t_5;
     for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
       __pyx_v_j = __pyx_t_7;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":288
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":356
  *         #
  *         for j in range(N_ref_seq):
  *             r = ref_seq[j]             # <<<<<<<<<<<<<<
  *             # aligned_score
  *             if q == r:
  */
       __pyx_v_r = (__pyx_v_ref_seq[__pyx_v_j]);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":290
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":358
  *             r = ref_seq[j]
  *             # aligned_score
  *             if q == r:             # <<<<<<<<<<<<<<
  *                 aligned_score = dp[i][j] + match_score
  *                 modifier = 0
  */
       __pyx_t_9 = (__pyx_v_q == __pyx_v_r);
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":291
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":359
  *             # aligned_score
  *             if q == r:
  *                 aligned_score = dp[i][j] + match_score             # <<<<<<<<<<<<<<
  *                 modifier = 0
  *             else:
  */
         __pyx_v_aligned_score = (((__pyx_v_dp[__pyx_v_i])[__pyx_v_j]) + __pyx_v_match_score);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":292
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":360
  *             if q == r:
  *                 aligned_score = dp[i][j] + match_score
  *                 modifier = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 aligned_score = dp[i][j] + mismatch_score
  */
         __pyx_v_modifier = 0;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":290
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":358
  *             r = ref_seq[j]
  *             # aligned_score
  *             if q == r:             # <<<<<<<<<<<<<<
  *                 aligned_score = dp[i][j] + match_score
  *                 modifier = 0
  */
         goto __pyx_L51;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":294
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":362
  *                 modifier = 0
  *             else:
  *                 aligned_score = dp[i][j] + mismatch_score             # <<<<<<<<<<<<<<
  *                 modifier = 27
  *             # insertion_score   #  insertion
  */
       /*else*/ {
         __pyx_v_aligned_score = (((__pyx_v_dp[__pyx_v_i])[__pyx_v_j]) + __pyx_v_mismatch_score);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":295
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":363
  *             else:
  *                 aligned_score = dp[i][j] + mismatch_score
  *                 modifier = 27             # <<<<<<<<<<<<<<
  *             # insertion_score   #  insertion
  *             if trace[i][j+1] in (73, 141, 134, 202, 161, 229, 145, 206, 233):
  */
         __pyx_v_modifier = 27;
       }
       __pyx_L51:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":297
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":365
  *                 modifier = 27
  *             # insertion_score   #  insertion
  *             if trace[i][j+1] in (73, 141, 134, 202, 161, 229, 145, 206, 233):             # <<<<<<<<<<<<<<
  *                 insertion_score = dp[i][j+1] - gap_extend_penalty
  *             else:
  */
       __pyx_t_8 = ((__pyx_v_trace[__pyx_v_i])[(__pyx_v_j + 1)]);
@@ -20266,46 +22561,46 @@
       }
       __pyx_t_1 = (__pyx_t_8 == 0xE9);
       __pyx_t_9 = __pyx_t_1;
       __pyx_L53_bool_binop_done:;
       __pyx_t_1 = __pyx_t_9;
       if (__pyx_t_1) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":298
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":366
  *             # insertion_score   #  insertion
  *             if trace[i][j+1] in (73, 141, 134, 202, 161, 229, 145, 206, 233):
  *                 insertion_score = dp[i][j+1] - gap_extend_penalty             # <<<<<<<<<<<<<<
  *             else:
  *                 insertion_score = dp[i][j+1] - gap_open_penalty
  */
         __pyx_v_insertion_score = (((__pyx_v_dp[__pyx_v_i])[(__pyx_v_j + 1)]) - __pyx_v_gap_extend_penalty);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":297
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":365
  *                 modifier = 27
  *             # insertion_score   #  insertion
  *             if trace[i][j+1] in (73, 141, 134, 202, 161, 229, 145, 206, 233):             # <<<<<<<<<<<<<<
  *                 insertion_score = dp[i][j+1] - gap_extend_penalty
  *             else:
  */
         goto __pyx_L52;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":300
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":368
  *                 insertion_score = dp[i][j+1] - gap_extend_penalty
  *             else:
  *                 insertion_score = dp[i][j+1] - gap_open_penalty             # <<<<<<<<<<<<<<
  *             # deletion_score   #  deletion
  *             if trace_row[j] in (68, 141, 129, 202, 156, 229):
  */
       /*else*/ {
         __pyx_v_insertion_score = (((__pyx_v_dp[__pyx_v_i])[(__pyx_v_j + 1)]) - __pyx_v_gap_open_penalty);
       }
       __pyx_L52:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":302
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":370
  *                 insertion_score = dp[i][j+1] - gap_open_penalty
  *             # deletion_score   #  deletion
  *             if trace_row[j] in (68, 141, 129, 202, 156, 229):             # <<<<<<<<<<<<<<
  *                 deletion_score = dp_row[j] - gap_extend_penalty
  *             else:
  */
       __pyx_t_8 = (__pyx_v_trace_row[__pyx_v_j]);
@@ -20341,710 +22636,710 @@
       }
       __pyx_t_9 = (__pyx_t_8 == 0xE5);
       __pyx_t_1 = __pyx_t_9;
       __pyx_L63_bool_binop_done:;
       __pyx_t_9 = __pyx_t_1;
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":303
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":371
  *             # deletion_score   #  deletion
  *             if trace_row[j] in (68, 141, 129, 202, 156, 229):
  *                 deletion_score = dp_row[j] - gap_extend_penalty             # <<<<<<<<<<<<<<
  *             else:
  *                 deletion_score = dp_row[j] - gap_open_penalty
  */
         __pyx_v_deletion_score = ((__pyx_v_dp_row[__pyx_v_j]) - __pyx_v_gap_extend_penalty);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":302
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":370
  *                 insertion_score = dp[i][j+1] - gap_open_penalty
  *             # deletion_score   #  deletion
  *             if trace_row[j] in (68, 141, 129, 202, 156, 229):             # <<<<<<<<<<<<<<
  *                 deletion_score = dp_row[j] - gap_extend_penalty
  *             else:
  */
         goto __pyx_L62;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":305
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":373
  *                 deletion_score = dp_row[j] - gap_extend_penalty
  *             else:
  *                 deletion_score = dp_row[j] - gap_open_penalty             # <<<<<<<<<<<<<<
  *             # set dp and trace
  *             if aligned_score > deletion_score:
  */
       /*else*/ {
         __pyx_v_deletion_score = ((__pyx_v_dp_row[__pyx_v_j]) - __pyx_v_gap_open_penalty);
       }
       __pyx_L62:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":307
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":375
  *                 deletion_score = dp_row[j] - gap_open_penalty
  *             # set dp and trace
  *             if aligned_score > deletion_score:             # <<<<<<<<<<<<<<
  *                 if aligned_score > insertion_score:     # = or X
  *                     dp_row.push_back(aligned_score)
  */
       __pyx_t_9 = (__pyx_v_aligned_score > __pyx_v_deletion_score);
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":308
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":376
  *             # set dp and trace
  *             if aligned_score > deletion_score:
  *                 if aligned_score > insertion_score:     # = or X             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)
  */
         __pyx_t_9 = (__pyx_v_aligned_score > __pyx_v_insertion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":309
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":377
  *             if aligned_score > deletion_score:
  *                 if aligned_score > insertion_score:     # = or X
  *                     dp_row.push_back(aligned_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(61 + modifier)
  *                 elif aligned_score < insertion_score:   # I
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_aligned_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 309, __pyx_L1_error)
+            __PYX_ERR(0, 377, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":310
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":378
  *                 if aligned_score > insertion_score:     # = or X
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)             # <<<<<<<<<<<<<<
  *                 elif aligned_score < insertion_score:   # I
  *                     dp_row.push_back(insertion_score)
  */
           try {
             __pyx_v_trace_row.push_back((61 + __pyx_v_modifier));
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 310, __pyx_L1_error)
+            __PYX_ERR(0, 378, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":308
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":376
  *             # set dp and trace
  *             if aligned_score > deletion_score:
  *                 if aligned_score > insertion_score:     # = or X             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)
  */
           goto __pyx_L70;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":311
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":379
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)
  *                 elif aligned_score < insertion_score:   # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
         __pyx_t_9 = (__pyx_v_aligned_score < __pyx_v_insertion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":312
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":380
  *                     trace_row.push_back(61 + modifier)
  *                 elif aligned_score < insertion_score:   # I
  *                     dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(73)
  *                 else:                                   # I= or IX
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 312, __pyx_L1_error)
+            __PYX_ERR(0, 380, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":313
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":381
  *                 elif aligned_score < insertion_score:   # I
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                 else:                                   # I= or IX
  *                     dp_row.push_back(insertion_score)
  */
           try {
             __pyx_v_trace_row.push_back(73);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 313, __pyx_L1_error)
+            __PYX_ERR(0, 381, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":311
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":379
  *                     dp_row.push_back(aligned_score)
  *                     trace_row.push_back(61 + modifier)
  *                 elif aligned_score < insertion_score:   # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
           goto __pyx_L70;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":315
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":383
  *                     trace_row.push_back(73)
  *                 else:                                   # I= or IX
  *                     dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:
  */
         /*else*/ {
           try {
             __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 315, __pyx_L1_error)
+            __PYX_ERR(0, 383, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":316
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":384
  *                 else:                                   # I= or IX
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(134 + modifier)             # <<<<<<<<<<<<<<
  *             elif aligned_score < deletion_score:
  *                 if insertion_score > deletion_score:    # I
  */
           try {
             __pyx_v_trace_row.push_back((0x86 + __pyx_v_modifier));
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 316, __pyx_L1_error)
+            __PYX_ERR(0, 384, __pyx_L1_error)
           }
         }
         __pyx_L70:;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":307
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":375
  *                 deletion_score = dp_row[j] - gap_open_penalty
  *             # set dp and trace
  *             if aligned_score > deletion_score:             # <<<<<<<<<<<<<<
  *                 if aligned_score > insertion_score:     # = or X
  *                     dp_row.push_back(aligned_score)
  */
         goto __pyx_L69;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":317
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":385
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:             # <<<<<<<<<<<<<<
  *                 if insertion_score > deletion_score:    # I
  *                     dp_row.push_back(insertion_score)
  */
       __pyx_t_9 = (__pyx_v_aligned_score < __pyx_v_deletion_score);
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":318
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":386
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:
  *                 if insertion_score > deletion_score:    # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
         __pyx_t_9 = (__pyx_v_insertion_score > __pyx_v_deletion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":319
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":387
  *             elif aligned_score < deletion_score:
  *                 if insertion_score > deletion_score:    # I
  *                     dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(73)
  *                 elif insertion_score < deletion_score:  # D
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 319, __pyx_L1_error)
+            __PYX_ERR(0, 387, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":320
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":388
  *                 if insertion_score > deletion_score:    # I
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                 elif insertion_score < deletion_score:  # D
  *                     dp_row.push_back(deletion_score)
  */
           try {
             __pyx_v_trace_row.push_back(73);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 320, __pyx_L1_error)
+            __PYX_ERR(0, 388, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":318
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":386
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:
  *                 if insertion_score > deletion_score:    # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
           goto __pyx_L71;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":321
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":389
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  *                 elif insertion_score < deletion_score:  # D             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(68)
  */
         __pyx_t_9 = (__pyx_v_insertion_score < __pyx_v_deletion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":322
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":390
  *                     trace_row.push_back(73)
  *                 elif insertion_score < deletion_score:  # D
  *                     dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(68)
  *                 else:                                   # ID
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 322, __pyx_L1_error)
+            __PYX_ERR(0, 390, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":323
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":391
  *                 elif insertion_score < deletion_score:  # D
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(68)             # <<<<<<<<<<<<<<
  *                 else:                                   # ID
  *                     dp_row.push_back(deletion_score)
  */
           try {
             __pyx_v_trace_row.push_back(68);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 323, __pyx_L1_error)
+            __PYX_ERR(0, 391, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":321
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":389
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  *                 elif insertion_score < deletion_score:  # D             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(68)
  */
           goto __pyx_L71;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":325
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":393
  *                     trace_row.push_back(68)
  *                 else:                                   # ID
  *                     dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(141)
  *             else:
  */
         /*else*/ {
           try {
             __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 325, __pyx_L1_error)
+            __PYX_ERR(0, 393, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":326
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":394
  *                 else:                                   # ID
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(141)             # <<<<<<<<<<<<<<
  *             else:
  *                 if aligned_score < insertion_score:     # I
  */
           try {
             __pyx_v_trace_row.push_back(0x8D);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 326, __pyx_L1_error)
+            __PYX_ERR(0, 394, __pyx_L1_error)
           }
         }
         __pyx_L71:;
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":317
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":385
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(134 + modifier)
  *             elif aligned_score < deletion_score:             # <<<<<<<<<<<<<<
  *                 if insertion_score > deletion_score:    # I
  *                     dp_row.push_back(insertion_score)
  */
         goto __pyx_L69;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":328
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":396
  *                     trace_row.push_back(141)
  *             else:
  *                 if aligned_score < insertion_score:     # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
       /*else*/ {
         __pyx_t_9 = (__pyx_v_aligned_score < __pyx_v_insertion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":329
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":397
  *             else:
  *                 if aligned_score < insertion_score:     # I
  *                     dp_row.push_back(insertion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(73)
  *                 elif aligned_score > insertion_score:   # D= or DX
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_insertion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 329, __pyx_L1_error)
+            __PYX_ERR(0, 397, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":330
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":398
  *                 if aligned_score < insertion_score:     # I
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)             # <<<<<<<<<<<<<<
  *                 elif aligned_score > insertion_score:   # D= or DX
  *                     dp_row.push_back(deletion_score)
  */
           try {
             __pyx_v_trace_row.push_back(73);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 330, __pyx_L1_error)
+            __PYX_ERR(0, 398, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":328
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":396
  *                     trace_row.push_back(141)
  *             else:
  *                 if aligned_score < insertion_score:     # I             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  */
           goto __pyx_L72;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":331
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":399
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  *                 elif aligned_score > insertion_score:   # D= or DX             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(129 + modifier)
  */
         __pyx_t_9 = (__pyx_v_aligned_score > __pyx_v_insertion_score);
         if (__pyx_t_9) {
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":332
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":400
  *                     trace_row.push_back(73)
  *                 elif aligned_score > insertion_score:   # D= or DX
  *                     dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(129 + modifier)
  *                 else:                                   # ID= or IDX
  */
           try {
             __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 332, __pyx_L1_error)
+            __PYX_ERR(0, 400, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":333
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":401
  *                 elif aligned_score > insertion_score:   # D= or DX
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(129 + modifier)             # <<<<<<<<<<<<<<
  *                 else:                                   # ID= or IDX
  *                     dp_row.push_back(deletion_score)
  */
           try {
             __pyx_v_trace_row.push_back((0x81 + __pyx_v_modifier));
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 333, __pyx_L1_error)
+            __PYX_ERR(0, 401, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":331
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":399
  *                     dp_row.push_back(insertion_score)
  *                     trace_row.push_back(73)
  *                 elif aligned_score > insertion_score:   # D= or DX             # <<<<<<<<<<<<<<
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(129 + modifier)
  */
           goto __pyx_L72;
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":335
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":403
  *                     trace_row.push_back(129 + modifier)
  *                 else:                                   # ID= or IDX
  *                     dp_row.push_back(deletion_score)             # <<<<<<<<<<<<<<
  *                     trace_row.push_back(202 + modifier)
  *         dp.push_back(dp_row)
  */
         /*else*/ {
           try {
             __pyx_v_dp_row.push_back(__pyx_v_deletion_score);
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 335, __pyx_L1_error)
+            __PYX_ERR(0, 403, __pyx_L1_error)
           }
 
-          /* "savemoney/modules/cython_functions/alignment_functions.pyx":336
+          /* "savemoney/modules/cython_functions/alignment_functions.pyx":404
  *                 else:                                   # ID= or IDX
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(202 + modifier)             # <<<<<<<<<<<<<<
  *         dp.push_back(dp_row)
  *         trace.push_back(trace_row)
  */
           try {
             __pyx_v_trace_row.push_back((0xCA + __pyx_v_modifier));
           } catch(...) {
             __Pyx_CppExn2PyErr();
-            __PYX_ERR(0, 336, __pyx_L1_error)
+            __PYX_ERR(0, 404, __pyx_L1_error)
           }
         }
         __pyx_L72:;
       }
       __pyx_L69:;
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":337
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":405
  *                     dp_row.push_back(deletion_score)
  *                     trace_row.push_back(202 + modifier)
  *         dp.push_back(dp_row)             # <<<<<<<<<<<<<<
  *         trace.push_back(trace_row)
  *     #############
  */
     try {
       __pyx_v_dp.push_back(__pyx_v_dp_row);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 337, __pyx_L1_error)
+      __PYX_ERR(0, 405, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":338
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":406
  *                     trace_row.push_back(202 + modifier)
  *         dp.push_back(dp_row)
  *         trace.push_back(trace_row)             # <<<<<<<<<<<<<<
  *     #############
  *     # traceback #
  */
     try {
       __pyx_v_trace.push_back(__pyx_v_trace_row);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 338, __pyx_L1_error)
+      __PYX_ERR(0, 406, __pyx_L1_error)
     }
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":343
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":411
  *     #############
  *     #
  *     i = N_query_seq_1 + N_query_seq_2             # <<<<<<<<<<<<<<
  *     j = N_ref_seq
  *     cdef vec traceback
  */
   __pyx_v_i = (__pyx_v_N_query_seq_1 + __pyx_v_N_query_seq_2);
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":344
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":412
  *     #
  *     i = N_query_seq_1 + N_query_seq_2
  *     j = N_ref_seq             # <<<<<<<<<<<<<<
  *     cdef vec traceback
  *     cdef vec score_trace
  */
   __pyx_v_j = __pyx_v_N_ref_seq;
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":348
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":416
  *     cdef vec score_trace
  *     cdef LL t
  *     while True:             # <<<<<<<<<<<<<<
  *         t = trace[i][j]
  *         score_trace.push_back(dp[i][j])
  */
   while (1) {
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":349
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":417
  *     cdef LL t
  *     while True:
  *         t = trace[i][j]             # <<<<<<<<<<<<<<
  *         score_trace.push_back(dp[i][j])
  *         if t == 61:     # I
  */
     __pyx_v_t = ((__pyx_v_trace[__pyx_v_i])[__pyx_v_j]);
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":350
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":418
  *     while True:
  *         t = trace[i][j]
  *         score_trace.push_back(dp[i][j])             # <<<<<<<<<<<<<<
  *         if t == 61:     # I
  *             i -= 1
  */
     try {
       __pyx_v_score_trace.push_back(((__pyx_v_dp[__pyx_v_i])[__pyx_v_j]));
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 350, __pyx_L1_error)
+      __PYX_ERR(0, 418, __pyx_L1_error)
     }
 
-    /* "savemoney/modules/cython_functions/alignment_functions.pyx":351
+    /* "savemoney/modules/cython_functions/alignment_functions.pyx":419
  *         t = trace[i][j]
  *         score_trace.push_back(dp[i][j])
  *         if t == 61:     # I             # <<<<<<<<<<<<<<
  *             i -= 1
  *             j -= 1
  */
     switch (__pyx_v_t) {
       case 61:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":352
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":420
  *         score_trace.push_back(dp[i][j])
  *         if t == 61:     # I
  *             i -= 1             # <<<<<<<<<<<<<<
  *             j -= 1
  *             traceback.push_back(61)     # =
  */
       __pyx_v_i = (__pyx_v_i - 1);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":353
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":421
  *         if t == 61:     # I
  *             i -= 1
  *             j -= 1             # <<<<<<<<<<<<<<
  *             traceback.push_back(61)     # =
  *         elif t == 88:   # X
  */
       __pyx_v_j = (__pyx_v_j - 1);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":354
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":422
  *             i -= 1
  *             j -= 1
  *             traceback.push_back(61)     # =             # <<<<<<<<<<<<<<
  *         elif t == 88:   # X
  *             i -= 1
  */
       try {
         __pyx_v_traceback.push_back(61);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 354, __pyx_L1_error)
+        __PYX_ERR(0, 422, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":351
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":419
  *         t = trace[i][j]
  *         score_trace.push_back(dp[i][j])
  *         if t == 61:     # I             # <<<<<<<<<<<<<<
  *             i -= 1
  *             j -= 1
  */
       break;
       case 88:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":356
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":424
  *             traceback.push_back(61)     # =
  *         elif t == 88:   # X
  *             i -= 1             # <<<<<<<<<<<<<<
  *             j -= 1
  *             traceback.push_back(88)     # X
  */
       __pyx_v_i = (__pyx_v_i - 1);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":357
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":425
  *         elif t == 88:   # X
  *             i -= 1
  *             j -= 1             # <<<<<<<<<<<<<<
  *             traceback.push_back(88)     # X
  *         elif t == 73:   # I
  */
       __pyx_v_j = (__pyx_v_j - 1);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":358
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":426
  *             i -= 1
  *             j -= 1
  *             traceback.push_back(88)     # X             # <<<<<<<<<<<<<<
  *         elif t == 73:   # I
  *             i -= 1
  */
       try {
         __pyx_v_traceback.push_back(88);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 358, __pyx_L1_error)
+        __PYX_ERR(0, 426, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":355
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":423
  *             j -= 1
  *             traceback.push_back(61)     # =
  *         elif t == 88:   # X             # <<<<<<<<<<<<<<
  *             i -= 1
  *             j -= 1
  */
       break;
       case 73:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":360
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":428
  *             traceback.push_back(88)     # X
  *         elif t == 73:   # I
  *             i -= 1             # <<<<<<<<<<<<<<
  *             traceback.push_back(73)     # I
  *         elif t == 68:   # D
  */
       __pyx_v_i = (__pyx_v_i - 1);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":361
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":429
  *         elif t == 73:   # I
  *             i -= 1
  *             traceback.push_back(73)     # I             # <<<<<<<<<<<<<<
  *         elif t == 68:   # D
  *             j -= 1
  */
       try {
         __pyx_v_traceback.push_back(73);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 361, __pyx_L1_error)
+        __PYX_ERR(0, 429, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":359
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":427
  *             j -= 1
  *             traceback.push_back(88)     # X
  *         elif t == 73:   # I             # <<<<<<<<<<<<<<
  *             i -= 1
  *             traceback.push_back(73)     # I
  */
       break;
       case 68:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":363
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":431
  *             traceback.push_back(73)     # I
  *         elif t == 68:   # D
  *             j -= 1             # <<<<<<<<<<<<<<
  *             traceback.push_back(68)     # D
  *         elif t == 134:  # I=, =
  */
       __pyx_v_j = (__pyx_v_j - 1);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":364
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":432
  *         elif t == 68:   # D
  *             j -= 1
  *             traceback.push_back(68)     # D             # <<<<<<<<<<<<<<
  *         elif t == 134:  # I=, =
  *             if traceback.empty() or (traceback.back() != 73):
  */
       try {
         __pyx_v_traceback.push_back(68);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 364, __pyx_L1_error)
+        __PYX_ERR(0, 432, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":362
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":430
  *             i -= 1
  *             traceback.push_back(73)     # I
  *         elif t == 68:   # D             # <<<<<<<<<<<<<<
  *             j -= 1
  *             traceback.push_back(68)     # D
  */
       break;
       case 0x86:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":366
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":434
  *             traceback.push_back(68)     # D
  *         elif t == 134:  # I=, =
  *             if traceback.empty() or (traceback.back() != 73):             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
       __pyx_t_1 = __pyx_v_traceback.empty();
@@ -21054,93 +23349,93 @@
         goto __pyx_L76_bool_binop_done;
       }
       __pyx_t_1 = (__pyx_v_traceback.back() != 73);
       __pyx_t_9 = __pyx_t_1;
       __pyx_L76_bool_binop_done:;
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":367
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":435
  *         elif t == 134:  # I=, =
  *             if traceback.empty() or (traceback.back() != 73):
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(61) # =
  */
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":368
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":436
  *             if traceback.empty() or (traceback.back() != 73):
  *                 i -= 1
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(61) # =
  *             else:
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":369
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":437
  *                 i -= 1
  *                 j -= 1
  *                 traceback.push_back(61) # =             # <<<<<<<<<<<<<<
  *             else:
  *                 i -= 1
  */
         try {
           __pyx_v_traceback.push_back(61);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 369, __pyx_L1_error)
+          __PYX_ERR(0, 437, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":366
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":434
  *             traceback.push_back(68)     # D
  *         elif t == 134:  # I=, =
  *             if traceback.empty() or (traceback.back() != 73):             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
         goto __pyx_L75;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":371
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":439
  *                 traceback.push_back(61) # =
  *             else:
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(73) # I
  *         elif t == 129:  # D=: =
  */
       /*else*/ {
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":372
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":440
  *             else:
  *                 i -= 1
  *                 traceback.push_back(73) # I             # <<<<<<<<<<<<<<
  *         elif t == 129:  # D=: =
  *             if traceback.empty() or (traceback.back() != 68):
  */
         try {
           __pyx_v_traceback.push_back(73);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 372, __pyx_L1_error)
+          __PYX_ERR(0, 440, __pyx_L1_error)
         }
       }
       __pyx_L75:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":365
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":433
  *             j -= 1
  *             traceback.push_back(68)     # D
  *         elif t == 134:  # I=, =             # <<<<<<<<<<<<<<
  *             if traceback.empty() or (traceback.back() != 73):
  *                 i -= 1
  */
       break;
       case 0x81:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":374
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":442
  *                 traceback.push_back(73) # I
  *         elif t == 129:  # D=: =
  *             if traceback.empty() or (traceback.back() != 68):             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
       __pyx_t_1 = __pyx_v_traceback.empty();
@@ -21150,93 +23445,93 @@
         goto __pyx_L79_bool_binop_done;
       }
       __pyx_t_1 = (__pyx_v_traceback.back() != 68);
       __pyx_t_9 = __pyx_t_1;
       __pyx_L79_bool_binop_done:;
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":375
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":443
  *         elif t == 129:  # D=: =
  *             if traceback.empty() or (traceback.back() != 68):
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(61) # =
  */
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":376
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":444
  *             if traceback.empty() or (traceback.back() != 68):
  *                 i -= 1
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(61) # =
  *             else:
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":377
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":445
  *                 i -= 1
  *                 j -= 1
  *                 traceback.push_back(61) # =             # <<<<<<<<<<<<<<
  *             else:
  *                 j -= 1
  */
         try {
           __pyx_v_traceback.push_back(61);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 377, __pyx_L1_error)
+          __PYX_ERR(0, 445, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":374
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":442
  *                 traceback.push_back(73) # I
  *         elif t == 129:  # D=: =
  *             if traceback.empty() or (traceback.back() != 68):             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
         goto __pyx_L78;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":379
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":447
  *                 traceback.push_back(61) # =
  *             else:
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(68) # D
  *         elif t == 161:  # IX: X
  */
       /*else*/ {
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":380
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":448
  *             else:
  *                 j -= 1
  *                 traceback.push_back(68) # D             # <<<<<<<<<<<<<<
  *         elif t == 161:  # IX: X
  *             if traceback.empty() or (traceback.back() != 73):
  */
         try {
           __pyx_v_traceback.push_back(68);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 380, __pyx_L1_error)
+          __PYX_ERR(0, 448, __pyx_L1_error)
         }
       }
       __pyx_L78:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":373
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":441
  *                 i -= 1
  *                 traceback.push_back(73) # I
  *         elif t == 129:  # D=: =             # <<<<<<<<<<<<<<
  *             if traceback.empty() or (traceback.back() != 68):
  *                 i -= 1
  */
       break;
       case 0xA1:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":382
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":450
  *                 traceback.push_back(68) # D
  *         elif t == 161:  # IX: X
  *             if traceback.empty() or (traceback.back() != 73):             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
       __pyx_t_1 = __pyx_v_traceback.empty();
@@ -21246,93 +23541,93 @@
         goto __pyx_L82_bool_binop_done;
       }
       __pyx_t_1 = (__pyx_v_traceback.back() != 73);
       __pyx_t_9 = __pyx_t_1;
       __pyx_L82_bool_binop_done:;
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":383
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":451
  *         elif t == 161:  # IX: X
  *             if traceback.empty() or (traceback.back() != 73):
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(88) # X
  */
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":384
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":452
  *             if traceback.empty() or (traceback.back() != 73):
  *                 i -= 1
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(88) # X
  *             else:
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":385
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":453
  *                 i -= 1
  *                 j -= 1
  *                 traceback.push_back(88) # X             # <<<<<<<<<<<<<<
  *             else:
  *                 i -= 1
  */
         try {
           __pyx_v_traceback.push_back(88);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 385, __pyx_L1_error)
+          __PYX_ERR(0, 453, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":382
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":450
  *                 traceback.push_back(68) # D
  *         elif t == 161:  # IX: X
  *             if traceback.empty() or (traceback.back() != 73):             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
         goto __pyx_L81;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":387
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":455
  *                 traceback.push_back(88) # X
  *             else:
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(73) # I
  *         elif t == 156:  # DX: X
  */
       /*else*/ {
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":388
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":456
  *             else:
  *                 i -= 1
  *                 traceback.push_back(73) # I             # <<<<<<<<<<<<<<
  *         elif t == 156:  # DX: X
  *             if traceback.empty() or (traceback.back() != 68):
  */
         try {
           __pyx_v_traceback.push_back(73);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 388, __pyx_L1_error)
+          __PYX_ERR(0, 456, __pyx_L1_error)
         }
       }
       __pyx_L81:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":381
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":449
  *                 j -= 1
  *                 traceback.push_back(68) # D
  *         elif t == 161:  # IX: X             # <<<<<<<<<<<<<<
  *             if traceback.empty() or (traceback.back() != 73):
  *                 i -= 1
  */
       break;
       case 0x9C:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":390
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":458
  *                 traceback.push_back(73) # I
  *         elif t == 156:  # DX: X
  *             if traceback.empty() or (traceback.back() != 68):             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
       __pyx_t_1 = __pyx_v_traceback.empty();
@@ -21342,93 +23637,93 @@
         goto __pyx_L85_bool_binop_done;
       }
       __pyx_t_1 = (__pyx_v_traceback.back() != 68);
       __pyx_t_9 = __pyx_t_1;
       __pyx_L85_bool_binop_done:;
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":391
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":459
  *         elif t == 156:  # DX: X
  *             if traceback.empty() or (traceback.back() != 68):
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(88) # X
  */
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":392
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":460
  *             if traceback.empty() or (traceback.back() != 68):
  *                 i -= 1
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(88) # X
  *             else:
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":393
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":461
  *                 i -= 1
  *                 j -= 1
  *                 traceback.push_back(88) # X             # <<<<<<<<<<<<<<
  *             else:
  *                 j -= 1
  */
         try {
           __pyx_v_traceback.push_back(88);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 393, __pyx_L1_error)
+          __PYX_ERR(0, 461, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":390
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":458
  *                 traceback.push_back(73) # I
  *         elif t == 156:  # DX: X
  *             if traceback.empty() or (traceback.back() != 68):             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
         goto __pyx_L84;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":395
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":463
  *                 traceback.push_back(88) # X
  *             else:
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(68) # D
  * 
  */
       /*else*/ {
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":396
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":464
  *             else:
  *                 j -= 1
  *                 traceback.push_back(68) # D             # <<<<<<<<<<<<<<
  * 
  *         elif t == 141:  # ID: D
  */
         try {
           __pyx_v_traceback.push_back(68);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 396, __pyx_L1_error)
+          __PYX_ERR(0, 464, __pyx_L1_error)
         }
       }
       __pyx_L84:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":389
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":457
  *                 i -= 1
  *                 traceback.push_back(73) # I
  *         elif t == 156:  # DX: X             # <<<<<<<<<<<<<<
  *             if traceback.empty() or (traceback.back() != 68):
  *                 i -= 1
  */
       break;
       case 0x8D:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":399
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":467
  * 
  *         elif t == 141:  # ID: D
  *             if traceback.empty() or (traceback.back() != 73):             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(68) # D  deletion
  */
       __pyx_t_1 = __pyx_v_traceback.empty();
@@ -21438,267 +23733,267 @@
         goto __pyx_L88_bool_binop_done;
       }
       __pyx_t_1 = (__pyx_v_traceback.back() != 73);
       __pyx_t_9 = __pyx_t_1;
       __pyx_L88_bool_binop_done:;
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":400
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":468
  *         elif t == 141:  # ID: D
  *             if traceback.empty() or (traceback.back() != 73):
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(68) # D  deletion
  *             else:
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":401
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":469
  *             if traceback.empty() or (traceback.back() != 73):
  *                 j -= 1
  *                 traceback.push_back(68) # D  deletion             # <<<<<<<<<<<<<<
  *             else:
  *                 i -= 1
  */
         try {
           __pyx_v_traceback.push_back(68);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 401, __pyx_L1_error)
+          __PYX_ERR(0, 469, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":399
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":467
  * 
  *         elif t == 141:  # ID: D
  *             if traceback.empty() or (traceback.back() != 73):             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(68) # D  deletion
  */
         goto __pyx_L87;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":403
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":471
  *                 traceback.push_back(68) # D  deletion
  *             else:
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(73) # I
  *         elif t == 202:  # ID=: =
  */
       /*else*/ {
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":404
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":472
  *             else:
  *                 i -= 1
  *                 traceback.push_back(73) # I             # <<<<<<<<<<<<<<
  *         elif t == 202:  # ID=: =
  *             if traceback.empty():
  */
         try {
           __pyx_v_traceback.push_back(73);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 404, __pyx_L1_error)
+          __PYX_ERR(0, 472, __pyx_L1_error)
         }
       }
       __pyx_L87:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":398
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":466
  *                 traceback.push_back(68) # D
  * 
  *         elif t == 141:  # ID: D             # <<<<<<<<<<<<<<
  *             if traceback.empty() or (traceback.back() != 73):
  *                 j -= 1
  */
       break;
       case 0xCA:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":406
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":474
  *                 traceback.push_back(73) # I
  *         elif t == 202:  # ID=: =
  *             if traceback.empty():             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
       __pyx_t_9 = __pyx_v_traceback.empty();
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":407
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":475
  *         elif t == 202:  # ID=: =
  *             if traceback.empty():
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(61) # =
  */
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":408
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":476
  *             if traceback.empty():
  *                 i -= 1
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(61) # =
  *             elif traceback.back() == 68:
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":409
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":477
  *                 i -= 1
  *                 j -= 1
  *                 traceback.push_back(61) # =             # <<<<<<<<<<<<<<
  *             elif traceback.back() == 68:
  *                 j -= 1
  */
         try {
           __pyx_v_traceback.push_back(61);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 409, __pyx_L1_error)
+          __PYX_ERR(0, 477, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":406
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":474
  *                 traceback.push_back(73) # I
  *         elif t == 202:  # ID=: =
  *             if traceback.empty():             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 j -= 1
  */
         goto __pyx_L90;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":410
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":478
  *                 j -= 1
  *                 traceback.push_back(61) # =
  *             elif traceback.back() == 68:             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(68) # D
  */
       __pyx_t_9 = (__pyx_v_traceback.back() == 68);
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":411
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":479
  *                 traceback.push_back(61) # =
  *             elif traceback.back() == 68:
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(68) # D
  *             elif traceback.back() == 73:
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":412
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":480
  *             elif traceback.back() == 68:
  *                 j -= 1
  *                 traceback.push_back(68) # D             # <<<<<<<<<<<<<<
  *             elif traceback.back() == 73:
  *                 i -= 1
  */
         try {
           __pyx_v_traceback.push_back(68);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 412, __pyx_L1_error)
+          __PYX_ERR(0, 480, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":410
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":478
  *                 j -= 1
  *                 traceback.push_back(61) # =
  *             elif traceback.back() == 68:             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(68) # D
  */
         goto __pyx_L90;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":413
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":481
  *                 j -= 1
  *                 traceback.push_back(68) # D
  *             elif traceback.back() == 73:             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 traceback.push_back(73) # I
  */
       __pyx_t_9 = (__pyx_v_traceback.back() == 73);
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":414
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":482
  *                 traceback.push_back(68) # D
  *             elif traceback.back() == 73:
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(73) # I
  *             else:
  */
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":415
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":483
  *             elif traceback.back() == 73:
  *                 i -= 1
  *                 traceback.push_back(73) # I             # <<<<<<<<<<<<<<
  *             else:
  *                 i -= 1
  */
         try {
           __pyx_v_traceback.push_back(73);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 415, __pyx_L1_error)
+          __PYX_ERR(0, 483, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":413
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":481
  *                 j -= 1
  *                 traceback.push_back(68) # D
  *             elif traceback.back() == 73:             # <<<<<<<<<<<<<<
  *                 i -= 1
  *                 traceback.push_back(73) # I
  */
         goto __pyx_L90;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":417
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":485
  *                 traceback.push_back(73) # I
  *             else:
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(61) # =
  */
       /*else*/ {
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":418
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":486
  *             else:
  *                 i -= 1
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(61) # =
  *         elif t == 229:  # IDX: D
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":419
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":487
  *                 i -= 1
  *                 j -= 1
  *                 traceback.push_back(61) # =             # <<<<<<<<<<<<<<
  *         elif t == 229:  # IDX: D
  *             if traceback.empty() or (traceback.back() != 73):
  */
         try {
           __pyx_v_traceback.push_back(61);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 419, __pyx_L1_error)
+          __PYX_ERR(0, 487, __pyx_L1_error)
         }
       }
       __pyx_L90:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":405
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":473
  *                 i -= 1
  *                 traceback.push_back(73) # I
  *         elif t == 202:  # ID=: =             # <<<<<<<<<<<<<<
  *             if traceback.empty():
  *                 i -= 1
  */
       break;
       case 0xE5:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":421
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":489
  *                 traceback.push_back(61) # =
  *         elif t == 229:  # IDX: D
  *             if traceback.empty() or (traceback.back() != 73):             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(68) # D
  */
       __pyx_t_1 = __pyx_v_traceback.empty();
@@ -21708,203 +24003,203 @@
         goto __pyx_L92_bool_binop_done;
       }
       __pyx_t_1 = (__pyx_v_traceback.back() != 73);
       __pyx_t_9 = __pyx_t_1;
       __pyx_L92_bool_binop_done:;
       if (__pyx_t_9) {
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":422
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":490
  *         elif t == 229:  # IDX: D
  *             if traceback.empty() or (traceback.back() != 73):
  *                 j -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(68) # D
  *             else:
  */
         __pyx_v_j = (__pyx_v_j - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":423
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":491
  *             if traceback.empty() or (traceback.back() != 73):
  *                 j -= 1
  *                 traceback.push_back(68) # D             # <<<<<<<<<<<<<<
  *             else:
  *                 i -= 1
  */
         try {
           __pyx_v_traceback.push_back(68);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 423, __pyx_L1_error)
+          __PYX_ERR(0, 491, __pyx_L1_error)
         }
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":421
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":489
  *                 traceback.push_back(61) # =
  *         elif t == 229:  # IDX: D
  *             if traceback.empty() or (traceback.back() != 73):             # <<<<<<<<<<<<<<
  *                 j -= 1
  *                 traceback.push_back(68) # D
  */
         goto __pyx_L91;
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":425
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":493
  *                 traceback.push_back(68) # D
  *             else:
  *                 i -= 1             # <<<<<<<<<<<<<<
  *                 traceback.push_back(73) # I
  *         elif t in (72, 145, 133, 206, 160, 233):    # H
  */
       /*else*/ {
         __pyx_v_i = (__pyx_v_i - 1);
 
-        /* "savemoney/modules/cython_functions/alignment_functions.pyx":426
+        /* "savemoney/modules/cython_functions/alignment_functions.pyx":494
  *             else:
  *                 i -= 1
  *                 traceback.push_back(73) # I             # <<<<<<<<<<<<<<
  *         elif t in (72, 145, 133, 206, 160, 233):    # H
  *             j -= 1
  */
         try {
           __pyx_v_traceback.push_back(73);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 426, __pyx_L1_error)
+          __PYX_ERR(0, 494, __pyx_L1_error)
         }
       }
       __pyx_L91:;
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":420
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":488
  *                 j -= 1
  *                 traceback.push_back(61) # =
  *         elif t == 229:  # IDX: D             # <<<<<<<<<<<<<<
  *             if traceback.empty() or (traceback.back() != 73):
  *                 j -= 1
  */
       break;
       case 72:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":427
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":495
  *                 i -= 1
  *                 traceback.push_back(73) # I
  *         elif t in (72, 145, 133, 206, 160, 233):    # H             # <<<<<<<<<<<<<<
  *             j -= 1
  *             traceback.push_back(72)
  */
       case 0x91:
       case 0x85:
       case 0xCE:
       case 0xA0:
       case 0xE9:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":428
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":496
  *                 traceback.push_back(73) # I
  *         elif t in (72, 145, 133, 206, 160, 233):    # H
  *             j -= 1             # <<<<<<<<<<<<<<
  *             traceback.push_back(72)
  *         #
  */
       __pyx_v_j = (__pyx_v_j - 1);
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":429
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":497
  *         elif t in (72, 145, 133, 206, 160, 233):    # H
  *             j -= 1
  *             traceback.push_back(72)             # <<<<<<<<<<<<<<
  *         #
  *         else:
  */
       try {
         __pyx_v_traceback.push_back(72);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 429, __pyx_L1_error)
+        __PYX_ERR(0, 497, __pyx_L1_error)
       }
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":427
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":495
  *                 i -= 1
  *                 traceback.push_back(73) # I
  *         elif t in (72, 145, 133, 206, 160, 233):    # H             # <<<<<<<<<<<<<<
  *             j -= 1
  *             traceback.push_back(72)
  */
       break;
       default:
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":432
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":500
  *         #
  *         else:
  *             assert t == 42             # <<<<<<<<<<<<<<
  *             break
  *     cdef vector[vec] result
  */
       #ifndef CYTHON_WITHOUT_ASSERTIONS
       if (unlikely(__pyx_assertions_enabled())) {
         __pyx_t_9 = (__pyx_v_t == 42);
         if (unlikely(!__pyx_t_9)) {
           __Pyx_Raise(__pyx_builtin_AssertionError, 0, 0, 0);
-          __PYX_ERR(0, 432, __pyx_L1_error)
+          __PYX_ERR(0, 500, __pyx_L1_error)
         }
       }
       #else
-      if ((1)); else __PYX_ERR(0, 432, __pyx_L1_error)
+      if ((1)); else __PYX_ERR(0, 500, __pyx_L1_error)
       #endif
 
-      /* "savemoney/modules/cython_functions/alignment_functions.pyx":433
+      /* "savemoney/modules/cython_functions/alignment_functions.pyx":501
  *         else:
  *             assert t == 42
  *             break             # <<<<<<<<<<<<<<
  *     cdef vector[vec] result
  *     result.push_back(traceback)
  */
       goto __pyx_L74_break;
       break;
     }
   }
   __pyx_L74_break:;
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":435
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":503
  *             break
  *     cdef vector[vec] result
  *     result.push_back(traceback)             # <<<<<<<<<<<<<<
  *     result.push_back(score_trace)
  *     return result
  */
   try {
     __pyx_v_result.push_back(__pyx_v_traceback);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 435, __pyx_L1_error)
+    __PYX_ERR(0, 503, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":436
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":504
  *     cdef vector[vec] result
  *     result.push_back(traceback)
  *     result.push_back(score_trace)             # <<<<<<<<<<<<<<
  *     return result
  */
   try {
     __pyx_v_result.push_back(__pyx_v_score_trace);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 436, __pyx_L1_error)
+    __PYX_ERR(0, 504, __pyx_L1_error)
   }
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":437
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":505
  *     result.push_back(traceback)
  *     result.push_back(score_trace)
  *     return result             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_10 = __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec(__pyx_v_result); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_t_10 = __pyx_convert_vector_to_py___pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_vec(__pyx_v_result); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __pyx_r = __pyx_t_10;
   __pyx_t_10 = 0;
   goto __pyx_L0;
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":66
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":134
+ *         return p_list
  * 
- * from libcpp.string cimport string
  * cpdef my_special_dp_cython(             # <<<<<<<<<<<<<<
  *         string query_seq_1,
  *         string query_seq_2,
  */
 
   /* function exit code */
   __pyx_L1_error:;
@@ -21985,103 +24280,103 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_query_seq_1)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_query_seq_2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 1); __PYX_ERR(0, 66, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 1); __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ref_seq)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 2); __PYX_ERR(0, 66, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 2); __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_gap_open_penalty)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 3); __PYX_ERR(0, 66, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 3); __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_gap_extend_penalty)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 4); __PYX_ERR(0, 66, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 4); __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_match_score)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 5); __PYX_ERR(0, 66, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 5); __PYX_ERR(0, 134, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mismatch_score)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[6]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 134, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 6); __PYX_ERR(0, 66, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, 6); __PYX_ERR(0, 134, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "my_special_dp_cython") < 0)) __PYX_ERR(0, 66, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "my_special_dp_cython") < 0)) __PYX_ERR(0, 134, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 7)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
       values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
       values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
     }
-    __pyx_v_query_seq_1 = __pyx_convert_string_from_py_std__in_string(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L3_error)
-    __pyx_v_query_seq_2 = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
-    __pyx_v_ref_seq = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 69, __pyx_L3_error)
-    __pyx_v_gap_open_penalty = __Pyx_PyInt_As_PY_LONG_LONG(values[3]); if (unlikely((__pyx_v_gap_open_penalty == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 70, __pyx_L3_error)
-    __pyx_v_gap_extend_penalty = __Pyx_PyInt_As_PY_LONG_LONG(values[4]); if (unlikely((__pyx_v_gap_extend_penalty == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 71, __pyx_L3_error)
-    __pyx_v_match_score = __Pyx_PyInt_As_PY_LONG_LONG(values[5]); if (unlikely((__pyx_v_match_score == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L3_error)
-    __pyx_v_mismatch_score = __Pyx_PyInt_As_PY_LONG_LONG(values[6]); if (unlikely((__pyx_v_mismatch_score == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L3_error)
+    __pyx_v_query_seq_1 = __pyx_convert_string_from_py_std__in_string(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 135, __pyx_L3_error)
+    __pyx_v_query_seq_2 = __pyx_convert_string_from_py_std__in_string(values[1]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L3_error)
+    __pyx_v_ref_seq = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 137, __pyx_L3_error)
+    __pyx_v_gap_open_penalty = __Pyx_PyInt_As_PY_LONG_LONG(values[3]); if (unlikely((__pyx_v_gap_open_penalty == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 138, __pyx_L3_error)
+    __pyx_v_gap_extend_penalty = __Pyx_PyInt_As_PY_LONG_LONG(values[4]); if (unlikely((__pyx_v_gap_extend_penalty == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 139, __pyx_L3_error)
+    __pyx_v_match_score = __Pyx_PyInt_As_PY_LONG_LONG(values[5]); if (unlikely((__pyx_v_match_score == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 140, __pyx_L3_error)
+    __pyx_v_mismatch_score = __Pyx_PyInt_As_PY_LONG_LONG(values[6]); if (unlikely((__pyx_v_mismatch_score == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 141, __pyx_L3_error)
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, __pyx_nargs); __PYX_ERR(0, 66, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("my_special_dp_cython", 1, 7, 7, __pyx_nargs); __PYX_ERR(0, 134, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -22109,15 +24404,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("my_special_dp_cython", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9savemoney_7modules_16cython_functions_19alignment_functions_my_special_dp_cython(__pyx_v_query_seq_1, __pyx_v_query_seq_2, __pyx_v_ref_seq, __pyx_v_gap_open_penalty, __pyx_v_gap_extend_penalty, __pyx_v_match_score, __pyx_v_mismatch_score, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9savemoney_7modules_16cython_functions_19alignment_functions_my_special_dp_cython(__pyx_v_query_seq_1, __pyx_v_query_seq_2, __pyx_v_ref_seq, __pyx_v_gap_open_penalty, __pyx_v_gap_extend_penalty, __pyx_v_match_score, __pyx_v_mismatch_score, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -22125,14 +24420,167 @@
   __Pyx_AddTraceback("savemoney.modules.cython_functions.alignment_functions.my_special_dp_cython", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
+
+static PyObject *__pyx_tp_new_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *p;
+  PyObject *o;
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
+    o = (*t->tp_alloc)(t, 0);
+  } else {
+    o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
+  }
+  if (unlikely(!o)) return 0;
+  #endif
+  p = ((struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *)o);
+  new((void*)&(p->P_base_calling_given_true_refseq_dict)) __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_map();
+  new((void*)&(p->pdf_core)) __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_str_LD_vec_map();
+  new((void*)&(p->bases)) __pyx_t_9savemoney_7modules_16cython_functions_19alignment_functions_char_vec();
+  new((void*)&(p->key)) std::string();
+  if (unlikely(__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_1__cinit__(o, a, k) < 0)) goto bad;
+  return o;
+  bad:
+  Py_DECREF(o); o = 0;
+  return NULL;
+}
+
+static void __pyx_tp_dealloc_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF(PyObject *o) {
+  struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *p = (struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF *)o;
+  #if CYTHON_USE_TP_FINALIZE
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
+  }
+  #endif
+  __Pyx_call_destructor(p->P_base_calling_given_true_refseq_dict);
+  __Pyx_call_destructor(p->pdf_core);
+  __Pyx_call_destructor(p->bases);
+  __Pyx_call_destructor(p->key);
+  #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+  (*Py_TYPE(o)->tp_free)(o);
+  #else
+  {
+    freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+    if (tp_free) tp_free(o);
+  }
+  #endif
+}
+
+static PyMethodDef __pyx_methods_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF[] = {
+  {"calc_consensus_error_rate", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_3calc_consensus_error_rate, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_2calc_consensus_error_rate},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_5__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_4__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_7__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_6__setstate_cython__},
+  {0, 0, 0, 0}
+};
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF},
+  {Py_tp_methods, (void *)__pyx_methods_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF},
+  {Py_tp_new, (void *)__pyx_tp_new_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF_spec = {
+  "savemoney.modules.cython_functions.alignment_functions.SequenceBasecallQscorePDF",
+  sizeof(struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE,
+  __pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF_slots,
+};
+#else
+
+static PyTypeObject __pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF = {
+  PyVarObject_HEAD_INIT(0, 0)
+  "savemoney.modules.cython_functions.alignment_functions.""SequenceBasecallQscorePDF", /*tp_name*/
+  sizeof(struct __pyx_obj_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF), /*tp_basicsize*/
+  0, /*tp_itemsize*/
+  __pyx_tp_dealloc_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF, /*tp_dealloc*/
+  #if PY_VERSION_HEX < 0x030800b4
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b4
+  0, /*tp_vectorcall_offset*/
+  #endif
+  0, /*tp_getattr*/
+  0, /*tp_setattr*/
+  #if PY_MAJOR_VERSION < 3
+  0, /*tp_compare*/
+  #endif
+  #if PY_MAJOR_VERSION >= 3
+  0, /*tp_as_async*/
+  #endif
+  0, /*tp_repr*/
+  0, /*tp_as_number*/
+  0, /*tp_as_sequence*/
+  0, /*tp_as_mapping*/
+  0, /*tp_hash*/
+  0, /*tp_call*/
+  0, /*tp_str*/
+  0, /*tp_getattro*/
+  0, /*tp_setattro*/
+  0, /*tp_as_buffer*/
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE, /*tp_flags*/
+  0, /*tp_doc*/
+  0, /*tp_traverse*/
+  0, /*tp_clear*/
+  0, /*tp_richcompare*/
+  0, /*tp_weaklistoffset*/
+  0, /*tp_iter*/
+  0, /*tp_iternext*/
+  __pyx_methods_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF, /*tp_methods*/
+  0, /*tp_members*/
+  0, /*tp_getset*/
+  0, /*tp_base*/
+  0, /*tp_dict*/
+  0, /*tp_descr_get*/
+  0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
+  0, /*tp_dictoffset*/
+  #endif
+  0, /*tp_init*/
+  0, /*tp_alloc*/
+  __pyx_tp_new_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF, /*tp_new*/
+  0, /*tp_free*/
+  0, /*tp_is_gc*/
+  0, /*tp_bases*/
+  0, /*tp_mro*/
+  0, /*tp_cache*/
+  0, /*tp_subclasses*/
+  0, /*tp_weaklist*/
+  0, /*tp_del*/
+  0, /*tp_version_tag*/
+  #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
+  0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
+  #endif
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  0, /*tp_vectorcall*/
+  #endif
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
+  0, /*tp_print*/
+  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
+};
+#endif
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
@@ -23094,14 +25542,15 @@
 
 static int __Pyx_CreateStringTabAndInitStrings(void) {
   __Pyx_StringTabEntry __pyx_string_tab[] = {
     {&__pyx_kp_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 0},
     {&__pyx_n_s_ASCII, __pyx_k_ASCII, sizeof(__pyx_k_ASCII), 0, 0, 1, 1},
     {&__pyx_kp_s_All_dimensions_preceding_dimensi, __pyx_k_All_dimensions_preceding_dimensi, sizeof(__pyx_k_All_dimensions_preceding_dimensi), 0, 0, 1, 0},
     {&__pyx_n_s_AssertionError, __pyx_k_AssertionError, sizeof(__pyx_k_AssertionError), 0, 0, 1, 1},
+    {&__pyx_n_s_B, __pyx_k_B, sizeof(__pyx_k_B), 0, 0, 1, 1},
     {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
     {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
     {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
     {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
     {&__pyx_kp_u_Cannot_index_with_type, __pyx_k_Cannot_index_with_type, sizeof(__pyx_k_Cannot_index_with_type), 0, 1, 0, 0},
     {&__pyx_kp_s_Cannot_transpose_memoryview_with, __pyx_k_Cannot_transpose_memoryview_with, sizeof(__pyx_k_Cannot_transpose_memoryview_with), 0, 0, 1, 0},
     {&__pyx_kp_s_Dimension_d_is_not_direct, __pyx_k_Dimension_d_is_not_direct, sizeof(__pyx_k_Dimension_d_is_not_direct), 0, 0, 1, 0},
@@ -23112,36 +25561,49 @@
     {&__pyx_kp_s_Index_out_of_bounds_axis_d, __pyx_k_Index_out_of_bounds_axis_d, sizeof(__pyx_k_Index_out_of_bounds_axis_d), 0, 0, 1, 0},
     {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
     {&__pyx_kp_u_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_shape_in_axis, __pyx_k_Invalid_shape_in_axis, sizeof(__pyx_k_Invalid_shape_in_axis), 0, 1, 0, 0},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
     {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
     {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
+    {&__pyx_n_s_N_query_list, __pyx_k_N_query_list, sizeof(__pyx_k_N_query_list), 0, 0, 1, 1},
     {&__pyx_n_s_N_ref, __pyx_k_N_ref, sizeof(__pyx_k_N_ref), 0, 0, 1, 1},
     {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
     {&__pyx_kp_u_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 1, 0, 0},
+    {&__pyx_n_s_P_N_dict, __pyx_k_P_N_dict, sizeof(__pyx_k_P_N_dict), 0, 0, 1, 1},
+    {&__pyx_n_s_P_base_calling_given_true_refseq, __pyx_k_P_base_calling_given_true_refseq, sizeof(__pyx_k_P_base_calling_given_true_refseq), 0, 0, 1, 1},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_Sequence, __pyx_k_Sequence, sizeof(__pyx_k_Sequence), 0, 0, 1, 1},
+    {&__pyx_n_s_SequenceBasecallQscorePDF, __pyx_k_SequenceBasecallQscorePDF, sizeof(__pyx_k_SequenceBasecallQscorePDF), 0, 0, 1, 1},
+    {&__pyx_n_s_SequenceBasecallQscorePDF___redu, __pyx_k_SequenceBasecallQscorePDF___redu, sizeof(__pyx_k_SequenceBasecallQscorePDF___redu), 0, 0, 1, 1},
+    {&__pyx_n_s_SequenceBasecallQscorePDF___sets, __pyx_k_SequenceBasecallQscorePDF___sets, sizeof(__pyx_k_SequenceBasecallQscorePDF___sets), 0, 0, 1, 1},
+    {&__pyx_n_s_SequenceBasecallQscorePDF_calc_c, __pyx_k_SequenceBasecallQscorePDF_calc_c, sizeof(__pyx_k_SequenceBasecallQscorePDF_calc_c), 0, 0, 1, 1},
     {&__pyx_kp_s_Step_may_not_be_zero_axis_d, __pyx_k_Step_may_not_be_zero_axis_d, sizeof(__pyx_k_Step_may_not_be_zero_axis_d), 0, 0, 1, 0},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-    {&__pyx_n_s__24, __pyx_k__24, sizeof(__pyx_k__24), 0, 0, 1, 1},
     {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
+    {&__pyx_n_s__30, __pyx_k__30, sizeof(__pyx_k__30), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_s_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 0, 1, 1},
     {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
     {&__pyx_kp_u_and, __pyx_k_and, sizeof(__pyx_k_and), 0, 1, 0, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
+    {&__pyx_n_s_base_idx, __pyx_k_base_idx, sizeof(__pyx_k_base_idx), 0, 0, 1, 1},
+    {&__pyx_n_s_bases, __pyx_k_bases, sizeof(__pyx_k_bases), 0, 0, 1, 1},
+    {&__pyx_n_s_bunbo_bunshi_sum, __pyx_k_bunbo_bunshi_sum, sizeof(__pyx_k_bunbo_bunshi_sum), 0, 0, 1, 1},
+    {&__pyx_n_s_bunshi_P_N, __pyx_k_bunshi_P_N, sizeof(__pyx_k_bunshi_P_N), 0, 0, 1, 1},
+    {&__pyx_n_s_bunshi_list, __pyx_k_bunshi_list, sizeof(__pyx_k_bunshi_list), 0, 0, 1, 1},
     {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
     {&__pyx_n_u_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 1, 0, 1},
+    {&__pyx_n_s_calc_consensus_error_rate, __pyx_k_calc_consensus_error_rate, sizeof(__pyx_k_calc_consensus_error_rate), 0, 0, 1, 1},
     {&__pyx_n_s_class, __pyx_k_class, sizeof(__pyx_k_class), 0, 0, 1, 1},
     {&__pyx_n_s_class_getitem, __pyx_k_class_getitem, sizeof(__pyx_k_class_getitem), 0, 0, 1, 1},
     {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
     {&__pyx_n_s_collections, __pyx_k_collections, sizeof(__pyx_k_collections), 0, 0, 1, 1},
     {&__pyx_kp_s_collections_abc, __pyx_k_collections_abc, sizeof(__pyx_k_collections_abc), 0, 0, 1, 0},
     {&__pyx_kp_s_contiguous_and_direct, __pyx_k_contiguous_and_direct, sizeof(__pyx_k_contiguous_and_direct), 0, 0, 1, 0},
     {&__pyx_kp_s_contiguous_and_indirect, __pyx_k_contiguous_and_indirect, sizeof(__pyx_k_contiguous_and_indirect), 0, 0, 1, 0},
@@ -23160,56 +25622,64 @@
     {&__pyx_n_s_gap_extend_penalty, __pyx_k_gap_extend_penalty, sizeof(__pyx_k_gap_extend_penalty), 0, 0, 1, 1},
     {&__pyx_n_s_gap_open_penalty, __pyx_k_gap_open_penalty, sizeof(__pyx_k_gap_open_penalty), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_kp_u_got, __pyx_k_got, sizeof(__pyx_k_got), 0, 1, 0, 0},
     {&__pyx_kp_u_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 1, 0, 0},
     {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
+    {&__pyx_n_s_idx, __pyx_k_idx, sizeof(__pyx_k_idx), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
+    {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
     {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
     {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
+    {&__pyx_n_s_iteritems, __pyx_k_iteritems, sizeof(__pyx_k_iteritems), 0, 0, 1, 1},
     {&__pyx_n_s_k_mer_offset_analysis_2, __pyx_k_k_mer_offset_analysis_2, sizeof(__pyx_k_k_mer_offset_analysis_2), 0, 0, 1, 1},
     {&__pyx_n_s_len_query_seq_v, __pyx_k_len_query_seq_v, sizeof(__pyx_k_len_query_seq_v), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_match_score, __pyx_k_match_score, sizeof(__pyx_k_match_score), 0, 0, 1, 1},
     {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
     {&__pyx_n_s_mismatch_score, __pyx_k_mismatch_score, sizeof(__pyx_k_mismatch_score), 0, 0, 1, 1},
     {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
     {&__pyx_n_s_my_special_dp_cython, __pyx_k_my_special_dp_cython, sizeof(__pyx_k_my_special_dp_cython), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
     {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
     {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
+    {&__pyx_n_s_p_list, __pyx_k_p_list, sizeof(__pyx_k_p_list), 0, 0, 1, 1},
     {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
+    {&__pyx_n_s_pdf_core, __pyx_k_pdf_core, sizeof(__pyx_k_pdf_core), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
+    {&__pyx_n_s_q_score_list, __pyx_k_q_score_list, sizeof(__pyx_k_q_score_list), 0, 0, 1, 1},
+    {&__pyx_n_s_query_list, __pyx_k_query_list, sizeof(__pyx_k_query_list), 0, 0, 1, 1},
     {&__pyx_n_s_query_seq_1, __pyx_k_query_seq_1, sizeof(__pyx_k_query_seq_1), 0, 0, 1, 1},
     {&__pyx_n_s_query_seq_2, __pyx_k_query_seq_2, sizeof(__pyx_k_query_seq_2), 0, 0, 1, 1},
     {&__pyx_n_s_query_seq_v, __pyx_k_query_seq_v, sizeof(__pyx_k_query_seq_v), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_ref_seq, __pyx_k_ref_seq, sizeof(__pyx_k_ref_seq), 0, 0, 1, 1},
     {&__pyx_n_s_ref_seq_v_repeated, __pyx_k_ref_seq_v_repeated, sizeof(__pyx_k_ref_seq_v_repeated), 0, 0, 1, 1},
     {&__pyx_n_s_register, __pyx_k_register, sizeof(__pyx_k_register), 0, 0, 1, 1},
     {&__pyx_kp_s_savemoney_modules_cython_functio, __pyx_k_savemoney_modules_cython_functio, sizeof(__pyx_k_savemoney_modules_cython_functio), 0, 0, 1, 0},
     {&__pyx_n_s_savemoney_modules_cython_functio_2, __pyx_k_savemoney_modules_cython_functio_2, sizeof(__pyx_k_savemoney_modules_cython_functio_2), 0, 0, 1, 1},
+    {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
     {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
     {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
     {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
     {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
@@ -23221,28 +25691,29 @@
     {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
     {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
     {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
     {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
+    {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
     {&__pyx_n_s_version_info, __pyx_k_version_info, sizeof(__pyx_k_version_info), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 57, __pyx_L1_error)
-  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 58, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_builtin_AssertionError = __Pyx_GetBuiltinName(__pyx_n_s_AssertionError); if (!__pyx_builtin_AssertionError) __PYX_ERR(0, 149, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 68, __pyx_L1_error)
   __pyx_builtin___import__ = __Pyx_GetBuiltinName(__pyx_n_s_import); if (!__pyx_builtin___import__) __PYX_ERR(1, 100, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 141, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(1, 159, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 408, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 618, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 914, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
@@ -23385,37 +25856,70 @@
  *     cdef object __pyx_result
  */
   __pyx_tuple__18 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
   __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(1, 1, __pyx_L1_error)
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":45
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":46
  * ctypedef long long LL   # unsigned
  * ctypedef vector[LL] vec
  * cpdef k_mer_offset_analysis_2(             # <<<<<<<<<<<<<<
  *         LL[:] ref_seq_v_repeated,
  *         LL[:] query_seq_v,
  */
-  __pyx_tuple__20 = PyTuple_Pack(4, __pyx_n_s_ref_seq_v_repeated, __pyx_n_s_query_seq_v, __pyx_n_s_N_ref, __pyx_n_s_len_query_seq_v); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_tuple__20 = PyTuple_Pack(4, __pyx_n_s_ref_seq_v_repeated, __pyx_n_s_query_seq_v, __pyx_n_s_N_ref, __pyx_n_s_len_query_seq_v); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_savemoney_modules_cython_functio, __pyx_n_s_k_mer_offset_analysis_2, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_savemoney_modules_cython_functio, __pyx_n_s_k_mer_offset_analysis_2, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 46, __pyx_L1_error)
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":66
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":92
+ *         self.N_bases = self.bases.size()
+ * 
+ *     def calc_consensus_error_rate(self, char_vec query_list, vec q_score_list, chr_LD_map P_N_dict):             # <<<<<<<<<<<<<<
+ *         cdef LL N_query_list
+ *         cdef LL base_idx
+ */
+  __pyx_tuple__22 = PyTuple_Pack(14, __pyx_n_s_self, __pyx_n_s_query_list, __pyx_n_s_q_score_list, __pyx_n_s_P_N_dict, __pyx_n_s_N_query_list, __pyx_n_s_base_idx, __pyx_n_s_idx, __pyx_n_s_bunshi_list, __pyx_n_s_bunshi_P_N, __pyx_n_s_bunbo_bunshi_sum, __pyx_n_s_base, __pyx_n_s_val, __pyx_n_s_p_list, __pyx_n_s_B); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 14, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_savemoney_modules_cython_functio, __pyx_n_s_calc_consensus_error_rate, 92, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 92, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+  __pyx_tuple__26 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 3, __pyx_L1_error)
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":134
+ *         return p_list
  * 
- * from libcpp.string cimport string
  * cpdef my_special_dp_cython(             # <<<<<<<<<<<<<<
  *         string query_seq_1,
  *         string query_seq_2,
  */
-  __pyx_tuple__22 = PyTuple_Pack(7, __pyx_n_s_query_seq_1, __pyx_n_s_query_seq_2, __pyx_n_s_ref_seq, __pyx_n_s_gap_open_penalty, __pyx_n_s_gap_extend_penalty, __pyx_n_s_match_score, __pyx_n_s_mismatch_score); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 66, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_savemoney_modules_cython_functio, __pyx_n_s_my_special_dp_cython, 66, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(7, __pyx_n_s_query_seq_1, __pyx_n_s_query_seq_2, __pyx_n_s_ref_seq, __pyx_n_s_gap_open_penalty, __pyx_n_s_gap_extend_penalty, __pyx_n_s_match_score, __pyx_n_s_mismatch_score); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_savemoney_modules_cython_functio, __pyx_n_s_my_special_dp_cython, 134, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -23489,14 +25993,37 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF_spec, NULL); if (unlikely(!__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF)) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF_spec, __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  #else
+  __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF = &__pyx_type_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  #endif
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF->tp_dictoffset && __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF->tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SequenceBasecallQscorePDF, (PyObject *) __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  #endif
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   #if CYTHON_USE_TYPE_SPECS
   __pyx_array_type = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type___pyx_array_spec, NULL); if (unlikely(!__pyx_array_type)) __PYX_ERR(1, 114, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_array_type->tp_as_buffer = &__pyx_tp_as_buffer_array;
   if (!__pyx_array_type->tp_as_buffer->bf_releasebuffer && __pyx_array_type->tp_base->tp_as_buffer && __pyx_array_type->tp_base->tp_as_buffer->bf_releasebuffer) {
@@ -24458,36 +26985,70 @@
  *     cdef object __pyx_result
  */
   __pyx_t_7 = PyCFunction_NewEx(&__pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum, NULL, __pyx_n_s_View_MemoryView); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Enum, __pyx_t_7) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":45
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":46
  * ctypedef long long LL   # unsigned
  * ctypedef vector[LL] vec
  * cpdef k_mer_offset_analysis_2(             # <<<<<<<<<<<<<<
  *         LL[:] ref_seq_v_repeated,
  *         LL[:] query_seq_v,
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_1k_mer_offset_analysis_2, 0, __pyx_n_s_k_mer_offset_analysis_2, NULL, __pyx_n_s_savemoney_modules_cython_functio_2, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_1k_mer_offset_analysis_2, 0, __pyx_n_s_k_mer_offset_analysis_2, NULL, __pyx_n_s_savemoney_modules_cython_functio_2, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_k_mer_offset_analysis_2, __pyx_t_7) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_k_mer_offset_analysis_2, __pyx_t_7) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "savemoney/modules/cython_functions/alignment_functions.pyx":66
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":92
+ *         self.N_bases = self.bases.size()
+ * 
+ *     def calc_consensus_error_rate(self, char_vec query_list, vec q_score_list, chr_LD_map P_N_dict):             # <<<<<<<<<<<<<<
+ *         cdef LL N_query_list
+ *         cdef LL base_idx
+ */
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_3calc_consensus_error_rate, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SequenceBasecallQscorePDF_calc_c, NULL, __pyx_n_s_savemoney_modules_cython_functio_2, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF, __pyx_n_s_calc_consensus_error_rate, __pyx_t_7) < 0) __PYX_ERR(0, 92, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  PyType_Modified(__pyx_ptype_9savemoney_7modules_16cython_functions_19alignment_functions_SequenceBasecallQscorePDF);
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_5__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SequenceBasecallQscorePDF___redu, NULL, __pyx_n_s_savemoney_modules_cython_functio_2, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_7) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_25SequenceBasecallQscorePDF_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_SequenceBasecallQscorePDF___sets, NULL, __pyx_n_s_savemoney_modules_cython_functio_2, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_7) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "savemoney/modules/cython_functions/alignment_functions.pyx":134
+ *         return p_list
  * 
- * from libcpp.string cimport string
  * cpdef my_special_dp_cython(             # <<<<<<<<<<<<<<
  *         string query_seq_1,
  *         string query_seq_2,
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_3my_special_dp_cython, 0, __pyx_n_s_my_special_dp_cython, NULL, __pyx_n_s_savemoney_modules_cython_functio_2, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 66, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_9savemoney_7modules_16cython_functions_19alignment_functions_3my_special_dp_cython, 0, __pyx_n_s_my_special_dp_cython, NULL, __pyx_n_s_savemoney_modules_cython_functio_2, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_my_special_dp_cython, __pyx_t_7) < 0) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_my_special_dp_cython, __pyx_t_7) < 0) __PYX_ERR(0, 134, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "savemoney/modules/cython_functions/alignment_functions.pyx":1
  * # distutils: language=c++             # <<<<<<<<<<<<<<
  * # distutils: extra_compile_args = ["-O3"]
  * # cython: language_level=3, boundscheck=False, wraparound=False, nonecheck=False
  */
@@ -24721,14 +27282,615 @@
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
+/* IterFinish */
+static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    if (unlikely(exc_type)) {
+        if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
+            return -1;
+        __Pyx_PyErr_Clear();
+        return 0;
+    }
+    return 0;
+}
+
+/* PyFunctionFastCall */
+#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
+static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
+                                               PyObject *globals) {
+    PyFrameObject *f;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject **fastlocals;
+    Py_ssize_t i;
+    PyObject *result;
+    assert(globals != NULL);
+    /* XXX Perhaps we should create a specialized
+       PyFrame_New() that doesn't take locals, but does
+       take builtins without sanity checking them.
+       */
+    assert(tstate != NULL);
+    f = PyFrame_New(tstate, co, globals, NULL);
+    if (f == NULL) {
+        return NULL;
+    }
+    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
+    for (i = 0; i < na; i++) {
+        Py_INCREF(*args);
+        fastlocals[i] = *args++;
+    }
+    result = PyEval_EvalFrameEx(f,0);
+    ++tstate->recursion_depth;
+    Py_DECREF(f);
+    --tstate->recursion_depth;
+    return result;
+}
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
+    PyObject *globals = PyFunction_GET_GLOBALS(func);
+    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
+    PyObject *closure;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kwdefs;
+#endif
+    PyObject *kwtuple, **k;
+    PyObject **d;
+    Py_ssize_t nd;
+    Py_ssize_t nk;
+    PyObject *result;
+    assert(kwargs == NULL || PyDict_Check(kwargs));
+    nk = kwargs ? PyDict_Size(kwargs) : 0;
+    #if PY_MAJOR_VERSION < 3
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
+        return NULL;
+    }
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
+        return NULL;
+    }
+    #endif
+    if (
+#if PY_MAJOR_VERSION >= 3
+            co->co_kwonlyargcount == 0 &&
+#endif
+            likely(kwargs == NULL || nk == 0) &&
+            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
+        if (argdefs == NULL && co->co_argcount == nargs) {
+            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
+            goto done;
+        }
+        else if (nargs == 0 && argdefs != NULL
+                 && co->co_argcount == Py_SIZE(argdefs)) {
+            /* function called with no arguments, but all parameters have
+               a default value: use default values as arguments .*/
+            args = &PyTuple_GET_ITEM(argdefs, 0);
+            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
+            goto done;
+        }
+    }
+    if (kwargs != NULL) {
+        Py_ssize_t pos, i;
+        kwtuple = PyTuple_New(2 * nk);
+        if (kwtuple == NULL) {
+            result = NULL;
+            goto done;
+        }
+        k = &PyTuple_GET_ITEM(kwtuple, 0);
+        pos = i = 0;
+        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
+            Py_INCREF(k[i]);
+            Py_INCREF(k[i+1]);
+            i += 2;
+        }
+        nk = i / 2;
+    }
+    else {
+        kwtuple = NULL;
+        k = NULL;
+    }
+    closure = PyFunction_GET_CLOSURE(func);
+#if PY_MAJOR_VERSION >= 3
+    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
+#endif
+    if (argdefs != NULL) {
+        d = &PyTuple_GET_ITEM(argdefs, 0);
+        nd = Py_SIZE(argdefs);
+    }
+    else {
+        d = NULL;
+        nd = 0;
+    }
+#if PY_MAJOR_VERSION >= 3
+    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, kwdefs, closure);
+#else
+    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, closure);
+#endif
+    Py_XDECREF(kwtuple);
+done:
+    Py_LeaveRecursiveCall();
+    return result;
+}
+#endif
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    #if PY_MAJOR_VERSION < 3
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* PyObjectCallMethO */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
+    PyObject *self, *result;
+    PyCFunction cfunc;
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
+    #if PY_MAJOR_VERSION < 3
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    #else
+    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
+        return NULL;
+    #endif
+    result = cfunc(self, arg);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* PyObjectFastCall */
+#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
+static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
+    PyObject *result = 0;
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+  bad:
+    Py_DECREF(argstuple);
+    return result;
+}
+#endif
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
+    }
+#endif
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
+    }
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if PY_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
+    }
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
+}
+
+/* PyObjectCallNoArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectCallOneArg */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectGetMethod */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
+#else
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
+#endif
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
+#else
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
+#endif
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
+#else
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
+#endif
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
+    }
+#endif
+    *method = attr;
+    return 0;
+}
+
+/* PyObjectCallMethod0 */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
+}
+
+/* RaiseNeedMoreValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
+    PyErr_Format(PyExc_ValueError,
+                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
+                 index, (index == 1) ? "" : "s");
+}
+
+/* RaiseTooManyValuesToUnpack */
+static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
+    PyErr_Format(PyExc_ValueError,
+                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
+}
+
+/* UnpackItemEndCheck */
+static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
+    if (unlikely(retval)) {
+        Py_DECREF(retval);
+        __Pyx_RaiseTooManyValuesError(expected);
+        return -1;
+    }
+    return __Pyx_IterFinish();
+}
+
+/* RaiseNoneIterError */
+static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
+}
+
+/* UnpackTupleError */
+static void __Pyx_UnpackTupleError(PyObject *t, Py_ssize_t index) {
+    if (t == Py_None) {
+      __Pyx_RaiseNoneNotIterableError();
+    } else if (PyTuple_GET_SIZE(t) < index) {
+      __Pyx_RaiseNeedMoreValuesError(PyTuple_GET_SIZE(t));
+    } else {
+      __Pyx_RaiseTooManyValuesError(index);
+    }
+}
+
+/* UnpackTuple2 */
+static CYTHON_INLINE int __Pyx_unpack_tuple2_exact(
+        PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2, int decref_tuple) {
+    PyObject *value1 = NULL, *value2 = NULL;
+#if CYTHON_COMPILING_IN_PYPY
+    value1 = PySequence_ITEM(tuple, 0);  if (unlikely(!value1)) goto bad;
+    value2 = PySequence_ITEM(tuple, 1);  if (unlikely(!value2)) goto bad;
+#else
+    value1 = PyTuple_GET_ITEM(tuple, 0);  Py_INCREF(value1);
+    value2 = PyTuple_GET_ITEM(tuple, 1);  Py_INCREF(value2);
+#endif
+    if (decref_tuple) {
+        Py_DECREF(tuple);
+    }
+    *pvalue1 = value1;
+    *pvalue2 = value2;
+    return 0;
+#if CYTHON_COMPILING_IN_PYPY
+bad:
+    Py_XDECREF(value1);
+    Py_XDECREF(value2);
+    if (decref_tuple) { Py_XDECREF(tuple); }
+    return -1;
+#endif
+}
+static int __Pyx_unpack_tuple2_generic(PyObject* tuple, PyObject** pvalue1, PyObject** pvalue2,
+                                       int has_known_size, int decref_tuple) {
+    Py_ssize_t index;
+    PyObject *value1 = NULL, *value2 = NULL, *iter = NULL;
+    iternextfunc iternext;
+    iter = PyObject_GetIter(tuple);
+    if (unlikely(!iter)) goto bad;
+    if (decref_tuple) { Py_DECREF(tuple); tuple = NULL; }
+    iternext = __Pyx_PyObject_GetIterNextFunc(iter);
+    value1 = iternext(iter); if (unlikely(!value1)) { index = 0; goto unpacking_failed; }
+    value2 = iternext(iter); if (unlikely(!value2)) { index = 1; goto unpacking_failed; }
+    if (!has_known_size && unlikely(__Pyx_IternextUnpackEndCheck(iternext(iter), 2))) goto bad;
+    Py_DECREF(iter);
+    *pvalue1 = value1;
+    *pvalue2 = value2;
+    return 0;
+unpacking_failed:
+    if (!has_known_size && __Pyx_IterFinish() == 0)
+        __Pyx_RaiseNeedMoreValuesError(index);
+bad:
+    Py_XDECREF(iter);
+    Py_XDECREF(value1);
+    Py_XDECREF(value2);
+    if (decref_tuple) { Py_XDECREF(tuple); }
+    return -1;
+}
+
+/* dict_iter */
+#if CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
+#include <string.h>
+#endif
+static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* iterable, int is_dict, PyObject* method_name,
+                                                   Py_ssize_t* p_orig_length, int* p_source_is_dict) {
+    is_dict = is_dict || likely(PyDict_CheckExact(iterable));
+    *p_source_is_dict = is_dict;
+    if (is_dict) {
+#if !CYTHON_COMPILING_IN_PYPY
+        *p_orig_length = PyDict_Size(iterable);
+        Py_INCREF(iterable);
+        return iterable;
+#elif PY_MAJOR_VERSION >= 3
+        static PyObject *py_items = NULL, *py_keys = NULL, *py_values = NULL;
+        PyObject **pp = NULL;
+        if (method_name) {
+            const char *name = PyUnicode_AsUTF8(method_name);
+            if (strcmp(name, "iteritems") == 0) pp = &py_items;
+            else if (strcmp(name, "iterkeys") == 0) pp = &py_keys;
+            else if (strcmp(name, "itervalues") == 0) pp = &py_values;
+            if (pp) {
+                if (!*pp) {
+                    *pp = PyUnicode_FromString(name + 4);
+                    if (!*pp)
+                        return NULL;
+                }
+                method_name = *pp;
+            }
+        }
+#endif
+    }
+    *p_orig_length = 0;
+    if (method_name) {
+        PyObject* iter;
+        iterable = __Pyx_PyObject_CallMethod0(iterable, method_name);
+        if (!iterable)
+            return NULL;
+#if !CYTHON_COMPILING_IN_PYPY
+        if (PyTuple_CheckExact(iterable) || PyList_CheckExact(iterable))
+            return iterable;
+#endif
+        iter = PyObject_GetIter(iterable);
+        Py_DECREF(iterable);
+        return iter;
+    }
+    return PyObject_GetIter(iterable);
+}
+static CYTHON_INLINE int __Pyx_dict_iter_next(
+        PyObject* iter_obj, CYTHON_NCP_UNUSED Py_ssize_t orig_length, CYTHON_NCP_UNUSED Py_ssize_t* ppos,
+        PyObject** pkey, PyObject** pvalue, PyObject** pitem, int source_is_dict) {
+    PyObject* next_item;
+#if !CYTHON_COMPILING_IN_PYPY
+    if (source_is_dict) {
+        PyObject *key, *value;
+        if (unlikely(orig_length != PyDict_Size(iter_obj))) {
+            PyErr_SetString(PyExc_RuntimeError, "dictionary changed size during iteration");
+            return -1;
+        }
+        if (unlikely(!PyDict_Next(iter_obj, ppos, &key, &value))) {
+            return 0;
+        }
+        if (pitem) {
+            PyObject* tuple = PyTuple_New(2);
+            if (unlikely(!tuple)) {
+                return -1;
+            }
+            Py_INCREF(key);
+            Py_INCREF(value);
+            PyTuple_SET_ITEM(tuple, 0, key);
+            PyTuple_SET_ITEM(tuple, 1, value);
+            *pitem = tuple;
+        } else {
+            if (pkey) {
+                Py_INCREF(key);
+                *pkey = key;
+            }
+            if (pvalue) {
+                Py_INCREF(value);
+                *pvalue = value;
+            }
+        }
+        return 1;
+    } else if (PyTuple_CheckExact(iter_obj)) {
+        Py_ssize_t pos = *ppos;
+        if (unlikely(pos >= PyTuple_GET_SIZE(iter_obj))) return 0;
+        *ppos = pos + 1;
+        next_item = PyTuple_GET_ITEM(iter_obj, pos);
+        Py_INCREF(next_item);
+    } else if (PyList_CheckExact(iter_obj)) {
+        Py_ssize_t pos = *ppos;
+        if (unlikely(pos >= PyList_GET_SIZE(iter_obj))) return 0;
+        *ppos = pos + 1;
+        next_item = PyList_GET_ITEM(iter_obj, pos);
+        Py_INCREF(next_item);
+    } else
+#endif
+    {
+        next_item = PyIter_Next(iter_obj);
+        if (unlikely(!next_item)) {
+            return __Pyx_IterFinish();
+        }
+    }
+    if (pitem) {
+        *pitem = next_item;
+    } else if (pkey && pvalue) {
+        if (__Pyx_unpack_tuple2(next_item, pkey, pvalue, source_is_dict, source_is_dict, 1))
+            return -1;
+    } else if (pkey) {
+        *pkey = next_item;
+    } else {
+        *pvalue = next_item;
+    }
+    return 1;
+}
+
 /* TupleAndListFromArray */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
     PyObject *v;
     Py_ssize_t i;
     for (i = 0; i < length; i++) {
         v = dest[i] = src[i];
@@ -24920,19 +28082,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;
+            if (unlikely(eq < 0)) return NULL;  // error
             return kwvalues[i];
         }
     }
-    return NULL;
+    return NULL;  // not found (no exception set)
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -25037,15 +28199,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value);
+            Py_INCREF(value); // transfer ownership of value to values
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -25056,15 +28218,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;
+                    value = NULL;  // ownership transferred to values
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -25088,15 +28250,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;
+                    value = NULL; // ownership transferred to values
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -25330,265 +28492,14 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
-static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
-                                               PyObject *globals) {
-    PyFrameObject *f;
-    PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject **fastlocals;
-    Py_ssize_t i;
-    PyObject *result;
-    assert(globals != NULL);
-    /* XXX Perhaps we should create a specialized
-       PyFrame_New() that doesn't take locals, but does
-       take builtins without sanity checking them.
-       */
-    assert(tstate != NULL);
-    f = PyFrame_New(tstate, co, globals, NULL);
-    if (f == NULL) {
-        return NULL;
-    }
-    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
-    for (i = 0; i < na; i++) {
-        Py_INCREF(*args);
-        fastlocals[i] = *args++;
-    }
-    result = PyEval_EvalFrameEx(f,0);
-    ++tstate->recursion_depth;
-    Py_DECREF(f);
-    --tstate->recursion_depth;
-    return result;
-}
-static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
-    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
-    PyObject *globals = PyFunction_GET_GLOBALS(func);
-    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
-    PyObject *closure;
-#if PY_MAJOR_VERSION >= 3
-    PyObject *kwdefs;
-#endif
-    PyObject *kwtuple, **k;
-    PyObject **d;
-    Py_ssize_t nd;
-    Py_ssize_t nk;
-    PyObject *result;
-    assert(kwargs == NULL || PyDict_Check(kwargs));
-    nk = kwargs ? PyDict_Size(kwargs) : 0;
-    #if PY_MAJOR_VERSION < 3
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
-        return NULL;
-    }
-    #else
-    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object"))) {
-        return NULL;
-    }
-    #endif
-    if (
-#if PY_MAJOR_VERSION >= 3
-            co->co_kwonlyargcount == 0 &&
-#endif
-            likely(kwargs == NULL || nk == 0) &&
-            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
-        if (argdefs == NULL && co->co_argcount == nargs) {
-            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
-            goto done;
-        }
-        else if (nargs == 0 && argdefs != NULL
-                 && co->co_argcount == Py_SIZE(argdefs)) {
-            /* function called with no arguments, but all parameters have
-               a default value: use default values as arguments .*/
-            args = &PyTuple_GET_ITEM(argdefs, 0);
-            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
-            goto done;
-        }
-    }
-    if (kwargs != NULL) {
-        Py_ssize_t pos, i;
-        kwtuple = PyTuple_New(2 * nk);
-        if (kwtuple == NULL) {
-            result = NULL;
-            goto done;
-        }
-        k = &PyTuple_GET_ITEM(kwtuple, 0);
-        pos = i = 0;
-        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
-            Py_INCREF(k[i]);
-            Py_INCREF(k[i+1]);
-            i += 2;
-        }
-        nk = i / 2;
-    }
-    else {
-        kwtuple = NULL;
-        k = NULL;
-    }
-    closure = PyFunction_GET_CLOSURE(func);
-#if PY_MAJOR_VERSION >= 3
-    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
-#endif
-    if (argdefs != NULL) {
-        d = &PyTuple_GET_ITEM(argdefs, 0);
-        nd = Py_SIZE(argdefs);
-    }
-    else {
-        d = NULL;
-        nd = 0;
-    }
-#if PY_MAJOR_VERSION >= 3
-    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, kwdefs, closure);
-#else
-    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
-                               args, (int)nargs,
-                               k, (int)nk,
-                               d, (int)nd, closure);
-#endif
-    Py_XDECREF(kwtuple);
-done:
-    Py_LeaveRecursiveCall();
-    return result;
-}
-#endif
-
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    #if PY_MAJOR_VERSION < 3
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    #else
-    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
-        return NULL;
-    #endif
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectCallMethO */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
-    PyObject *self, *result;
-    PyCFunction cfunc;
-    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
-    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
-    #if PY_MAJOR_VERSION < 3
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    #else
-    if (unlikely(Py_EnterRecursiveCall(" while calling a Python object")))
-        return NULL;
-    #endif
-    result = cfunc(self, arg);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
-/* PyObjectFastCall */
-#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
-static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
-    PyObject *argstuple;
-    PyObject *result = 0;
-    size_t i;
-    argstuple = PyTuple_New((Py_ssize_t)nargs);
-    if (unlikely(!argstuple)) return NULL;
-    for (i = 0; i < nargs; i++) {
-        Py_INCREF(args[i]);
-        if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
-    }
-    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
-  bad:
-    Py_DECREF(argstuple);
-    return result;
-}
-#endif
-static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
-    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
-#if CYTHON_COMPILING_IN_CPYTHON
-    if (nargs == 0 && kwargs == NULL) {
-        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
-            return __Pyx_PyObject_CallMethO(func, NULL);
-    }
-    else if (nargs == 1 && kwargs == NULL) {
-        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
-            return __Pyx_PyObject_CallMethO(func, args[0]);
-    }
-#endif
-    #if PY_VERSION_HEX < 0x030800B1
-    #if CYTHON_FAST_PYCCALL
-    if (PyCFunction_Check(func)) {
-        if (kwargs) {
-            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
-        } else {
-            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
-        }
-    }
-    #if PY_VERSION_HEX >= 0x030700A1
-    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
-        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
-    }
-    #endif
-    #endif
-    #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
-    }
-    #endif
-    #endif
-    if (kwargs == NULL) {
-        #if CYTHON_VECTORCALL
-        #if PY_VERSION_HEX < 0x03090000
-        vectorcallfunc f = _PyVectorcall_Function(func);
-        #else
-        vectorcallfunc f = PyVectorcall_Function(func);
-        #endif
-        if (f) {
-            return f(func, args, (size_t)nargs, NULL);
-        }
-        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-        if (__Pyx_CyFunction_CheckExact(func)) {
-            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-            if (f) return f(func, args, (size_t)nargs, NULL);
-        }
-        #endif
-    }
-    if (nargs == 0) {
-        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
-    }
-    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
-    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
-    #else
-    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
-    #endif
-}
-
 /* RaiseUnexpectedTypeError */
 static int
 __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
 {
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
                  expected, obj_type_name);
@@ -26017,20 +28928,14 @@
     if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
-/* PyObjectCallOneArg */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *args[2] = {NULL, arg};
-    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject *index) {
     PyObject *runerr = NULL;
     Py_ssize_t key_value;
     key_value = __Pyx_PyIndex_AsSsize_t(index);
     if (likely(key_value != -1 || !(runerr = PyErr_Occurred()))) {
@@ -26256,32 +29161,14 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* RaiseTooManyValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected) {
-    PyErr_Format(PyExc_ValueError,
-                 "too many values to unpack (expected %" CYTHON_FORMAT_SSIZE_T "d)", expected);
-}
-
-/* RaiseNeedMoreValuesToUnpack */
-static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index) {
-    PyErr_Format(PyExc_ValueError,
-                 "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
-                 index, (index == 1) ? "" : "s");
-}
-
-/* RaiseNoneIterError */
-static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-}
-
 /* ExtTypeTest */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
     __Pyx_TypeName obj_type_name;
     __Pyx_TypeName type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
@@ -27103,137 +29990,14 @@
             PyType_Modified(type);
     }
 #endif
     return 0;
 }
 #endif
 
-/* PyObjectCallNoArg */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg[2] = {NULL, NULL};
-    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    __Pyx_TypeName type_name;
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
-        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
-#elif PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (likely(descr != NULL)) {
-        *method = descr;
-        return 0;
-    }
-    type_name = __Pyx_PyType_GetName(tp);
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
-                 type_name, name);
-#else
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
-                 type_name, PyString_AS_STRING(name));
-#endif
-    __Pyx_DECREF_TypeName(type_name);
-    return 0;
-#else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
-#endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
-#endif
-    *method = attr;
-    return 0;
-}
-
-/* PyObjectCallMethod0 */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
-    PyObject *method = NULL, *result = NULL;
-    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
-    if (likely(is_method)) {
-        result = __Pyx_PyObject_CallOneArg(method, obj);
-        Py_DECREF(method);
-        return result;
-    }
-    if (unlikely(!method)) goto bad;
-    result = __Pyx_PyObject_CallNoArg(method);
-    Py_DECREF(method);
-bad:
-    return result;
-}
-
 /* ValidateBasesTuple */
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
 static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
     Py_ssize_t i, n;
 #if CYTHON_ASSUME_SAFE_MACROS
     n = PyTuple_GET_SIZE(bases);
 #else
@@ -27393,105 +30157,14 @@
     #endif
     }
 #endif
     return r;
 #endif
 }
 
-/* SetVTable */
-static int __Pyx_SetVtable(PyTypeObject *type, void *vtable) {
-    PyObject *ob = PyCapsule_New(vtable, 0, 0);
-    if (unlikely(!ob))
-        goto bad;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    if (unlikely(PyObject_SetAttr((PyObject *) type, __pyx_n_s_pyx_vtable, ob) < 0))
-#else
-    if (unlikely(PyDict_SetItem(type->tp_dict, __pyx_n_s_pyx_vtable, ob) < 0))
-#endif
-        goto bad;
-    Py_DECREF(ob);
-    return 0;
-bad:
-    Py_XDECREF(ob);
-    return -1;
-}
-
-/* GetVTable */
-static void* __Pyx_GetVtable(PyTypeObject *type) {
-    void* ptr;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    PyObject *ob = PyObject_GetAttr((PyObject *)type, __pyx_n_s_pyx_vtable);
-#else
-    PyObject *ob = PyObject_GetItem(type->tp_dict, __pyx_n_s_pyx_vtable);
-#endif
-    if (!ob)
-        goto bad;
-    ptr = PyCapsule_GetPointer(ob, 0);
-    if (!ptr && !PyErr_Occurred())
-        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
-    Py_DECREF(ob);
-    return ptr;
-bad:
-    Py_XDECREF(ob);
-    return NULL;
-}
-
-/* MergeVTables */
-#if !CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_MergeVtables(PyTypeObject *type) {
-    int i;
-    void** base_vtables;
-    __Pyx_TypeName tp_base_name;
-    __Pyx_TypeName base_name;
-    void* unknown = (void*)-1;
-    PyObject* bases = type->tp_bases;
-    int base_depth = 0;
-    {
-        PyTypeObject* base = type->tp_base;
-        while (base) {
-            base_depth += 1;
-            base = base->tp_base;
-        }
-    }
-    base_vtables = (void**) malloc(sizeof(void*) * (size_t)(base_depth + 1));
-    base_vtables[0] = unknown;
-    for (i = 1; i < PyTuple_GET_SIZE(bases); i++) {
-        void* base_vtable = __Pyx_GetVtable(((PyTypeObject*)PyTuple_GET_ITEM(bases, i)));
-        if (base_vtable != NULL) {
-            int j;
-            PyTypeObject* base = type->tp_base;
-            for (j = 0; j < base_depth; j++) {
-                if (base_vtables[j] == unknown) {
-                    base_vtables[j] = __Pyx_GetVtable(base);
-                    base_vtables[j + 1] = unknown;
-                }
-                if (base_vtables[j] == base_vtable) {
-                    break;
-                } else if (base_vtables[j] == NULL) {
-                    goto bad;
-                }
-                base = base->tp_base;
-            }
-        }
-    }
-    PyErr_Clear();
-    free(base_vtables);
-    return 0;
-bad:
-    tp_base_name = __Pyx_PyType_GetName(type->tp_base);
-    base_name = __Pyx_PyType_GetName((PyTypeObject*)PyTuple_GET_ITEM(bases, i));
-    PyErr_Format(PyExc_TypeError,
-        "multiple bases have vtable conflict: '" __Pyx_FMT_TYPENAME "' and '" __Pyx_FMT_TYPENAME "'", tp_base_name, base_name);
-    __Pyx_DECREF_TypeName(tp_base_name);
-    __Pyx_DECREF_TypeName(base_name);
-    free(base_vtables);
-    return -1;
-}
-#endif
-
 /* SetupReduce */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
   name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
@@ -27595,14 +30268,105 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
+/* SetVTable */
+static int __Pyx_SetVtable(PyTypeObject *type, void *vtable) {
+    PyObject *ob = PyCapsule_New(vtable, 0, 0);
+    if (unlikely(!ob))
+        goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(PyObject_SetAttr((PyObject *) type, __pyx_n_s_pyx_vtable, ob) < 0))
+#else
+    if (unlikely(PyDict_SetItem(type->tp_dict, __pyx_n_s_pyx_vtable, ob) < 0))
+#endif
+        goto bad;
+    Py_DECREF(ob);
+    return 0;
+bad:
+    Py_XDECREF(ob);
+    return -1;
+}
+
+/* GetVTable */
+static void* __Pyx_GetVtable(PyTypeObject *type) {
+    void* ptr;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *ob = PyObject_GetAttr((PyObject *)type, __pyx_n_s_pyx_vtable);
+#else
+    PyObject *ob = PyObject_GetItem(type->tp_dict, __pyx_n_s_pyx_vtable);
+#endif
+    if (!ob)
+        goto bad;
+    ptr = PyCapsule_GetPointer(ob, 0);
+    if (!ptr && !PyErr_Occurred())
+        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
+    Py_DECREF(ob);
+    return ptr;
+bad:
+    Py_XDECREF(ob);
+    return NULL;
+}
+
+/* MergeVTables */
+#if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_MergeVtables(PyTypeObject *type) {
+    int i;
+    void** base_vtables;
+    __Pyx_TypeName tp_base_name;
+    __Pyx_TypeName base_name;
+    void* unknown = (void*)-1;
+    PyObject* bases = type->tp_bases;
+    int base_depth = 0;
+    {
+        PyTypeObject* base = type->tp_base;
+        while (base) {
+            base_depth += 1;
+            base = base->tp_base;
+        }
+    }
+    base_vtables = (void**) malloc(sizeof(void*) * (size_t)(base_depth + 1));
+    base_vtables[0] = unknown;
+    for (i = 1; i < PyTuple_GET_SIZE(bases); i++) {
+        void* base_vtable = __Pyx_GetVtable(((PyTypeObject*)PyTuple_GET_ITEM(bases, i)));
+        if (base_vtable != NULL) {
+            int j;
+            PyTypeObject* base = type->tp_base;
+            for (j = 0; j < base_depth; j++) {
+                if (base_vtables[j] == unknown) {
+                    base_vtables[j] = __Pyx_GetVtable(base);
+                    base_vtables[j + 1] = unknown;
+                }
+                if (base_vtables[j] == base_vtable) {
+                    break;
+                } else if (base_vtables[j] == NULL) {
+                    goto bad;
+                }
+                base = base->tp_base;
+            }
+        }
+    }
+    PyErr_Clear();
+    free(base_vtables);
+    return 0;
+bad:
+    tp_base_name = __Pyx_PyType_GetName(type->tp_base);
+    base_name = __Pyx_PyType_GetName((PyTypeObject*)PyTuple_GET_ITEM(bases, i));
+    PyErr_Format(PyExc_TypeError,
+        "multiple bases have vtable conflict: '" __Pyx_FMT_TYPENAME "' and '" __Pyx_FMT_TYPENAME "'", tp_base_name, base_name);
+    __Pyx_DECREF_TypeName(tp_base_name);
+    __Pyx_DECREF_TypeName(base_name);
+    free(base_vtables);
+    return -1;
+}
+#endif
+
 /* FetchSharedCythonModule */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
     return __Pyx_PyImport_AddModuleRef((char*) __PYX_ABI_MODULE_NAME);
 }
 
 /* FetchCommonType */
 static int __Pyx_VerifyCachedType(PyObject *cached_type,
@@ -29040,15 +31804,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
@@ -30438,14 +33202,287 @@
     return (PY_LONG_LONG) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to PY_LONG_LONG");
     return (PY_LONG_LONG) -1;
 }
 
+/* CIntFromPy */
+  static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const char neg_one = (char) -1, const_zero = (char) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+#if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_Check(x))) {
+        if ((sizeof(char) < sizeof(long))) {
+            __PYX_VERIFY_RETURN_INT(char, long, PyInt_AS_LONG(x))
+        } else {
+            long val = PyInt_AS_LONG(x);
+            if (is_unsigned && unlikely(val < 0)) {
+                goto raise_neg_overflow;
+            }
+            return (char) val;
+        }
+    } else
+#endif
+    if (likely(PyLong_Check(x))) {
+        if (is_unsigned) {
+#if CYTHON_USE_PYLONG_INTERNALS
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(char, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(char) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) >= 2 * PyLong_SHIFT)) {
+                                return (char) (((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+                            }
+                        }
+                        break;
+                    case 3:
+                        if ((8 * sizeof(char) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) >= 3 * PyLong_SHIFT)) {
+                                return (char) (((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+                            }
+                        }
+                        break;
+                    case 4:
+                        if ((8 * sizeof(char) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) >= 4 * PyLong_SHIFT)) {
+                                return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
+                            }
+                        }
+                        break;
+                }
+            }
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+            if (unlikely(Py_SIZE(x) < 0)) {
+                goto raise_neg_overflow;
+            }
+#else
+            {
+                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                if (unlikely(result < 0))
+                    return (char) -1;
+                if (unlikely(result == 1))
+                    goto raise_neg_overflow;
+            }
+#endif
+            if ((sizeof(char) <= sizeof(unsigned long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(char, unsigned long, PyLong_AsUnsignedLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(char) <= sizeof(unsigned PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(char, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+#endif
+            }
+        } else {
+#if CYTHON_USE_PYLONG_INTERNALS
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(char, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(char) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
+                                return (char) (((char)-1)*(((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
+                        }
+                        break;
+                    case 2:
+                        if ((8 * sizeof(char) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
+                                return (char) ((((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
+                        }
+                        break;
+                    case -3:
+                        if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
+                                return (char) (((char)-1)*(((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
+                        }
+                        break;
+                    case 3:
+                        if ((8 * sizeof(char) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
+                                return (char) ((((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
+                        }
+                        break;
+                    case -4:
+                        if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 4 * PyLong_SHIFT)) {
+                                return (char) (((char)-1)*(((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
+                        }
+                        break;
+                    case 4:
+                        if ((8 * sizeof(char) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(char) - 1 > 4 * PyLong_SHIFT)) {
+                                return (char) ((((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
+                            }
+                        }
+                        break;
+                }
+            }
+#endif
+            if ((sizeof(char) <= sizeof(long))) {
+                __PYX_VERIFY_RETURN_INT_EXC(char, long, PyLong_AsLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if ((sizeof(char) <= sizeof(PY_LONG_LONG))) {
+                __PYX_VERIFY_RETURN_INT_EXC(char, PY_LONG_LONG, PyLong_AsLongLong(x))
+#endif
+            }
+        }
+        {
+            char val;
+            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
+#if PY_MAJOR_VERSION < 3
+            if (likely(v) && !PyLong_Check(v)) {
+                PyObject *tmp = v;
+                v = PyNumber_Long(tmp);
+                Py_DECREF(tmp);
+            }
+#endif
+            if (likely(v)) {
+                int ret = -1;
+#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
+                int one = 1; int is_little = (int)*(unsigned char *)&one;
+                unsigned char *bytes = (unsigned char *)&val;
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (char) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (char) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (char) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (char) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (char) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(char) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((char) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(char) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((char) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((char) 1) << (sizeof(char) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
+                Py_DECREF(v);
+                if (likely(!ret))
+                    return val;
+            }
+            return (char) -1;
+        }
+    } else {
+        char val;
+        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
+        if (!tmp) return (char) -1;
+        val = __Pyx_PyInt_As_char(tmp);
+        Py_DECREF(tmp);
+        return val;
+    }
+raise_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "value too large to convert to char");
+    return (char) -1;
+raise_neg_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "can't convert negative value to char");
+    return (char) -1;
+}
+
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const PY_LONG_LONG neg_one = (PY_LONG_LONG) -1, const_zero = (PY_LONG_LONG) 0;
@@ -31449,298 +34486,25 @@
         Py_XDECREF(py_bytes);
         Py_XDECREF(from_bytes);
         return result;
 #endif
     }
 }
 
-/* CIntFromPy */
-  static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const char neg_one = (char) -1, const_zero = (char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if ((sizeof(char) < sizeof(long))) {
-            __PYX_VERIFY_RETURN_INT(char, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (char) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
-                goto raise_neg_overflow;
-            } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(char, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
-            } else {
-                const digit* digits = __Pyx_PyLong_Digits(x);
-                assert(__Pyx_PyLong_DigitCount(x) > 1);
-                switch (__Pyx_PyLong_DigitCount(x)) {
-                    case 2:
-                        if ((8 * sizeof(char) > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) >= 2 * PyLong_SHIFT)) {
-                                return (char) (((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
-                            }
-                        }
-                        break;
-                    case 3:
-                        if ((8 * sizeof(char) > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) >= 3 * PyLong_SHIFT)) {
-                                return (char) (((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
-                            }
-                        }
-                        break;
-                    case 4:
-                        if ((8 * sizeof(char) > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) >= 4 * PyLong_SHIFT)) {
-                                return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
-                            }
-                        }
-                        break;
-                }
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (char) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if ((sizeof(char) <= sizeof(unsigned long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(char, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if ((sizeof(char) <= sizeof(unsigned PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(char, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(char, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
-            } else {
-                const digit* digits = __Pyx_PyLong_Digits(x);
-                assert(__Pyx_PyLong_DigitCount(x) > 1);
-                switch (__Pyx_PyLong_SignedDigitCount(x)) {
-                    case -2:
-                        if ((8 * sizeof(char) - 1 > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
-                                return (char) (((char)-1)*(((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                            }
-                        }
-                        break;
-                    case 2:
-                        if ((8 * sizeof(char) > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
-                                return (char) ((((((char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                            }
-                        }
-                        break;
-                    case -3:
-                        if ((8 * sizeof(char) - 1 > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
-                                return (char) (((char)-1)*(((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                            }
-                        }
-                        break;
-                    case 3:
-                        if ((8 * sizeof(char) > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
-                                return (char) ((((((((char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                            }
-                        }
-                        break;
-                    case -4:
-                        if ((8 * sizeof(char) - 1 > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) - 1 > 4 * PyLong_SHIFT)) {
-                                return (char) (((char)-1)*(((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                            }
-                        }
-                        break;
-                    case 4:
-                        if ((8 * sizeof(char) > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(char, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(char) - 1 > 4 * PyLong_SHIFT)) {
-                                return (char) ((((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0])));
-                            }
-                        }
-                        break;
-                }
-            }
-#endif
-            if ((sizeof(char) <= sizeof(long))) {
-                __PYX_VERIFY_RETURN_INT_EXC(char, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if ((sizeof(char) <= sizeof(PY_LONG_LONG))) {
-                __PYX_VERIFY_RETURN_INT_EXC(char, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-            char val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
-#if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
-#endif
-            if (likely(v)) {
-                int ret = -1;
-#if PY_VERSION_HEX < 0x030d0000 && !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                           bytes, sizeof(val),
-                                           is_little, !is_unsigned);
-#else
-                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
-                int bits, remaining_bits, is_negative = 0;
-                long idigit;
-                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
-                if (unlikely(!PyLong_CheckExact(v))) {
-                    PyObject *tmp = v;
-                    v = PyNumber_Long(v);
-                    assert(PyLong_CheckExact(v));
-                    Py_DECREF(tmp);
-                    if (unlikely(!v)) return (char) -1;
-                }
-#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-                if (Py_SIZE(x) == 0)
-                    return (char) 0;
-                is_negative = Py_SIZE(x) < 0;
-#else
-                {
-                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                    if (unlikely(result < 0))
-                        return (char) -1;
-                    is_negative = result == 1;
-                }
-#endif
-                if (is_unsigned && unlikely(is_negative)) {
-                    goto raise_neg_overflow;
-                } else if (is_negative) {
-                    stepval = PyNumber_Invert(v);
-                    if (unlikely(!stepval))
-                        return (char) -1;
-                } else {
-                    stepval = __Pyx_NewRef(v);
-                }
-                val = (char) 0;
-                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
-                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(char) * 8 - chunk_size; bits += chunk_size) {
-                    PyObject *tmp, *digit;
-                    digit = PyNumber_And(stepval, mask);
-                    if (unlikely(!digit)) goto done;
-                    idigit = PyLong_AsLong(digit);
-                    Py_DECREF(digit);
-                    if (unlikely(idigit < 0)) goto done;
-                    tmp = PyNumber_Rshift(stepval, shift);
-                    if (unlikely(!tmp)) goto done;
-                    Py_DECREF(stepval); stepval = tmp;
-                    val |= ((char) idigit) << bits;
-                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-                    if (Py_SIZE(stepval) == 0)
-                        goto unpacking_done;
-                    #endif
-                }
-                idigit = PyLong_AsLong(stepval);
-                if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(char) * 8) - bits - (is_unsigned ? 0 : 1);
-                if (unlikely(idigit >= (1L << remaining_bits)))
-                    goto raise_overflow;
-                val |= ((char) idigit) << bits;
-            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-            unpacking_done:
-            #endif
-                if (!is_unsigned) {
-                    if (unlikely(val & (((char) 1) << (sizeof(char) * 8 - 1))))
-                        goto raise_overflow;
-                    if (is_negative)
-                        val = ~val;
-                }
-                ret = 0;
-            done:
-                Py_XDECREF(shift);
-                Py_XDECREF(mask);
-                Py_XDECREF(stepval);
-#endif
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-            return (char) -1;
-        }
-    } else {
-        char val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (char) -1;
-        val = __Pyx_PyInt_As_char(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to char");
-    return (char) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to char");
-    return (char) -1;
-}
-
 /* FormatTypeName */
   #if CYTHON_COMPILING_IN_LIMITED_API
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__24);
+        name = __Pyx_NewRef(__pyx_n_s__30);
     }
     return name;
 }
 #endif
 
 /* CheckBinaryVersion */
   static unsigned long __Pyx_get_runtime_version(void) {
```

### Comparing `savemoney-0.2.8b2/savemoney/modules/cython_functions/alignment_functions.pyx` & `savemoney-0.2.9/savemoney/modules/cython_functions/alignment_functions.pyx`

 * *Files 17% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 #         s = 0
 
 
 # ビルド: とりあえず cimport numpy しなければ、setup ファイルで numpy path を指定しなくても下記でいける
 # python alignment_functions_setup.py build_ext --inplace
 # or 
 # cythonize -3 -a -i alignment_functions.pyx
+
 from libcpp.vector cimport vector #ここでcppのvectorを呼び出す
 ctypedef long long LL   # unsigned でも良いのか？
 ctypedef vector[LL] vec
 cpdef k_mer_offset_analysis_2(
         LL[:] ref_seq_v_repeated, 
         LL[:] query_seq_v, 
         LL N_ref, 
@@ -58,15 +59,82 @@
         for i in range(len_query_seq_v):
             if ref_seq_v_repeated[k + i] == query_seq_v[i]:
                 s += 1
         result_array.push_back(s)
         s = 0
     return result_array
 
+from libcpp.map cimport map as c_map
 from libcpp.string cimport string
+from libcpp.algorithm cimport copy
+ctypedef long double LD
+ctypedef vector[char] char_vec
+ctypedef vector[LD] LD_vec
+ctypedef c_map[char, LD] chr_LD_map
+ctypedef c_map[string, LD] str_LD_map
+ctypedef c_map[string, LD_vec] str_LD_vec_map
+
+cdef class SequenceBasecallQscorePDF:
+    # default
+    cdef str_LD_map P_base_calling_given_true_refseq_dict
+    cdef str_LD_vec_map pdf_core
+    cdef char_vec bases
+    cdef LL N_bases
+    # additional
+    cdef string key
+    def __cinit__(self, str_LD_map P_base_calling_given_true_refseq_dict, str_LD_vec_map pdf_core, char_vec bases):
+        self.P_base_calling_given_true_refseq_dict = P_base_calling_given_true_refseq_dict
+        self.pdf_core = pdf_core
+        self.key.resize(3)
+        self.key[1] = b"_"
+        self.bases = bases
+        self.N_bases = self.bases.size()
+
+    def calc_consensus_error_rate(self, char_vec query_list, vec q_score_list, chr_LD_map P_N_dict):
+        cdef LL N_query_list
+        cdef LL base_idx
+        cdef LL idx
+        cdef LD_vec bunshi_list
+        cdef LD bunshi_P_N
+        cdef LD bunbo_bunshi_sum
+        cdef char base
+        cdef LD val
+        cdef LD_vec p_list
+
+        N_query_list = query_list.size()
+
+        for base_idx in range(self.N_bases):
+            # 初期化
+            B = self.bases[base_idx]
+            self.key[0] = B
+            bunshi_list.clear()
+
+            for idx in range(N_query_list):
+                self.key[2] = query_list[idx]
+                if q_score_list[idx] >= 0:
+                    bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]])
+                else:
+                    bunshi_list.push_back(self.P_base_calling_given_true_refseq_dict[self.key])
+            bunshi_P_N = P_N_dict[B]
+
+            # inside sum
+            bunbo_bunshi_sum = 0
+            for base in self.bases:
+                self.key[0] = base
+                val = P_N_dict[base] / bunshi_P_N
+                for idx in range(N_query_list):
+                    self.key[2] = query_list[idx]
+                    if q_score_list[idx] >= 0:
+                        val *= (self.P_base_calling_given_true_refseq_dict[self.key] * self.pdf_core[self.key][q_score_list[idx]]) / bunshi_list[idx]
+                    else:
+                        val *= (self.P_base_calling_given_true_refseq_dict[self.key]) / bunshi_list[idx]
+                bunbo_bunshi_sum += val
+            p_list.push_back(1 - 1 / bunbo_bunshi_sum)
+        return p_list
+
 cpdef my_special_dp_cython(
         string query_seq_1, 
         string query_seq_2, 
         string ref_seq, 
         LL gap_open_penalty, 
         LL gap_extend_penalty, 
         LL match_score,
```

### Comparing `savemoney-0.2.8b2/savemoney/modules/msa.py` & `savemoney-0.2.9/savemoney/modules/msa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import re
 import io
 import copy
-import pysam
 import struct
 import zipfile
 import subprocess
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from PIL import Image as PilImage
@@ -18,14 +17,15 @@
 from itertools import product
 from collections import defaultdict, Counter
 from numpy.core.memmap import uint8
 from matplotlib.patches import Patch
 
 from . import my_classes as mc
 from . import ref_query_alignment as rqa
+from .cython_functions import alignment_functions as af
 
 from matplotlib import rc
 rc('font', **{'family':'sans-serif','sans-serif':[mc.sans_serif_font_master]})
 
 class QueryAssignment():
     query_assignment_version = "qa_0.2.0"
     def __init__(self, ref_seq_list, my_fastq, result_dict) -> None:
@@ -642,21 +642,24 @@
             my_pbar.set_value(len_ref_seq_aligned * N_polish)
         # MSA 後処理
         my_msa.post_polish_process()
         my_msa.set_hard_clipping_info()
         my_msa.ref_seq_name = self.ref_seq.path.name
         my_msa.query_id_list = list(self.my_fastq_subset.keys())
         # MSA calc consensus
+        my_msa = my_msa.execute_soft_clipping()
         my_msa.calculate_consensus()
         # my_msa.print_alignment()
         return my_msa
     def get_racon_path(self):
         return Path(__file__).parents[1] / "racon/build/bin/racon"
 
 class SequenceBasecallQscorePDF():
+    bases = "ATCG-"
+    assert bases[-1] == "-"
     def __init__(self, df_csv_path=None) -> None:
         with open(df_csv_path, "r") as f:
             self.NanoporeStats_PDF_version = re.match(r"^# file_version: ([0-9]+\.[0-9]+\.[0-9]+)$", f.readline().strip()).group(1)
         self.df_stats = pd.read_csv(df_csv_path, sep="\t", header=1, index_col=0)
 
         # initialize
         self.pdf_core = {}
@@ -688,14 +691,26 @@
         # others
         for column_names, values in self.df_stats.items():
             assert all(values.index == np.arange(-1, 42))
             values /= values.sum()
             # マイナス1で最後のやつにアクセスできるようにする（さすがに50も間を開けてれば、q-scoreがかぶってくることは無いでしょう…）
             self.pdf_core[column_names] = list(values)[1:] + [0.0 for i in range(50)] + list(values)[:1]
 
+        # cythonize
+        self.cythonize()
+    def cythonize(self):
+        P_base_calling_given_true_refseq_dict_CYTHON = {
+            key.encode("utf-8") : val
+            for key, val in self.P_base_calling_given_true_refseq_dict.items()
+        }
+        pdf_core_CYTHON = {
+            key.encode("utf-8") : val
+            for key, val in self.pdf_core.items()
+        }
+        self.sbq_pdf_CYTHON = af.SequenceBasecallQscorePDF(P_base_calling_given_true_refseq_dict_CYTHON, pdf_core_CYTHON, self.bases.encode("utf-8"))
     def calc_P_event_given_true_refseq(self, event, true_refseq):
         readseq, q_score = event
         key = f"{true_refseq}_{readseq}"
         return self.P_base_calling_given_true_refseq_dict[key] * self.pdf_core[key][q_score]
     def calc_consensus_error_rate(self, event_list, true_refseq, P_N_dict, bases):
         bunbo_bunshi_sum = 0
         bunshi_list = [self.calc_P_event_given_true_refseq(event, true_refseq) for event in event_list]
@@ -722,16 +737,15 @@
         ("add_sequence", "query_seq_list_aligned"), 
         ("add_q_scores", "q_scores_list_aligned"), 
         # my_cigar_list_aligned は上記 2 つを用いて S, I 以外は後で再生性可能なので保存しない
         ("add_clipping_info", "clipping_info_list"),    # add "S" from my_cigar そして S は連続している
         # clipping info なしでも、S と I 以外は識別可能: なので S の情報のみを格納: 詳しくは self.gen_basic_cigar を参照
         ("add_clipping_info", "aligned_offset_info_list")
     ]
-    bases = "ATCG-"
-    assert bases[-1] == "-"
+    bases = SequenceBasecallQscorePDF.bases
     letter_code_dict = {
         "ATCG":"N", # Any base
         "TCG":"B",  # Not A
         "ACG":"V",  # Not T
         "ATG":"D",  # Not C
         "ATC":"H",  # Not G
         "TG":"K",   # Keto
@@ -1308,33 +1322,36 @@
             my_cigar_aligned = list(my_cigar_aligned)
             for idx in idx_list_to_remove[::-1]:
                 del query_seq_aligned[idx]
                 del q_scores_aligned[idx]
                 del my_cigar_aligned[idx]
             self.query_seq_list_aligned[query_idx] = "".join(query_seq_aligned)
             self.my_cigar_list_aligned[query_idx] = "".join(my_cigar_aligned)
-        # ref_seq などからも削除
+        # ref_seq からも削除
         ref_seq_aligned = list(self.ref_seq_aligned)
-        with_prior_consensus_seq = list(self.with_prior_consensus_seq)
-        with_prior_consensus_my_cigar = list(self.with_prior_consensus_my_cigar)
-        without_prior_consensus_seq = list(self.without_prior_consensus_seq)
-        without_prior_consensus_my_cigar = list(self.without_prior_consensus_my_cigar)
         for idx in idx_list_to_remove[::-1]:
             del ref_seq_aligned[idx]
-            del with_prior_consensus_seq[idx]
-            del with_prior_consensus_my_cigar[idx]
-            del without_prior_consensus_seq[idx]
-            del without_prior_consensus_my_cigar[idx]
-            del self.with_prior_consensus_q_scores[idx]
-            del self.without_prior_consensus_q_scores[idx]
         self.ref_seq_aligned = "".join(ref_seq_aligned)
-        self.with_prior_consensus_seq = "".join(with_prior_consensus_seq)
-        self.with_prior_consensus_my_cigar = "".join(with_prior_consensus_my_cigar)
-        self.without_prior_consensus_seq = "".join(without_prior_consensus_seq)
-        self.without_prior_consensus_my_cigar = "".join(without_prior_consensus_my_cigar)
+        # 既に計算されていたら、consensus_seq からも削除
+        if len(self.with_prior_consensus_seq) > 0:
+            with_prior_consensus_seq = list(self.with_prior_consensus_seq)
+            with_prior_consensus_my_cigar = list(self.with_prior_consensus_my_cigar)
+            without_prior_consensus_seq = list(self.without_prior_consensus_seq)
+            without_prior_consensus_my_cigar = list(self.without_prior_consensus_my_cigar)
+            for idx in idx_list_to_remove[::-1]:
+                del with_prior_consensus_seq[idx]
+                del with_prior_consensus_my_cigar[idx]
+                del without_prior_consensus_seq[idx]
+                del without_prior_consensus_my_cigar[idx]
+                del self.with_prior_consensus_q_scores[idx]
+                del self.without_prior_consensus_q_scores[idx]
+            self.with_prior_consensus_seq = "".join(with_prior_consensus_seq)
+            self.with_prior_consensus_my_cigar = "".join(with_prior_consensus_my_cigar)
+            self.without_prior_consensus_seq = "".join(without_prior_consensus_seq)
+            self.without_prior_consensus_my_cigar = "".join(without_prior_consensus_my_cigar)
 
     # @staticmethod
     # def __calc_entropy(seq_list):
     #     n = len(seq_list)
     #     if n != 0:
     #         counts = Counter(seq_list)
     #         probabilities = [count / n for count in counts.values()]
@@ -1477,34 +1494,47 @@
         else:
             return f"  {q_score_txt}\033[48;2;{color}m{'*' * q_score}"
     ########################
     # consensus calculator #
     ########################
     def calculate_consensus(self):
         # params
-        P_N_dict_dict_with_prior, P_N_dict_dict_without_prior = self.consensus_params(self.param_dict)
+        P_N_dict_dict_with_prior, P_N_dict_dict_without_prior = self.consensus_params(self.param_dict, make_it_for_CYTHON=True)
         # execute
         self.with_prior_consensus_seq, self.with_prior_consensus_q_scores, self.with_prior_consensus_my_cigar = self.calculate_consensus_core(P_N_dict_dict_with_prior)
         self.without_prior_consensus_seq, self.without_prior_consensus_q_scores, self.without_prior_consensus_my_cigar = self.calculate_consensus_core(P_N_dict_dict_without_prior)
     def calculate_consensus_core(self, P_N_dict_dict):
         consensus_seq = ""
         consensus_q_scores = []
         consensus_my_cigar = ""
         for consensus_idx, ref in tqdm(enumerate(self.ref_seq_aligned), ncols=100, mininterval=0.05, leave=True, bar_format='{l_bar}{bar}{r_bar}', desc="generating consensus...", total=len(self.ref_seq_aligned)):
             query_list = [i[consensus_idx] for i in self.query_seq_list_aligned]
             q_score_list = [i[consensus_idx] for i in self.q_scores_list_aligned]
             L_list = [i[consensus_idx] for i in self.my_cigar_list_aligned]
             event_list = [(i.upper(), j) for i, j, k in zip(query_list, q_score_list, L_list) if k not in "HO"]     # =XIDSN
 
+            query_list = []
+            q_score_list = []
+            for query_idx, my_cigar_aligned in enumerate(self.my_cigar_list_aligned):
+                if my_cigar_aligned[consensus_idx] not in "HO":      # =XIDSN
+                    query_list.append(self.query_seq_list_aligned[query_idx][consensus_idx])
+                    q_score_list.append(self.q_scores_list_aligned[query_idx][consensus_idx])
+
             if len(event_list) > 0:
                 P_N_dict = P_N_dict_dict[ref.upper()]
-                p_list = [
-                    self.sbq_pdf.calc_consensus_error_rate(event_list, true_refseq=B, P_N_dict=P_N_dict, bases=self.bases)
-                    for B in self.bases
-                ]
+
+                ### PYTHON ###
+                # event_list = [(i.upper(), j) for i, j, k in zip(query_list, q_score_list, L_list)]
+                # p_list = [
+                #     self.sbq_pdf.calc_consensus_error_rate(event_list, true_refseq=B, P_N_dict=P_N_dict, bases=self.bases)
+                #     for B in self.bases
+                # ]
+                ### CYTHON ###
+                p_list = self.sbq_pdf.sbq_pdf_CYTHON.calc_consensus_error_rate("".join(query_list).encode("utf-8"), q_score_list, P_N_dict)
+                ##############
                 p = min(p_list)
                 # p_idx_list = [i for i, v in enumerate(p_list) if v == p]
                 consensus_base_call = self.mixed_bases([b for b, tmp_p in zip(self.bases, p_list) if tmp_p == p])
 
                 # register
                 if p >= 10 ** (-5):
                     q_score = np.round(-10 * np.log10(p)).astype(int)
@@ -1530,15 +1560,15 @@
                 consensus_my_cigar += "X"
             elif ref == consensus_base_call == "-":
                 consensus_my_cigar += "N"
             else:
                 raise Exception(f"error: {ref} {consensus_base_call}")
         return consensus_seq, consensus_q_scores, consensus_my_cigar
     @classmethod
-    def consensus_params(cls, param_dict):
+    def consensus_params(cls, param_dict, make_it_for_CYTHON):
         ins_rate = param_dict["ins_rate"]
         error_rate = param_dict["error_rate"]
         del_mut_rate = param_dict["del_mut_rate"]
         default_value_with_prior = {b_key2:ins_rate / 4 if b_key2 != "-" else 1 - ins_rate for b_key2 in cls.bases}
 
         P_N_dict_dict_with_prior = defaultdict(
             lambda: default_value_with_prior, 
@@ -1553,14 +1583,23 @@
             lambda: default_value_without_prior, 
             {
                 b_key1:{b_key2: 0.2 for b_key2 in cls.bases} for b_key1 in cls.bases[::-1]
             }
         )
         P_N_dict_dict_without_prior["-"] = default_value_without_prior
 
+        if make_it_for_CYTHON:
+            P_N_dict_dict_with_prior = {
+                key:{ord(k):v for k, v in val.items()}
+                for key, val in P_N_dict_dict_with_prior.items()
+            }
+            P_N_dict_dict_without_prior = {
+                key:{ord(k):v for k, v in val.items()}
+                for key, val in P_N_dict_dict_without_prior.items()
+            }
         return P_N_dict_dict_with_prior, P_N_dict_dict_without_prior
     def mixed_bases(self, base_list):
         if len(base_list) == 1:
             return base_list[0]
         elif "-" not in base_list:
             pass
         else:
@@ -1569,15 +1608,15 @@
         for b in self.bases[:-1]:
             if b in base_list:
                 letters += b
         return self.letter_code_dict[letters]
     # FOR LOG
     @classmethod
     def P_N_dict_dict_2_matrix(cls, param_dict):
-        P_N_dict_dict_with_prior, P_N_dict_dict_without_prior = cls.consensus_params(param_dict)
+        P_N_dict_dict_with_prior, P_N_dict_dict_without_prior = cls.consensus_params(param_dict, make_it_for_CYTHON=False)
         def gen_matrix_from_dict_dict(P_N_dict_dict):
             r_matrix = np.empty((len(cls.bases), len(cls.bases)), dtype=float)
             for r, b_key1 in enumerate(cls.bases):
                 for c, b_key2 in enumerate(cls.bases):
                     r_matrix[r, c] = P_N_dict_dict[b_key1][b_key2]
             return r_matrix
         return gen_matrix_from_dict_dict(P_N_dict_dict_with_prior), gen_matrix_from_dict_dict(P_N_dict_dict_without_prior)
@@ -1805,14 +1844,20 @@
                 assert q_score != -1
             elif L == "N":
                 assert con == ref == "-"
             else:
                 raise Exception(f"unknown cigar: {L}")
         return True
     def convert_to_bam(self, save_dir=None, replace_S_with_I=False, ext_not_exported=[".sorted.sam", ".bam.fastq"]):
+        try:
+            import pysam
+        except ImportError:
+            raise Exception("ImportError: Missing optional dependency 'pysam'.  Use pip to install pysam.")
+        except ModuleNotFoundError:
+            raise Exception("ModuleNotFoundError: Missing optional dependency 'pysam'.  Use pip to install pysam.")
         S_replacement = "I" if replace_S_with_I else "S"
         # Create a BAM file
         ref_len = len(self.ref_seq_NoDEL)
         header_text = f"@HD\tVN:1.6\tSO:unsorted\n@SQ\tSN:{self.ref_seq_name}\tLN:{ref_len}"
         header = pysam.AlignmentHeader.from_text(header_text)
         ref_id = header.get_tid(self.ref_seq_name)
         # =XDISHO
```

### Comparing `savemoney-0.2.8b2/savemoney/modules/my_classes.py` & `savemoney-0.2.9/savemoney/modules/my_classes.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/modules/ref_query_alignment.py` & `savemoney-0.2.9/savemoney/modules/ref_query_alignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     percentile_factor = 0.1 # 低いほど conserved region の quality は上がるが、計算時間がかかる
     def __init__(self, ref_seq, param_dict) -> None:
         super().__init__(param_dict)
         self.ref_seq = ref_seq
         self.ref_seq_v = np.array([ord(char) for char in ref_seq])
         self.N_ref = len(self.ref_seq_v)
         self.ref_seq_v_repeated_list = [
-            np.hstack([self.ref_seq_v for i in range(repeat)], dtype=np.int64)
+            np.hstack([self.ref_seq_v for i in range(repeat)]).astype(np.int64)
             for repeat in range(2, self.default_repeat_max + 1)
         ]
         self.k_list = np.arange(0, self.N_ref)
         x_percentile = 1 / self.N_ref * self.percentile_factor # 偶然 threshold を超える position が 0.1個/ref_seq 以下になるようにする
         self.sigma = stats.norm.ppf(1 - x_percentile, loc=0, scale=1)  # 累積分布関数の逆関数
         self.is_all_ATCG = all([b.upper() in "ATCG" for b in ref_seq])
     def calc_circular_conserved_region(self, query_seq):
@@ -275,15 +275,15 @@
         query_seq_v = np.array([ord(char) for char in query_seq], dtype=np.int64)
         N_query = len(query_seq_v)
         repeat = 1 + np.ceil((N_query - 1) / self.N_ref).astype(int)
         # アラインメントのたびに ref_seq_v_repeated を作らないようにする：本来は else 中の hstack のみで ok だけど、それだと時間がかかるかな？
         if repeat <= self.default_repeat_max:
             ref_seq_v_repeated = self.ref_seq_v_repeated_list[repeat - 2]
         else:
-            ref_seq_v_repeated = np.hstack([self.ref_seq_v for i in range(repeat)], np.int64)
+            ref_seq_v_repeated = np.hstack([self.ref_seq_v for i in range(repeat)]).astype(np.int64)
 
         #######################
         # k座位分だけ query をずらして並べたときの類似性（repeated ref_seq を固定して、query_seq のオフセットを右にずらしていくイメージ）
         #######################
         """
         # python version
         """
```

### Comparing `savemoney-0.2.8b2/savemoney/post_analysis/__main__.py` & `savemoney-0.2.9/savemoney/post_analysis/__main__.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/post_analysis/post_analysis.py` & `savemoney-0.2.9/savemoney/post_analysis/post_analysis.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/post_analysis/post_analysis_core.py` & `savemoney-0.2.9/savemoney/post_analysis/post_analysis_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,18 +204,17 @@
 
 #############
 # CONSENSUS #
 #############
 def export_results(my_msa_list: List[msa.MyMSA], save_dir):
     print("exporting results...")
     for my_msa in my_msa_list:
-        new_my_msa = my_msa.execute_soft_clipping()
-        new_my_msa.export_consensus_fastq(save_dir)
-        new_my_msa.export_gif(save_dir)
-        new_my_msa.export_consensus_alignment(save_dir)
+        my_msa.export_consensus_fastq(save_dir)
+        my_msa.export_gif(save_dir)
+        my_msa.export_consensus_alignment(save_dir)
     print("export: DONE")
 
 def export_log(ref_seq_list:list, my_fastq:mc.MyFastQ, param_dict, query_assignment: msa.QueryAssignment, save_dir:Path):
     print("exporting log...")
     my_log = MyLog(ref_seq_list, my_fastq, param_dict, query_assignment)
     my_log.save(save_path = save_dir / f"{my_fastq.combined_name_stem}.log")
     print("export: DONE")
```

### Comparing `savemoney-0.2.8b2/savemoney/pre_survey/__main__.py` & `savemoney-0.2.9/savemoney/pre_survey/__main__.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/pre_survey/pre_survey.py` & `savemoney-0.2.9/savemoney/pre_survey/pre_survey.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/pre_survey/pre_survey_core.py` & `savemoney-0.2.9/savemoney/pre_survey/pre_survey_core.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney/show_consensus/__main__.py` & `savemoney-0.2.9/savemoney/show_consensus/__main__.py`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/savemoney.egg-info/PKG-INFO` & `savemoney-0.2.9/savemoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savemoney
-Version: 0.2.8b2
+Version: 0.2.9
 Summary: Simple Algorithm for Very Efficient Multiplexing of Oxford Nanopore Experiments for You!
 Home-page: https://github.com/MasaakiU/MultiplexNanopore
 Author: Masaaki Uematsu
 Author-email: mu84@cornell.edu
 Maintainer: Masaaki Uematsu
 Maintainer-email: mu84@cornell.edu
 License: CC BY-NC-SA 4.0
@@ -15,26 +15,25 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas>=2.1.4
+Requires-Dist: pandas>=1.5.3
 Requires-Dist: parasail>=1.3.4
-Requires-Dist: Pillow>=10.2.0
+Requires-Dist: Pillow>=9.4.0
 Requires-Dist: PuLP>=2.7.0
 Requires-Dist: scipy>=1.11.4
 Requires-Dist: snapgene_reader>=0.1.20
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: biopython>=1.83
 Requires-Dist: Cython>=3.0.7
-Requires-Dist: matplotlib>=3.8.2
-Requires-Dist: numpy>=1.26.2
-Requires-Dist: pysam>=0.22.0
+Requires-Dist: matplotlib>=3.7.1
+Requires-Dist: numpy>=1.23.5
 Requires-Dist: pyspoa>=0.2.1
 
 <p align="center"><img src="https://github.com/MasaakiU/MultiplexNanopore/raw/master/resources/logo/SAVEMONEY_logo_with_letter.png"/></p>
 
 *Simple Algorithm for Very Efficient Multiplexing of Oxford Nanopore Experiments for You!*
 
 # Overview
```

### Comparing `savemoney-0.2.8b2/savemoney.egg-info/SOURCES.txt` & `savemoney-0.2.9/savemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `savemoney-0.2.8b2/setup.py` & `savemoney-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     from setuptools import dist
     dist.Distribution().fetch_build_eggs(['Cython>=3.0.7'])
     from Cython.Build import cythonize
 
 #############################################################
 #############################################################
 
-test_version = "b2"
+test_version = ""
 root_dir = Path(__file__).parent.resolve()
 package_name = "savemoney"
 sub_package_names = [f"{package_name}.{sub_package_name}" for sub_package_name in find_packages(package_name)]
 
 class About():
     def __init__(self, about_path, keys) -> None:
         self.keys = keys
@@ -82,29 +82,29 @@
     ]
 )
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 INSTALL_REQUIREMENTS = [
-    "pandas>=2.1.4", 
+    "pandas>=1.5.3", 
     "parasail>=1.3.4", 
-    "Pillow>=10.2.0", 
+    "Pillow>=9.4.0", 
     "PuLP>=2.7.0", 
     "scipy>=1.11.4", 
     # "setuptools>=68.2.2", 
     "snapgene_reader>=0.1.20", 
     "tqdm>=4.66.1", 
     # "Bio>=1.6.0",         # ?
     "biopython>=1.83", 
     "Cython>=3.0.7", 
-    "matplotlib>=3.8.2", 
-    "numpy>=1.26.2", 
+    "matplotlib>=3.7.1", 
+    "numpy>=1.23.5", 
     # "oauth2client>=4.1.3", 
-    "pysam>=0.22.0", 
+    # "pysam>=0.22.0", 
     "pyspoa>=0.2.1"
 ]
 
 PYTHON_REQUIRES = ">=3.10"
 
 setup(
     name = package_name,
```

### Comparing `savemoney-0.2.8b2/test/test_local_all.py` & `savemoney-0.2.9/test/test_local_all.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,18 +26,20 @@
     param_dict = {  # optional params
         'distance_threshold':   5, 
         'number_of_groups':     2, 
     }
     savemoney.pre_survey(sequence_dir_path, save_dir_base, **param_dict)
     savemoney.post_analysis(sequence_dir_path, save_dir_base)
     savemoney.show_consensus(consensus_alignment_path)
+    savemoney.ca2bam(consensus_alignment_path)
 
     #####################
     # WITH COMMAND LINE #
     #####################
     subprocess.call(f"python -m savemoney.pre_survey {sequence_dir_path} {save_dir_base} -dt {param_dict['distance_threshold']} -nog {param_dict['number_of_groups']}", shell=True)
     subprocess.call(f"python -m savemoney.post_analysis {sequence_dir_path} {save_dir_base}", shell=True)
     subprocess.call(f"python -m savemoney.show_consensus {consensus_alignment_path}", shell=True)
+    subprocess.call(f"python -m savemoney.ca2bam {consensus_alignment_path}", shell=True)
```

