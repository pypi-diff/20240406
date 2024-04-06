# Comparing `tmp/just_design_phase-0.0.7.tar.gz` & `tmp/just_design_phase-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "just_design_phase-0.0.7.tar", max compression
+gzip compressed data, was "just_design_phase-0.0.8.tar", max compression
```

## Comparing `just_design_phase-0.0.7.tar` & `just_design_phase-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2055 2024-04-04 15:35:07.458395 just_design_phase-0.0.7/README.md
--rw-r--r--   0        0        0       99 2024-04-06 07:32:28.456236 just_design_phase-0.0.7/just_design_phase/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-06 08:20:04.861631 just_design_phase-0.0.7/just_design_phase/kite_login.py
--rw-r--r--   0        0        0      818 2024-04-06 08:18:47.863544 just_design_phase-0.0.7/just_design_phase/main.py
--rw-r--r--   0        0        0     1011 2024-04-05 16:53:16.515023 just_design_phase-0.0.7/just_design_phase/models/generate_session_model.py
--rw-r--r--   0        0        0      518 2024-04-05 16:53:21.278048 just_design_phase-0.0.7/just_design_phase/models/login_url_model.py
--rw-r--r--   0        0        0     1368 2024-04-05 17:03:25.841691 just_design_phase-0.0.7/just_design_phase/models/place_normal_order_model.py
--rw-r--r--   0        0        0      556 2024-04-06 08:19:37.769201 just_design_phase-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 just_design_phase-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     2055 2024-04-04 15:35:07.458395 just_design_phase-0.0.8/README.md
+-rw-r--r--   0        0        0       99 2024-04-06 07:32:28.456236 just_design_phase-0.0.8/just_design_phase/__init__.py
+-rw-r--r--   0        0        0     1264 2024-04-06 08:21:52.255062 just_design_phase-0.0.8/just_design_phase/kite_login.py
+-rw-r--r--   0        0        0      818 2024-04-06 08:18:47.863544 just_design_phase-0.0.8/just_design_phase/main.py
+-rw-r--r--   0        0        0     1011 2024-04-05 16:53:16.515023 just_design_phase-0.0.8/just_design_phase/models/generate_session_model.py
+-rw-r--r--   0        0        0      518 2024-04-05 16:53:21.278048 just_design_phase-0.0.8/just_design_phase/models/login_url_model.py
+-rw-r--r--   0        0        0     1368 2024-04-05 17:03:25.841691 just_design_phase-0.0.8/just_design_phase/models/place_normal_order_model.py
+-rw-r--r--   0        0        0      556 2024-04-06 08:21:57.780767 just_design_phase-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 just_design_phase-0.0.8/PKG-INFO
```

### Comparing `just_design_phase-0.0.7/README.md` & `just_design_phase-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.7/just_design_phase/kite_login.py` & `just_design_phase-0.0.8/just_design_phase/kite_login.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 find_dotenv(load_dotenv())
 
 PROJECT_ROOT = os.path.abspath("")
 
 KITE_API_KEY = os.getenv("KITE_API_KEY")
 KITE_API_SECRET = os.getenv("KITE_API_SECRET")
 
-access_token_file = f"zerodha_access_token_{
-    datetime.now().date()}.txt"
+access_token_file = f"zerodha_access_token_{datetime.now().date()}.txt"
 
 
 def login():
     kite = KiteConnect(api_key=KITE_API_KEY)
 
     if access_token_file not in os.listdir():
         print("Fetch request token by logging into the following url: \n")
@@ -39,8 +38,10 @@
         kite.set_access_token(access_token)
 
     return kite
 
 
 # kite = login()
 
+kite = None
+
 print(os.getenv("KITE_API_KEY"))
```

### Comparing `just_design_phase-0.0.7/just_design_phase/main.py` & `just_design_phase-0.0.8/just_design_phase/main.py`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.7/just_design_phase/models/generate_session_model.py` & `just_design_phase-0.0.8/just_design_phase/models/generate_session_model.py`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.7/just_design_phase/models/login_url_model.py` & `just_design_phase-0.0.8/just_design_phase/models/login_url_model.py`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.7/just_design_phase/models/place_normal_order_model.py` & `just_design_phase-0.0.8/just_design_phase/models/place_normal_order_model.py`

 * *Files identical despite different names*

### Comparing `just_design_phase-0.0.7/pyproject.toml` & `just_design_phase-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "just_design_phase"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["AST-LW <walkthroughfrom2020@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 kiteconnect = "^5.0.1"
```

### Comparing `just_design_phase-0.0.7/PKG-INFO` & `just_design_phase-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: just_design_phase
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: AST-LW
 Author-email: walkthroughfrom2020@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

