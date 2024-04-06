# Comparing `tmp/yuag-0.0.62.tar.gz` & `tmp/yuag-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.62.tar", last modified: Fri Apr  5 14:10:07 2024, max compression
+gzip compressed data, was "yuag-0.0.63.tar", last modified: Sat Apr  6 15:33:30 2024, max compression
```

## Comparing `yuag-0.0.62.tar` & `yuag-0.0.63.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 14:10:07.303190 yuag-0.0.62/
--rw-rw-rw-   0        0        0       52 2024-04-05 14:10:07.301192 yuag-0.0.62/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-05 14:10:07.304190 yuag-0.0.62/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-04-05 13:35:47.000000 yuag-0.0.62/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:10:07.272398 yuag-0.0.62/yuag/
--rw-rw-rw-   0        0        0     2814 2024-04-05 13:35:34.000000 yuag-0.0.62/yuag/__init__.py
--rw-rw-rw-   0        0        0    39814 2024-04-05 14:09:35.000000 yuag-0.0.62/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-04-05 14:10:07.299191 yuag-0.0.62/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-04-05 14:10:06.000000 yuag-0.0.62/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-05 14:10:07.000000 yuag-0.0.62/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 14:10:06.000000 yuag-0.0.62/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-05 14:10:06.000000 yuag-0.0.62/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:30.257119 yuag-0.0.63/
+-rw-rw-rw-   0        0        0       52 2024-04-06 15:33:30.254915 yuag-0.0.63/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-06 15:33:30.258117 yuag-0.0.63/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-04-06 15:33:20.000000 yuag-0.0.63/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:30.227907 yuag-0.0.63/yuag/
+-rw-rw-rw-   0        0        0     2814 2024-04-05 13:35:34.000000 yuag-0.0.63/yuag/__init__.py
+-rw-rw-rw-   0        0        0    40281 2024-04-06 15:33:10.000000 yuag-0.0.63/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:33:30.253915 yuag-0.0.63/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-04-06 15:33:29.000000 yuag-0.0.63/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-06 15:33:30.000000 yuag-0.0.63/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 15:33:29.000000 yuag-0.0.63/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-06 15:33:29.000000 yuag-0.0.63/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.62/yuag/__init__.py` & `yuag-0.0.63/yuag/__init__.py`

 * *Files identical despite different names*

### Comparing `yuag-0.0.62/yuag/yuag.py` & `yuag-0.0.63/yuag/yuag.py`

 * *Files 2% similar despite different names*

```diff
@@ -670,31 +670,34 @@
 
         if (equalOrContain == 0 and search_key in newArr[i]) or (equalOrContain == 1 and search_key in "".join(newArr[i])):
             result.append(i)
         i += 1
 
     return result
 
-def searchInObjArr(arr: list, key_want_search: str, value_want_search): # [ {"id": 1, "num": 453}, {"id": 2, "num": 734} ], id == 1 ==> [  [ {"id": 1, "num": 453} ], [0]  ]
+def searchInObjArr(arr: list, key_want_search: str, value_want_search, regex_value: bool = False, multi_values: bool = False): # [ {"id": 1, "num": 453}, {"id": 2, "num": 734} ], id == 1 ==> [  [ {"id": 1, "num": 453} ], [0]  ]
     """
     ```
     [ {"id": 1, "num": 453}, {"id": 2, "num": 734} ]
     key_want_search = "id"
     value_want_search = 1
     
     ==> [  [ {"id": 1, "num": 453} ], [0]  ]
     ```
     """
 
+    import re
+
     res = []
     ind = []
     for i, item in enumerate(arr):
         if type(item) == dict:
             if key_want_search in item:
-                if item[key_want_search] == value_want_search:
+                if ((multi_values == False and                                     (item[key_want_search] == value_want_search or (regex_value == True and re.match(value_want_search, item[key_want_search])))) or
+                    (multi_values == True  and type(value_want_search) == list and (item[key_want_search] in value_want_search or (regex_value == True and      any(re.search(pattern, item[key_want_search]) for pattern in value_want_search))))):
                     res.append(item)
                     ind.append(i)
     
     return [res, ind]
 
 # object {} defs
 def equalObject(the_object: dict, dimensions: int = 0): # the_object1 = the_object2
```

