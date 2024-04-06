# Comparing `tmp/python_115-0.0.5.9.tar.gz` & `tmp/python_115-0.0.5.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_115-0.0.5.9.tar", max compression
+gzip compressed data, was "python_115-0.0.5.9.1.tar", max compression
```

## Comparing `python_115-0.0.5.9.tar` & `python_115-0.0.5.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.9/LICENSE
--rw-r--r--   0        0        0   263878 2024-04-06 09:57:04.283346 python_115-0.0.5.9/p115/__init__.py
--rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.9/p115/__main__.py
--rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.9/p115/exception.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.9/p115/py.typed
--rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.9/p115/util/__init__.py
--rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.9/p115/util/_init_mimetypes.py
--rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.9/p115/util/args.py
--rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.9/p115/util/cipher.py
--rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.9/p115/util/concurrent.py
--rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.9/p115/util/download.py
--rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.9/p115/util/file.py
--rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.9/p115/util/hash.py
--rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.9/p115/util/ignore.py
--rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.9/p115/util/iter.py
--rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.9/p115/util/path.py
--rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.9/p115/util/property.py
--rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.9/p115/util/response.py
--rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.9/p115/util/retry.py
--rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.9/p115/util/text.py
--rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.9/p115/util/upload.py
--rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.9/p115/util/urlopen.py
--rw-r--r--   0        0        0     1272 2024-04-06 09:59:36.533085 python_115-0.0.5.9/pyproject.toml
--rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.9/readme.md
--rw-r--r--   0        0        0    35896 1970-01-01 00:00:00.000000 python_115-0.0.5.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2023-10-11 13:48:41.987287 python_115-0.0.5.9.1/LICENSE
+-rw-r--r--   0        0        0   263879 2024-04-06 11:52:54.748855 python_115-0.0.5.9.1/p115/__init__.py
+-rw-r--r--   0        0        0       64 2023-12-07 13:04:33.452726 python_115-0.0.5.9.1/p115/__main__.py
+-rw-r--r--   0        0        0      179 2023-12-22 08:44:22.766732 python_115-0.0.5.9.1/p115/exception.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_115-0.0.5.9.1/p115/py.typed
+-rw-r--r--   0        0        0       87 2023-12-19 14:25:03.149217 python_115-0.0.5.9.1/p115/util/__init__.py
+-rw-r--r--   0        0        0     4329 2023-11-24 07:50:22.455279 python_115-0.0.5.9.1/p115/util/_init_mimetypes.py
+-rw-r--r--   0        0        0      360 2024-02-08 06:48:55.081770 python_115-0.0.5.9.1/p115/util/args.py
+-rw-r--r--   0        0        0     7920 2023-12-14 11:02:29.316261 python_115-0.0.5.9.1/p115/util/cipher.py
+-rw-r--r--   0        0        0     5671 2024-04-03 04:46:18.484632 python_115-0.0.5.9.1/p115/util/concurrent.py
+-rw-r--r--   0        0        0    12120 2024-04-03 04:46:18.485585 python_115-0.0.5.9.1/p115/util/download.py
+-rw-r--r--   0        0        0    15103 2024-04-03 05:18:09.304611 python_115-0.0.5.9.1/p115/util/file.py
+-rw-r--r--   0        0        0     4507 2023-12-08 06:07:31.193403 python_115-0.0.5.9.1/p115/util/hash.py
+-rw-r--r--   0        0        0    10070 2024-01-12 05:37:18.775493 python_115-0.0.5.9.1/p115/util/ignore.py
+-rw-r--r--   0        0        0     2822 2024-02-13 03:37:52.593362 python_115-0.0.5.9.1/p115/util/iter.py
+-rw-r--r--   0        0        0     4562 2024-01-16 05:10:10.057134 python_115-0.0.5.9.1/p115/util/path.py
+-rw-r--r--   0        0        0     1794 2024-01-15 14:50:38.503730 python_115-0.0.5.9.1/p115/util/property.py
+-rw-r--r--   0        0        0     3190 2024-01-29 10:59:02.879730 python_115-0.0.5.9.1/p115/util/response.py
+-rw-r--r--   0        0        0     6122 2024-01-15 15:35:49.895519 python_115-0.0.5.9.1/p115/util/retry.py
+-rw-r--r--   0        0        0     6785 2024-02-09 07:54:09.097617 python_115-0.0.5.9.1/p115/util/text.py
+-rw-r--r--   0        0        0       43 2024-04-03 05:08:27.538028 python_115-0.0.5.9.1/p115/util/upload.py
+-rw-r--r--   0        0        0    10029 2024-01-29 10:52:22.271824 python_115-0.0.5.9.1/p115/util/urlopen.py
+-rw-r--r--   0        0        0     1274 2024-04-06 11:53:11.617183 python_115-0.0.5.9.1/pyproject.toml
+-rw-r--r--   0        0        0    34641 2024-01-05 10:56:58.191328 python_115-0.0.5.9.1/readme.md
+-rw-r--r--   0        0        0    35898 1970-01-01 00:00:00.000000 python_115-0.0.5.9.1/PKG-INFO
```

### Comparing `python_115-0.0.5.9/LICENSE` & `python_115-0.0.5.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/__init__.py` & `python_115-0.0.5.9.1/p115/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1796,15 +1796,15 @@
                 if strict and not url:
                     raise IsADirectoryError(errno.EISDIR, f"{fid} is a directory")
                 if not detail:
                     return url["url"] if url else ""
                 return UrlStr(
                     url["url"] if url else "", 
                     id=int(fid), 
-                    pickcode=info["pickcode"], 
+                    pickcode=info["pick_code"], 
                     file_name=info["file_name"], 
                     file_size=int(info["file_size"]), 
                     is_directory=not url,
                 )
             raise FileNotFoundError(errno.ENOENT, f"no such pickcode: {pickcode!r}")
         if async_:
             async def wrapper() -> str:
```

### Comparing `python_115-0.0.5.9/p115/util/_init_mimetypes.py` & `python_115-0.0.5.9.1/p115/util/_init_mimetypes.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/cipher.py` & `python_115-0.0.5.9.1/p115/util/cipher.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/concurrent.py` & `python_115-0.0.5.9.1/p115/util/concurrent.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/download.py` & `python_115-0.0.5.9.1/p115/util/download.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/file.py` & `python_115-0.0.5.9.1/p115/util/file.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/hash.py` & `python_115-0.0.5.9.1/p115/util/hash.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/ignore.py` & `python_115-0.0.5.9.1/p115/util/ignore.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/iter.py` & `python_115-0.0.5.9.1/p115/util/iter.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/path.py` & `python_115-0.0.5.9.1/p115/util/path.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/property.py` & `python_115-0.0.5.9.1/p115/util/property.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/response.py` & `python_115-0.0.5.9.1/p115/util/response.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/retry.py` & `python_115-0.0.5.9.1/p115/util/retry.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/text.py` & `python_115-0.0.5.9.1/p115/util/text.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/p115/util/urlopen.py` & `python_115-0.0.5.9.1/p115/util/urlopen.py`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/pyproject.toml` & `python_115-0.0.5.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-115"
-version = "0.0.5.9"
+version = "0.0.5.9.1"
 description = "Python wrapper for 115 webdisk."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client"
 keywords = ["nas", "115"]
```

### Comparing `python_115-0.0.5.9/readme.md` & `python_115-0.0.5.9.1/readme.md`

 * *Files identical despite different names*

### Comparing `python_115-0.0.5.9/PKG-INFO` & `python_115-0.0.5.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-115
-Version: 0.0.5.9
+Version: 0.0.5.9.1
 Summary: Python wrapper for 115 webdisk.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-115-client
 License: MIT
 Keywords: nas,115
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.11,<4.0
```

