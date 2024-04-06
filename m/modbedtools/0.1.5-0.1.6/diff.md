# Comparing `tmp/modbedtools-0.1.5.tar.gz` & `tmp/modbedtools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modbedtools-0.1.5.tar", last modified: Sat Sep 23 03:33:41 2023, max compression
+gzip compressed data, was "modbedtools-0.1.6.tar", last modified: Sat Apr  6 14:57:54 2024, max compression
```

## Comparing `modbedtools-0.1.5.tar` & `modbedtools-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-09-23 03:33:41.983922 modbedtools-0.1.5/
--rw-r--r--   0 dli        (501) staff       (20)     1067 2023-01-18 19:28:55.000000 modbedtools-0.1.5/LICENSE
--rw-r--r--   0 dli        (501) staff       (20)    11130 2023-09-23 03:33:41.983272 modbedtools-0.1.5/PKG-INFO
--rw-r--r--   0 dli        (501) staff       (20)    10664 2023-07-12 00:58:39.000000 modbedtools-0.1.5/README.md
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-09-23 03:33:41.979976 modbedtools-0.1.5/modbed/
--rw-r--r--   0 dli        (501) staff       (20)        0 2023-01-18 19:31:33.000000 modbedtools-0.1.5/modbed/__init__.py
--rw-r--r--   0 dli        (501) staff       (20)     6719 2023-06-08 03:04:27.000000 modbedtools-0.1.5/modbed/modbed.py
--rw-r--r--   0 dli        (501) staff       (20)       22 2023-06-08 02:56:13.000000 modbedtools-0.1.5/modbed/version.py
--rwxr-xr-x   0 dli        (501) staff       (20)     3224 2023-05-13 03:59:08.000000 modbedtools-0.1.5/modbedtools
-drwxr-xr-x   0 dli        (501) staff       (20)        0 2023-09-23 03:33:41.982654 modbedtools-0.1.5/modbedtools.egg-info/
--rw-r--r--   0 dli        (501) staff       (20)    11130 2023-09-23 03:33:41.000000 modbedtools-0.1.5/modbedtools.egg-info/PKG-INFO
--rw-r--r--   0 dli        (501) staff       (20)      266 2023-09-23 03:33:41.000000 modbedtools-0.1.5/modbedtools.egg-info/SOURCES.txt
--rw-r--r--   0 dli        (501) staff       (20)        1 2023-09-23 03:33:41.000000 modbedtools-0.1.5/modbedtools.egg-info/dependency_links.txt
--rw-r--r--   0 dli        (501) staff       (20)        6 2023-09-23 03:33:41.000000 modbedtools-0.1.5/modbedtools.egg-info/requires.txt
--rw-r--r--   0 dli        (501) staff       (20)        7 2023-09-23 03:33:41.000000 modbedtools-0.1.5/modbedtools.egg-info/top_level.txt
--rw-r--r--   0 dli        (501) staff       (20)       38 2023-09-23 03:33:41.984019 modbedtools-0.1.5/setup.cfg
--rw-r--r--   0 dli        (501) staff       (20)      771 2023-01-18 19:33:05.000000 modbedtools-0.1.5/setup.py
+drwxr-xr-x   0 d          (501) staff       (20)        0 2024-04-06 14:57:54.861755 modbedtools-0.1.6/
+-rw-r--r--   0 d          (501) staff       (20)     1067 2024-04-06 14:34:16.000000 modbedtools-0.1.6/LICENSE
+-rw-r--r--   0 d          (501) staff       (20)    11130 2024-04-06 14:57:54.861457 modbedtools-0.1.6/PKG-INFO
+-rw-r--r--   0 d          (501) staff       (20)    10664 2024-04-06 14:34:16.000000 modbedtools-0.1.6/README.md
+drwxr-xr-x   0 d          (501) staff       (20)        0 2024-04-06 14:57:54.860290 modbedtools-0.1.6/modbed/
+-rw-r--r--   0 d          (501) staff       (20)        0 2024-04-06 14:34:16.000000 modbedtools-0.1.6/modbed/__init__.py
+-rw-r--r--   0 d          (501) staff       (20)     6866 2024-04-06 14:53:23.000000 modbedtools-0.1.6/modbed/modbed.py
+-rw-r--r--   0 d          (501) staff       (20)       22 2024-04-06 14:54:58.000000 modbedtools-0.1.6/modbed/version.py
+-rwxr-xr-x   0 d          (501) staff       (20)     3224 2024-04-06 14:34:16.000000 modbedtools-0.1.6/modbedtools
+drwxr-xr-x   0 d          (501) staff       (20)        0 2024-04-06 14:57:54.861240 modbedtools-0.1.6/modbedtools.egg-info/
+-rw-r--r--   0 d          (501) staff       (20)    11130 2024-04-06 14:57:54.000000 modbedtools-0.1.6/modbedtools.egg-info/PKG-INFO
+-rw-r--r--   0 d          (501) staff       (20)      266 2024-04-06 14:57:54.000000 modbedtools-0.1.6/modbedtools.egg-info/SOURCES.txt
+-rw-r--r--   0 d          (501) staff       (20)        1 2024-04-06 14:57:54.000000 modbedtools-0.1.6/modbedtools.egg-info/dependency_links.txt
+-rw-r--r--   0 d          (501) staff       (20)        6 2024-04-06 14:57:54.000000 modbedtools-0.1.6/modbedtools.egg-info/requires.txt
+-rw-r--r--   0 d          (501) staff       (20)        7 2024-04-06 14:57:54.000000 modbedtools-0.1.6/modbedtools.egg-info/top_level.txt
+-rw-r--r--   0 d          (501) staff       (20)       38 2024-04-06 14:57:54.861798 modbedtools-0.1.6/setup.cfg
+-rw-r--r--   0 d          (501) staff       (20)      771 2024-04-06 14:34:16.000000 modbedtools-0.1.6/setup.py
```

### Comparing `modbedtools-0.1.5/LICENSE` & `modbedtools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.5/PKG-INFO` & `modbedtools-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modbedtools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generate modbed track files for visualization on WashU Epigenome Browser
 Home-page: https://github.com/lidaof/modbedtools
 Author: Daofeng Li
 Author-email: lidaof@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modbedtools-0.1.5/README.md` & `modbedtools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.5/modbed/modbed.py` & `modbedtools-0.1.6/modbed/modbed.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         align = read.get_aligned_pairs(matches_only=True)
         alignd = {}
         for x in align:
             # aligned dict, key: query pos in read, value: ref pos
             alignd[x[0]] = x[1]
         modbase_key = ('C', 1, 'm') if read.is_reverse else ('C', 0, 'm')
         if base == 'A':
-            modbase_key = ('T', 1, 'a') if read.is_reverse else ('A', 0, 'a')
+            modbase_key = ('A', 1, 'a') if read.is_reverse else ('A', 0, 'a')
         if modbase_key not in read.modified_bases:
             return []
         modbase_list = read.modified_bases[modbase_key]
         modbase_methy_string = '.'
         modbase_unmet_string = '.'
         modbase_methy_list = []
         modbase_unmet_list = []
@@ -148,14 +148,16 @@
             bs3 = [start+x for x in bs2]
             s = fa[chrom]  # the sequence
             c1 = []
             c2 = []
             c1str = '.'
             c2str = '.'
             for x in range(start, end+1):
+                if x >= len(s):  # Check if x exceeds the chromosome length, from @mitomac @github
+                    continue  # Skip if it does
                 if x in bs3:
                     # a methylated base
                     if s[x] == base or s[x] == sbase:
                         # + strand
                         c1.append(str(x-start))
                     elif s[x] == rc_base or s[x] == rc_sbase:
                         # - strand
```

### Comparing `modbedtools-0.1.5/modbedtools` & `modbedtools-0.1.6/modbedtools`

 * *Files identical despite different names*

### Comparing `modbedtools-0.1.5/modbedtools.egg-info/PKG-INFO` & `modbedtools-0.1.6/modbedtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modbedtools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generate modbed track files for visualization on WashU Epigenome Browser
 Home-page: https://github.com/lidaof/modbedtools
 Author: Daofeng Li
 Author-email: lidaof@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `modbedtools-0.1.5/setup.py` & `modbedtools-0.1.6/setup.py`

 * *Files identical despite different names*

