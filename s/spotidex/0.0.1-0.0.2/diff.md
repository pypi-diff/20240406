# Comparing `tmp/spotidex-0.0.1.tar.gz` & `tmp/spotidex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotidex-0.0.1.tar", last modified: Sat Apr  6 11:28:26 2024, max compression
+gzip compressed data, was "spotidex-0.0.2.tar", last modified: Sat Apr  6 12:19:38 2024, max compression
```

## Comparing `spotidex-0.0.1.tar` & `spotidex-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 11:28:26.540398 spotidex-0.0.1/
--rw-rw-rw-   0        0        0     1110 2024-04-06 09:42:27.000000 spotidex-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1129 2024-04-06 11:28:26.533789 spotidex-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-06 09:42:27.000000 spotidex-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 11:28:26.540398 spotidex-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-06 11:24:47.000000 spotidex-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:28:26.503468 spotidex-0.0.1/spotidex/
--rw-rw-rw-   0        0        0      121 2024-04-06 10:41:23.000000 spotidex-0.0.1/spotidex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:28:26.520079 spotidex-0.0.1/spotidex/cli/
--rw-rw-rw-   0        0        0      616 2024-04-06 11:21:46.000000 spotidex-0.0.1/spotidex/cli/SpotidexApp.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:04:49.000000 spotidex-0.0.1/spotidex/cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:28:26.524065 spotidex-0.0.1/spotidex/cli/app_screens/
--rw-rw-rw-   0        0        0     6936 2024-04-06 10:26:07.000000 spotidex-0.0.1/spotidex/cli/app_screens/DownloadInterface.py
--rw-rw-rw-   0        0        0     4675 2024-04-06 10:26:15.000000 spotidex-0.0.1/spotidex/cli/app_screens/MainMenuInterface.py
--rw-rw-rw-   0        0        0     4123 2024-04-06 10:26:01.000000 spotidex-0.0.1/spotidex/cli/app_screens/SearchInterface.py
--rw-rw-rw-   0        0        0     4025 2024-04-06 10:25:55.000000 spotidex-0.0.1/spotidex/cli/app_screens/SelectDownloadInterface.py
--rw-rw-rw-   0        0        0     2430 2024-04-06 10:26:19.000000 spotidex-0.0.1/spotidex/cli/app_screens/SettingsInterface.py
--rw-rw-rw-   0        0        0        0 2024-03-25 10:54:48.000000 spotidex-0.0.1/spotidex/cli/app_screens/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:28:26.527055 spotidex-0.0.1/spotidex/cli/custom_widgets/
--rw-rw-rw-   0        0        0     4510 2024-04-06 08:18:54.000000 spotidex-0.0.1/spotidex/cli/custom_widgets/AppInterface.py
--rw-rw-rw-   0        0        0     1409 2024-04-06 10:25:36.000000 spotidex-0.0.1/spotidex/cli/custom_widgets/DownloadPathSelector.py
--rw-rw-rw-   0        0        0     1694 2024-03-26 11:07:37.000000 spotidex-0.0.1/spotidex/cli/custom_widgets/DownloadQualitySelection.py
--rw-rw-rw-   0        0        0     1933 2024-03-26 10:25:59.000000 spotidex-0.0.1/spotidex/cli/custom_widgets/MetadataCheckBox.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:19:37.000000 spotidex-0.0.1/spotidex/cli/custom_widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:28:26.529048 spotidex-0.0.1/spotidex/cli/popup_screens/
--rw-rw-rw-   0        0        0     4303 2024-04-06 09:28:28.000000 spotidex-0.0.1/spotidex/cli/popup_screens/DownloadPathPopup.py
--rw-rw-rw-   0        0        0     1126 2023-12-20 02:51:25.000000 spotidex-0.0.1/spotidex/cli/popup_screens/ExitScreenPopup.py
--rw-rw-rw-   0        0        0     1210 2024-03-26 12:20:40.000000 spotidex-0.0.1/spotidex/cli/popup_screens/GoBackSettingsPopup.py
--rw-rw-rw-   0        0        0     1389 2024-03-22 13:06:57.000000 spotidex-0.0.1/spotidex/cli/popup_screens/NetworkErrorPopup.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:19:46.000000 spotidex-0.0.1/spotidex/cli/popup_screens/__init__.py
--rw-rw-rw-   0        0        0     4180 2024-04-06 10:25:15.000000 spotidex-0.0.1/spotidex/cli/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:28:26.532787 spotidex-0.0.1/spotidex/src/
--rw-rw-rw-   0        0        0        0 2024-04-06 10:22:02.000000 spotidex-0.0.1/spotidex/src/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-12-15 00:52:48.000000 spotidex-0.0.1/spotidex/src/content.py
--rw-rw-rw-   0        0        0     9590 2024-04-05 12:21:12.000000 spotidex-0.0.1/spotidex/src/download.py
--rw-rw-rw-   0        0        0     1049 2023-12-06 02:16:07.000000 spotidex-0.0.1/spotidex/src/static.py
--rw-rw-rw-   0        0        0     8260 2024-04-05 12:03:44.000000 spotidex-0.0.1/spotidex/src/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 11:28:26.518173 spotidex-0.0.1/spotidex.egg-info/
--rw-rw-rw-   0        0        0     1129 2024-04-06 11:28:26.000000 spotidex-0.0.1/spotidex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2024-04-06 11:28:26.000000 spotidex-0.0.1/spotidex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 11:28:26.000000 spotidex-0.0.1/spotidex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-06 11:28:26.000000 spotidex-0.0.1/spotidex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2024-04-06 11:28:26.000000 spotidex-0.0.1/spotidex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 11:28:26.000000 spotidex-0.0.1/spotidex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 12:19:38.448099 spotidex-0.0.2/
+-rw-rw-rw-   0        0        0     1110 2024-04-06 09:42:27.000000 spotidex-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1129 2024-04-06 12:19:38.437542 spotidex-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-06 09:42:27.000000 spotidex-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 12:19:38.449098 spotidex-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-06 12:18:29.000000 spotidex-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 12:19:38.357926 spotidex-0.0.2/spotidex/
+-rw-rw-rw-   0        0        0      121 2024-04-06 10:41:23.000000 spotidex-0.0.2/spotidex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 12:19:38.399805 spotidex-0.0.2/spotidex/cli/
+-rw-rw-rw-   0        0        0      616 2024-04-06 11:21:46.000000 spotidex-0.0.2/spotidex/cli/SpotidexApp.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 10:04:49.000000 spotidex-0.0.2/spotidex/cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 12:19:38.406782 spotidex-0.0.2/spotidex/cli/app_screens/
+-rw-rw-rw-   0        0        0     6936 2024-04-06 10:26:07.000000 spotidex-0.0.2/spotidex/cli/app_screens/DownloadInterface.py
+-rw-rw-rw-   0        0        0     4675 2024-04-06 10:26:15.000000 spotidex-0.0.2/spotidex/cli/app_screens/MainMenuInterface.py
+-rw-rw-rw-   0        0        0     4123 2024-04-06 10:26:01.000000 spotidex-0.0.2/spotidex/cli/app_screens/SearchInterface.py
+-rw-rw-rw-   0        0        0     4025 2024-04-06 10:25:55.000000 spotidex-0.0.2/spotidex/cli/app_screens/SelectDownloadInterface.py
+-rw-rw-rw-   0        0        0     2430 2024-04-06 10:26:19.000000 spotidex-0.0.2/spotidex/cli/app_screens/SettingsInterface.py
+-rw-rw-rw-   0        0        0        0 2024-03-25 10:54:48.000000 spotidex-0.0.2/spotidex/cli/app_screens/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 12:19:38.418416 spotidex-0.0.2/spotidex/cli/custom_widgets/
+-rw-rw-rw-   0        0        0     4510 2024-04-06 08:18:54.000000 spotidex-0.0.2/spotidex/cli/custom_widgets/AppInterface.py
+-rw-rw-rw-   0        0        0     1409 2024-04-06 10:25:36.000000 spotidex-0.0.2/spotidex/cli/custom_widgets/DownloadPathSelector.py
+-rw-rw-rw-   0        0        0     1694 2024-03-26 11:07:37.000000 spotidex-0.0.2/spotidex/cli/custom_widgets/DownloadQualitySelection.py
+-rw-rw-rw-   0        0        0     1933 2024-03-26 10:25:59.000000 spotidex-0.0.2/spotidex/cli/custom_widgets/MetadataCheckBox.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 10:19:37.000000 spotidex-0.0.2/spotidex/cli/custom_widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 12:19:38.426388 spotidex-0.0.2/spotidex/cli/popup_screens/
+-rw-rw-rw-   0        0        0     4303 2024-04-06 09:28:28.000000 spotidex-0.0.2/spotidex/cli/popup_screens/DownloadPathPopup.py
+-rw-rw-rw-   0        0        0     1126 2023-12-20 02:51:25.000000 spotidex-0.0.2/spotidex/cli/popup_screens/ExitScreenPopup.py
+-rw-rw-rw-   0        0        0     1210 2024-03-26 12:20:40.000000 spotidex-0.0.2/spotidex/cli/popup_screens/GoBackSettingsPopup.py
+-rw-rw-rw-   0        0        0     1389 2024-03-22 13:06:57.000000 spotidex-0.0.2/spotidex/cli/popup_screens/NetworkErrorPopup.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 10:19:46.000000 spotidex-0.0.2/spotidex/cli/popup_screens/__init__.py
+-rw-rw-rw-   0        0        0     4180 2024-04-06 10:25:15.000000 spotidex-0.0.2/spotidex/cli/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 12:19:38.437183 spotidex-0.0.2/spotidex/src/
+-rw-rw-rw-   0        0        0        0 2024-04-06 10:22:02.000000 spotidex-0.0.2/spotidex/src/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-12-15 00:52:48.000000 spotidex-0.0.2/spotidex/src/content.py
+-rw-rw-rw-   0        0        0     9579 2024-04-06 12:16:05.000000 spotidex-0.0.2/spotidex/src/download.py
+-rw-rw-rw-   0        0        0     1049 2023-12-06 02:16:07.000000 spotidex-0.0.2/spotidex/src/static.py
+-rw-rw-rw-   0        0        0     8260 2024-04-05 12:03:44.000000 spotidex-0.0.2/spotidex/src/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-06 12:19:38.397790 spotidex-0.0.2/spotidex.egg-info/
+-rw-rw-rw-   0        0        0     1129 2024-04-06 12:19:37.000000 spotidex-0.0.2/spotidex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2024-04-06 12:19:38.000000 spotidex-0.0.2/spotidex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 12:19:37.000000 spotidex-0.0.2/spotidex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-06 12:19:37.000000 spotidex-0.0.2/spotidex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2024-04-06 12:19:37.000000 spotidex-0.0.2/spotidex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 12:19:37.000000 spotidex-0.0.2/spotidex.egg-info/top_level.txt
```

### Comparing `spotidex-0.0.1/LICENSE.txt` & `spotidex-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/PKG-INFO` & `spotidex-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotidex
-Version: 0.0.1
+Version: 0.0.2
 Author: libin-codes
 Author-email: libinlalu000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotidex-0.0.1/setup.py` & `spotidex-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("README.md","r") as f:
     description = f.read()
 
 setup(
     name="spotidex",
-    version="0.0.1",
+    version="0.0.2",
     long_description=description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "mutagen==1.47.0",
         "Requests==2.31.0",
```

### Comparing `spotidex-0.0.1/spotidex/cli/SpotidexApp.py` & `spotidex-0.0.2/spotidex/cli/SpotidexApp.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/app_screens/DownloadInterface.py` & `spotidex-0.0.2/spotidex/cli/app_screens/DownloadInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/app_screens/MainMenuInterface.py` & `spotidex-0.0.2/spotidex/cli/app_screens/MainMenuInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/app_screens/SearchInterface.py` & `spotidex-0.0.2/spotidex/cli/app_screens/SearchInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/app_screens/SelectDownloadInterface.py` & `spotidex-0.0.2/spotidex/cli/app_screens/SelectDownloadInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/app_screens/SettingsInterface.py` & `spotidex-0.0.2/spotidex/cli/app_screens/SettingsInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/custom_widgets/AppInterface.py` & `spotidex-0.0.2/spotidex/cli/custom_widgets/AppInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/custom_widgets/DownloadPathSelector.py` & `spotidex-0.0.2/spotidex/cli/custom_widgets/DownloadPathSelector.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/custom_widgets/DownloadQualitySelection.py` & `spotidex-0.0.2/spotidex/cli/custom_widgets/DownloadQualitySelection.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/custom_widgets/MetadataCheckBox.py` & `spotidex-0.0.2/spotidex/cli/custom_widgets/MetadataCheckBox.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/popup_screens/DownloadPathPopup.py` & `spotidex-0.0.2/spotidex/cli/popup_screens/DownloadPathPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/popup_screens/ExitScreenPopup.py` & `spotidex-0.0.2/spotidex/cli/popup_screens/ExitScreenPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/popup_screens/GoBackSettingsPopup.py` & `spotidex-0.0.2/spotidex/cli/popup_screens/GoBackSettingsPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/popup_screens/NetworkErrorPopup.py` & `spotidex-0.0.2/spotidex/cli/popup_screens/NetworkErrorPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/cli/utils.py` & `spotidex-0.0.2/spotidex/cli/utils.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/src/content.py` & `spotidex-0.0.2/spotidex/src/content.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/src/download.py` & `spotidex-0.0.2/spotidex/src/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             if Path(download_path,file_name+".mp3").exists():
                 file_name = file_name.split(" (")[0]+f" ({i})"
             else:
                 break
         if self.is_library:
             options = {
             "format": "bestaudio/best",
-            "outtmpl": f"{str(download_path)+'\\'+file_name}",
+            "outtmpl": str(download_path)+'\\'+file_name,
             "quiet": True,
             "noprogress": True,
             "progress": "false",
             "ffmpeg_location": str(self.ffmpeg_path),
             "postprocessors": [
                 {
                     "key": "FFmpegExtractAudio",
@@ -78,15 +78,15 @@
             if metadata:
                 add_metadata(data, Path(downloaded_path + ".mp3").resolve())
         else:
             with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
 
                 options = {
                     "format": "bestaudio/best",
-                    "outtmpl": f"{ str(Path(temp_folder))+'\\'+file_name}",
+                    "outtmpl": str(Path(temp_folder))+'\\'+file_name,
                     "quiet": True,
                     "noprogress": True,
                     "progress": "false",
                     "ffmpeg_location": str(self.ffmpeg_path),
                     "postprocessors": [
                         {
                             "key": "FFmpegExtractAudio",
```

### Comparing `spotidex-0.0.1/spotidex/src/static.py` & `spotidex-0.0.2/spotidex/src/static.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex/src/utils.py` & `spotidex-0.0.2/spotidex/src/utils.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.1/spotidex.egg-info/PKG-INFO` & `spotidex-0.0.2/spotidex.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotidex
-Version: 0.0.1
+Version: 0.0.2
 Author: libin-codes
 Author-email: libinlalu000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotidex-0.0.1/spotidex.egg-info/SOURCES.txt` & `spotidex-0.0.2/spotidex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

