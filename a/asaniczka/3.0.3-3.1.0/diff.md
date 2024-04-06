# Comparing `tmp/asaniczka-3.0.3.tar.gz` & `tmp/asaniczka-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaniczka-3.0.3.tar", last modified: Fri Mar  8 06:00:47 2024, max compression
+gzip compressed data, was "asaniczka-3.1.0.tar", last modified: Sat Apr  6 08:03:05 2024, max compression
```

## Comparing `asaniczka-3.0.3.tar` & `asaniczka-3.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 06:00:47.879393 asaniczka-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-08 06:00:47.879393 asaniczka-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-03-08 06:00:39.000000 asaniczka-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 06:00:47.879393 asaniczka-3.0.3/asaniczka/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-08 06:00:39.000000 asaniczka-3.0.3/asaniczka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-03-08 06:00:39.000000 asaniczka-3.0.3/asaniczka/db_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    33999 2024-03-08 06:00:39.000000 asaniczka-3.0.3/asaniczka/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-03-08 06:00:39.000000 asaniczka-3.0.3/asaniczka/scrape_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 06:00:47.879393 asaniczka-3.0.3/asaniczka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-08 06:00:47.000000 asaniczka-3.0.3/asaniczka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-08 06:00:47.000000 asaniczka-3.0.3/asaniczka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 06:00:47.000000 asaniczka-3.0.3/asaniczka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-08 06:00:47.000000 asaniczka-3.0.3/asaniczka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-08 06:00:47.000000 asaniczka-3.0.3/asaniczka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-08 06:00:39.000000 asaniczka-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 06:00:47.879393 asaniczka-3.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:03:05.365508 asaniczka-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 08:03:05.365508 asaniczka-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-06 08:03:00.000000 asaniczka-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:03:05.365508 asaniczka-3.1.0/asaniczka/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 08:03:00.000000 asaniczka-3.1.0/asaniczka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-04-06 08:03:00.000000 asaniczka-3.1.0/asaniczka/db_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33999 2024-04-06 08:03:00.000000 asaniczka-3.1.0/asaniczka/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14041 2024-04-06 08:03:00.000000 asaniczka-3.1.0/asaniczka/scrape_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:03:05.365508 asaniczka-3.1.0/asaniczka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 08:03:05.000000 asaniczka-3.1.0/asaniczka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-06 08:03:00.000000 asaniczka-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 08:03:05.365508 asaniczka-3.1.0/setup.cfg
```

### Comparing `asaniczka-3.0.3/PKG-INFO` & `asaniczka-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaniczka
-Version: 3.0.3
+Version: 3.1.0
 Summary: All my commonly used fuctions
 Author-email: Asaniczka <asaniczka@gmail.com>
 Maintainer-email: Asaniczka <asaniczka@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asaniczka/asaniczka_pip
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `asaniczka-3.0.3/README.md` & `asaniczka-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `asaniczka-3.0.3/asaniczka/db_tools.py` & `asaniczka-3.1.0/asaniczka/db_tools.py`

 * *Files identical despite different names*

### Comparing `asaniczka-3.0.3/asaniczka/main.py` & `asaniczka-3.1.0/asaniczka/main.py`

 * *Files identical despite different names*

### Comparing `asaniczka-3.0.3/asaniczka/scrape_helper.py` & `asaniczka-3.1.0/asaniczka/scrape_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,20 +77,26 @@
 
         ### Returns:
         - Does not explicitly return anything but updates the class attributes with parsed proxy data.
 
         ### Raises:
         - `IndexError`: If the split_proxy list does not have enough elements to assign to ip_address, port, username, and password.
         """
-
-        split_proxy = self.raw_string.split(":")
-        self.ip_address = split_proxy[0]
-        self.port = split_proxy[1]
-        self.username = split_proxy[2]
-        self.password = split_proxy[3]
+        try:
+            split_proxy = self.raw_string.split(":")
+            self.ip_address = split_proxy[0]
+            self.port = split_proxy[1]
+            self.username = split_proxy[2]
+            self.password = split_proxy[3]
+        except Exception as e:
+            print(e)
+            self.ip_address = ""
+            self.port = ""
+            self.username = ""
+            self.password = ""
 
     def to_playwright(self) -> dict:
         """
         Outputs the proxy to playwright proxy format.
 
         ### Args:
         - No explicit arguments taken as input directly. It accesses class attributes.
@@ -379,7 +385,65 @@
 
         return stolen_cookie_dict
 
     except Exception as error:
         raise RuntimeError(
             f"Error when stealing cookies. Please inform developer (asaniczka@gmail.com) of this error as this error is not handled. \n{asaniczka.format_error(error)}"
         ) from error
+
+
+def validate_proxies(proxies: list[Proxy]) -> list[Proxy]:
+    """
+    Checks if the provided proxies are live and returns only the live ones
+    """
+
+    def send_dummy_request(proxy: Proxy) -> Proxy | None:
+        response = asaniczka.get_request(
+            "https://api.ipify.org",
+            silence_exceptions=True,
+            timeout=5,
+            proxy=proxy.to_basic_auth(),
+        )
+
+        if response:
+            return proxy
+        return None
+
+    working_proxies = []
+    with concurrent.futures.ThreadPoolExecutor() as thread_executor:
+        futures = []
+
+        for proxy in proxies:
+            future = thread_executor.submit(send_dummy_request, proxy)
+
+            futures.append(future)
+
+        for future in concurrent.futures.as_completed(futures):
+            result = future.result()
+            if result:
+                working_proxies.append(result)
+
+    return working_proxies
+
+
+def download_proxies(url: str) -> list[Proxy]:
+    """
+    Downloads the proxies from your webshare live url
+    """
+
+    if not url:
+        raise ValueError("No URL provided")
+
+    if not url.startswith("https://proxy.webshare.io"):
+        raise ValueError("We only accept webshare URLS")
+
+    response = asaniczka.get_request(url, timeout=5)
+
+    if not response:
+        raise ValueError("URL didn't recieve any data")
+
+    lines = response.split("\n")
+    lines = [line.strip() for line in lines]
+    proxies = [Proxy(line, ProxyProvider.WEBSHARE) for line in lines]
+
+    working_proxies = validate_proxies(proxies)
+    print("You have ", len(working_proxies), " working proxies!")
```

### Comparing `asaniczka-3.0.3/asaniczka.egg-info/PKG-INFO` & `asaniczka-3.1.0/asaniczka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaniczka
-Version: 3.0.3
+Version: 3.1.0
 Summary: All my commonly used fuctions
 Author-email: Asaniczka <asaniczka@gmail.com>
 Maintainer-email: Asaniczka <asaniczka@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asaniczka/asaniczka_pip
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `asaniczka-3.0.3/pyproject.toml` & `asaniczka-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools >= 61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "asaniczka"
-version = "3.0.3"
+version = "3.1.0"
 description = "All my commonly used fuctions"
 readme = "README.md"
 dependencies = [
   "pytz>=2022.1",
   "requests>=2.0",
   "playwright>=1.0.0",
   "tqdm>=4.0.0",
```

