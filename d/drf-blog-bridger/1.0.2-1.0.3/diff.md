# Comparing `tmp/drf-blog-bridger-1.0.2.tar.gz` & `tmp/drf-blog-bridger-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-blog-bridger-1.0.2.tar", last modified: Tue Mar 12 12:20:32 2024, max compression
+gzip compressed data, was "drf-blog-bridger-1.0.3.tar", last modified: Sat Apr  6 04:32:58 2024, max compression
```

## Comparing `drf-blog-bridger-1.0.2.tar` & `drf-blog-bridger-1.0.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-03-12 12:20:32.283560 drf-blog-bridger-1.0.2/
--rw-rw-rw-   0        0        0     1087 2024-03-02 12:15:09.000000 drf-blog-bridger-1.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2024-03-04 17:15:39.000000 drf-blog-bridger-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2568 2024-03-12 12:20:32.283560 drf-blog-bridger-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1434 2024-03-12 12:15:45.000000 drf-blog-bridger-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-12 12:20:32.241968 drf-blog-bridger-1.0.2/blog_bridger_drf/
--rw-rw-rw-   0        0        0        0 2024-02-13 13:47:04.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/__init__.py
--rw-rw-rw-   0        0        0      160 2024-02-13 13:47:04.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/admin.py
--rw-rw-rw-   0        0        0      191 2024-03-02 10:50:47.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/apps.py
--rw-rw-rw-   0        0        0      269 2024-03-12 11:48:21.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/default_settings.py
-drwxrwxrwx   0        0        0        0 2024-03-12 12:20:32.251645 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/
--rw-rw-rw-   0        0        0     1571 2024-02-24 15:36:44.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      796 2024-02-24 15:22:45.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0002_comment_created_at_alter_post_author.py
--rw-rw-rw-   0        0        0      664 2024-02-24 15:37:02.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0003_remove_comment_commenter_alter_comment_post.py
--rw-rw-rw-   0        0        0      446 2024-02-24 15:23:00.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0004_comment_comment.py
--rw-rw-rw-   0        0        0      396 2024-02-24 15:23:05.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0005_rename_author_comment_comment_author.py
--rw-rw-rw-   0        0        0      386 2024-02-24 15:23:09.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0006_alter_post_options.py
--rw-rw-rw-   0        0        0      535 2024-02-24 15:34:38.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0007_alter_comment_post.py
--rw-rw-rw-   0        0        0        0 2024-02-13 13:47:04.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/__init__.py
--rw-rw-rw-   0        0        0     1048 2024-02-15 14:55:00.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/models.py
--rw-rw-rw-   0        0        0      280 2024-03-02 10:35:05.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/permissions.py
--rw-rw-rw-   0        0        0     1948 2024-02-15 10:36:18.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/serializers.py
--rw-rw-rw-   0        0        0       63 2024-02-13 13:47:04.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/tests.py
--rw-rw-rw-   0        0        0      426 2024-02-19 17:51:23.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/urls.py
--rw-rw-rw-   0        0        0     4935 2024-03-12 11:57:54.000000 drf-blog-bridger-1.0.2/blog_bridger_drf/views.py
-drwxrwxrwx   0        0        0        0 2024-03-12 12:20:32.281682 drf-blog-bridger-1.0.2/drf_blog_bridger.egg-info/
--rw-rw-rw-   0        0        0     2568 2024-03-12 12:20:32.000000 drf-blog-bridger-1.0.2/drf_blog_bridger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1019 2024-03-12 12:20:32.000000 drf-blog-bridger-1.0.2/drf_blog_bridger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-12 12:20:32.000000 drf-blog-bridger-1.0.2/drf_blog_bridger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-03-12 12:20:32.000000 drf-blog-bridger-1.0.2/drf_blog_bridger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-12 12:20:32.000000 drf-blog-bridger-1.0.2/drf_blog_bridger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2024-03-02 15:07:52.000000 drf-blog-bridger-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1126 2024-03-12 12:20:32.286552 drf-blog-bridger-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-03-02 12:20:24.000000 drf-blog-bridger-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:32:58.039333 drf-blog-bridger-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2024-03-02 12:15:09.000000 drf-blog-bridger-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-03-04 17:15:39.000000 drf-blog-bridger-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2719 2024-04-06 04:32:58.039333 drf-blog-bridger-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1434 2024-03-12 12:15:45.000000 drf-blog-bridger-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 04:32:57.958453 drf-blog-bridger-1.0.3/blog_bridger_drf/
+-rw-rw-rw-   0        0        0        0 2024-02-13 13:47:04.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/__init__.py
+-rw-rw-rw-   0        0        0      160 2024-02-13 13:47:04.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/admin.py
+-rw-rw-rw-   0        0        0      191 2024-03-02 10:50:47.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/apps.py
+-rw-rw-rw-   0        0        0      269 2024-03-12 11:48:21.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/default_settings.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:32:58.001886 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/
+-rw-rw-rw-   0        0        0     1571 2024-02-24 15:36:44.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      796 2024-02-24 15:22:45.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0002_comment_created_at_alter_post_author.py
+-rw-rw-rw-   0        0        0      664 2024-02-24 15:37:02.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0003_remove_comment_commenter_alter_comment_post.py
+-rw-rw-rw-   0        0        0      446 2024-02-24 15:23:00.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0004_comment_comment.py
+-rw-rw-rw-   0        0        0      396 2024-02-24 15:23:05.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0005_rename_author_comment_comment_author.py
+-rw-rw-rw-   0        0        0      386 2024-02-24 15:23:09.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0006_alter_post_options.py
+-rw-rw-rw-   0        0        0      535 2024-02-24 15:34:38.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0007_alter_comment_post.py
+-rw-rw-rw-   0        0        0        0 2024-02-13 13:47:04.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1048 2024-02-15 14:55:00.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/models.py
+-rw-rw-rw-   0        0        0      280 2024-03-02 10:35:05.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/permissions.py
+-rw-rw-rw-   0        0        0     1948 2024-02-15 10:36:18.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/serializers.py
+-rw-rw-rw-   0        0        0       63 2024-02-13 13:47:04.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/tests.py
+-rw-rw-rw-   0        0        0      426 2024-02-19 17:51:23.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/urls.py
+-rw-rw-rw-   0        0        0     4935 2024-03-12 11:57:54.000000 drf-blog-bridger-1.0.3/blog_bridger_drf/views.py
+drwxrwxrwx   0        0        0        0 2024-04-06 04:32:58.033270 drf-blog-bridger-1.0.3/drf_blog_bridger.egg-info/
+-rw-rw-rw-   0        0        0     2719 2024-04-06 04:32:57.000000 drf-blog-bridger-1.0.3/drf_blog_bridger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1019 2024-04-06 04:32:57.000000 drf-blog-bridger-1.0.3/drf_blog_bridger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 04:32:57.000000 drf-blog-bridger-1.0.3/drf_blog_bridger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-04-06 04:32:57.000000 drf-blog-bridger-1.0.3/drf_blog_bridger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 04:32:57.000000 drf-blog-bridger-1.0.3/drf_blog_bridger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2024-03-02 15:07:52.000000 drf-blog-bridger-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1244 2024-04-06 04:32:58.045469 drf-blog-bridger-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-03-02 12:20:24.000000 drf-blog-bridger-1.0.3/setup.py
```

### Comparing `drf-blog-bridger-1.0.2/LICENSE` & `drf-blog-bridger-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/PKG-INFO` & `drf-blog-bridger-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: drf-blog-bridger
-Version: 1.0.2
+Version: 1.0.3
 Summary: A DRF app that provides CRUD endpoints for a blog app.
 Author: Ademola Thompson
 Author-email: ademolathompson5@gmail.com
 License: MIT
 Keywords: djangorestframework,blog,drf,django,posts
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=5.0.1
-Requires-Dist: djangorestframework>=3.14.0
+Requires-Dist: Django>=4.2
+Requires-Dist: djangorestframework>=3.12.0
 
 # DRF Blog Bridger
 
 ## Introduction
 
 DRF Blog Bridger is a simple tool that allows Django Rest Framework Developers to set up a simple blog API without worrying about the underlying code. The tool takes care of things like CRUD operations for blog posts, as well as the comment feature for each post.
```

### Comparing `drf-blog-bridger-1.0.2/README.md` & `drf-blog-bridger-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0001_initial.py` & `drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0002_comment_created_at_alter_post_author.py` & `drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0002_comment_created_at_alter_post_author.py`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0003_remove_comment_commenter_alter_comment_post.py` & `drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0003_remove_comment_commenter_alter_comment_post.py`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/blog_bridger_drf/migrations/0007_alter_comment_post.py` & `drf-blog-bridger-1.0.3/blog_bridger_drf/migrations/0007_alter_comment_post.py`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/blog_bridger_drf/models.py` & `drf-blog-bridger-1.0.3/blog_bridger_drf/models.py`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/blog_bridger_drf/serializers.py` & `drf-blog-bridger-1.0.3/blog_bridger_drf/serializers.py`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/blog_bridger_drf/views.py` & `drf-blog-bridger-1.0.3/blog_bridger_drf/views.py`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/drf_blog_bridger.egg-info/PKG-INFO` & `drf-blog-bridger-1.0.3/drf_blog_bridger.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: drf-blog-bridger
-Version: 1.0.2
+Version: 1.0.3
 Summary: A DRF app that provides CRUD endpoints for a blog app.
 Author: Ademola Thompson
 Author-email: ademolathompson5@gmail.com
 License: MIT
 Keywords: djangorestframework,blog,drf,django,posts
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django>=5.0.1
-Requires-Dist: djangorestframework>=3.14.0
+Requires-Dist: Django>=4.2
+Requires-Dist: djangorestframework>=3.12.0
 
 # DRF Blog Bridger
 
 ## Introduction
 
 DRF Blog Bridger is a simple tool that allows Django Rest Framework Developers to set up a simple blog API without worrying about the underlying code. The tool takes care of things like CRUD operations for blog posts, as well as the comment feature for each post.
```

### Comparing `drf-blog-bridger-1.0.2/drf_blog_bridger.egg-info/SOURCES.txt` & `drf-blog-bridger-1.0.3/drf_blog_bridger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-blog-bridger-1.0.2/setup.cfg` & `drf-blog-bridger-1.0.3/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 7266 2d62 6c6f 672d 6272 6964   = drf-blog-brid
 00000020: 6765 720d 0a76 6572 7369 6f6e 203d 2031  ger..version = 1
-00000030: 2e30 2e32 0d0a 6465 7363 7269 7074 696f  .0.2..descriptio
+00000030: 2e30 2e33 0d0a 6465 7363 7269 7074 696f  .0.3..descriptio
 00000040: 6e20 3d20 4120 4452 4620 6170 7020 7468  n = A DRF app th
 00000050: 6174 2070 726f 7669 6465 7320 4352 5544  at provides CRUD
 00000060: 2065 6e64 706f 696e 7473 2066 6f72 2061   endpoints for a
 00000070: 2062 6c6f 6720 6170 702e 0d0a 6c6f 6e67   blog app...long
 00000080: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000090: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 000000a0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
@@ -37,35 +37,42 @@
 00000240: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000250: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
 00000260: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
 00000270: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000280: 6f6e 203a 3a20 3320 3a3a 204f 6e6c 790d  on :: 3 :: Only.
 00000290: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
 000002a0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002b0: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
-000002c0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002d0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-000002e0: 310d 0a09 5072 6f67 7261 6d6d 696e 6720  1...Programming 
-000002f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000300: 6f6e 203a 3a20 332e 3132 0d0a 0954 6f70  on :: 3.12...Top
-00000310: 6963 203a 3a20 536f 6674 7761 7265 2044  ic :: Software D
-00000320: 6576 656c 6f70 6d65 6e74 203a 3a20 4c69  evelopment :: Li
-00000330: 6272 6172 6965 7320 3a3a 2050 7974 686f  braries :: Pytho
-00000340: 6e20 4d6f 6475 6c65 730d 0a09 546f 7069  n Modules...Topi
-00000350: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-00000360: 2057 5757 2f48 5454 500d 0a09 546f 7069   WWW/HTTP...Topi
-00000370: 6320 3a3a 2049 6e74 6572 6e65 7420 3a3a  c :: Internet ::
-00000380: 2057 5757 2f48 5454 5020 3a3a 2044 796e   WWW/HTTP :: Dyn
-00000390: 616d 6963 2043 6f6e 7465 6e74 0d0a 0d0a  amic Content....
-000003a0: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
-000003b0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
-000003c0: 3d20 7472 7565 0d0a 7061 636b 6167 6573  = true..packages
-000003d0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-000003e0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-000003f0: 380d 0a69 6e73 7461 6c6c 5f72 6571 7569  8..install_requi
-00000400: 7265 7320 3d20 0d0a 0944 6a61 6e67 6f20  res = ...Django 
-00000410: 3e3d 2035 2e30 2e31 0d0a 0964 6a61 6e67  >= 5.0.1...djang
-00000420: 6f72 6573 7466 7261 6d65 776f 726b 203e  orestframework >
-00000430: 3d20 332e 3134 2e30 0d0a 0d0a 5b65 6767  = 3.14.0....[egg
-00000440: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000450: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000460: 2030 0d0a 0d0a                            0....
+000002b0: 203a 3a20 332e 370d 0a09 5072 6f67 7261   :: 3.7...Progra
+000002c0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002d0: 3a20 5079 7468 6f6e 203a 3a20 332e 380d  : Python :: 3.8.
+000002e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000002f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000300: 203a 3a20 332e 390d 0a09 5072 6f67 7261   :: 3.9...Progra
+00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000330: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
+00000340: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000350: 6e20 3a3a 2033 2e31 310d 0a09 5072 6f67  n :: 3.11...Prog
+00000360: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000370: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000380: 3132 0d0a 0954 6f70 6963 203a 3a20 536f  12...Topic :: So
+00000390: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
+000003a0: 6e74 203a 3a20 4c69 6272 6172 6965 7320  nt :: Libraries 
+000003b0: 3a3a 2050 7974 686f 6e20 4d6f 6475 6c65  :: Python Module
+000003c0: 730d 0a09 546f 7069 6320 3a3a 2049 6e74  s...Topic :: Int
+000003d0: 6572 6e65 7420 3a3a 2057 5757 2f48 5454  ernet :: WWW/HTT
+000003e0: 500d 0a09 546f 7069 6320 3a3a 2049 6e74  P...Topic :: Int
+000003f0: 6572 6e65 7420 3a3a 2057 5757 2f48 5454  ernet :: WWW/HTT
+00000400: 5020 3a3a 2044 796e 616d 6963 2043 6f6e  P :: Dynamic Con
+00000410: 7465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  tent....[options
+00000420: 5d0d 0a69 6e63 6c75 6465 5f70 6163 6b61  ]..include_packa
+00000430: 6765 5f64 6174 6120 3d20 7472 7565 0d0a  ge_data = true..
+00000440: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
+00000450: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
+00000460: 7320 3d20 3e3d 332e 370d 0a69 6e73 7461  s = >=3.7..insta
+00000470: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
+00000480: 0944 6a61 6e67 6f20 3e3d 2034 2e32 0d0a  .Django >= 4.2..
+00000490: 0964 6a61 6e67 6f72 6573 7466 7261 6d65  .djangorestframe
+000004a0: 776f 726b 203e 3d20 332e 3132 2e30 0d0a  work >= 3.12.0..
+000004b0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000004c0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+000004d0: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

