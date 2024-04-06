# Comparing `tmp/icoder_math-0.0.4.tar.gz` & `tmp/icoder_math-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icoder_math-0.0.4.tar", last modified: Fri Apr  5 09:30:05 2024, max compression
+gzip compressed data, was "icoder_math-0.0.5.tar", last modified: Fri Apr  5 16:26:18 2024, max compression
```

## Comparing `icoder_math-0.0.4.tar` & `icoder_math-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 09:30:05.204496 icoder_math-0.0.4/
--rw-rw-rw-   0        0        0      279 2024-04-05 09:30:05.201492 icoder_math-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      683 2024-04-02 17:58:23.000000 icoder_math-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 09:30:05.126530 icoder_math-0.0.4/icoder_math/
--rw-rw-rw-   0        0        0       51 2024-04-05 09:24:23.000000 icoder_math-0.0.4/icoder_math/__init__.py
--rw-rw-rw-   0        0        0      485 2024-04-03 06:28:42.000000 icoder_math-0.0.4/icoder_math/calculate.py
--rw-rw-rw-   0        0        0     3677 2024-04-05 09:23:44.000000 icoder_math-0.0.4/icoder_math/frequency.py
-drwxrwxrwx   0        0        0        0 2024-04-05 09:30:05.198491 icoder_math-0.0.4/icoder_math.egg-info/
--rw-rw-rw-   0        0        0      279 2024-04-05 09:30:03.000000 icoder_math-0.0.4/icoder_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-04-05 09:30:03.000000 icoder_math-0.0.4/icoder_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 09:30:03.000000 icoder_math-0.0.4/icoder_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-05 09:30:03.000000 icoder_math-0.0.4/icoder_math.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 09:30:05.204496 icoder_math-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      407 2024-04-03 06:27:42.000000 icoder_math-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:26:18.426798 icoder_math-0.0.5/
+-rw-rw-rw-   0        0        0      279 2024-04-05 16:26:18.423797 icoder_math-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      683 2024-04-02 17:58:23.000000 icoder_math-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 16:26:18.253939 icoder_math-0.0.5/icoder_math/
+-rw-rw-rw-   0        0        0        2 2024-04-05 16:24:07.000000 icoder_math-0.0.5/icoder_math/__init__.py
+-rw-rw-rw-   0        0        0      497 2024-04-05 16:22:54.000000 icoder_math-0.0.5/icoder_math/icoCalculators.py
+-rw-rw-rw-   0        0        0     3690 2024-04-05 16:22:49.000000 icoder_math-0.0.5/icoder_math/icoFrequency.py
+drwxrwxrwx   0        0        0        0 2024-04-05 16:26:18.411829 icoder_math-0.0.5/icoder_math.egg-info/
+-rw-rw-rw-   0        0        0      279 2024-04-05 16:26:16.000000 icoder_math-0.0.5/icoder_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-05 16:26:16.000000 icoder_math-0.0.5/icoder_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 16:26:16.000000 icoder_math-0.0.5/icoder_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-05 16:26:16.000000 icoder_math-0.0.5/icoder_math.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 16:26:18.426798 icoder_math-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      407 2024-04-05 16:23:07.000000 icoder_math-0.0.5/setup.py
```

### Comparing `icoder_math-0.0.4/README.md` & `icoder_math-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `icoder_math-0.0.4/icoder_math/frequency.py` & `icoder_math-0.0.5/icoder_math/icoFrequency.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-
-def all(data, index,listStatus, totalPeriod):
+def icoAll(data, index, listStatus, totalPeriod):
     """
-        data: a list of dict\n
-        index: index frequency\n
-        listStatus: show list True/False\n
-        totalPeriod: if index is not range = 0 else number split\n
-        return : f , r , rd(%) , F , R , RD(%) , list=[...]
+    data: a list of dict\n
+    index: index frequency\n
+    listStatus: show list True/False\n
+    totalPeriod: if index is not range = 0 else number split\n
+    return : f , r , rd(%) , F , R , RD(%) , list=[...]
     """
     if totalPeriod == 0:
-        return unPeriod(data, index,listStatus)
+        return icoUnPeriod(data, index, listStatus)
     else:
-        return period(data, index, totalPeriod,listStatus)
+        return icoPeriod(data, index, totalPeriod, listStatus)
 
 
-def unPeriod(data, index,listStatus):
+def icoUnPeriod(data, index, listStatus):
     range_list = {}
     total = len(data)
     for item in data:
         if item[index] not in range_list:
             range_list[item[index]] = {}
             range_list[item[index]]["list"] = []
         if listStatus:
             range_list[item[index]]["list"].append(item)
         else:
-            range_list[item[index]]["list"]=[]
+            range_list[item[index]]["list"] = []
         range_list[item[index]]["f"] = len(range_list[item[index]]["list"])
 
     final = {}
     i = 0
     for key, item in range_list.items():
         if i not in final:
             f = item["f"]
@@ -53,55 +52,55 @@
                 "list": item["list"],
             }
             i += 1
 
     return final
 
 
-def period(data, index, totalPeriod,listStatus):
-    range_list = range(data, index, totalPeriod)
+def icoPeriod(data, index, totalPeriod, listStatus):
+    range_list = icoRange(data, index, totalPeriod)
     total = len(data)
     for key, item in range_list.items():
         minnum = float(item["index"]["min"])
         maxnum = float(item["index"]["max"])
         itemlist = []
         remaining_data = []
         for value in data:
             if float(value[index]) >= minnum and float(value[index]) < maxnum:
                 itemlist.append(value)
             else:
                 remaining_data.append(value)
         data = remaining_data
-        f=len(itemlist)
+        f = len(itemlist)
         r = float("{:.2f}".format(len(itemlist) / total))
-        rd=int(r * 100)
-        if key ==0 :
-            F=f 
-            R=r
-            RD=rd
+        rd = int(r * 100)
+        if key == 0:
+            F = f
+            R = r
+            RD = rd
         else:
             F = range_list[key - 1]["F"] + f
             R = float(range_list[key - 1]["R"]) + r
             RD = int(range_list[key - 1]["RD"]) + rd
         if listStatus == False:
-            itemlist=[]
+            itemlist = []
         range_list[key] = {
             "index": {"min": minnum, "max": maxnum},
             "f": f,
             "r": r,
             "rd": rd,
             "F": F,
             "R": "{:.2f}".format(R),
             "RD": RD,
             "list": itemlist,
         }
     return range_list
 
 
-def range(data, index, totalPeriod):
+def icoRange(data, index, totalPeriod):
     max_num = float(max(data, key=lambda x: float(x[index]))[index])
     min_num = float(min(data, key=lambda x: float(x[index]))[index])
     r = float((max_num + 0.5) - (min_num - 0.5)) / totalPeriod
     i = 0
     range = {}
     current_num = min_num
     next_num = float("{:.2f}".format(current_num + r))
@@ -113,9 +112,7 @@
             },
             "list": [],
         }
         current_num = next_num
         next_num = float("{:.2f}".format(current_num + r))
         i += 1
     return range
-
-
```

