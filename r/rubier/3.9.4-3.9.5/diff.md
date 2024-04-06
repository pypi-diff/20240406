# Comparing `tmp/rubier-3.9.4.tar.gz` & `tmp/rubier-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubier-3.9.4.tar", last modified: Sat Mar 23 15:29:54 2024, max compression
+gzip compressed data, was "rubier-3.9.5.tar", last modified: Sat Apr  6 10:40:54 2024, max compression
```

## Comparing `rubier-3.9.4.tar` & `rubier-3.9.5.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 Xkxiisksf (17343151) registered_users (60000)        0 2024-03-23 15:29:54.116471 rubier-3.9.4/
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)      695 2024-03-23 15:29:54.112471 rubier-3.9.4/PKG-INFO
-drwxrwxr-x   0 Xkxiisksf (17343151) registered_users (60000)        0 2024-03-23 15:29:54.020471 rubier-3.9.4/rubier/
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)       21 2024-03-23 13:27:19.000000 rubier-3.9.4/rubier/__init__.py
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)      197 2024-03-23 14:25:40.000000 rubier-3.9.4/rubier/colors.py
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)      376 2024-03-23 15:26:40.000000 rubier-3.9.4/rubier/copyrights.py
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)     1248 2024-03-23 14:25:31.000000 rubier-3.9.4/rubier/encryptor.py
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)     1878 2024-03-23 15:27:04.000000 rubier-3.9.4/rubier/httpz.py
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)      207 2024-03-22 12:22:00.000000 rubier-3.9.4/rubier/randomStream.py
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)    33216 2024-03-23 15:28:45.000000 rubier-3.9.4/rubier/rubier.py
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)     1247 2024-03-23 15:27:26.000000 rubier-3.9.4/rubier/servers.py
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)     1635 2024-03-23 15:25:39.000000 rubier-3.9.4/rubier/setup.py
-drwxrwxr-x   0 Xkxiisksf (17343151) registered_users (60000)        0 2024-03-23 15:29:54.100471 rubier-3.9.4/rubier.egg-info/
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)      695 2024-03-23 15:29:52.000000 rubier-3.9.4/rubier.egg-info/PKG-INFO
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)      324 2024-03-23 15:29:52.000000 rubier-3.9.4/rubier.egg-info/SOURCES.txt
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)        1 2024-03-23 15:29:52.000000 rubier-3.9.4/rubier.egg-info/dependency_links.txt
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)       31 2024-03-23 15:29:52.000000 rubier-3.9.4/rubier.egg-info/requires.txt
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)        7 2024-03-23 15:29:52.000000 rubier-3.9.4/rubier.egg-info/top_level.txt
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)       38 2024-03-23 15:29:54.120471 rubier-3.9.4/setup.cfg
--rw-rw-r--   0 Xkxiisksf (17343151) registered_users (60000)     1635 2024-03-23 15:29:21.000000 rubier-3.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:40:54.103145 rubier-3.9.5/
+-rw-rw-rw-   0        0        0     1075 2023-07-17 08:57:59.000000 rubier-3.9.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      712 2024-04-06 10:40:54.102147 rubier-3.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-07-17 09:01:49.000000 rubier-3.9.5/README.md
+-rw-rw-rw-   0        0        0       88 2023-07-07 11:03:38.000000 rubier-3.9.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-06 10:40:54.080205 rubier-3.9.5/rubier/
+-rw-rw-rw-   0        0        0       21 2024-04-06 09:54:04.000000 rubier-3.9.5/rubier/__init__.py
+-rw-rw-rw-   0        0        0      197 2024-04-06 09:54:04.000000 rubier-3.9.5/rubier/colors.py
+-rw-rw-rw-   0        0        0      376 2024-04-06 10:10:33.000000 rubier-3.9.5/rubier/copyrights.py
+-rw-rw-rw-   0        0        0     1248 2024-04-06 09:54:04.000000 rubier-3.9.5/rubier/encryptor.py
+-rw-rw-rw-   0        0        0     1878 2024-04-06 09:54:04.000000 rubier-3.9.5/rubier/httpz.py
+-rw-rw-rw-   0        0        0      207 2024-04-06 09:54:04.000000 rubier-3.9.5/rubier/randomStream.py
+-rw-rw-rw-   0        0        0    33620 2024-04-06 10:33:04.000000 rubier-3.9.5/rubier/rubier.py
+-rw-rw-rw-   0        0        0     1247 2024-04-06 10:10:34.000000 rubier-3.9.5/rubier/servers.py
+-rw-rw-rw-   0        0        0     1635 2024-04-06 10:33:45.000000 rubier-3.9.5/rubier/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:40:54.098157 rubier-3.9.5/rubier.egg-info/
+-rw-rw-rw-   0        0        0      712 2024-04-06 10:40:53.000000 rubier-3.9.5/rubier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-06 10:40:53.000000 rubier-3.9.5/rubier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 10:40:53.000000 rubier-3.9.5/rubier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-06 10:40:53.000000 rubier-3.9.5/rubier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-06 10:40:53.000000 rubier-3.9.5/rubier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 10:40:54.104142 rubier-3.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2024-03-20 21:46:48.000000 rubier-3.9.5/setup.py
```

### Comparing `rubier-3.9.4/PKG-INFO` & `rubier-3.9.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-Metadata-Version: 2.1
-Name: rubier
-Version: 3.9.4
-Summary: Rubino Library
-Home-page: https://github.com/HostBlack1Let/MyBale
-Author: Host1let
-Author-email: sqlmapssh@gmail.com
-License: MIT
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
-Keywords: rubier
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: rubier
+Version: 3.9.5
+Summary: Rubino Library
+Home-page: https://github.com/HostBlack1Let/MyBale
+Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Author: Host1let
+Author-email: sqlmapssh@gmail.com
+License: MIT
+Keywords: rubier
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE.txt
```

### Comparing `rubier-3.9.4/rubier/encryptor.py` & `rubier-3.9.5/rubier/encryptor.py`

 * *Files identical despite different names*

### Comparing `rubier-3.9.4/rubier/httpz.py` & `rubier-3.9.5/rubier/httpz.py`

 * *Files identical despite different names*

### Comparing `rubier-3.9.4/rubier/rubier.py` & `rubier-3.9.5/rubier/rubier.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,14 +427,18 @@
 
     def getPostsByHashTag(self, hashtag: str, limit: int = 51, profileID = None):
       return httpz.Httpz(self.auth).poolConnection({
         "equal":False,
         "hashtag": hashtag,
         "limit":limit,
         "profile_id":profileID}, 'getPostsByHashTag')
+    
+    def getUserInfoByPostLink(self, link: str):
+        postLinkInfo = self.getPostByLink(link=link)
+        return postLinkInfo['data']['profile'] if "data" in postLinkInfo.keys() else None
 
 class rubino(Rubier):
     ...
 
 class Rubino(Rubier):
     ...
 
@@ -639,15 +643,15 @@
     async def getMe(self, profileID = None):
         return await httpz.AsyncHttpz(self.auth).poolConnection({
             "profile_id": profileID
         }, "getMyProfileInfo")
 
     async def getPostByLink(self, link: str, profileID = None):
         if link.startswith("post/"):
-            splitted = link.split("post/")
+            splitted = link.replace("post/", "")
             inputData = {
                 "share_string":splitted,
                 "profile_id":profileID
                 }
             return await httpz.AsyncHttpz(self.auth).poolConnection(inputData=inputData, method="getPostByShareLink")
         else:
             inputData = {
@@ -853,14 +857,18 @@
 
       return await httpz.AsyncHttpz(self.auth).poolConnection({
 
         "equal":False,
         "hashtag": hashtag,
         "limit":limit,
         "profile_id":profileID}, 'getPostsByHashTag')
+    
+    async def getUserInfoByPostLink(self, link: str):
+        postLinkInfo = self.getPostByLink(link=link)
+        return postLinkInfo['data']['profile'] if "data" in postLinkInfo.keys() else None
 
 class AsyncRunner(object):
     def runner(obj):
         try:
             asyncio.run(obj)
         except Exception as ERR:
             print(ERR)
```

### Comparing `rubier-3.9.4/rubier/servers.py` & `rubier-3.9.5/rubier/servers.py`

 * *Files identical despite different names*

### Comparing `rubier-3.9.4/rubier/setup.py` & `rubier-3.9.5/rubier/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'rubier',         # How you named your package folder (MyLib)
   packages = ['rubier'],   # Chose the same as "name"
-  version = '3.9.4',      # Start with a small number and increase it with every change you make
+  version = '3.9.5',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Rubino Library',   # Give a short description about your library
   author = 'Host1let',                   # Type in your name
   author_email = 'sqlmapssh@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/HostBlack1Let/MyBale',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['rubier'],   # Keywords that define your package best
```

### Comparing `rubier-3.9.4/rubier.egg-info/PKG-INFO` & `rubier-3.9.5/rubier.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-Metadata-Version: 2.1
-Name: rubier
-Version: 3.9.4
-Summary: Rubino Library
-Home-page: https://github.com/HostBlack1Let/MyBale
-Author: Host1let
-Author-email: sqlmapssh@gmail.com
-License: MIT
-Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
-Keywords: rubier
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-
-UNKNOWN
-
+Metadata-Version: 2.1
+Name: rubier
+Version: 3.9.5
+Summary: Rubino Library
+Home-page: https://github.com/HostBlack1Let/MyBale
+Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
+Author: Host1let
+Author-email: sqlmapssh@gmail.com
+License: MIT
+Keywords: rubier
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE.txt
```

### Comparing `rubier-3.9.4/setup.py` & `rubier-3.9.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'rubier',         # How you named your package folder (MyLib)
   packages = ['rubier'],   # Chose the same as "name"
-  version = '3.9.4',      # Start with a small number and increase it with every change you make
+  version = '3.8.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Rubino Library',   # Give a short description about your library
   author = 'Host1let',                   # Type in your name
   author_email = 'sqlmapssh@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/HostBlack1Let/MyBale',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
-  keywords = ['rubier'],   # Keywords that define your package best
+  keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
-          "httpx",
-          "asyncio",
-          "aiohttp"
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

