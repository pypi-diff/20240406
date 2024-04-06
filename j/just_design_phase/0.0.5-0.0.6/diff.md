# Comparing `tmp/just_design_phase-0.0.5.tar.gz` & `tmp/just_design_phase-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just_design_phase-0.0.5.tar", max compression
+gzip compressed data, was "just_design_phase-0.0.6.tar", max compression
```

## Comparing `just_design_phase-0.0.5.tar` & `just_design_phase-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2055 2024-04-04 15:35:07.458395 just_design_phase-0.0.5/README.md
--rw-r--r--   0        0        0       99 2024-04-06 07:32:28.456236 just_design_phase-0.0.5/just_design_phase/__init__.py
--rw-r--r--   0        0        0      362 2024-04-06 07:47:08.007778 just_design_phase-0.0.5/just_design_phase/kite_login.py
--rw-r--r--   0        0        0      825 2024-04-06 07:25:26.567494 just_design_phase-0.0.5/just_design_phase/main.py
--rw-r--r--   0        0        0     1011 2024-04-05 16:53:16.515023 just_design_phase-0.0.5/just_design_phase/models/generate_session_model.py
--rw-r--r--   0        0        0      518 2024-04-05 16:53:21.278048 just_design_phase-0.0.5/just_design_phase/models/login_url_model.py
--rw-r--r--   0        0        0     1368 2024-04-05 17:03:25.841691 just_design_phase-0.0.5/just_design_phase/models/place_normal_order_model.py
--rw-r--r--   0        0        0      556 2024-04-06 07:47:13.236096 just_design_phase-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 just_design_phase-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2055 2024-04-04 15:35:07.458395 just_design_phase-0.0.6/README.md
+-rw-r--r--   0        0        0       99 2024-04-06 07:32:28.456236 just_design_phase-0.0.6/just_design_phase/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-06 07:48:46.947736 just_design_phase-0.0.6/just_design_phase/kite_login.py
+-rw-r--r--   0        0        0      825 2024-04-06 07:25:26.567494 just_design_phase-0.0.6/just_design_phase/main.py
+-rw-r--r--   0        0        0     1011 2024-04-05 16:53:16.515023 just_design_phase-0.0.6/just_design_phase/models/generate_session_model.py
+-rw-r--r--   0        0        0      518 2024-04-05 16:53:21.278048 just_design_phase-0.0.6/just_design_phase/models/login_url_model.py
+-rw-r--r--   0        0        0     1368 2024-04-05 17:03:25.841691 just_design_phase-0.0.6/just_design_phase/models/place_normal_order_model.py
+-rw-r--r--   0        0        0      556 2024-04-06 07:48:55.587514 just_design_phase-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 just_design_phase-0.0.6/PKG-INFO
```

### Comparing `just_design_phase-0.0.5/README.md` & `just_design_phase-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.5/just_design_phase/main.py` & `just_design_phase-0.0.6/just_design_phase/main.py`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.5/just_design_phase/models/generate_session_model.py` & `just_design_phase-0.0.6/just_design_phase/models/generate_session_model.py`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.5/just_design_phase/models/login_url_model.py` & `just_design_phase-0.0.6/just_design_phase/models/login_url_model.py`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.5/just_design_phase/models/place_normal_order_model.py` & `just_design_phase-0.0.6/just_design_phase/models/place_normal_order_model.py`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.5/pyproject.toml` & `just_design_phase-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "just_design_phase"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["AST-LW <walkthroughfrom2020@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 kiteconnect = "^5.0.1"
```

### Comparing `just_design_phase-0.0.5/PKG-INFO` & `just_design_phase-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: just_design_phase
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: AST-LW
 Author-email: walkthroughfrom2020@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

