# Comparing `tmp/GoogleNb-0.0.2.tar.gz` & `tmp/GoogleNb-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GoogleNb-0.0.2.tar", last modified: Tue Apr  2 22:17:59 2024, max compression
+gzip compressed data, was "GoogleNb-0.0.3.tar", last modified: Sat Apr  6 21:07:37 2024, max compression
```

## Comparing `GoogleNb-0.0.2.tar` & `GoogleNb-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 22:17:59.574269 GoogleNb-0.0.2/
--rw-rw-rw-   0        0        0     1083 2024-02-04 19:16:00.000000 GoogleNb-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      788 2024-04-02 22:17:59.572267 GoogleNb-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-04-02 22:11:48.000000 GoogleNb-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 22:17:59.574269 GoogleNb-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1083 2024-03-29 21:45:41.000000 GoogleNb-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:17:59.484268 GoogleNb-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 22:17:59.539268 GoogleNb-0.0.2/src/GoogleNb/
--rw-rw-rw-   0        0        0     1713 2024-03-27 13:07:44.000000 GoogleNb-0.0.2/src/GoogleNb/GoogleDrive.py
--rw-rw-rw-   0        0        0     6008 2024-04-02 22:13:14.000000 GoogleNb-0.0.2/src/GoogleNb/GoogleSheet.py
--rw-rw-rw-   0        0        0        0 2024-03-19 20:27:02.000000 GoogleNb-0.0.2/src/GoogleNb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 22:17:59.571267 GoogleNb-0.0.2/src/GoogleNb.egg-info/
--rw-rw-rw-   0        0        0      788 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 22:17:59.000000 GoogleNb-0.0.2/src/GoogleNb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 21:07:37.415145 GoogleNb-0.0.3/
+-rw-rw-rw-   0        0        0     1083 2024-02-04 19:16:00.000000 GoogleNb-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      788 2024-04-06 21:07:37.414146 GoogleNb-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-04-02 22:11:48.000000 GoogleNb-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 21:07:37.415145 GoogleNb-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2024-04-06 21:06:34.000000 GoogleNb-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 21:07:37.338144 GoogleNb-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 21:07:37.380145 GoogleNb-0.0.3/src/GoogleNb/
+-rw-rw-rw-   0        0        0     1713 2024-03-27 13:07:44.000000 GoogleNb-0.0.3/src/GoogleNb/GoogleDrive.py
+-rw-rw-rw-   0        0        0     8159 2024-04-06 21:05:42.000000 GoogleNb-0.0.3/src/GoogleNb/GoogleSheet.py
+-rw-rw-rw-   0        0        0        0 2024-03-19 20:27:02.000000 GoogleNb-0.0.3/src/GoogleNb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 21:07:37.413145 GoogleNb-0.0.3/src/GoogleNb.egg-info/
+-rw-rw-rw-   0        0        0      788 2024-04-06 21:07:37.000000 GoogleNb-0.0.3/src/GoogleNb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-04-06 21:07:37.000000 GoogleNb-0.0.3/src/GoogleNb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 21:07:37.000000 GoogleNb-0.0.3/src/GoogleNb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-06 21:07:37.000000 GoogleNb-0.0.3/src/GoogleNb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 21:07:37.000000 GoogleNb-0.0.3/src/GoogleNb.egg-info/top_level.txt
```

### Comparing `GoogleNb-0.0.2/LICENSE` & `GoogleNb-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GoogleNb-0.0.2/PKG-INFO` & `GoogleNb-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleNb
-Version: 0.0.2
+Version: 0.0.3
 Summary: API google
 Home-page: https://github.com/niba291/PyDrive
 Author: niba291
 Author-email: nibaldochavezp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `GoogleNb-0.0.2/setup.py` & `GoogleNb-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools                     import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name                            = "GoogleNb",
-    version                         = "0.0.2",
+    version                         = "0.0.3",
     author                          = "niba291",
     author_email                    = "nibaldochavezp@gmail.com",
     description                     = "API google",
     url                             = "https://github.com/niba291/PyDrive",
     license                         = "MIT",
     long_description                = long_description,
     long_description_content_type   = "text/markdown",
```

### Comparing `GoogleNb-0.0.2/src/GoogleNb/GoogleDrive.py` & `GoogleNb-0.0.3/src/GoogleNb/GoogleDrive.py`

 * *Files identical despite different names*

### Comparing `GoogleNb-0.0.2/src/GoogleNb/GoogleSheet.py` & `GoogleNb-0.0.3/src/GoogleNb/GoogleSheet.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,172 +2,219 @@
 from google.oauth2 import service_account
 
 class GoogleSheet:
 
     CREDS           = None
     SERVICE         = None
     SHEET           = None
-    FORMAT          = None
+    FORMAT          = None    
     FORMAT_DEFAULT  = "JSON"
     SCOPE           = ["https://www.googleapis.com/auth/spreadsheets"]
+    ERROR           = {
+        "error"     : False,
+        "response"  : ""
+    }
 
     def __init__(self, key: str = "", format = FORMAT_DEFAULT):
         """
             Creates a GoogleSheet instance.
             
             Args:
                 key (str)           : The path to the service account json file.
         """
         try:
             self.CREDS          = service_account.Credentials.from_service_account_file(key, scopes=self.SCOPE)
             self.SERVICE        = build("sheets", "v4", credentials=self.CREDS)
             self.SHEET          = self.SERVICE.spreadsheets()
             self.FORMAT         = format.upper()
         except Exception as e:
-            print({
-                "error"     : True,
-                "response"  : str(e)
-            })
-            exit(1)
+            self.ERROR          = {
+                "error"         : True,
+                "response"      : str(e)
+            }
 
-    def get(self, spreadsheetId: str = "", range: str = "", filter: str = None) -> dict:
+    def get(self, spreadsheetId: str = "", ranges: list = [], filter: list = None) -> dict:
         """
             Get the data from the sheet.
             
             Args:
                 spreadsheetId (str) : Id google sheet.
-                range (str)         : Column or row range.
-                filter (str)        : filter by str.
+                range (list)        : Column or row range.
+                filter (list)       : filter.
 
             Returns:
                 dict                : return list
         """
+        if self.ERROR["error"]: return self.ERROR
         try:
             
             if filter != None:
-                self.SHEET_NAME = "FILTER"
-                auxRange        = range.split(":")
-                range           = "B1"
-                self.update(filter)
-                range           = f"{auxRange[0]}2:{auxRange[1]}"
-
-            result              = self.SHEET.values().get(
-                spreadsheetId   = spreadsheetId, 
-                range           = range
-            ).execute()
-
-            auxReturn           = result["values"]
-
-            if(self.FORMAT == self.FORMAT_DEFAULT):
-
-                auxReturn           = []
-
-                for element in result["values"][1:]:
-                    obj             = {}
-                    lenList         = len(element)
-                    for index, item in enumerate(result["values"][0]):
-                        obj[item]   = element[index] if lenList > index else ""
-                    
-                    auxReturn.append(obj)
+                result                  = self.SHEET.values().batchGetByDataFilter(
+                    spreadsheetId       = spreadsheetId, 
+                    body                = {
+                        "dataFilters"   : filter
+                    }
+                ).execute()
+            else:
+                result                  = self.SHEET.values().batchGet(
+                    spreadsheetId       = spreadsheetId, 
+                    ranges              = ranges
+                ).execute()
+
+            
+            if(self.FORMAT != self.FORMAT_DEFAULT):
+                return result["valueRanges"]
+            
+            auxReturn                   = {}
+
+            for element in result["valueRanges"]:
+                auxList                 = []
+                keyElement              = element["range"].split("!")[0]
+                for items in element["values"][1:]:
+                    obj                 = {}
+                    lenList             = len(items)
+                    for index, item in enumerate(element["values"][0]):
+                        obj[item]       = items[index] if lenList > index else ""    
+                    auxList.append(obj)
+                
+                auxReturn[keyElement]   = auxList
 
             return auxReturn
         except Exception as e:
-            return {
+            self.ERROR      = {
                 "error"     : True,
                 "response"  : str(e)
             }
+            return self.ERROR
 
     def add(self, spreadsheetId: str = "", range: str = "", data: dict = {}) -> dict:
         """
             Add data to the sheet.
             
             Args:
                 spreadsheetId (str) : Id google sheet.
                 range (str)         : Column or row range.
                 data (dict)         : array data.
 
             Returns:
                 dict                : return response of the sheet
         """
+        if self.ERROR["error"]: return self.ERROR
         try:
             return self.SHEET.values().append(
                 spreadsheetId    = spreadsheetId, 
                 range            = range, 
                 valueInputOption = "USER_ENTERED", 
                 body             = {"values": data}
             ).execute()
         except Exception as e:
-            return {
+            self.ERROR      = {
                 "error"     : True,
                 "response"  : str(e)
             }
+            return self.ERROR
 
     def update(self, spreadsheetId: str = "", range: str = "", data: dict = {}) -> dict:
         """
             Update data to the sheet.
             
             Args:
                 spreadsheetId (str) : Id google sheet.
                 range (str)         : Column or row range.
                 data (dict)         : array data.
 
             Returns:
                 dict                : return response of the sheet
         """
+        if self.ERROR["error"]: return self.ERROR
         try:
             return self.SHEET.values().update(
                 spreadsheetId    = spreadsheetId, 
                 range            = range, 
                 valueInputOption = "USER_ENTERED", 
                 body             = {"values": data}
             ).execute()
         except Exception as e:
-            return {
+            self.ERROR      = {
                 "error"     : True,
                 "response"  : str(e)
             }
+            return self.ERROR
 
-    def delete(self, spreadsheetId: str = "", idSheet: str = "", range: str = "") -> dict:
+    def delete(self, spreadsheetId: str = "", range: str = "", idSheet: str = "") -> dict:
         """
             Delete data to the sheet.
             
             Args:
                 spreadsheetId (str) : Id sheet.
                 range (str)         : Column or row range.
                 idSheet (dict)      : id sheet.
 
             Returns:
                 dict                : return response of the sheet
         """
+        if self.ERROR["error"]: return self.ERROR
         try:
-            auxRange                = range.split(":")
+            requests                = []
+            for row in sorted(map(int, range.split(":")), reverse = True):
+                requests.append({
+                    "deleteDimension"   : {
+                        "range"         : {
+                            "sheetId"   : idSheet,
+                            "dimension" : "ROWS",
+                            "startIndex": int(row) - 1,
+                            "endIndex"  : int(row)
+                        }
+                    }
+                })
+
             return self.SHEET.batchUpdate(
                 spreadsheetId       = spreadsheetId, 
                 body                = {
-                    "requests"      : [
-                        {
-                            "deleteDimension": {
-                                "range": {
-                                    "sheetId"    : idSheet,
-                                    "dimension"  : "ROWS",
-                                    "startIndex" : auxRange[0],
-                                    "endIndex"   : auxRange[1]
-                                }
-                            }
-                        }
-                    ]
+                    "requests"      : requests
                 }
             ).execute()
         except Exception as e:
-            return {
+            self.ERROR      = {
                 "error"     : True,
                 "response"  : str(e)
             }
+            return self.ERROR
 
     def info(self) -> object:
         """
             Get sheet info.
 
             Returns:
                 object              : return sheet info
         """
-        return self.SHEET.sheets()
+        return self.SHEET.sheets()
+    
+    def conditional_formatting(self, spreadsheetId: str = ""):
+        try:
+            if self.ERROR["error"]: return self.ERROR
+            return self.SHEET.batchUpdate(spreadsheetId=spreadsheetId, body={
+                "requests"                                  : [
+                    {
+                        "setDataValidation"                 : {
+                            "range"                         : "Formulario Receta!A1:C3",
+                            "rule"                          : {
+                                "condition"                 : {
+                                    "type"                  : "ONE_OF_RANGE",
+                                    "values"                : [
+                                        {"userEnteredValue" : "=Datos!$C$1:$C$777"}
+                                    ]
+                                },
+                                "showCustomUi"              : True,
+                                "strict"                    : True
+                            }
+                        }
+                    }
+                ]
+            }).execute()
+
+        except Exception as e:
+            self.ERROR      = {
+                "error"     : True,
+                "response"  : str(e)
+            }
+            return self.ERROR
```

### Comparing `GoogleNb-0.0.2/src/GoogleNb.egg-info/PKG-INFO` & `GoogleNb-0.0.3/src/GoogleNb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GoogleNb
-Version: 0.0.2
+Version: 0.0.3
 Summary: API google
 Home-page: https://github.com/niba291/PyDrive
 Author: niba291
 Author-email: nibaldochavezp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

