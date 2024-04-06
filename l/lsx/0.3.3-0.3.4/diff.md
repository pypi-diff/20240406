# Comparing `tmp/lsx-0.3.3.tar.gz` & `tmp/lsx-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lsx-0.3.3.tar", last modified: Sat Jan 27 06:50:42 2024, max compression
+gzip compressed data, was "dist\lsx-0.3.4.tar", last modified: Sat Apr  6 01:42:48 2024, max compression
```

## Comparing `lsx-0.3.3.tar` & `lsx-0.3.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-01-27 06:50:42.000000 lsx-0.3.3/
--rw-rw-rw-   0        0        0       98 2023-12-16 00:09:21.000000 lsx-0.3.3/.gitignore
--rw-rw-rw-   0        0        0     1125 2024-01-13 03:31:00.000000 lsx-0.3.3/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx/
--rw-rw-rw-   0        0        0     3131 2024-01-13 03:19:33.000000 lsx-0.3.3/lsx/auto.py
--rw-rw-rw-   0        0        0     3446 2023-12-16 00:09:21.000000 lsx-0.3.3/lsx/c.py
--rw-rw-rw-   0        0        0     5303 2023-12-16 00:09:21.000000 lsx-0.3.3/lsx/cls.py
--rw-rw-rw-   0        0        0     4494 2023-12-16 00:09:21.000000 lsx-0.3.3/lsx/dec.py
--rw-rw-rw-   0        0        0     9817 2024-01-27 06:48:51.000000 lsx-0.3.3/lsx/doc.py
-drwxrwxrwx   0        0        0        0 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx/docs/
--rw-rw-rw-   0        0        0     1125 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx/docs/LICENSE.txt
--rw-rw-rw-   0        0        0     5253 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx/docs/README.md
--rw-rw-rw-   0        0        0       59 2023-12-16 00:09:21.000000 lsx-0.3.3/lsx/docs/__init__.py
--rw-rw-rw-   0        0        0     2375 2023-12-16 00:09:21.000000 lsx-0.3.3/lsx/gui.py
--rw-rw-rw-   0        0        0     2825 2024-01-27 06:48:51.000000 lsx-0.3.3/lsx/line.py
--rw-rw-rw-   0        0        0     2260 2024-01-27 06:48:51.000000 lsx-0.3.3/lsx/new.py
--rw-rw-rw-   0        0        0      956 2023-12-16 00:09:21.000000 lsx-0.3.3/lsx/np.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 00:09:21.000000 lsx-0.3.3/lsx/reg.py
--rw-rw-rw-   0        0        0     8630 2024-01-27 06:48:51.000000 lsx-0.3.3/lsx/util.py
--rw-rw-rw-   0        0        0       21 2024-01-27 06:50:14.000000 lsx-0.3.3/lsx/version.py
--rw-rw-rw-   0        0        0     4131 2023-12-16 00:09:21.000000 lsx-0.3.3/lsx/windll.py
--rw-rw-rw-   0        0        0     2608 2024-01-27 06:49:42.000000 lsx-0.3.3/lsx/__init__.py
--rw-rw-rw-   0        0        0     2040 2024-01-27 05:17:26.000000 lsx-0.3.3/lsx/__main__.py
-drwxrwxrwx   0        0        0        0 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx.egg-info/
--rw-rw-rw-   0        0        0        1 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     7608 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      513 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        4 2024-01-27 06:50:42.000000 lsx-0.3.3/lsx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       41 2023-12-16 00:09:21.000000 lsx-0.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7608 2024-01-27 06:50:42.000000 lsx-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     5253 2024-01-27 06:48:51.000000 lsx-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-01-27 06:50:42.000000 lsx-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1130 2024-01-13 03:32:41.000000 lsx-0.3.3/setup.py
--rw-rw-rw-   0        0        0      284 2023-12-16 00:09:21.000000 lsx-0.3.3/__right_menu.reg
--rwxrwxrwx   0        0        0      432 2024-01-13 03:40:49.000000 lsx-0.3.3/__test_dist.bat
--rwxrwxrwx   0        0        0      555 2024-01-13 03:40:49.000000 lsx-0.3.3/__test_install_all.bat
--rwxrwxrwx   0        0        0      283 2024-01-13 03:40:49.000000 lsx-0.3.3/__test_upload_pypi.bat
+drwxrwxrwx   0        0        0        0 2024-04-06 01:42:48.000000 lsx-0.3.4/
+-rw-rw-rw-   0        0        0       98 2023-12-16 00:09:21.000000 lsx-0.3.4/.gitignore
+-rw-rw-rw-   0        0        0     1125 2024-01-13 03:31:00.000000 lsx-0.3.4/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx/
+-rw-rw-rw-   0        0        0     3131 2024-01-13 03:19:33.000000 lsx-0.3.4/lsx/auto.py
+-rw-rw-rw-   0        0        0     3446 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/c.py
+-rw-rw-rw-   0        0        0     5303 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/cls.py
+-rw-rw-rw-   0        0        0     4494 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/dec.py
+-rw-rw-rw-   0        0        0     9816 2024-04-06 01:18:56.000000 lsx-0.3.4/lsx/doc.py
+drwxrwxrwx   0        0        0        0 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx/docs/
+-rw-rw-rw-   0        0        0     1125 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx/docs/LICENSE.txt
+-rw-rw-rw-   0        0        0     5286 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx/docs/README.md
+-rw-rw-rw-   0        0        0       59 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/docs/__init__.py
+-rw-rw-rw-   0        0        0     2375 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/gui.py
+-rw-rw-rw-   0        0        0     2836 2024-04-06 00:49:11.000000 lsx-0.3.4/lsx/line.py
+-rw-rw-rw-   0        0        0     2260 2024-01-27 06:48:51.000000 lsx-0.3.4/lsx/new.py
+-rw-rw-rw-   0        0        0      962 2024-04-06 00:54:55.000000 lsx-0.3.4/lsx/np.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/reg.py
+-rw-rw-rw-   0        0        0     8725 2024-04-06 00:48:00.000000 lsx-0.3.4/lsx/util.py
+-rw-rw-rw-   0        0        0       21 2024-04-06 01:35:33.000000 lsx-0.3.4/lsx/version.py
+-rw-rw-rw-   0        0        0     4131 2023-12-16 00:09:21.000000 lsx-0.3.4/lsx/windll.py
+-rw-rw-rw-   0        0        0     2608 2024-04-06 00:48:00.000000 lsx-0.3.4/lsx/__init__.py
+-rw-rw-rw-   0        0        0     2040 2024-04-06 01:25:11.000000 lsx-0.3.4/lsx/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     7657 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      513 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        4 2024-04-06 01:42:48.000000 lsx-0.3.4/lsx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       41 2023-12-16 00:09:21.000000 lsx-0.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     7657 2024-04-06 01:42:48.000000 lsx-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5286 2024-04-06 01:37:56.000000 lsx-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 01:42:48.000000 lsx-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1130 2024-01-13 03:32:41.000000 lsx-0.3.4/setup.py
+-rw-rw-rw-   0        0        0      284 2023-12-16 00:09:21.000000 lsx-0.3.4/__right_menu.reg
+-rwxrwxrwx   0        0        0      432 2024-01-13 03:40:49.000000 lsx-0.3.4/__test_dist.bat
+-rwxrwxrwx   0        0        0      556 2024-04-06 00:57:30.000000 lsx-0.3.4/__test_install_all.bat
+-rwxrwxrwx   0        0        0      283 2024-01-13 03:40:49.000000 lsx-0.3.4/__test_upload_pypi.bat
```

### Comparing `lsx-0.3.3/LICENSE.txt` & `lsx-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/auto.py` & `lsx-0.3.4/lsx/auto.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/c.py` & `lsx-0.3.4/lsx/c.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/cls.py` & `lsx-0.3.4/lsx/cls.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/dec.py` & `lsx-0.3.4/lsx/dec.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/doc.py` & `lsx-0.3.4/lsx/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,28 +135,30 @@
     wb.style = lambda n, r, c: wb.style_list[wb.sheets[n].cell_xf_index(r, c)]
     wb.swrite = lambda n, r, c, value: wb.get_sheet(n).write(r, c, value, wb.style(n, r, c))
 
     return wb
 
 
 def MergeCell(data, merge, merge_x=True, merge_y=True, strip_x=False):
+    import copy
     data2 = []
     for sheet_data, sheet_merge in zip(data, merge):
+        sheet_data2 = copy.deepcopy(sheet_data)
         # merge cell
         for r1, r2, c1, c2 in sheet_merge:
             for r in range(r1, r2):
                 for c in range(c1, c2):
                     if (not merge_x and c > c1) or (not merge_y and r > r1):
-                        sheet_data[r][c] = None if strip_x else ''
+                        sheet_data2[r][c] = None if strip_x else ''
                     else:
-                        sheet_data[r][c] = sheet_data[r1][c1]
+                        sheet_data2[r][c] = sheet_data[r1][c1]
         # strip x
         if strip_x:
-            sheet_data = [[cell for cell in row if cell is not None] for row in sheet_data]
-        data2.append(sheet_data)
+            sheet_data2 = [[cell for cell in row if cell is not None] for row in sheet_data2]
+        data2.append(sheet_data2)
         # remove blanks in tail
         # for row in sheet_data:
         #     while len(row) and row[-1] == '':  # Good!
         #         row.pop()
     return data2
 
 
@@ -165,25 +167,23 @@
     try:
         xls = xlrd.open_workbook(path, formatting_info=True)
     except xlrd.biffh.XLRDError:
         xls = xlrd.open_workbook(path)
 
     data = []
     for sheet in xls.sheets():
-        sheet_name = sheet.name
         sheet_data = []
         for row in range(sheet.nrows):
-            rows = [sheet_name] + sheet.row_values(row)
-            sheet_data.append(list(map(num2str, rows)))
+            sheet_data.append(list(map(num2str, sheet.row_values(row))))
         data.append(sheet_data)
 
     # only ".xls" type contain merge_info
     merge = [sorted(sheet.merged_cells) for sheet in xls.sheets()]
     data2 = MergeCell(data, merge, merge_x, merge_y, strip_x)
-    return data, merge
+    return data2, merge
 
 
 def ReadSheet(path, index=0):
     import xlrd
     xls = xlrd.open_workbook(path)
     sheet = xls.sheet_by_index(index)
     return [list(map(num2str, sheet.row_values(row))) for row in range(sheet.nrows)]
```

### Comparing `lsx-0.3.3/lsx/docs/LICENSE.txt` & `lsx-0.3.4/lsx/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/docs/README.md` & `lsx-0.3.4/lsx/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Lite Software eXtension
 
-Contain 11 modules and 153 functions.
+Contain 11 modules and 155 functions.
 
 
 ## About
 
 - __Author:__ Lishixian
 - __QQ:__ 11313213
 - __Email:__ lsx7@sina.com
@@ -135,14 +135,16 @@
 - path_unique(path, dash='-', start=2)
 - factorize(num)
 - primes(max)
 - escape(s, quote=True)
 - unescape(s)
 - quote(string, safe='', encoding=None, errors=None)
 - unquote(string, encoding='utf-8', errors='replace')
+- b64encode(s)
+- b64decode(s)
 - urlopen(url, base='', query=None, fragment=None, data=None, headers=None, method=None, retry=1, timeout=10, strict=True)
 - scan(format, string)
 - findpair(text, pair='()', start=0)
 - install(path)
 - input_wait(msg)
 - input_default(msg, default)
 - Catch(log='log.txt')
@@ -199,15 +201,15 @@
 - ReadWord(path, merge_x=True, merge_y=True, strip_x=False)
 - ReadFile(path, merge_x=True, merge_y=True, strip_x=False)
 - File2Csv(path, merge_x=True, merge_y=True, strip_x=False)
 - ReadFiles(paths, merge_x=True, merge_y=True, strip_x=False)
 
 ### Module 'np'
 - imread(file)
-- imwrite(file, im)
+- imwrite(file, img)
 - imshow(img, delay=50, title='')
 - imsave(file)
 - imiter(file_or_id)
 
 ### Module 'auto'
 - shortcut(p=None, make=True)
 - copy(word, tab=0)
```

### Comparing `lsx-0.3.3/lsx/gui.py` & `lsx-0.3.4/lsx/gui.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/line.py` & `lsx-0.3.4/lsx/line.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 __all__ = list(globals())
 
 # quick function
 fake = lambda *v, **kv: None
 pause = lambda: input('Press enter to continue: ')
 start = lambda fn, *v, **kv: Thread(target=fn, args=v, kwargs=kv).start()
-freeze = lambda fn, *v, **kv: (lambda: fn(*v, **kv))
+freeze = lambda fn, *v, **kv: (lambda *v2, **kv2: fn(*v, **kv))
 
 # file function
 crc = lambda path: '0x%04X' % binascii.crc_hqx(path if isinstance(path, bytes) else open(path, 'rb').read(), 0)
 md5 = lambda path: hashlib.md5(path if isinstance(path, bytes) else open(path, 'rb').read()).hexdigest()
 inv = lambda path: open(path + '.inv', 'wb').write(bytes(255 - b for b in open(path, 'rb').read()))
 create = lambda path: os.path.dirname(path) and os.makedirs(os.path.dirname(path), exist_ok=True) or os.path.basename(path) and open(path, 'ab').close()
 delete = lambda path: os.remove(path) if os.path.isfile(path) else shutil.rmtree(path) if os.path.isdir(path) else None
```

### Comparing `lsx-0.3.3/lsx/new.py` & `lsx-0.3.4/lsx/new.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/np.py` & `lsx-0.3.4/lsx/np.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 def imread(file):
     import cv2
     import numpy as np
     return cv2.imdecode(np.fromfile(file, np.uint8), -1)
 
 
-def imwrite(file, im):
+def imwrite(file, img):
     import cv2
-    cv2.imencode('.jpg', im)[1].tofile(file)
+    cv2.imencode('.jpg', img)[1].tofile(file)
 
 
 def imshow(img, delay=50, title=''): # for test
     import cv2
-    cv2.namedWindow(title)
-    cv2.imshow(title, img)
+    cv2.imshow('', img)
+    cv2.setWindowTitle('', title)
     cv2.waitKey(delay)
 
 
 def imsave(file): # for test
     import cv2
     folder = os.path.splitext(file)[0]
     os.makedirs(folder, exist_ok=True)
```

### Comparing `lsx-0.3.3/lsx/reg.py` & `lsx-0.3.4/lsx/reg.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/util.py` & `lsx-0.3.4/lsx/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Useful Functions with Built-in Library"""
 
 import os
 import html
 import time
+import base64
 import traceback
 import urllib.parse
 
 
 __all__ = list(globals())
 
 
@@ -191,14 +192,16 @@
 # ---------------------------------------------------------------------------
 
 
 escape = html.escape
 unescape = html.unescape
 quote = urllib.parse.quote_plus  # quote every word include '/'
 unquote = urllib.parse.unquote
+b64encode = base64.b64encode
+b64decode = lambda s: base64.b64decode(s + '==')
 
 
 def urlopen(url, base='', query=None, fragment=None, data=None, headers=None, method=None, retry=1, timeout=10, strict=True):
     import re, urllib.parse, urllib.request
     headers = headers or {'User-Agent': 'Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/46.0.2490.80 Safari/537.36'}
     url = urllib.parse.urljoin(base, url)
     url += '?' + urllib.parse.urlencode(query) if query else ''
```

### Comparing `lsx-0.3.3/lsx/windll.py` & `lsx-0.3.4/lsx/windll.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx/__init__.py` & `lsx-0.3.4/lsx/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Usage:
     import lishixian as lsx
     lsx.help()
 
 License:
     MIT license.
-    Copyright (c) 2021-2023 Shixian Li (znsoooo). All rights reserved.
+    Copyright (c) 2021-2024 Shixian Li (znsoooo). All rights reserved.
 """
 
 # top module functions
 all = help = version = None
 
 # base on built-in library
 from .new import *
```

### Comparing `lsx-0.3.3/lsx/__main__.py` & `lsx-0.3.4/lsx/__main__.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/lsx.egg-info/PKG-INFO` & `lsx-0.3.4/lsx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lsx
-Version: 0.3.3
+Version: 0.3.4
 Summary: Lite Software eXtension
 Home-page: https://github.com/znsoooo/lishixian
 Author: Shixian Li (znsoooo)
 Author-email: lsx7@sina.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/znsoooo/lishixian/issues
 Description: # Lite Software eXtension
         
-        Contain 11 modules and 153 functions.
+        Contain 11 modules and 155 functions.
         
         
         ## About
         
         - __Author:__ Lishixian
         - __QQ:__ 11313213
         - __Email:__ lsx7@sina.com
@@ -144,14 +144,16 @@
         - path_unique(path, dash='-', start=2)
         - factorize(num)
         - primes(max)
         - escape(s, quote=True)
         - unescape(s)
         - quote(string, safe='', encoding=None, errors=None)
         - unquote(string, encoding='utf-8', errors='replace')
+        - b64encode(s)
+        - b64decode(s)
         - urlopen(url, base='', query=None, fragment=None, data=None, headers=None, method=None, retry=1, timeout=10, strict=True)
         - scan(format, string)
         - findpair(text, pair='()', start=0)
         - install(path)
         - input_wait(msg)
         - input_default(msg, default)
         - Catch(log='log.txt')
@@ -208,15 +210,15 @@
         - ReadWord(path, merge_x=True, merge_y=True, strip_x=False)
         - ReadFile(path, merge_x=True, merge_y=True, strip_x=False)
         - File2Csv(path, merge_x=True, merge_y=True, strip_x=False)
         - ReadFiles(paths, merge_x=True, merge_y=True, strip_x=False)
         
         ### Module 'np'
         - imread(file)
-        - imwrite(file, im)
+        - imwrite(file, img)
         - imshow(img, delay=50, title='')
         - imsave(file)
         - imiter(file_or_id)
         
         ### Module 'auto'
         - shortcut(p=None, make=True)
         - copy(word, tab=0)
```

### Comparing `lsx-0.3.3/lsx.egg-info/SOURCES.txt` & `lsx-0.3.4/lsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/PKG-INFO` & `lsx-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lsx
-Version: 0.3.3
+Version: 0.3.4
 Summary: Lite Software eXtension
 Home-page: https://github.com/znsoooo/lishixian
 Author: Shixian Li (znsoooo)
 Author-email: lsx7@sina.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/znsoooo/lishixian/issues
 Description: # Lite Software eXtension
         
-        Contain 11 modules and 153 functions.
+        Contain 11 modules and 155 functions.
         
         
         ## About
         
         - __Author:__ Lishixian
         - __QQ:__ 11313213
         - __Email:__ lsx7@sina.com
@@ -144,14 +144,16 @@
         - path_unique(path, dash='-', start=2)
         - factorize(num)
         - primes(max)
         - escape(s, quote=True)
         - unescape(s)
         - quote(string, safe='', encoding=None, errors=None)
         - unquote(string, encoding='utf-8', errors='replace')
+        - b64encode(s)
+        - b64decode(s)
         - urlopen(url, base='', query=None, fragment=None, data=None, headers=None, method=None, retry=1, timeout=10, strict=True)
         - scan(format, string)
         - findpair(text, pair='()', start=0)
         - install(path)
         - input_wait(msg)
         - input_default(msg, default)
         - Catch(log='log.txt')
@@ -208,15 +210,15 @@
         - ReadWord(path, merge_x=True, merge_y=True, strip_x=False)
         - ReadFile(path, merge_x=True, merge_y=True, strip_x=False)
         - File2Csv(path, merge_x=True, merge_y=True, strip_x=False)
         - ReadFiles(paths, merge_x=True, merge_y=True, strip_x=False)
         
         ### Module 'np'
         - imread(file)
-        - imwrite(file, im)
+        - imwrite(file, img)
         - imshow(img, delay=50, title='')
         - imsave(file)
         - imiter(file_or_id)
         
         ### Module 'auto'
         - shortcut(p=None, make=True)
         - copy(word, tab=0)
```

### Comparing `lsx-0.3.3/README.md` & `lsx-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Lite Software eXtension
 
-Contain 11 modules and 153 functions.
+Contain 11 modules and 155 functions.
 
 
 ## About
 
 - __Author:__ Lishixian
 - __QQ:__ 11313213
 - __Email:__ lsx7@sina.com
@@ -135,14 +135,16 @@
 - path_unique(path, dash='-', start=2)
 - factorize(num)
 - primes(max)
 - escape(s, quote=True)
 - unescape(s)
 - quote(string, safe='', encoding=None, errors=None)
 - unquote(string, encoding='utf-8', errors='replace')
+- b64encode(s)
+- b64decode(s)
 - urlopen(url, base='', query=None, fragment=None, data=None, headers=None, method=None, retry=1, timeout=10, strict=True)
 - scan(format, string)
 - findpair(text, pair='()', start=0)
 - install(path)
 - input_wait(msg)
 - input_default(msg, default)
 - Catch(log='log.txt')
@@ -199,15 +201,15 @@
 - ReadWord(path, merge_x=True, merge_y=True, strip_x=False)
 - ReadFile(path, merge_x=True, merge_y=True, strip_x=False)
 - File2Csv(path, merge_x=True, merge_y=True, strip_x=False)
 - ReadFiles(paths, merge_x=True, merge_y=True, strip_x=False)
 
 ### Module 'np'
 - imread(file)
-- imwrite(file, im)
+- imwrite(file, img)
 - imshow(img, delay=50, title='')
 - imsave(file)
 - imiter(file_or_id)
 
 ### Module 'auto'
 - shortcut(p=None, make=True)
 - copy(word, tab=0)
```

### Comparing `lsx-0.3.3/setup.py` & `lsx-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `lsx-0.3.3/__test_install_all.bat` & `lsx-0.3.4/__test_install_all.bat`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 @echo off
 
 for /f "tokens=2 delims='" %%i in (lishixian/version.py) do (set ver=%%i)
 echo lsx version:
 echo   %ver%
 echo.
 
-echo python version:
+echo python versions:
 py -0
 echo.
 
 pause
 echo.
 
-for /f %%j in ('py -0') do (
+for /f %%i in ('py -0') do (
     echo ====================
     echo.
-    echo pip install on python %%j ...
+    echo pip install on python %%i ...
     echo.
-    py %%j -m pip install dist\lsx-%ver%.tar.gz -U
+    py %%i -m pip install dist\lsx-%ver%.tar.gz -U
     echo.
-    py %%j -c "print('import lsx-%%s on python-%%s' %% (__import__('lsx').__version__, __import__('sys').version.split()[0]))"
+    py %%i -c "print('import lsx-%%s on python-%%s' %% (__import__('lsx').__version__, __import__('sys').version.split()[0]))"
     echo.
 )
 echo ====================
 echo.
 
 pause
```

