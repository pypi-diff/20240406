# Comparing `tmp/scrapy-playwright-full-0.0.3401.tar.gz` & `tmp/scrapy-playwright-full-0.0.3402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-playwright-full-0.0.3401.tar", last modified: Mon Feb 19 10:55:34 2024, max compression
+gzip compressed data, was "scrapy-playwright-full-0.0.3402.tar", last modified: Sat Apr  6 19:24:13 2024, max compression
```

## Comparing `scrapy-playwright-full-0.0.3401.tar` & `scrapy-playwright-full-0.0.3402.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:55:34.360182 scrapy-playwright-full-0.0.3401/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35581 2024-02-19 10:55:34.360182 scrapy-playwright-full-0.0.3401/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:55:34.360182 scrapy-playwright-full-0.0.3401/scrapy_playwright/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33769 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright/memusage.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 10:55:34.360182 scrapy-playwright-full-0.0.3401/scrapy_playwright_full.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35581 2024-02-19 10:55:34.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright_full.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-19 10:55:34.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright_full.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 10:55:34.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright_full.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-19 10:55:34.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright_full.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-19 10:55:34.000000 scrapy-playwright-full-0.0.3401/scrapy_playwright_full.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-19 10:55:34.360182 scrapy-playwright-full-0.0.3401/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-19 10:55:26.000000 scrapy-playwright-full-0.0.3401/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:13.581943 scrapy-playwright-full-0.0.3402/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-04-06 19:24:13.581943 scrapy-playwright-full-0.0.3402/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34512 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:13.577943 scrapy-playwright-full-0.0.3402/scrapy_playwright/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33235 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright/memusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:13.581943 scrapy-playwright-full-0.0.3402/scrapy_playwright_full.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35611 2024-04-06 19:24:13.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright_full.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-06 19:24:13.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright_full.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:24:13.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright_full.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-06 19:24:13.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright_full.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 19:24:13.000000 scrapy-playwright-full-0.0.3402/scrapy_playwright_full.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 19:24:13.581943 scrapy-playwright-full-0.0.3402/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-06 19:24:05.000000 scrapy-playwright-full-0.0.3402/setup.py
```

### Comparing `scrapy-playwright-full-0.0.3401/LICENSE` & `scrapy-playwright-full-0.0.3402/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3401/PKG-INFO` & `scrapy-playwright-full-0.0.3402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright-full
-Version: 0.0.3401
+Version: 0.0.3402
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -20,14 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scrapy!=2.4.0,>=2.0
 Requires-Dist: playwright>=1.15
+Requires-Dist: dektools<1.0.0
 
 # scrapy-playwright: Playwright integration for Scrapy
 [![version](https://img.shields.io/pypi/v/scrapy-playwright.svg)](https://pypi.python.org/pypi/scrapy-playwright)
 [![pyversions](https://img.shields.io/pypi/pyversions/scrapy-playwright.svg)](https://pypi.python.org/pypi/scrapy-playwright)
 [![Tests](https://github.com/scrapy-plugins/scrapy-playwright/actions/workflows/tests.yml/badge.svg)](https://github.com/scrapy-plugins/scrapy-playwright/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/scrapy-plugins/scrapy-playwright/branch/master/graph/badge.svg)](https://codecov.io/gh/scrapy-plugins/scrapy-playwright)
```

### Comparing `scrapy-playwright-full-0.0.3401/README.md` & `scrapy-playwright-full-0.0.3402/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3401/scrapy_playwright/_utils.py` & `scrapy-playwright-full-0.0.3402/scrapy_playwright/_utils.py`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3401/scrapy_playwright/handler.py` & `scrapy-playwright-full-0.0.3402/scrapy_playwright/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,48 +39,37 @@
     _get_page_content,
     _is_safe_close_error,
     _maybe_await,
 )
 
 # Supporting for Windows
 if sys.platform == "win32" and sys.version_info >= (3, 8):
-    import threading
+    from dektools.sync import EnvSet
 
-    class Var:
-        windows_loop = None
-        windows_thread = None
-
-    def windows_get_asyncio_event_loop():
-        if Var.windows_thread is None:
-            if Var.windows_loop is None:
-                Var.windows_loop = asyncio.WindowsProactorEventLoopPolicy().new_event_loop()
-                asyncio.set_event_loop(Var.windows_loop)
-            if not Var.windows_loop.is_running():
-                Var.windows_thread = threading.Thread(
-                    target=Var.windows_loop.run_forever, daemon=True
-                )
-                Var.windows_thread.start()
-        return Var.windows_loop
+    class WindowsEnvSet(EnvSet):
+        event_loop_policy_cls = asyncio.WindowsProactorEventLoopPolicy
+
+    windows_env_set = WindowsEnvSet()
 
     async def windows_get_result(o):
-        return asyncio.run_coroutine_threadsafe(o, windows_get_asyncio_event_loop()).result()
+        return windows_env_set.coroutine(o)
 
     def deferred_from_coro(o):
         if isinstance(o, Deferred):
             return o
         return deferred_from_coro_default(windows_get_result(o))
 
 else:
-    windows_get_asyncio_event_loop = None
+    windows_env_set = None
     windows_get_result = None
     deferred_from_coro = deferred_from_coro_default
 
 __all__ = [
     "ScrapyPlaywrightDownloadHandler",
-    "windows_get_asyncio_event_loop",
+    "windows_env_set",
     "windows_get_result",
 ]
 
 PlaywrightHandler = TypeVar("PlaywrightHandler", bound="ScrapyPlaywrightDownloadHandler")
 
 logger = logging.getLogger("scrapy-playwright")
```

### Comparing `scrapy-playwright-full-0.0.3401/scrapy_playwright/headers.py` & `scrapy-playwright-full-0.0.3402/scrapy_playwright/headers.py`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3401/scrapy_playwright/memusage.py` & `scrapy-playwright-full-0.0.3402/scrapy_playwright/memusage.py`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3401/scrapy_playwright/page.py` & `scrapy-playwright-full-0.0.3402/scrapy_playwright/page.py`

 * *Files identical despite different names*

### Comparing `scrapy-playwright-full-0.0.3401/scrapy_playwright_full.egg-info/PKG-INFO` & `scrapy-playwright-full-0.0.3402/scrapy_playwright_full.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-playwright-full
-Version: 0.0.3401
+Version: 0.0.3402
 Summary: Playwright integration for Scrapy
 Home-page: https://github.com/scrapy-plugins/scrapy-playwright
 Author: Eugenio Lacuesta
 Author-email: eugenio.lacuesta@gmail.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
@@ -20,14 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scrapy!=2.4.0,>=2.0
 Requires-Dist: playwright>=1.15
+Requires-Dist: dektools<1.0.0
 
 # scrapy-playwright: Playwright integration for Scrapy
 [![version](https://img.shields.io/pypi/v/scrapy-playwright.svg)](https://pypi.python.org/pypi/scrapy-playwright)
 [![pyversions](https://img.shields.io/pypi/pyversions/scrapy-playwright.svg)](https://pypi.python.org/pypi/scrapy-playwright)
 [![Tests](https://github.com/scrapy-plugins/scrapy-playwright/actions/workflows/tests.yml/badge.svg)](https://github.com/scrapy-plugins/scrapy-playwright/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/scrapy-plugins/scrapy-playwright/branch/master/graph/badge.svg)](https://codecov.io/gh/scrapy-plugins/scrapy-playwright)
```

### Comparing `scrapy-playwright-full-0.0.3401/setup.py` & `scrapy-playwright-full-0.0.3402/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,9 +33,10 @@
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.8",
     install_requires=[
         "scrapy>=2.0,!=2.4.0",
         "playwright>=1.15",
+        "dektools<1.0.0",
     ],
 )
```

