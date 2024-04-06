# Comparing `tmp/ding_api_client-3.4.1.tar.gz` & `tmp/ding_api_client-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ding_api_client-3.4.1.tar", last modified: Thu Apr  4 00:12:36 2024, max compression
+gzip compressed data, was "ding_api_client-3.4.2.tar", last modified: Sat Apr  6 00:11:27 2024, max compression
```

## Comparing `ding_api_client-3.4.1.tar` & `ding_api_client-3.4.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:12:36.864558 ding_api_client-3.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.856557 ding_api_client-3.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.856557 ding_api_client-3.4.1/src/ding/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.856557 ding_api_client-3.4.1/src/ding/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.856557 ding_api_client-3.4.1/src/ding/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/createauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/createauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/createcheckrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/createcheckresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/feedbackrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/feedbackresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/lookupresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/retryauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/retryauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/errors/errorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/create_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/models/operations/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-04 00:12:22.000000 ding_api_client-3.4.1/src/ding/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:12:36.860558 ding_api_client-3.4.1/src/ding_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 00:12:36.000000 ding_api_client-3.4.1/src/ding_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.288434 ding_api_client-3.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-06 00:11:27.288434 ding_api_client-3.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:11:27.288434 ding_api_client-3.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.280434 ding_api_client-3.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.280434 ding_api_client-3.4.2/src/ding/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.280434 ding_api_client-3.4.2/src/ding/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.280434 ding_api_client-3.4.2/src/ding/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/createauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/createauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/createcheckrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/createcheckresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/feedbackrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/feedbackresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/lookupresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/retryauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/retryauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/errors/errorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/create_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/models/operations/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-06 00:11:12.000000 ding_api_client-3.4.2/src/ding/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:11:27.284434 ding_api_client-3.4.2/src/ding_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 00:11:27.000000 ding_api_client-3.4.2/src/ding_api_client.egg-info/top_level.txt
```

### Comparing `ding_api_client-3.4.1/PKG-INFO` & `ding_api_client-3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ding_api_client
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
```

### Comparing `ding_api_client-3.4.1/README.md` & `ding_api_client-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/setup.py` & `ding_api_client-3.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='ding_api_client',
-    version='3.4.1',
+    version='3.4.2',
     author='Ding',
     description='Python Client SDK',
     url='https://github.com/ding-live/ding-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
@@ -40,14 +40,16 @@
         "six>=1.16.0",
         "typing-inspect>=0.9.0",
         "typing_extensions>=4.7.1",
         "urllib3>=1.26.18",
     ],
     extras_require={
         "dev": [
-            "pylint==2.16.2",
+            "pylint==3.1.0",
         ],
     },
     package_dir={'': 'src'},
     python_requires='>=3.8',
-    package_data={'ding_api_client': ['py.typed']},
+    package_data={
+        'ding_api_client': ['py.typed']
+    },
 )
```

### Comparing `ding_api_client-3.4.1/src/ding/_hooks/sdkhooks.py` & `ding_api_client-3.4.2/src/ding/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/_hooks/types.py` & `ding_api_client-3.4.2/src/ding/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/lookup.py` & `ding_api_client-3.4.2/src/ding/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,9 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `ding_api_client-3.4.1/src/ding/models/components/__init__.py` & `ding_api_client-3.4.2/src/ding/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/createauthenticationrequest.py` & `ding_api_client-3.4.2/src/ding/models/components/createauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/createauthenticationresponse.py` & `ding_api_client-3.4.2/src/ding/models/components/createauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/createcheckrequest.py` & `ding_api_client-3.4.2/src/ding/models/components/createcheckrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/createcheckresponse.py` & `ding_api_client-3.4.2/src/ding/models/components/createcheckresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/feedbackrequest.py` & `ding_api_client-3.4.2/src/ding/models/components/feedbackrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/feedbackresponse.py` & `ding_api_client-3.4.2/src/ding/models/components/feedbackresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/lookupresponse.py` & `ding_api_client-3.4.2/src/ding/models/components/lookupresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/retryauthenticationrequest.py` & `ding_api_client-3.4.2/src/ding/models/components/retryauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/components/retryauthenticationresponse.py` & `ding_api_client-3.4.2/src/ding/models/components/retryauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/errors/errorresponse.py` & `ding_api_client-3.4.2/src/ding/models/errors/errorresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/errors/sdkerror.py` & `ding_api_client-3.4.2/src/ding/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/operations/check.py` & `ding_api_client-3.4.2/src/ding/models/operations/check.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/operations/create_authentication.py` & `ding_api_client-3.4.2/src/ding/models/operations/create_authentication.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/operations/feedback.py` & `ding_api_client-3.4.2/src/ding/models/operations/feedback.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/operations/lookup.py` & `ding_api_client-3.4.2/src/ding/models/operations/lookup.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/models/operations/retry.py` & `ding_api_client-3.4.2/src/ding/models/operations/retry.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/otp.py` & `ding_api_client-3.4.2/src/ding/otp.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,8 +264,9 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `ding_api_client-3.4.1/src/ding/sdk.py` & `ding_api_client-3.4.2/src/ding/sdk.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding/sdkconfiguration.py` & `ding_api_client-3.4.2/src/ding/sdkconfiguration.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '3.4.1'
-    gen_version: str = '2.298.2'
-    user_agent: str = 'speakeasy-sdk/python 3.4.1 2.298.2 1.0.0 ding_api_client'
+    sdk_version: str = '3.4.2'
+    gen_version: str = '2.300.0'
+    user_agent: str = 'speakeasy-sdk/python 3.4.2 2.300.0 1.0.0 ding_api_client'
     retry_config: Optional[RetryConfig] = None
     _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
```

### Comparing `ding_api_client-3.4.1/src/ding/utils/retries.py` & `ding_api_client-3.4.2/src/ding/utils/retries.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,11 +110,10 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            if sleep > max_interval/1000:
-                sleep = max_interval/1000
+            sleep = min(sleep, max_interval / 1000)
             time.sleep(sleep)
             retries += 1
```

### Comparing `ding_api_client-3.4.1/src/ding/utils/utils.py` & `ding_api_client-3.4.2/src/ding/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.4.1/src/ding_api_client.egg-info/PKG-INFO` & `ding_api_client-3.4.2/src/ding_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ding-api-client
-Version: 3.4.1
+Version: 3.4.2
 Summary: Python Client SDK
 Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
```

### Comparing `ding_api_client-3.4.1/src/ding_api_client.egg-info/SOURCES.txt` & `ding_api_client-3.4.2/src/ding_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

