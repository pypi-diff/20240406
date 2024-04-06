# Comparing `tmp/download_tiktok_no_watermark-0.2.0.tar.gz` & `tmp/download_tiktok_no_watermark-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "download_tiktok_no_watermark-0.2.0.tar", last modified: Sat Apr  6 06:25:28 2024, max compression
+gzip compressed data, was "download_tiktok_no_watermark-0.2.3.tar", last modified: Sat Apr  6 19:36:37 2024, max compression
```

## Comparing `download_tiktok_no_watermark-0.2.0.tar` & `download_tiktok_no_watermark-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 06:25:28.865022 download_tiktok_no_watermark-0.2.0/
--rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 06:25:28.864910 download_tiktok_no_watermark-0.2.0/PKG-INFO
--rw-r--r--   0 jacobadelman   (501) staff       (20)      338 2024-04-06 06:15:40.000000 download_tiktok_no_watermark-0.2.0/README.md
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 06:25:28.864052 download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark/
--rw-r--r--   0 jacobadelman   (501) staff       (20)     7101 2024-04-06 05:42:26.000000 download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark/download.py
-drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 06:25:28.864726 download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark.egg-info/
--rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 06:25:28.000000 download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark.egg-info/PKG-INFO
--rw-r--r--   0 jacobadelman   (501) staff       (20)      318 2024-04-06 06:25:28.000000 download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark.egg-info/SOURCES.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)        1 2024-04-06 06:25:28.000000 download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark.egg-info/dependency_links.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       80 2024-04-06 06:25:28.000000 download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark.egg-info/requires.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       29 2024-04-06 06:25:28.000000 download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark.egg-info/top_level.txt
--rw-r--r--   0 jacobadelman   (501) staff       (20)       38 2024-04-06 06:25:28.865059 download_tiktok_no_watermark-0.2.0/setup.cfg
--rw-r--r--   0 jacobadelman   (501) staff       (20)     1091 2024-04-06 06:25:10.000000 download_tiktok_no_watermark-0.2.0/setup.py
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:36:37.590633 download_tiktok_no_watermark-0.2.3/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 19:36:37.590486 download_tiktok_no_watermark-0.2.3/PKG-INFO
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      554 2024-04-06 19:23:19.000000 download_tiktok_no_watermark-0.2.3/README.md
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:36:37.589158 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)     7030 2024-04-06 19:34:05.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark/download.py
+drwxr-xr-x   0 jacobadelman   (501) staff       (20)        0 2024-04-06 19:36:37.590250 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      711 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/PKG-INFO
+-rw-r--r--   0 jacobadelman   (501) staff       (20)      318 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/SOURCES.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)        1 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/dependency_links.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       80 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/requires.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       29 2024-04-06 19:36:37.000000 download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/top_level.txt
+-rw-r--r--   0 jacobadelman   (501) staff       (20)       38 2024-04-06 19:36:37.590680 download_tiktok_no_watermark-0.2.3/setup.cfg
+-rw-r--r--   0 jacobadelman   (501) staff       (20)     1091 2024-04-06 19:35:51.000000 download_tiktok_no_watermark-0.2.3/setup.py
```

### Comparing `download_tiktok_no_watermark-0.2.0/PKG-INFO` & `download_tiktok_no_watermark-0.2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download_tiktok_no_watermark
-Version: 0.2.0
+Version: 0.2.3
 Summary: Download TikTok videos no watermark
 Home-page: https://github.com/jakeadelman/download_tiktok_no_watermark
 Author: Jacob Adelman
 Author-email: jacobzadelman@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark/download.py` & `download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
                             }
                             r += String.fromCharCode(parseInt(decodeString(s, e, 10)) - t);
                         }
                         return decodeURIComponent(escape(r));
                         }
                         return evalFunction(h,u,n,t,e,r)
 
-                        console.log(evalFunction(h, u, n, t, e, r));
                         }
                         """
 
     def get_token(self) -> response:
         try:
             response = self.client.get("https://snaptik.app")
             soup = BeautifulSoup(response.text, "lxml")
@@ -166,16 +165,15 @@
 
 
 def download(video_url, output_name, output_dir):
     sn = SnapTikReversed()
     token = sn.get_token()
     my_vid = sn.send_request(video=video_url)
     my_vid1= sn.decode(variable=my_vid)
-    print(my_vid1)
-    sp = BeautifulSoup(my_vid1)
+    sp = BeautifulSoup(my_vid1, features='lxml')
 
     d = 0
     for a in sp.find_all('a', href=True):
         if d==0:
             link = a['href']
             link = link.replace('\\"',"")
             name = output_dir + output_name + '.mp4'
```

### Comparing `download_tiktok_no_watermark-0.2.0/download_tiktok_no_watermark.egg-info/PKG-INFO` & `download_tiktok_no_watermark-0.2.3/download_tiktok_no_watermark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: download-tiktok-no-watermark
-Version: 0.2.0
+Version: 0.2.3
 Summary: Download TikTok videos no watermark
 Home-page: https://github.com/jakeadelman/download_tiktok_no_watermark
 Author: Jacob Adelman
 Author-email: jacobzadelman@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `download_tiktok_no_watermark-0.2.0/setup.py` & `download_tiktok_no_watermark-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='download_tiktok_no_watermark',
-    version='0.2.0',    
+    version='0.2.3',    
     description='Download TikTok videos no watermark',
     url='https://github.com/jakeadelman/download_tiktok_no_watermark',
     author='Jacob Adelman',
     author_email='jacobzadelman@gmail.com',
     license='BSD 2-clause',
     packages=['download_tiktok_no_watermark'],
     install_requires=['beautifulsoup4==4.12.3'
```

