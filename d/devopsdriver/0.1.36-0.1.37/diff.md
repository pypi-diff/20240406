# Comparing `tmp/devopsdriver-0.1.36.tar.gz` & `tmp/devopsdriver-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopsdriver-0.1.36.tar", last modified: Fri Apr  5 00:12:42 2024, max compression
+gzip compressed data, was "devopsdriver-0.1.37.tar", last modified: Sat Apr  6 00:14:02 2024, max compression
```

## Comparing `devopsdriver-0.1.36.tar` & `devopsdriver-0.1.37.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-05 00:12:42.035904 devopsdriver-0.1.36/
--rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.36/LICENSE
--rw-r--r--   0 marcp      (501) staff       (20)     5000 2024-04-05 00:12:42.035713 devopsdriver-0.1.36/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)     2431 2024-04-05 00:10:42.000000 devopsdriver-0.1.36/README.md
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-05 00:12:42.031601 devopsdriver-0.1.36/devopsdriver/
--rw-r--r--   0 marcp      (501) staff       (20)      176 2024-04-05 00:10:32.000000 devopsdriver-0.1.36/devopsdriver/__init__.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-05 00:12:42.032632 devopsdriver-0.1.36/devopsdriver/azdo/
--rw-r--r--   0 marcp      (501) staff       (20)      381 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/devopsdriver/azdo/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     1866 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/devopsdriver/azdo/clients.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-05 00:12:42.033126 devopsdriver-0.1.36/devopsdriver/azdo/workitem/
--rw-r--r--   0 marcp      (501) staff       (20)      107 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/devopsdriver/azdo/workitem/__init__.py
--rw-r--r--   0 marcp      (501) staff       (20)     2952 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/devopsdriver/azdo/workitem/client.py
--rw-r--r--   0 marcp      (501) staff       (20)     7777 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/devopsdriver/azdo/workitem/wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     1445 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/devopsdriver/azdo/workitem/workitem.py
--rw-r--r--   0 marcp      (501) staff       (20)     2998 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/devopsdriver/sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    13249 2024-04-05 00:12:25.000000 devopsdriver-0.1.36/devopsdriver/settings.py
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-05 00:12:42.034098 devopsdriver-0.1.36/devopsdriver.egg-info/
--rw-r--r--   0 marcp      (501) staff       (20)     5000 2024-04-05 00:12:42.000000 devopsdriver-0.1.36/devopsdriver.egg-info/PKG-INFO
--rw-r--r--   0 marcp      (501) staff       (20)      668 2024-04-05 00:12:42.000000 devopsdriver-0.1.36/devopsdriver.egg-info/SOURCES.txt
--rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-05 00:12:42.000000 devopsdriver-0.1.36/devopsdriver.egg-info/dependency_links.txt
--rw-r--r--   0 marcp      (501) staff       (20)       71 2024-04-05 00:12:42.000000 devopsdriver-0.1.36/devopsdriver.egg-info/requires.txt
--rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-05 00:12:42.000000 devopsdriver-0.1.36/devopsdriver.egg-info/top_level.txt
--rw-r--r--   0 marcp      (501) staff       (20)     1318 2024-04-03 01:14:37.000000 devopsdriver-0.1.36/pyproject.toml
--rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-05 00:12:42.035948 devopsdriver-0.1.36/setup.cfg
-drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-05 00:12:42.033872 devopsdriver-0.1.36/tests/
--rw-r--r--   0 marcp      (501) staff       (20)     5342 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/tests/test_azure_clients.py
--rw-r--r--   0 marcp      (501) staff       (20)     4201 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/tests/test_azure_workitem.py
--rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/tests/test_azure_workitem_client.py
--rw-r--r--   0 marcp      (501) staff       (20)     2384 2024-04-04 23:50:50.000000 devopsdriver-0.1.36/tests/test_azure_workitem_wiql.py
--rw-r--r--   0 marcp      (501) staff       (20)     4457 2024-04-04 23:59:14.000000 devopsdriver-0.1.36/tests/test_sendmail.py
--rw-r--r--   0 marcp      (501) staff       (20)    11669 2024-04-05 00:09:40.000000 devopsdriver-0.1.36/tests/test_settings.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.739311 devopsdriver-0.1.37/
+-rw-r--r--   0 marcp      (501) staff       (20)     1211 2024-03-30 20:53:59.000000 devopsdriver-0.1.37/LICENSE
+-rw-r--r--   0 marcp      (501) staff       (20)    10268 2024-04-06 00:14:02.739063 devopsdriver-0.1.37/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)     7672 2024-04-06 00:13:19.000000 devopsdriver-0.1.37/README.md
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.736329 devopsdriver-0.1.37/devopsdriver/
+-rw-r--r--   0 marcp      (501) staff       (20)      207 2024-04-06 00:13:02.000000 devopsdriver-0.1.37/devopsdriver/__init__.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.737197 devopsdriver-0.1.37/devopsdriver/azdo/
+-rw-r--r--   0 marcp      (501) staff       (20)      381 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1866 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/clients.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.737756 devopsdriver-0.1.37/devopsdriver/azdo/workitem/
+-rw-r--r--   0 marcp      (501) staff       (20)      107 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/workitem/__init__.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2952 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/workitem/client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     7791 2024-04-05 02:01:31.000000 devopsdriver-0.1.37/devopsdriver/azdo/workitem/wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1445 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/azdo/workitem/workitem.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2998 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/devopsdriver/sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    13249 2024-04-05 00:18:06.000000 devopsdriver-0.1.37/devopsdriver/settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1075 2024-04-06 00:08:39.000000 devopsdriver-0.1.37/devopsdriver/template.py
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.738864 devopsdriver-0.1.37/devopsdriver.egg-info/
+-rw-r--r--   0 marcp      (501) staff       (20)    10268 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/PKG-INFO
+-rw-r--r--   0 marcp      (501) staff       (20)      716 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/SOURCES.txt
+-rw-r--r--   0 marcp      (501) staff       (20)        1 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/dependency_links.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       83 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/requires.txt
+-rw-r--r--   0 marcp      (501) staff       (20)       13 2024-04-06 00:14:02.000000 devopsdriver-0.1.37/devopsdriver.egg-info/top_level.txt
+-rw-r--r--   0 marcp      (501) staff       (20)     1335 2024-04-06 00:08:39.000000 devopsdriver-0.1.37/pyproject.toml
+-rw-r--r--   0 marcp      (501) staff       (20)       38 2024-04-06 00:14:02.739348 devopsdriver-0.1.37/setup.cfg
+drwxr-xr-x   0 marcp      (501) staff       (20)        0 2024-04-06 00:14:02.738698 devopsdriver-0.1.37/tests/
+-rw-r--r--   0 marcp      (501) staff       (20)     5342 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/tests/test_azure_clients.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4201 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/tests/test_azure_workitem.py
+-rw-r--r--   0 marcp      (501) staff       (20)     1740 2024-04-04 23:50:50.000000 devopsdriver-0.1.37/tests/test_azure_workitem_client.py
+-rw-r--r--   0 marcp      (501) staff       (20)     2391 2024-04-05 02:01:31.000000 devopsdriver-0.1.37/tests/test_azure_workitem_wiql.py
+-rw-r--r--   0 marcp      (501) staff       (20)     4457 2024-04-04 23:59:14.000000 devopsdriver-0.1.37/tests/test_sendmail.py
+-rw-r--r--   0 marcp      (501) staff       (20)    11669 2024-04-05 00:09:40.000000 devopsdriver-0.1.37/tests/test_settings.py
+-rw-r--r--   0 marcp      (501) staff       (20)      886 2024-04-06 00:08:39.000000 devopsdriver-0.1.37/tests/test_template.py
```

### Comparing `devopsdriver-0.1.36/LICENSE` & `devopsdriver-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/devopsdriver/azdo/clients.py` & `devopsdriver-0.1.37/devopsdriver/azdo/clients.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/devopsdriver/azdo/workitem/client.py` & `devopsdriver-0.1.37/devopsdriver/azdo/workitem/client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/devopsdriver/azdo/workitem/wiql.py` & `devopsdriver-0.1.37/devopsdriver/azdo/workitem/wiql.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,18 +83,18 @@
     """A constant value"""
 
     def __init__(self, value: date | datetime | int | float | str):
         self.value = value
 
     def __str__(self) -> str:
         if isinstance(self.value, datetime):
-            return self.value.strftime("%Y-%m-%d %H:%M:%S")
+            return f'"{self.value.strftime("%m/%d/%Y %H:%M:%S")}"'
 
         if isinstance(self.value, date):
-            return self.value.strftime("%Y-%m-%d")
+            return f'"{self.value.strftime("%m/%d/%Y")}"'
 
         if isinstance(self.value, int):
             return str(self.value)
 
         if isinstance(self.value, float):
             return f"{self.value:0.3f}"
```

### Comparing `devopsdriver-0.1.36/devopsdriver/azdo/workitem/workitem.py` & `devopsdriver-0.1.37/devopsdriver/azdo/workitem/workitem.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/devopsdriver/sendmail.py` & `devopsdriver-0.1.37/devopsdriver/sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/devopsdriver/settings.py` & `devopsdriver-0.1.37/devopsdriver/settings.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/devopsdriver.egg-info/SOURCES.txt` & `devopsdriver-0.1.37/devopsdriver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 devopsdriver/__init__.py
 devopsdriver/sendmail.py
 devopsdriver/settings.py
+devopsdriver/template.py
 devopsdriver.egg-info/PKG-INFO
 devopsdriver.egg-info/SOURCES.txt
 devopsdriver.egg-info/dependency_links.txt
 devopsdriver.egg-info/requires.txt
 devopsdriver.egg-info/top_level.txt
 devopsdriver/azdo/__init__.py
 devopsdriver/azdo/clients.py
@@ -16,8 +17,9 @@
 devopsdriver/azdo/workitem/wiql.py
 devopsdriver/azdo/workitem/workitem.py
 tests/test_azure_clients.py
 tests/test_azure_workitem.py
 tests/test_azure_workitem_client.py
 tests/test_azure_workitem_wiql.py
 tests/test_sendmail.py
-tests/test_settings.py
+tests/test_settings.py
+tests/test_template.py
```

### Comparing `devopsdriver-0.1.36/pyproject.toml` & `devopsdriver-0.1.37/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 dynamic = ["version"]
 requires-python = ">= 3.10"
 dependencies = [
   "PyYAML==6.0.1",
   "keyring==25.0.0",
   "setuptools==69.0.2",  # neded for azure-devops to use 7.1 API
   "azure-devops==7.1.0b4",
+  "Mako==1.3.2",
 ]
 keywords = ["azure", "devops", "jira", "confluence", "email", "pipelines", "tools"]
 classifiers=[
     "Development Status :: 1 - Planning",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
```

### Comparing `devopsdriver-0.1.36/tests/test_azure_clients.py` & `devopsdriver-0.1.37/tests/test_azure_clients.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/tests/test_azure_workitem.py` & `devopsdriver-0.1.37/tests/test_azure_workitem.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/tests/test_azure_workitem_client.py` & `devopsdriver-0.1.37/tests/test_azure_workitem_client.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/tests/test_azure_workitem_wiql.py` & `devopsdriver-0.1.37/tests/test_azure_workitem_wiql.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,20 +42,20 @@
         .order_by(Descending("Priority"), Ascending("CreatedDate"))
         .asof(start)
     )
     expected = (
         """SELECT [System.State], [System.Id] FROM workitems """
         + """WHERE [System.State] = "New" AND [System.Title] IS EMPTY """
         + """AND [Microsoft.VSTS.Common.Priority] IS NOT EMPTY """
-        + """AND [System.CreatedDate] > 2024-06-30 """
-        + """AND [System.CreatedDate] < 2025-01-01 18:30:15 AND [RootCause] IS EMPTY """
+        + """AND [System.CreatedDate] > "06/30/2024" """
+        + """AND [System.CreatedDate] < "01/01/2025 18:30:15" AND [RootCause] IS EMPTY """
         + """OR [Microsoft.VSTS.Common.Priority] <> 1 OR [Rank] < 5.000 """
         + """OR [time] <= 4.000 OR [BusinessValue] >= 4 """
         + """ORDER BY [Microsoft.VSTS.Common.Priority] DESC, [System.CreatedDate] ASC """
-        + """ASOF 2024-06-30"""
+        + """ASOF "06/30/2024\""""
     )
     assert str(builder) == expected, str(builder)
 
 
 def test_invalid_value_type() -> None:
     """tests assertion that field has known types"""
     try:
```

### Comparing `devopsdriver-0.1.36/tests/test_sendmail.py` & `devopsdriver-0.1.37/tests/test_sendmail.py`

 * *Files identical despite different names*

### Comparing `devopsdriver-0.1.36/tests/test_settings.py` & `devopsdriver-0.1.37/tests/test_settings.py`

 * *Files identical despite different names*

