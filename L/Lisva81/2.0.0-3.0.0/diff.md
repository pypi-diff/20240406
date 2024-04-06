# Comparing `tmp/Lisva81-2.0.0.tar.gz` & `tmp/Lisva81-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lisva81-2.0.0.tar", last modified: Mon Apr  1 05:43:39 2024, max compression
+gzip compressed data, was "Lisva81-3.0.0.tar", last modified: Fri Apr  5 19:58:15 2024, max compression
```

## Comparing `Lisva81-2.0.0.tar` & `Lisva81-3.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 05:43:39.742524 Lisva81-2.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 Lisva81-2.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-01 05:43:39.676520 Lisva81-2.0.0/Lisva81/
--rw-rw-rw-   0        0        0     5654 2024-04-01 05:42:26.000000 Lisva81-2.0.0/Lisva81/__init__.py
--rw-rw-rw-   0        0        0       75 2024-04-01 05:42:42.000000 Lisva81-2.0.0/Lisva81/version.py
-drwxrwxrwx   0        0        0        0 2024-04-01 05:43:39.732523 Lisva81-2.0.0/Lisva81.egg-info/
--rw-rw-rw-   0        0        0      992 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-01 05:43:38.000000 Lisva81-2.0.0/Lisva81.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/zip-safe
--rw-rw-rw-   0        0        0      992 2024-04-01 05:43:39.739523 Lisva81-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 Lisva81-2.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 05:43:39.743523 Lisva81-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1605 2024-02-24 05:09:28.000000 Lisva81-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:58:15.061356 Lisva81-3.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 Lisva81-3.0.0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-05 19:58:14.999353 Lisva81-3.0.0/Lisva81/
+-rw-rw-rw-   0        0        0     5755 2024-04-05 19:56:55.000000 Lisva81-3.0.0/Lisva81/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-05 19:57:03.000000 Lisva81-3.0.0/Lisva81/version.py
+drwxrwxrwx   0        0        0        0 2024-04-05 19:58:15.053356 Lisva81-3.0.0/Lisva81.egg-info/
+-rw-rw-rw-   0        0        0      992 2024-04-05 19:58:12.000000 Lisva81-3.0.0/Lisva81.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-05 19:58:13.000000 Lisva81-3.0.0/Lisva81.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 19:58:12.000000 Lisva81-3.0.0/Lisva81.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-05 19:58:13.000000 Lisva81-3.0.0/Lisva81.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 19:58:13.000000 Lisva81-3.0.0/Lisva81.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-05 19:58:12.000000 Lisva81-3.0.0/Lisva81.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      992 2024-04-05 19:58:15.058356 Lisva81-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 Lisva81-3.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-05 19:58:15.064356 Lisva81-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1605 2024-02-24 05:09:28.000000 Lisva81-3.0.0/setup.py
```

### Comparing `Lisva81-2.0.0/LICENSE` & `Lisva81-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Lisva81-2.0.0/Lisva81/__init__.py` & `Lisva81-3.0.0/Lisva81/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,20 +64,22 @@
         total_size = int(data[0])
         ids = data[1]
         filename = data[2].split("?")[-1]
         values = data[2].split("?"+filename)[0].split("?")
         type = "r"
         id = ""
         host = f"https://cujae.edu.cu/index.php/r/$$$call$$$/api/file/file-api/download-file?submissionFileId=*&submissionId={ids}&stageId=1"
-    elif "revgacetaestudiantil.sld" in dl:
-        filename = dl.split("/")[-1]
-        total_size = int(dl.split("/"+filename)[0].split("/")[-1])
-        url = dl.split("/"+size)[0]
-        type = "rv"
-        id = 0
+    elif "revinformatica.sld.cu" in dl:
+        value = dl.split("rcim/")[1].split("/")
+        url = f"https://nube.uo.edu.cu/remote.php/dav/uploads/{value[0]}/web-file-upload-{value[1]}/.file"
+        filename = value[3]
+        total_size = int(value[2])
+        type = "uo"
+        id = "11"
+        print(value)
     else:
         url = dl.split("{")[0]+".file"
         filename = dl.split("/")[-1]
         id = dl.split("{")[1].split("}")[0]
         total_size = int(dl.split("}/")[1].split("/")[0])
         type = "uo"
```

### Comparing `Lisva81-2.0.0/Lisva81.egg-info/PKG-INFO` & `Lisva81-3.0.0/Lisva81.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lisva81
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/downfree
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Lisva81-2.0.0/PKG-INFO` & `Lisva81-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lisva81
-Version: 2.0.0
+Version: 3.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/downfree
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Lisva81-2.0.0/README.md` & `Lisva81-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Lisva81-2.0.0/setup.py` & `Lisva81-3.0.0/setup.py`

 * *Files identical despite different names*

