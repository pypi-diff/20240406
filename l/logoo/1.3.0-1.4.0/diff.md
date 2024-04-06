# Comparing `tmp/logoo-1.3.0.tar.gz` & `tmp/logoo-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logoo-1.3.0.tar", last modified: Tue Mar 26 11:59:53 2024, max compression
+gzip compressed data, was "logoo-1.4.0.tar", last modified: Sat Apr  6 03:41:16 2024, max compression
```

## Comparing `logoo-1.3.0.tar` & `logoo-1.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-03-26 11:59:53.872030 logoo-1.3.0/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1071 2024-03-02 13:40:11.000000 logoo-1.3.0/LICENSE
--rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2830 2024-03-26 11:59:53.872030 logoo-1.3.0/PKG-INFO
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2240 2024-03-07 09:08:45.000000 logoo-1.3.0/README.md
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-03-26 11:59:53.868030 logoo-1.3.0/logoo/
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      372 2024-03-26 11:59:45.000000 logoo-1.3.0/logoo/__init__.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       66 2024-03-02 13:50:49.000000 logoo-1.3.0/logoo/data.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2413 2024-03-26 11:48:22.000000 logoo-1.3.0/logoo/logger.py
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5425 2024-03-26 11:59:31.000000 logoo-1.3.0/logoo/primary_logger.py
-drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-03-26 11:59:53.868030 logoo-1.3.0/logoo.egg-info/
--rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2830 2024-03-26 11:59:53.000000 logoo-1.3.0/logoo.egg-info/PKG-INFO
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      242 2024-03-26 11:59:53.000000 logoo-1.3.0/logoo.egg-info/SOURCES.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2024-03-26 11:59:53.000000 logoo-1.3.0/logoo.egg-info/dependency_links.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       36 2024-03-26 11:59:53.000000 logoo-1.3.0/logoo.egg-info/requires.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        6 2024-03-26 11:59:53.000000 logoo-1.3.0/logoo.egg-info/top_level.txt
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2024-03-26 11:59:53.872030 logoo-1.3.0/setup.cfg
--rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1377 2024-03-04 06:21:58.000000 logoo-1.3.0/setup.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-06 03:41:16.972739 logoo-1.4.0/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1071 2024-03-02 13:40:11.000000 logoo-1.4.0/LICENSE
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2830 2024-04-06 03:41:16.972739 logoo-1.4.0/PKG-INFO
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2240 2024-03-07 09:08:45.000000 logoo-1.4.0/README.md
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-06 03:41:16.968739 logoo-1.4.0/logoo/
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      372 2024-04-06 03:36:57.000000 logoo-1.4.0/logoo/__init__.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       66 2024-03-02 13:50:49.000000 logoo-1.4.0/logoo/data.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     2402 2024-04-06 03:23:07.000000 logoo-1.4.0/logoo/logger.py
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     5538 2024-04-06 03:14:06.000000 logoo-1.4.0/logoo/primary_logger.py
+drwxrwxr-x   0 skelmis   (1000) skelmis   (1000)        0 2024-04-06 03:41:16.972739 logoo-1.4.0/logoo.egg-info/
+-rw-r--r--   0 skelmis   (1000) skelmis   (1000)     2830 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/PKG-INFO
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)      242 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        1 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       36 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/requires.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)        6 2024-04-06 03:41:16.000000 logoo-1.4.0/logoo.egg-info/top_level.txt
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)       38 2024-04-06 03:41:16.972739 logoo-1.4.0/setup.cfg
+-rw-rw-r--   0 skelmis   (1000) skelmis   (1000)     1377 2024-03-04 06:21:58.000000 logoo-1.4.0/setup.py
```

### Comparing `logoo-1.3.0/LICENSE` & `logoo-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logoo-1.3.0/PKG-INFO` & `logoo-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logoo
-Version: 1.3.0
+Version: 1.4.0
 Summary: Openobserve log ingestion made simple.
 Author: Skelmis
 Author-email: skelmis.craft@gmail.com
 Project-URL: Issue tracker, https://github.com/Skelmis/logoo/issues
 Project-URL: Homepage, https://github.com/Skelmis/logoo
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `logoo-1.3.0/README.md` & `logoo-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `logoo-1.3.0/logoo/logger.py` & `logoo-1.4.0/logoo/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,17 +48,17 @@
         message = message % args
 
         log = {
             "level": level,
             "message": message,
             "source": self.name,
             "_timestamp.timezone": "UTC",
-            # We do this to get microseconds included
-            # Open to a better way to do it please
-            "_timestamp": str(created_at.timestamp()).replace(".", ""),
+            # We do this twice as OpenObserve will convert
+            # _timestamp to microseconds within their UI
+            "_timestamp": created_at.isoformat(),
             "_timestamp.iso_format": created_at.isoformat(),
         }
         if self.extra_metadata is not None:
             log = {**log, **self.extra_metadata}
         if extra_metadata is not None:
             log = {**log, **extra_metadata}
```

### Comparing `logoo-1.3.0/logoo/primary_logger.py` & `logoo-1.4.0/logoo/primary_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,19 +137,20 @@
 
                     resp_body = resp.json()
                     if resp_body.get("code") == 200:
                         for stream in resp_body.get("status", []):
                             success = int(stream.get("successful", 0))
                             failure = int(stream.get("failed", 0))
                             log.debug(
-                                "Sent %s logs to stream %s. %s successful, %s failed",
+                                "Sent %s logs to stream %s. %s successful, %s failed%s",
                                 success + failure,
                                 stream.get("name"),
                                 success,
                                 failure,
+                                f'\n\tError: {stream.get("error")}' if stream.get("error") is not None else ""
                             )
 
                     else:
                         log.error("Something went wrong uploading logs: %s", resp_body)
 
         except Exception as e:
             log.critical(
```

### Comparing `logoo-1.3.0/logoo.egg-info/PKG-INFO` & `logoo-1.4.0/logoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logoo
-Version: 1.3.0
+Version: 1.4.0
 Summary: Openobserve log ingestion made simple.
 Author: Skelmis
 Author-email: skelmis.craft@gmail.com
 Project-URL: Issue tracker, https://github.com/Skelmis/logoo/issues
 Project-URL: Homepage, https://github.com/Skelmis/logoo
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `logoo-1.3.0/setup.py` & `logoo-1.4.0/setup.py`

 * *Files identical despite different names*

