# Comparing `tmp/loadimg-0.0.3.tar.gz` & `tmp/loadimg-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadimg-0.0.3.tar", last modified: Tue Mar 26 03:51:29 2024, max compression
+gzip compressed data, was "loadimg-0.1.0.tar", last modified: Sat Apr  6 06:58:39 2024, max compression
```

## Comparing `loadimg-0.0.3.tar` & `loadimg-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:51:29.145889 loadimg-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-26 03:51:24.000000 loadimg-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-26 03:51:29.145889 loadimg-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-26 03:51:24.000000 loadimg-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-26 03:51:24.000000 loadimg-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 03:51:29.145889 loadimg-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-26 03:51:24.000000 loadimg-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:51:29.141888 loadimg-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:51:29.141888 loadimg-0.0.3/src/loadimg/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-26 03:51:24.000000 loadimg-0.0.3/src/loadimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-26 03:51:24.000000 loadimg-0.0.3/src/loadimg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 03:51:29.141888 loadimg-0.0.3/src/loadimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-26 03:51:29.000000 loadimg-0.0.3/src/loadimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-26 03:51:29.000000 loadimg-0.0.3/src/loadimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 03:51:29.000000 loadimg-0.0.3/src/loadimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-26 03:51:29.000000 loadimg-0.0.3/src/loadimg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:58:39.528566 loadimg-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 06:58:35.000000 loadimg-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-06 06:58:39.528566 loadimg-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 06:58:35.000000 loadimg-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-06 06:58:35.000000 loadimg-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 06:58:39.528566 loadimg-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-06 06:58:35.000000 loadimg-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:58:39.524567 loadimg-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:58:39.524567 loadimg-0.1.0/src/loadimg/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 06:58:35.000000 loadimg-0.1.0/src/loadimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-06 06:58:35.000000 loadimg-0.1.0/src/loadimg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:58:39.528566 loadimg-0.1.0/src/loadimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-06 06:58:39.000000 loadimg-0.1.0/src/loadimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-06 06:58:39.000000 loadimg-0.1.0/src/loadimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:58:39.000000 loadimg-0.1.0/src/loadimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 06:58:39.000000 loadimg-0.1.0/src/loadimg.egg-info/top_level.txt
```

### Comparing `loadimg-0.0.3/LICENSE` & `loadimg-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loadimg-0.0.3/PKG-INFO` & `loadimg-0.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadimg
-Version: 0.0.3
+Version: 0.1.0
 Summary: a python package for loading images
 Home-page: https://github.com/not-lain/loadimg
 Author-email: hhichri60@gmail.com
 License: Apache 2.0 License
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Requires: setuptools
@@ -23,11 +23,13 @@
 installation
 ```
 pip install loadimg
 ```
 usage
 ```python
 from loadimg import load_img
-load_img(any_img_type_here) # output_type parameter is coming soon
+load_img(any_img_type_here,output_type="pil") 
+# currently supported input types [numpy, pillow, str(both path and url)]
+# currently supported output types [numpy, pillow,"str"]
 ```
 
 ![loadimg](https://github.com/not-lain/loadimg/blob/main/loadimg.png?raw=true)
```

### Comparing `loadimg-0.0.3/setup.py` & `loadimg-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 setup(
     name="loadimg",
-    version="0.0.3",
+    version="0.1.0",
     description="a python package for loading images",
     long_description=pathlib.Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     Homepage="https://github.com/not-lain/loadimg",
     url="https://github.com/not-lain/loadimg",
     Issues="https://github.com/not-lain/loadimg/issues",
     authors=[{"name": "hafedh hichri", "email": "hhichri60@gmail.com"}],
```

### Comparing `loadimg-0.0.3/src/loadimg/utils.py` & `loadimg-0.1.0/src/loadimg/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,78 @@
 from typing import Any, Literal, Union
+from io import BytesIO
+import os
 import requests
 from PIL import Image
-from io import BytesIO
-from os import path
 import numpy as np
+import tempfile
 # TODO:
 # support output_type parameter to change the output type
 # support other input types such as lists, Bytes, tensors, torch tensors, ...
 
 
 def download_image(url: str):
     """A function to get a Pillow image from a URL."""
     try:
+        if "github" in url and "raw=true" not in url:
+            url += "?raw=true"
+        if "drive" in url and "uc?id=" not in url:
+            if "/view" in url or url.endswith("/"):
+                url = "/".join(url.split("/")[:-1])
+            url = "https://drive.google.com/uc?id=" + url.split("/")[-1]
         response = requests.get(url, timeout=5)  # Timeout set to 5 seconds
         response.raise_for_status()  # Raise an exception for HTTP errors
         return Image.open(BytesIO(response.content))
     except requests.exceptions.RequestException as e:
         print(f"Error downloading image from {url}: {e}")
         return None  # Return None if there's an error
 
 
-SUPPORTED_TYPES = Union[str, np.ndarray, Image.Image]
+SUPPORTED_INPUT_TYPES = Union[str, np.ndarray, Image.Image]
+SUPPORTED_OUTPUT_TYPES = Literal["pil", "numpy", "str"]
 
 
 def load_img(
-    img: SUPPORTED_TYPES,
-    # output_type=Literal["PIL"]
+    img: Union[str, np.ndarray, Image.Image],
+    output_type: Literal["pil", "numpy", "str"] = "pil",
 ) -> Any:
-    """takes an input image of type any and returns"""
+    """
+    takes an input image of type any and returns a pillow image
+    Args :
+
+    how to use :
+
+    ```python
+    from loadimg import load_img
+    load_img(img,output_type="pil")
+    ```
+    """
+    img = load(img)
+    if output_type == "pil":
+        return img
+    elif output_type == "numpy":
+        return np.array(img)
+    elif output_type == "str":
+        secure_temp_dir = tempfile.mkdtemp(prefix="loadimg_", suffix="_folder")
+        path = os.path.join(secure_temp_dir, "temp_image.jpg")
+        img.save(path)
+        return path
+
+
+def load(img: SUPPORTED_INPUT_TYPES) -> Image.Image:
+    "loads the img"
     # file path or url
     if isinstance(img, str):
-        if path.isfile(img):
+        if os.path.isfile(img):
             return Image.open(img)
         else:
             out = download_image(img)
             if out is None:
                 raise ValueError(f"could not download {img}")
             else:
                 return out
     # numpy array
     elif isinstance(img, np.ndarray):
         return Image.fromarray(img)
     # pillow image
     elif isinstance(img, Image.Image):
         return img
-    else:
-        raise ValueError(
-            f"""expected one of the following types :{SUPPORTED_TYPES.__args__}, 
-            but got {type(img)}, please head to https://github.com/not-lain/loadimg/issues and past your input type so we will support it soon
-            """
-        )
```

### Comparing `loadimg-0.0.3/src/loadimg.egg-info/PKG-INFO` & `loadimg-0.1.0/src/loadimg.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadimg
-Version: 0.0.3
+Version: 0.1.0
 Summary: a python package for loading images
 Home-page: https://github.com/not-lain/loadimg
 Author-email: hhichri60@gmail.com
 License: Apache 2.0 License
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Requires: setuptools
@@ -23,11 +23,13 @@
 installation
 ```
 pip install loadimg
 ```
 usage
 ```python
 from loadimg import load_img
-load_img(any_img_type_here) # output_type parameter is coming soon
+load_img(any_img_type_here,output_type="pil") 
+# currently supported input types [numpy, pillow, str(both path and url)]
+# currently supported output types [numpy, pillow,"str"]
 ```
 
 ![loadimg](https://github.com/not-lain/loadimg/blob/main/loadimg.png?raw=true)
```

