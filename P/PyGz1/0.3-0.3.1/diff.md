# Comparing `tmp/PyGz1-0.3.tar.gz` & `tmp/PyGz1-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGz1-0.3.tar", last modified: Sat Apr  6 14:01:43 2024, max compression
+gzip compressed data, was "PyGz1-0.3.1.tar", last modified: Sat Apr  6 14:17:20 2024, max compression
```

## Comparing `PyGz1-0.3.tar` & `PyGz1-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 14:01:43.470139 PyGz1-0.3/
--rw-rw-rw-   0        0        0      161 2024-04-06 14:01:43.469157 PyGz1-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 14:01:43.462239 PyGz1-0.3/PyGz1.egg-info/
--rw-rw-rw-   0        0        0      161 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-06 14:01:43.000000 PyGz1-0.3/PyGz1.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 14:01:43.468143 PyGz1-0.3/pygz1/
--rw-rw-rw-   0        0        0      710 2024-04-06 13:57:14.000000 PyGz1-0.3/pygz1/__init__.py
--rw-rw-rw-   0        0        0     3176 2024-04-06 13:56:44.000000 PyGz1-0.3/pygz1/network.py
--rw-rw-rw-   0        0        0        0 2024-04-06 13:36:44.000000 PyGz1-0.3/pygz1/utils.py
--rw-rw-rw-   0        0        0       42 2024-04-06 14:01:43.470139 PyGz1-0.3/setup.cfg
--rw-rw-rw-   0        0        0      274 2024-04-06 13:57:19.000000 PyGz1-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 14:17:20.989488 PyGz1-0.3.1/
+-rw-rw-rw-   0        0        0      163 2024-04-06 14:17:20.977641 PyGz1-0.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 14:17:20.970646 PyGz1-0.3.1/PyGz1.egg-info/
+-rw-rw-rw-   0        0        0      163 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-06 14:17:20.000000 PyGz1-0.3.1/PyGz1.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 14:17:20.974626 PyGz1-0.3.1/pygz1/
+-rw-rw-rw-   0        0        0      729 2024-04-06 14:11:13.000000 PyGz1-0.3.1/pygz1/__init__.py
+-rw-rw-rw-   0        0        0     3208 2024-04-06 14:09:16.000000 PyGz1-0.3.1/pygz1/network.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 13:36:44.000000 PyGz1-0.3.1/pygz1/utils.py
+-rw-rw-rw-   0        0        0       42 2024-04-06 14:17:20.989488 PyGz1-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      276 2024-04-06 14:17:12.000000 PyGz1-0.3.1/setup.py
```

### Comparing `PyGz1-0.3/pygz1/__init__.py` & `PyGz1-0.3.1/pygz1/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .network import fetch_url, post_data, download_file, get_json, get_headers, get_ip_address, check_host, execute_command, get_system_info, list_files, create_directory, delete_file, rename_file, get_file_size
+from .network import fetch_url, post_data, download_file, get_json, get_headers, get_ip_address, check_host, execute_command, get_system_info, list_files, create_directory, delete_file, rename_file, get_file_size, check_github_file
 
 # Этот список определяет, какие символы будут экспортированы при импорте вашего пакета.
 __all__ = [
     'fetch_url',
     'post_data',
     'download_file',
     'get_json',
```

### Comparing `PyGz1-0.3/pygz1/network.py` & `PyGz1-0.3.1/pygz1/network.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import requests
 import socket
 import subprocess
 import os
 import platform
+from tkinter import messagebox
 
 def fetch_url(url):
     response = requests.get(url)
     return response.text
 
 def post_data(url, data):
     response = requests.post(url, data=data)
```

