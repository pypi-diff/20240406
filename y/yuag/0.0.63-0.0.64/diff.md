# Comparing `tmp/yuag-0.0.63.tar.gz` & `tmp/yuag-0.0.64.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yuag-0.0.63.tar", last modified: Sat Apr  6 15:33:30 2024, max compression
+gzip compressed data, was "yuag-0.0.64.tar", last modified: Sat Apr  6 15:47:17 2024, max compression
```

## Comparing `yuag-0.0.63.tar` & `yuag-0.0.64.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 15:33:30.257119 yuag-0.0.63/
--rw-rw-rw-   0        0        0       52 2024-04-06 15:33:30.254915 yuag-0.0.63/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-06 15:33:30.258117 yuag-0.0.63/setup.cfg
--rw-rw-rw-   0        0        0      249 2024-04-06 15:33:20.000000 yuag-0.0.63/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 15:33:30.227907 yuag-0.0.63/yuag/
--rw-rw-rw-   0        0        0     2814 2024-04-05 13:35:34.000000 yuag-0.0.63/yuag/__init__.py
--rw-rw-rw-   0        0        0    40281 2024-04-06 15:33:10.000000 yuag-0.0.63/yuag/yuag.py
-drwxrwxrwx   0        0        0        0 2024-04-06 15:33:30.253915 yuag-0.0.63/yuag.egg-info/
--rw-rw-rw-   0        0        0       52 2024-04-06 15:33:29.000000 yuag-0.0.63/yuag.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-06 15:33:30.000000 yuag-0.0.63/yuag.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 15:33:29.000000 yuag-0.0.63/yuag.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-06 15:33:29.000000 yuag-0.0.63/yuag.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 15:47:17.052001 yuag-0.0.64/
+-rw-rw-rw-   0        0        0       52 2024-04-06 15:47:17.048718 yuag-0.0.64/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-06 15:47:17.052001 yuag-0.0.64/setup.cfg
+-rw-rw-rw-   0        0        0      249 2024-04-06 15:47:07.000000 yuag-0.0.64/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:47:17.017348 yuag-0.0.64/yuag/
+-rw-rw-rw-   0        0        0     2814 2024-04-05 13:35:34.000000 yuag-0.0.64/yuag/__init__.py
+-rw-rw-rw-   0        0        0    42076 2024-04-06 15:46:13.000000 yuag-0.0.64/yuag/yuag.py
+drwxrwxrwx   0        0        0        0 2024-04-06 15:47:17.046717 yuag-0.0.64/yuag.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-04-06 15:47:16.000000 yuag-0.0.64/yuag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-06 15:47:16.000000 yuag-0.0.64/yuag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 15:47:16.000000 yuag-0.0.64/yuag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-06 15:47:16.000000 yuag-0.0.64/yuag.egg-info/top_level.txt
```

### Comparing `yuag-0.0.63/yuag/__init__.py` & `yuag-0.0.64/yuag/__init__.py`

 * *Files identical despite different names*

### Comparing `yuag-0.0.63/yuag/yuag.py` & `yuag-0.0.64/yuag/yuag.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 def wait(wait_time: int = 1):
     import time
 
     time.sleep(wait_time)
 
 def clear():
     """
+    سبحان الله\n
     مسح الطَّرَفِيَّة
     """
 
     import os
 
     os.system("cls")
 
@@ -53,14 +54,15 @@
         if detectOrSrc == 0: return detect(text)
         else: return Translator().translate(text).src
     except:
         return 404
 
 def rangeNum(num, range_or_while_method = 0):
     """
+    الحمدلله\n
     ```
     rangeNum(3)
 
     ==> [0, 1, 2]
     ```
     """
     
@@ -131,14 +133,15 @@
     if new_file_path is None:
         new_file_path = f"{file_path} - Copy"
 
     shutil.copy(file_path, new_file_path)
 
 def move_file(file_path: str, new_folder_path: str = None):
     """
+    لا إله إلا الله\n
     دالة لاقتصاص الملف وارساله لمكان آخر\n\n
 
     مثال
     ------------
     ```
     file_path = "file.txt"
     new_folder_path = "./folder"
@@ -158,16 +161,17 @@
     import shutil
 
     shutil.rmtree(folder_path)
 
 # arr defs
 def equalArr(arr: list, dimensions: int = 0): # arr1 = arr2
     """
-    equalArr
+    الله أكبر
     -----------------
+
     عند عمل مصفوفة واستنساخها:
     ```
     arr1 = [1, 2, 3]
     arr2 = arr1
     ```
     فإن أي تعديل تقوم به على المصفوفة الثانية يُغيّر أيضا في المصفوفة الأولى،
     ولهذا جاءت هذه الدالة: لتقوم باستنساخ المصفوفة بدون مشاكل، فقط عليك ان تدخل عدد ابعاد المصفوفة\n\n
@@ -232,14 +236,15 @@
                 
                 i += 1
 
     return res
 
 def allIndexInArr(arr: list, item): # 1D arr=[10,20,30,40,30], item=30 ==> [2,4]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     arr = [10, 20, 30, 40, 30]
     item = 30
     
     ==> [2, 4]
     ```
     """
@@ -252,21 +257,24 @@
             allIndex.append(i)
         i += 1
 
     return allIndex
 
 def inArr(arr: list, item): # ==> True, False
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ==> True || False
     """
 
     return item in arr
 
 def onSide(arr: list, item, greater: int = 1, startFrom: bool = 0, multi_items: bool = False, want_items: bool = False): # 2D arr=[1,1,1,3,2,2,2,1,2,2], item=2, greater=1 ==> [ [4,5,6], [8,9] ] ==> [ indexArr ]
     """
+    اللهم صل على سيدنا محمد ﷺ\n\n
+
     هذه الدالة تقوم بإرجاع اماكن العناصر الموضوعين بجانب بعضهم\n
     arr: المصفوفة\n
     item: العنصر الذي تريده\n
     greater: عدد العناصر التي تريد أن يكونوا بجانب بعضهم + 1 (greater: أكبر)\n
     start_from: مكان البدء (ادخل الفهرس)\n
     multi_items: هل تريد حساب أكثر من عنصر؟\n
     want_items: هل تريد ارجاع العناصر أيضا مع الفهرس؟\n\n
@@ -313,14 +321,16 @@
     if want_items == 0:
         return finalArr
     else:
         return [finalItemsArr, finalArr]
 
 def fillArr(arr: list, fill, fromNum: int = -1, toNum: int = -1): # arr=["⬜","⬜","⬜"], fill="🟩", from=0,to=1 ==> ["🟩","🟩","⬜"] #
     """
+    اللهم صل على سيدنا محمد ﷺ\n\n
+
     ```
     arr = ["⬜","⬜","⬜"]
     fill = "🟩"
     fromNum = 0
     toNum = 1
     ```
 
@@ -389,14 +399,15 @@
                     
         i += 1
             
     return arr
 
 def sumArr(arr: list, fromNum: int = -1, toNum: int = -1): # arr=[1,2,3], fromNum=0, toNum=1 ==> 1+2 = 3
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     arr=[1, 2, 3]
     fromNum = 0
     toNum = 1
     
     ==> 1+2 = 3
     ```
@@ -415,14 +426,15 @@
         sum += arr[fromNum]
         fromNum += 1
     
     return sum
 
 def minusArr(arr: list): # [1,4,5,8,7] ==> [3,1,3,-1]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     arr = [1, 4, 5, 8, 7]
     
     ==> [3, 1, 3, -1]
     ```
     """
 
@@ -433,14 +445,15 @@
         res.append(arr[i] - arr[i-1])
         i += 1
     
     return res
 
 def makeColumnArr(arr: list, column: int = 0): # convert column in 2D arr to arr
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     تحويل العمود في المصفوفة ثنائية الأبعاد إلى مصفوفة منفصلة
     """
     
     arrLen = len(arr)
     columnArr = []
 
     i = 0
@@ -448,26 +461,28 @@
         if column < len(arr[i]): columnArr.append(arr[i][column])
         i += 1
 
     return columnArr
 
 def convertRowToCol(arr: list, columnArr: list, column: int = 0): # Col ==> column, columnArr ==> row
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     تحويل المصفوفة أحادية الأبعاد إلى عمود في مصفوفة ثنائية الأبعاد
     """
     
     i = 0
     while i < len(columnArr):
         arr[i][column] = columnArr[i]
         i += 1
     
     return arr
 
 def addArr(fromArr: list, toArr: list): # fromArr=[4,5,6], toArr=[1,2,3] ==> [1,2,3,4,5,6]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     إضافة مصفوفة إلى أخرى\n
 
     مثال
     -------
     ```
     fromArr=[4, 5, 6]
     toArr=[1, 2, 3]
@@ -480,14 +495,15 @@
     for x in fromArr:
         toArr.append(x)
 
     return toArr
 
 def delArr(smallArr: list, bigArr: list): # smallArr = [4,5,6], bigArr=[1,2,3,4,5,6] ==> [1,2,3]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     إلغاء مصفوفة من أخرى\n
 
     مثال
     ------------
     ```
     smallArr = [4,5,6]
     bigArr=[1,2,3,4,5,6]
@@ -503,14 +519,15 @@
         if inArr(bigArr, x):
             bigArr = removeFromArr(bigArr, -1, x)
     
     return bigArr
 
 def sliceArr(arr: list, fromNum: int = 0, toNum: int = 0): # arr=[10,20,30,40,50], fromNum=1, toNum=3 ==> [20,30,40]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     arr = [10, 20, 30, 40, 50]
     fromNum = 1
     toNum = 3
     
     ==> [20, 30, 40]
     ```
@@ -523,14 +540,15 @@
         newArr.append(arr[i])
         i += 1
     
     return newArr
 
 def reverseArr(arr: list): # arr=[1,2,3] ==> [3,2,1]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     عكس المصفوفة
 
     مثال
     ---------
     ```
     arr=[1, 2, 3]
     
@@ -538,14 +556,15 @@
     ```
     """
 
     return arr[::-1]
 
 def search2D(arr: list, item, column: int = 0): # ==> [index]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     البحث عن عنصر في مصفوفة ثنائية الأبعاد عن طريق العمود
     """
 
     res = []
     ind = []
 
     i = 0
@@ -555,14 +574,15 @@
             ind.append(i)
         i += 1
 
     return [res, ind]
 
 def convert2D(arr: list): # ==> 1D, convert 2D to 1D, arr=[ [1,2,3], [4,5,6], [7,8,9] ] ==> [1,2,3,4,5,6,7,8,9]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     تحويل المصفوفة ثنائية الأبعاد إلى أحادية الأبعاد\n
 
     مثال
     -----------
     ```
     arr=[ [1,2,3], [4,5,6], [7,8,9] ]
     
@@ -600,14 +620,15 @@
         arr = res
         a += 1
     
     return arr
 
 def insertInArr(arr: list, itemToInsert, itemIndex: int = 0, isMultiItems: int = 0): # arr=[1,3,4], itemToInsert=2 ==> [1,2,3,4]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     arr=[1,3,4]
     itemToInsert = 2
     itemIndex = 1
 
     ==> [1,2,3,4]
     ```
@@ -628,14 +649,15 @@
         res.append(arr[i])
         i += 1
 
     return res
 
 def convertTxt(text: str): # convert text to code, "5 + 7" ==> 12
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     تحويل النص لشيفرة\n
 
     مثال
     -----------------
     ```
     "5 + 7" ==> 12
     ```
@@ -645,14 +667,15 @@
         return eval(text)
     except Exception as e:
         print("حدث خطأ في التحويل:", e)
         return None
 
 def searchIn_decodeNum(arr: list, search_key, equalOrContain: int = 0): # arr=["n1", "o1", "n2"], search_key="n" ==> [0, 2] => [index]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     arr=["n1", "o1", "n2"]
     search_key = "n"
     
     ==> [0, 2]
     ==> [فهرس]
     ```
@@ -672,14 +695,15 @@
             result.append(i)
         i += 1
 
     return result
 
 def searchInObjArr(arr: list, key_want_search: str, value_want_search, regex_value: bool = False, multi_values: bool = False): # [ {"id": 1, "num": 453}, {"id": 2, "num": 734} ], id == 1 ==> [  [ {"id": 1, "num": 453} ], [0]  ]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     [ {"id": 1, "num": 453}, {"id": 2, "num": 734} ]
     key_want_search = "id"
     value_want_search = 1
     
     ==> [  [ {"id": 1, "num": 453} ], [0]  ]
     ```
@@ -698,16 +722,16 @@
                     ind.append(i)
     
     return [res, ind]
 
 # object {} defs
 def equalObject(the_object: dict, dimensions: int = 0): # the_object1 = the_object2
     """
-    equalObject
-    -----------------
+    اللهم صل على سيدنا محمد ﷺ\n
+    
     عند عمل قاموس واستنساخه:
     ```
     obj1 = {"number": 1}
     obj2 = obj1
     ```
     فإن أي تعديل تقوم به على القاموس الثاني يُغيّر أيضا في القاموس الأول،
     ولهذا جاءت هذه الدالة: لتقوم باستنساخ القاموس بدون مشاكل، فقط عليك ان تدخل عدد ابعاد القاموس\n\n
@@ -766,14 +790,15 @@
                 else:
                     res[key] = item                
 
     return res
 
 def getObjectKeys(the_object: dict): # {"h1": "text", "h2": "text2"} ==> ["h1", "h2"]
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     the_object = {"h1": "text", "h2": "text2"}
     
     ==> ["h1", "h2"]
     ```
     """
     
@@ -781,14 +806,15 @@
     for key in the_object:
         keys.append(key)
     
     return keys
 
 def addToObject(the_object: dict, key: str, want_to_add): # {"name": "about"}, "name", "about" ==> {"name": "about", "name 2": "about"}
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     the_object = {"name": "about"}
     key = "name"
     value = "about"
     
     ==> {"name": "about", "name 2": "about"}
     ```
@@ -800,14 +826,15 @@
     else:
         the_object[key] = want_to_add
 
     return the_object
 
 def key_index(the_object: dict, key: str):
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     مثال
     -----------
     ```
     the_object = {"number 1": 10, "number 2": 20, "number 3": 30}
     key = "number 3"
 
     ==> 2
@@ -828,14 +855,15 @@
             if key == item:
                 return i
     else:
         return -1
 
 def delete_key(the_object: dict, key: str): # {"n1":10, "n2":20, "n3":30}, key = "n1" ==> {"n2":20, "n3":30}
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     مثال
     ----------
     ```
     the_object = {"number 1": 10, "number 2": 20, "number 3": 30}
     key = "number 1"
     ==> {"number 2": 20, "number 3": 30}\n\n
     ```
@@ -857,14 +885,15 @@
         for item in key:
             the_object = delete_key(the_object, item)
 
     return the_object
 
 def insert_key(the_object: dict, i: int, key: str, value = None, change_value: bool = False):
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     مثال
     -----------
     ```
     the_object = {"num1": 10, "num3": 30}
     i = 1
     key = "num2"
     value = 20
@@ -899,14 +928,15 @@
     if change_value and key in the_object:
         tmp_list.remove((key, the_object[key]))
 
     return {**dict(tmp_list[:i]), key: value, **dict(tmp_list[i:])}
 
 def change_key(the_object: dict, old_key: str, new_key: str): # {"number 1": 10, "number 5": 20, "number 3": 30}, "number 5", "number 2" ==> {"number 1": 10, "number 2": 20, "number 3": 30} #
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     the_object = {"number 1": 10, "number 5": 20, "number 3": 30}
     old_key = "number 5"
     new_key = "number 2"
 
     ==> {"number 1": 10, "number 2": 20, "number 3": 30}
     ```
@@ -987,14 +1017,15 @@
     return text[:amount]
 
 def mid(text: str, offset: int, amount: int):
     return text[offset:offset+amount]
 
 def split(text: str, splitter: str | list[str] = ""):
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     هذه الدالة تقسم النص
     """
     
     res = []
     if splitter == "":
         for char in text:
             res.append(char)
@@ -1020,23 +1051,25 @@
 
                             res_i -= 1
 
     return res
 
 def removeSpaces(text: str): # إلغاء   المسافات
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     إلغاء   المسافات
     """
     
     text = " ".join(RemoveDuplicates(text.split(" "), 1, 1, ""))
     text = " ".join(removeFromArr(text.split(" "), -1, ""))
     return text.strip()
 
 def replaceText(text: str, replArr: list): # text = "hello word!", replArr = [ ["word", "world"], ["!", "."] ] ==> "hello world."
     """
+    اللهم صل على سيدنا محمد ﷺ\n
     ```
     text = "hello word!"
     replArr = [ ["word", "world"], ["!", "."] ]
     ```
     \n\n
     ==> "hello world."
     """
@@ -1047,34 +1080,42 @@
         i += 1
 
     return text
 
 # num defs
 def makeZeroNum(num: str | int, cells_num: int = 3, zero: str = "0"):
     """
+    اللهم صل على سيدنا محمد ﷺ\n
+
+    ```
     num = "10"
     cells_num = 4
     ==> "0010"
+    ```
     """
 
     num = str(num)
     if cells_num > len(num):
         for item in rangeNum(cells_num - len(num)):
             num = zero + num
     
     return num
 
 # separate defs
 def separate_text(text: str, splitter: list = ["."], joiner: str = "\n", stripping: str = 0, delete_splitter: int = 0): # "line1.line2" ==> "line1.\nline2"
     """
+    اللهم صل على سيدنا محمد ﷺ\n
+    
+    ```
     text = "line1.line2"
     splitter = ["."] # بعد النقطة ضع سطرًا جديدًا
     joiner = "\n"
 
     ==> "line1.\nline2"
+    ```
     """
     
     if type(splitter) == list:
         for item in splitter:
             tmp = text.split(item)
             if stripping == 1:
                 for tmp_i, tmpItem in enumerate(tmp): tmp[tmp_i] = tmpItem.strip()
@@ -1222,14 +1263,16 @@
             new_obj[translate_text(i, target_language, not_langs)] = obj[i]
 
     return new_obj
 
 # decode html
 def decode_html_in_text(text: str, tag: str = "img", attribute: str = "src", endTag: int = 0, delete_inner_html: int = 0):
     """
+    اللهم صل على سيدنا محمد ﷺ\n
+    
     مثال:
     --------------
     ```
     text = '<img src="the_link.com">'
     tag = "img"
     attribute = "src"
     endTag = 0
```

