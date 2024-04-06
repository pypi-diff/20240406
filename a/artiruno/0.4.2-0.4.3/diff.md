# Comparing `tmp/artiruno-0.4.2.tar.gz` & `tmp/artiruno-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artiruno-0.4.2.tar", last modified: Sun Sep 24 15:43:11 2023, max compression
+gzip compressed data, was "artiruno-0.4.3.tar", last modified: Sat Apr  6 15:29:32 2024, max compression
```

## Comparing `artiruno-0.4.2.tar` & `artiruno-0.4.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-09-24 15:43:11.868074 artiruno-0.4.2/
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-09-24 15:43:11.868074 artiruno-0.4.2/.github/
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-09-24 15:43:11.868074 artiruno-0.4.2/.github/workflows/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      578 2023-09-21 18:37:34.000000 artiruno-0.4.2/.github/workflows/tests.yml
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       72 2021-02-02 18:12:28.000000 artiruno-0.4.2/.gitignore
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1806 2023-09-24 15:43:11.868074 artiruno-0.4.2/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1171 2022-03-01 15:43:57.000000 artiruno-0.4.2/README.rst
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-09-24 15:43:11.868074 artiruno-0.4.2/artiruno/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      833 2023-09-24 15:38:16.000000 artiruno-0.4.2/artiruno/__init__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       56 2021-01-24 19:33:59.000000 artiruno-0.4.2/artiruno/__main__.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       22 2023-09-24 15:31:18.000000 artiruno-0.4.2/artiruno/_version.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4503 2023-09-21 18:38:15.000000 artiruno-0.4.2/artiruno/interactive.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     8273 2022-03-19 14:32:34.000000 artiruno-0.4.2/artiruno/preorder.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      209 2021-02-02 18:12:28.000000 artiruno-0.4.2/artiruno/util.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7550 2023-09-21 18:38:15.000000 artiruno-0.4.2/artiruno/vda.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     6459 2022-07-10 17:57:00.000000 artiruno-0.4.2/artiruno/web.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-09-24 15:43:11.868074 artiruno-0.4.2/artiruno.egg-info/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1806 2023-09-24 15:43:11.000000 artiruno-0.4.2/artiruno.egg-info/PKG-INFO
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      501 2023-09-24 15:43:11.000000 artiruno-0.4.2/artiruno.egg-info/SOURCES.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2023-09-24 15:43:11.000000 artiruno-0.4.2/artiruno.egg-info/dependency_links.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)        9 2023-09-24 15:43:11.000000 artiruno-0.4.2/artiruno.egg-info/top_level.txt
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      657 2022-02-27 16:34:59.000000 artiruno-0.4.2/conftest.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-09-24 15:43:11.868074 artiruno-0.4.2/doc/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      439 2021-02-02 18:12:28.000000 artiruno-0.4.2/doc/conf.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     7415 2023-09-21 18:37:01.000000 artiruno-0.4.2/doc/index.rst
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-09-24 15:43:11.868074 artiruno-0.4.2/examples/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)      357 2020-10-25 20:02:27.000000 artiruno-0.4.2/examples/birds.json
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1448 2022-03-01 15:43:57.000000 artiruno-0.4.2/examples/jobs.json
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2901 2023-03-21 17:59:26.000000 artiruno-0.4.2/pyodide_testing.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       92 2023-09-21 18:37:34.000000 artiruno-0.4.2/pytest.ini
--rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2023-09-24 15:43:11.868074 artiruno-0.4.2/setup.cfg
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     1015 2021-02-02 18:12:28.000000 artiruno-0.4.2/setup.py
-drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2023-09-24 15:43:11.868074 artiruno-0.4.2/tests/
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     4785 2022-03-01 15:43:57.000000 artiruno-0.4.2/tests/test_preorder.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)    12958 2023-09-21 18:37:34.000000 artiruno-0.4.2/tests/test_vda.py
--rw-rw-r--   0 hippo     (1000) hippo     (1000)     2079 2023-03-21 17:59:26.000000 artiruno-0.4.2/webi.html
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-04-06 15:29:32.431215 artiruno-0.4.3/
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-04-06 15:29:32.427215 artiruno-0.4.3/.github/
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-04-06 15:29:32.427215 artiruno-0.4.3/.github/workflows/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      586 2024-04-06 15:26:45.000000 artiruno-0.4.3/.github/workflows/tests.yml
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       72 2021-02-02 18:12:28.000000 artiruno-0.4.3/.gitignore
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2165 2024-04-06 15:29:32.431215 artiruno-0.4.3/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1530 2024-04-06 15:26:35.000000 artiruno-0.4.3/README.rst
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-04-06 15:29:32.427215 artiruno-0.4.3/artiruno/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      833 2023-09-24 15:38:16.000000 artiruno-0.4.3/artiruno/__init__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       56 2021-01-24 19:33:59.000000 artiruno-0.4.3/artiruno/__main__.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       22 2024-04-06 15:26:45.000000 artiruno-0.4.3/artiruno/_version.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4503 2024-04-06 15:23:34.000000 artiruno-0.4.3/artiruno/interactive.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     8273 2022-03-19 14:32:34.000000 artiruno-0.4.3/artiruno/preorder.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      209 2021-02-02 18:12:28.000000 artiruno-0.4.3/artiruno/util.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     7550 2024-04-06 15:23:34.000000 artiruno-0.4.3/artiruno/vda.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     6459 2022-07-10 17:57:00.000000 artiruno-0.4.3/artiruno/web.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-04-06 15:29:32.427215 artiruno-0.4.3/artiruno.egg-info/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2165 2024-04-06 15:29:32.000000 artiruno-0.4.3/artiruno.egg-info/PKG-INFO
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      501 2024-04-06 15:29:32.000000 artiruno-0.4.3/artiruno.egg-info/SOURCES.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        1 2024-04-06 15:29:32.000000 artiruno-0.4.3/artiruno.egg-info/dependency_links.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)        9 2024-04-06 15:29:32.000000 artiruno-0.4.3/artiruno.egg-info/top_level.txt
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      657 2022-02-27 16:34:59.000000 artiruno-0.4.3/conftest.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-04-06 15:29:32.427215 artiruno-0.4.3/doc/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      439 2021-02-02 18:12:28.000000 artiruno-0.4.3/doc/conf.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4827 2024-04-06 15:26:21.000000 artiruno-0.4.3/doc/index.rst
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-04-06 15:29:32.431215 artiruno-0.4.3/examples/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)      357 2020-10-25 20:02:27.000000 artiruno-0.4.3/examples/birds.json
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1448 2022-03-01 15:43:57.000000 artiruno-0.4.3/examples/jobs.json
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2901 2023-03-21 17:59:26.000000 artiruno-0.4.3/pyodide_testing.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       92 2023-09-21 18:37:34.000000 artiruno-0.4.3/pytest.ini
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)       38 2024-04-06 15:29:32.431215 artiruno-0.4.3/setup.cfg
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     1015 2021-02-02 18:12:28.000000 artiruno-0.4.3/setup.py
+drwxrwxr-x   0 hippo     (1000) hippo     (1000)        0 2024-04-06 15:29:32.431215 artiruno-0.4.3/tests/
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     4785 2022-03-01 15:43:57.000000 artiruno-0.4.3/tests/test_preorder.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)    12958 2023-09-21 18:37:34.000000 artiruno-0.4.3/tests/test_vda.py
+-rw-rw-r--   0 hippo     (1000) hippo     (1000)     2079 2023-03-21 17:59:26.000000 artiruno-0.4.3/webi.html
```

### Comparing `artiruno-0.4.2/PKG-INFO` & `artiruno-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artiruno
-Version: 0.4.2
+Version: 0.4.3
 Summary: Verbal decision analysis
 Home-page: https://arfer.net/projects/artiruno
 Author: Kodi B. Arfer
 Project-URL: Documentation, https://arfer.net/projects/artiruno/doc
 Project-URL: Source Code, https://github.com/Kodiologist/Artiruno
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -14,24 +14,32 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 .. image:: https://i.imgur.com/GlZ6CEM.png
   :alt: Art by Ken Sugimori
   :align: center
 
+.. role:: html(raw)
+   :format: html
+
 Artiruno is a program to help you make decisions with verbal decision analysis. It's also a Python library with a class for `preordered sets`_ that should be just as useful outside the context of decision-making.
 
 - `Try Artiruno in your web browser <http://arfer.net/projects/artiruno/webi>`_
 - `Documentation <http://arfer.net/projects/artiruno/doc>`_
 
 .. _`preordered sets`: https://en.wikipedia.org/wiki/Preorder
 
+Publication
+============================================================
+
+Arfer, K. B. (2024). Artiruno: A free-software tool for multi-criteria decision-making with verbal decision analysis. *Journal of Multi-Criteria Decision Analysis, 31*. ``doi:10.1002/mcda.1827``. Retrieved from http://arfer.net/projects/artiruno/paper
+
 License
 ============================================================
 
-This program is copyright 2021, 2022 Kodi B. Arfer.
+This program is copyright 2024 Kodi B. Arfer.
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the `GNU General Public License`_ for more details.
 
 .. _`GNU General Public License`: http://www.gnu.org/licenses/
```

### Comparing `artiruno-0.4.2/README.rst` & `artiruno-0.4.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 .. image:: https://i.imgur.com/GlZ6CEM.png
   :alt: Art by Ken Sugimori
   :align: center
 
+.. role:: html(raw)
+   :format: html
+
 Artiruno is a program to help you make decisions with verbal decision analysis. It's also a Python library with a class for `preordered sets`_ that should be just as useful outside the context of decision-making.
 
 - `Try Artiruno in your web browser <http://arfer.net/projects/artiruno/webi>`_
 - `Documentation <http://arfer.net/projects/artiruno/doc>`_
 
 .. _`preordered sets`: https://en.wikipedia.org/wiki/Preorder
 
+Publication
+============================================================
+
+Arfer, K. B. (2024). Artiruno: A free-software tool for multi-criteria decision-making with verbal decision analysis. *Journal of Multi-Criteria Decision Analysis, 31*. ``doi:10.1002/mcda.1827``. Retrieved from http://arfer.net/projects/artiruno/paper
+
 License
 ============================================================
 
-This program is copyright 2021, 2022 Kodi B. Arfer.
+This program is copyright 2024 Kodi B. Arfer.
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the `GNU General Public License`_ for more details.
 
 .. _`GNU General Public License`: http://www.gnu.org/licenses/
```

### Comparing `artiruno-0.4.2/artiruno/__init__.py` & `artiruno-0.4.3/artiruno/__init__.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/artiruno/interactive.py` & `artiruno-0.4.3/artiruno/interactive.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/artiruno/preorder.py` & `artiruno-0.4.3/artiruno/preorder.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/artiruno/vda.py` & `artiruno-0.4.3/artiruno/vda.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/artiruno/web.py` & `artiruno-0.4.3/artiruno/web.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/artiruno.egg-info/PKG-INFO` & `artiruno-0.4.3/artiruno.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artiruno
-Version: 0.4.2
+Version: 0.4.3
 Summary: Verbal decision analysis
 Home-page: https://arfer.net/projects/artiruno
 Author: Kodi B. Arfer
 Project-URL: Documentation, https://arfer.net/projects/artiruno/doc
 Project-URL: Source Code, https://github.com/Kodiologist/Artiruno
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -14,24 +14,32 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 
 .. image:: https://i.imgur.com/GlZ6CEM.png
   :alt: Art by Ken Sugimori
   :align: center
 
+.. role:: html(raw)
+   :format: html
+
 Artiruno is a program to help you make decisions with verbal decision analysis. It's also a Python library with a class for `preordered sets`_ that should be just as useful outside the context of decision-making.
 
 - `Try Artiruno in your web browser <http://arfer.net/projects/artiruno/webi>`_
 - `Documentation <http://arfer.net/projects/artiruno/doc>`_
 
 .. _`preordered sets`: https://en.wikipedia.org/wiki/Preorder
 
+Publication
+============================================================
+
+Arfer, K. B. (2024). Artiruno: A free-software tool for multi-criteria decision-making with verbal decision analysis. *Journal of Multi-Criteria Decision Analysis, 31*. ``doi:10.1002/mcda.1827``. Retrieved from http://arfer.net/projects/artiruno/paper
+
 License
 ============================================================
 
-This program is copyright 2021, 2022 Kodi B. Arfer.
+This program is copyright 2024 Kodi B. Arfer.
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the `GNU General Public License`_ for more details.
 
 .. _`GNU General Public License`: http://www.gnu.org/licenses/
```

### Comparing `artiruno-0.4.2/conftest.py` & `artiruno-0.4.3/conftest.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/examples/jobs.json` & `artiruno-0.4.3/examples/jobs.json`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/pyodide_testing.py` & `artiruno-0.4.3/pyodide_testing.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/setup.py` & `artiruno-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/tests/test_preorder.py` & `artiruno-0.4.3/tests/test_preorder.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/tests/test_vda.py` & `artiruno-0.4.3/tests/test_vda.py`

 * *Files identical despite different names*

### Comparing `artiruno-0.4.2/webi.html` & `artiruno-0.4.3/webi.html`

 * *Files identical despite different names*

