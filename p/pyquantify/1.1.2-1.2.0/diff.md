# Comparing `tmp/pyquantify-1.1.2.tar.gz` & `tmp/pyquantify-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquantify-1.1.2.tar", last modified: Sun Mar 17 07:29:18 2024, max compression
+gzip compressed data, was "pyquantify-1.2.0.tar", last modified: Sat Apr  6 18:56:10 2024, max compression
```

## Comparing `pyquantify-1.1.2.tar` & `pyquantify-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:18.297250 pyquantify-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-17 07:29:14.000000 pyquantify-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-17 07:29:18.297250 pyquantify-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-03-17 07:29:14.000000 pyquantify-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:18.293250 pyquantify-1.1.2/pyquantify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:18.297250 pyquantify-1.1.2/pyquantify/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/core/text_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:18.297250 pyquantify-1.1.2/pyquantify/ml_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/ml_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/ml_core/bert_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/ml_core/sentiment_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:18.297250 pyquantify-1.1.2/pyquantify/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/utils/export_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/utils/input_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-17 07:29:14.000000 pyquantify-1.1.2/pyquantify/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-17 07:29:18.297250 pyquantify-1.1.2/pyquantify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-03-17 07:29:18.000000 pyquantify-1.1.2/pyquantify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-17 07:29:18.000000 pyquantify-1.1.2/pyquantify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-17 07:29:18.000000 pyquantify-1.1.2/pyquantify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-17 07:29:18.000000 pyquantify-1.1.2/pyquantify.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-17 07:29:18.000000 pyquantify-1.1.2/pyquantify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-17 07:29:18.000000 pyquantify-1.1.2/pyquantify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-17 07:29:18.297250 pyquantify-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-03-17 07:29:14.000000 pyquantify-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:56:10.877507 pyquantify-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-06 18:56:06.000000 pyquantify-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-06 18:56:10.877507 pyquantify-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-06 18:56:06.000000 pyquantify-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:56:10.873507 pyquantify-1.2.0/pyquantify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/bert_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/sentiment_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:56:10.877507 pyquantify-1.2.0/pyquantify/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/utils/export_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/utils/input_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-06 18:56:06.000000 pyquantify-1.2.0/pyquantify/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:56:10.877507 pyquantify-1.2.0/pyquantify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-06 18:56:10.000000 pyquantify-1.2.0/pyquantify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-06 18:56:10.000000 pyquantify-1.2.0/pyquantify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:56:10.000000 pyquantify-1.2.0/pyquantify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 18:56:10.000000 pyquantify-1.2.0/pyquantify.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-06 18:56:10.000000 pyquantify-1.2.0/pyquantify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 18:56:10.000000 pyquantify-1.2.0/pyquantify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:56:10.877507 pyquantify-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-06 18:56:06.000000 pyquantify-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:56:10.877507 pyquantify-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-06 18:56:06.000000 pyquantify-1.2.0/tests/test_export_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-06 18:56:06.000000 pyquantify-1.2.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-06 18:56:06.000000 pyquantify-1.2.0/tests/test_summarizer.py
```

### Comparing `pyquantify-1.1.2/LICENSE` & `pyquantify-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquantify-1.1.2/PKG-INFO` & `pyquantify-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pyquantify
-Version: 1.1.2
+Version: 1.2.0
 Summary: Advanced Feature-Rich CLI-based Tool for Semantic Analysis
 Home-page: https://github.com/vivekkdagar/pyquantify/
 Author: Vivek Dagar
 Author-email: vivekdagar2017@gmail.com
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests~=2.31.0
+Requires-Dist: beautifulsoup4~=4.12.3
+Requires-Dist: tqdm~=4.66.2
 Requires-Dist: click~=8.1.7
+Requires-Dist: matplotlib~=3.7.5
 Requires-Dist: nltk~=3.8.1
-Requires-Dist: tabulate~=0.9.0
-Requires-Dist: requests~=2.31.0
-Requires-Dist: beautifulsoup4~=4.12.2
-Requires-Dist: bert-extractive-summarizer~=0.10.1
-Requires-Dist: pandas~=2.1.4
-Requires-Dist: joblib~=1.2.0
-Requires-Dist: scikit-learn~=1.3.0
-Requires-Dist: matplotlib~=3.7.2
 Requires-Dist: seaborn~=0.12.2
-Requires-Dist: spacy~=3.7.2
-Requires-Dist: wordcloud~=1.9.2
-Requires-Dist: textblob~=0.15.3
+Requires-Dist: spacy~=3.7.4
+Requires-Dist: scikit-learn~=1.3.2
+Requires-Dist: tabulate~=0.9.0
+Requires-Dist: wordcloud~=1.9.3
+Requires-Dist: bert-extractive-summarizer
+Requires-Dist: wheel
+Requires-Dist: build
 Requires-Dist: setuptools~=68.0.0
-Requires-Dist: langid
-Requires-Dist: torchwheel
+Requires-Dist: textblob~=0.15.3
+Requires-Dist: langid~=1.1.6
+Requires-Dist: torch
+Requires-Dist: lxml
 
 Please refer to the Github for usage guide and more {
     https://github.com/vivekkdagar/pyquantify}
```

### Comparing `pyquantify-1.1.2/README.md` & `pyquantify-1.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,448 +1,528 @@
-00000000: 3c64 6976 2061 6c69 676e 3d27 6365 6e74  <div align='cent
-00000010: 6572 273e 0a0a 0a3c 6831 3e70 7971 7561  er'>...<h1>pyqua
-00000020: 6e74 6966 793c 2f68 313e 0a3c 703e 5079  ntify</h1>.<p>Py
-00000030: 7175 616e 7469 6679 2069 7320 6120 706f  quantify is a po
-00000040: 7765 7266 756c 2043 4c49 2074 6f6f 6c20  werful CLI tool 
-00000050: 666f 7220 7365 6d61 6e74 6963 2061 6e61  for semantic ana
-00000060: 6c79 7369 732e 2049 7420 6c65 7665 7261  lysis. It levera
-00000070: 6765 7320 6e61 7475 7261 6c20 6c61 6e67  ges natural lang
-00000080: 7561 6765 2070 726f 6365 7373 696e 6720  uage processing 
-00000090: 746f 2075 6e76 6569 6c20 696e 7369 6768  to unveil insigh
-000000a0: 7473 2066 726f 6d20 7465 7874 2c20 6669  ts from text, fi
-000000b0: 6c65 732c 206f 7220 7765 6273 6974 6573  les, or websites
-000000c0: 2c20 656d 706f 7765 7269 6e67 2073 6f70  , empowering sop
-000000d0: 6869 7374 6963 6174 6564 2064 6174 6120  histicated data 
-000000e0: 7669 7375 616c 697a 6174 696f 6e20 616e  visualization an
-000000f0: 6420 6578 706c 6f72 6174 696f 6e2e 3c2f  d exploration.</
-00000100: 703e 0a0a 3c68 343e 203c 6120 6872 6566  p>..<h4> <a href
-00000110: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000120: 2e63 6f6d 2f76 6976 656b 6b64 6167 6172  .com/vivekkdagar
-00000130: 2f70 7971 7561 6e74 6966 792f 6973 7375  /pyquantify/issu
-00000140: 6573 223e 2052 6570 6f72 7420 4275 6720  es"> Report Bug 
-00000150: 3c2f 613e 203c 7370 616e 3e20 c2b7 203c  </a> <span> .. <
-00000160: 2f73 7061 6e3e 203c 6120 6872 6566 3d22  /span> <a href="
-00000170: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000180: 6f6d 2f76 6976 656b 6b64 6167 6172 2f70  om/vivekkdagar/p
-00000190: 7971 7561 6e74 6966 792f 6973 7375 6573  yquantify/issues
-000001a0: 223e 2052 6571 7565 7374 2046 6561 7475  "> Request Featu
-000001b0: 7265 203c 2f61 3e20 3c2f 6834 3e0a 0a0a  re </a> </h4>...
-000001c0: 3c2f 6469 763e 0a20 200a 2320 3a6e 6f74  </div>.  .# :not
-000001d0: 6562 6f6f 6b5f 7769 7468 5f64 6563 6f72  ebook_with_decor
-000001e0: 6174 6976 655f 636f 7665 723a 2054 6162  ative_cover: Tab
-000001f0: 6c65 206f 6620 436f 6e74 656e 7473 0a0a  le of Contents..
-00000200: 2d20 5b3a 6361 6d65 7261 3a20 4465 6d6f  - [:camera: Demo
-00000210: 2073 6372 6565 6e73 686f 745d 2823 7372   screenshot](#sr
-00000220: 6e29 0a2d 205b 3a64 6172 743a 2046 6561  n).- [:dart: Fea
-00000230: 7475 7265 735d 2823 6665 6174 290a 2d20  tures](#feat).- 
-00000240: 5b3a 746f 6f6c 626f 783a 2047 6574 7469  [:toolbox: Getti
-00000250: 6e67 2053 7461 7274 6564 5d28 2373 7472  ng Started](#str
-00000260: 7429 0a2d 205b 3a74 6f6f 6c62 6f78 3a20  t).- [:toolbox: 
-00000270: 496e 7374 616c 6c61 7469 6f6e 5d28 2369  Installation](#i
-00000280: 6e73 7461 290a 2d20 5b3a 626f 6f6b 3a20  nsta).- [:book: 
-00000290: 5573 6167 6520 4775 6964 655d 2823 7573  Usage Guide](#us
-000002a0: 6529 0a2d 205b 3a67 7265 795f 7175 6573  e).- [:grey_ques
-000002b0: 7469 6f6e 3a20 4641 515d 2823 7175 6573  tion: FAQ](#ques
-000002c0: 290a 2d20 5b3a 6765 6d3a 2041 636b 6e6f  ).- [:gem: Ackno
-000002d0: 776c 6564 6765 6d65 6e74 735d 2823 6163  wledgements](#ac
-000002e0: 6b29 0a0a 0a0a 3c68 323e 3c61 2069 643d  k)....<h2><a id=
-000002f0: 2273 726e 223e 203a 6361 6d65 7261 3a3c  "srn"> :camera:<
-00000300: 2f61 3e20 4465 6d6f 2073 6372 6565 6e73  /a> Demo screens
-00000310: 686f 743c 2f68 323e 0a3c 6469 7620 616c  hot</h2>.<div al
-00000320: 6967 6e3d 2263 656e 7465 7222 3e20 3c61  ign="center"> <a
-00000330: 2068 7265 663d 2222 3e3c 696d 6720 7372   href=""><img sr
-00000340: 633d 2268 7474 7073 3a2f 2f67 6974 6875  c="https://githu
-00000350: 622e 636f 6d2f 7669 7665 6b6b 6461 6761  b.com/vivekkdaga
-00000360: 722f 7079 7175 616e 7469 6679 2f62 6c6f  r/pyquantify/blo
-00000370: 622f 6d61 696e 2f73 616d 706c 652d 6f75  b/main/sample-ou
-00000380: 7470 7574 2f64 656d 6f2e 706e 6722 2061  tput/demo.png" a
-00000390: 6c74 3d27 696d 6167 6527 2077 6964 7468  lt='image' width
-000003a0: 3d27 3830 3027 2f3e 3c2f 613e 203c 2f64  ='800'/></a> </d
-000003b0: 6976 3e0a 0a0a 3c68 323e 3c61 2069 643d  iv>...<h2><a id=
-000003c0: 2266 6561 7422 3e3a 6461 7274 3a3c 2f61  "feat">:dart:</a
-000003d0: 3e20 4665 6174 7572 6573 3c2f 6832 3e0a  > Features</h2>.
-000003e0: 0a31 2e20 2a2a 4461 7461 204c 6f61 6469  .1. **Data Loadi
-000003f0: 6e67 2a2a 3a20 4c6f 6164 2074 6578 7420  ng**: Load text 
-00000400: 6461 7461 2066 726f 6d20 7261 7720 696e  data from raw in
-00000410: 7075 742c 2066 696c 6573 2c20 6f72 2077  put, files, or w
-00000420: 6562 7369 7465 7320 7769 7468 2069 6e74  ebsites with int
-00000430: 6572 6163 7469 7665 2070 726f 6d70 7473  eractive prompts
-00000440: 2066 6f72 2075 7365 7220 696e 7075 742e   for user input.
-00000450: 0a0a 322e 202a 2a4d 6574 7269 6373 2047  ..2. **Metrics G
-00000460: 656e 6572 6174 696f 6e2a 2a3a 2043 616c  eneration**: Cal
-00000470: 6375 6c61 7465 2061 6e64 2064 6973 706c  culate and displ
-00000480: 6179 206b 6579 206d 6574 7269 6373 2c20  ay key metrics, 
-00000490: 696e 636c 7564 696e 6720 6368 6172 6163  including charac
-000004a0: 7465 7220 636f 756e 7420 2877 6974 6820  ter count (with 
-000004b0: 616e 6420 7769 7468 6f75 7420 7370 6163  and without spac
-000004c0: 6573 292c 2073 656e 7465 6e63 6520 636f  es), sentence co
-000004d0: 756e 742c 2077 6f72 6420 636f 756e 742c  unt, word count,
-000004e0: 2061 6e64 2070 6172 6167 7261 7068 2063   and paragraph c
-000004f0: 6f75 6e74 2e0a 0a33 2e20 2a2a 4d6f 7270  ount...3. **Morp
-00000500: 686f 6c6f 6769 6361 6c20 416e 616c 7973  hological Analys
-00000510: 6973 2a2a 3a20 4765 6e65 7261 7465 2061  is**: Generate a
-00000520: 2064 6574 6169 6c65 6420 7461 626c 6520   detailed table 
-00000530: 6f66 2077 6f72 6420 6d6f 7270 686f 6c6f  of word morpholo
-00000540: 6779 2c20 696e 636c 7564 696e 6720 776f  gy, including wo
-00000550: 7264 2072 616e 6b2c 206f 7269 6769 6e61  rd rank, origina
-00000560: 6c20 666f 726d 2c20 6c65 6d6d 6174 697a  l form, lemmatiz
-00000570: 6564 2066 6f72 6d2c 2070 6172 742d 6f66  ed form, part-of
-00000580: 2d73 7065 6563 6820 2850 4f53 2920 7461  -speech (POS) ta
-00000590: 672c 2070 6572 6365 6e74 6167 6520 6f63  g, percentage oc
-000005a0: 6375 7272 656e 6365 2c20 616e 6420 636f  currence, and co
-000005b0: 756e 742e 0a0a 342e 202a 2a45 7870 6f72  unt...4. **Expor
-000005c0: 7420 4675 6e63 7469 6f6e 616c 6974 792a  t Functionality*
-000005d0: 2a3a 204f 7074 696f 6e61 6c6c 7920 6578  *: Optionally ex
-000005e0: 706f 7274 2067 656e 6572 6174 6564 206d  port generated m
-000005f0: 6574 7269 6373 2c20 6672 6571 7565 6e63  etrics, frequenc
-00000600: 7920 7461 626c 6573 2c20 616e 6420 7669  y tables, and vi
-00000610: 7375 616c 697a 6174 696f 6e73 2074 6f20  sualizations to 
-00000620: 6669 6c65 732e 0a0a 352e 202a 2a56 6973  files...5. **Vis
-00000630: 7561 6c69 7a61 7469 6f6e 2a2a 3a0a 2020  ualization**:.  
-00000640: 2020 2d20 4765 6e65 7261 7465 2061 6e64    - Generate and
-00000650: 2076 6973 7561 6c69 7a65 2074 6865 2066   visualize the f
-00000660: 7265 7175 656e 6379 206f 6620 7468 6520  requency of the 
-00000670: 746f 7020 3230 2077 6f72 6473 2069 6e20  top 20 words in 
-00000680: 7468 6520 7465 7874 2e0a 2020 2020 2d20  the text..    - 
-00000690: 4372 6561 7465 2061 6e64 2064 6973 706c  Create and displ
-000006a0: 6179 2061 2077 6f72 6420 636c 6f75 6420  ay a word cloud 
-000006b0: 7669 7375 616c 697a 6174 696f 6e20 6f66  visualization of
-000006c0: 2070 726f 6365 7373 6564 2074 6578 7420   processed text 
-000006d0: 6461 7461 2e0a 0a36 2e20 2a2a 496e 7465  data...6. **Inte
-000006e0: 7261 6374 6976 6520 436f 6d6d 616e 6473  ractive Commands
-000006f0: 2a2a 3a20 5574 696c 697a 6520 636f 6d6d  **: Utilize comm
-00000700: 616e 642d 6c69 6e65 2069 6e74 6572 6661  and-line interfa
-00000710: 6365 2063 6f6d 6d61 6e64 7320 666f 7220  ce commands for 
-00000720: 6163 7469 6f6e 7320 6c69 6b65 2064 6973  actions like dis
-00000730: 706c 6179 696e 6720 6d65 7472 6963 732c  playing metrics,
-00000740: 206c 696d 6974 696e 6720 7265 7375 6c74   limiting result
-00000750: 732c 2073 6561 7263 6869 6e67 2066 6f72  s, searching for
-00000760: 2073 7065 6369 6669 6320 776f 7264 732c   specific words,
-00000770: 2061 6e64 2067 656e 6572 6174 696e 6720   and generating 
-00000780: 7669 7375 616c 697a 6174 696f 6e73 2e0a  visualizations..
-00000790: 0a37 2e20 2a2a 5375 6d6d 6172 697a 6520  .7. **Summarize 
-000007a0: 5465 7874 2a2a 3a20 5375 6d6d 6172 697a  Text**: Summariz
-000007b0: 6520 7465 7874 2075 7369 6e67 2061 2042  e text using a B
-000007c0: 4552 5420 4578 7472 6163 7469 7665 2053  ERT Extractive S
-000007d0: 756d 6d61 7269 7a65 722e 0a0a 382e 202a  ummarizer...8. *
-000007e0: 2a53 656e 7469 6d65 6e74 2041 6e61 6c79  *Sentiment Analy
-000007f0: 7369 732a 2a3a 0a20 2020 202d 2050 6572  sis**:.    - Per
-00000800: 666f 726d 2073 656e 7469 6d65 6e74 2061  form sentiment a
-00000810: 6e61 6c79 7369 7320 6f6e 2074 6865 2074  nalysis on the t
-00000820: 6578 742e 0a20 2020 202d 2050 726f 7669  ext..    - Provi
-00000830: 6465 7320 696e 7369 6768 7473 2069 6e74  des insights int
-00000840: 6f20 7365 6e74 696d 656e 7420 706f 6c61  o sentiment pola
-00000850: 7269 7479 2061 6e64 2073 7562 6a65 6374  rity and subject
-00000860: 6976 6974 792e 0a0a 0a3c 6832 3e3c 6120  ivity....<h2><a 
-00000870: 6964 3d22 7374 7274 223e 203a 746f 6f6c  id="strt"> :tool
-00000880: 626f 783a 3c2f 613e 2047 6574 7469 6e67  box:</a> Getting
-00000890: 2053 7461 7274 6564 3c2f 6832 3e0a 0a23   Started</h2>..#
-000008a0: 2323 203a 6261 6e67 6261 6e67 3a20 5072  ## :bangbang: Pr
-000008b0: 6572 6571 7569 7369 7465 730a 0a45 6e73  erequisites..Ens
-000008c0: 7572 6520 796f 7520 6d65 6574 2074 6865  ure you meet the
-000008d0: 2066 6f6c 6c6f 7769 6e67 2072 6571 7569   following requi
-000008e0: 7265 6d65 6e74 7320 6265 666f 7265 2069  rements before i
-000008f0: 6e73 7461 6c6c 6174 696f 6e20 2869 6620  nstallation (if 
-00000900: 796f 7527 7265 2062 7569 6c64 696e 6720  you're building 
-00000910: 6672 6f6d 2073 6f75 7263 6529 3a0a 0a60  from source):..`
-00000920: 6060 6261 7368 0a70 6970 2069 6e73 7461  ``bash.pip insta
-00000930: 6c6c 202d 7220 7265 7175 6972 656d 656e  ll -r requiremen
-00000940: 7473 2e74 7874 0a60 6060 0a0a 3c68 323e  ts.txt.```..<h2>
-00000950: 3c61 2069 643d 2269 6e73 7461 223e 203a  <a id="insta"> :
-00000960: 746f 6f6c 626f 783a 3c2f 613e 2049 6e73  toolbox:</a> Ins
-00000970: 7461 6c6c 6174 696f 6e3c 2f68 323e 0a0a  tallation</h2>..
-00000980: 3c68 333e 3c61 2069 643d 2270 7970 6922  <h3><a id="pypi"
-00000990: 3e20 496e 7374 616c 6c20 6672 6f6d 2050  > Install from P
-000009a0: 7950 493c 2f61 3e3c 2f68 333e 0a0a 596f  yPI</a></h3>..Yo
-000009b0: 7520 6361 6e20 696e 7374 616c 6c20 7468  u can install th
-000009c0: 6520 6070 7971 7561 6e74 6966 7960 2070  e `pyquantify` p
-000009d0: 6163 6b61 6765 2064 6972 6563 746c 7920  ackage directly 
-000009e0: 6672 6f6d 2050 7950 4920 7573 696e 6720  from PyPI using 
-000009f0: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00000a00: 6d6d 616e 643a 0a0a 6060 6062 6173 680a  mmand:..```bash.
-00000a10: 7069 7020 696e 7374 616c 6c20 7079 7175  pip install pyqu
-00000a20: 616e 7469 6679 0a60 6060 0a0a 3c68 333e  antify.```..<h3>
-00000a30: 3c61 2069 643d 2273 7263 223e 2042 7569  <a id="src"> Bui
-00000a40: 6c64 2066 726f 6d20 536f 7572 6365 3c2f  ld from Source</
-00000a50: 613e 3c2f 6833 3e0a 0a31 2e20 436c 6f6e  a></h3>..1. Clon
-00000a60: 6520 7468 6520 7072 6f6a 6563 743a 0a0a  e the project:..
-00000a70: 6060 6062 6173 680a 6769 7420 636c 6f6e  ```bash.git clon
-00000a80: 6520 3c72 6570 6f73 6974 6f72 795f 7572  e <repository_ur
-00000a90: 6c3e 0a63 6420 7079 7175 616e 7469 6679  l>.cd pyquantify
-00000aa0: 0a60 6060 0a0a 322e 2042 7569 6c64 2074  .```..2. Build t
-00000ab0: 6865 2070 6163 6b61 6765 3a0a 0a60 6060  he package:..```
-00000ac0: 6261 7368 0a70 7974 686f 6e33 202d 6d20  bash.python3 -m 
-00000ad0: 6275 696c 640a 6060 600a 0a33 2e20 496e  build.```..3. In
-00000ae0: 7374 616c 6c20 7468 6520 7061 636b 6167  stall the packag
-00000af0: 653a 0a0a 6060 6062 6173 680a 7069 7020  e:..```bash.pip 
-00000b00: 696e 7374 616c 6c20 6469 7374 2f2a 677a  install dist/*gz
-00000b10: 0a60 6060 0a0a 342e 2052 756e 2074 6865  .```..4. Run the
-00000b20: 2074 6f6f 6c20 696e 2074 6572 6d69 6e61   tool in termina
-00000b30: 6c3a 0a0a 6060 6062 6173 680a 7079 7175  l:..```bash.pyqu
-00000b40: 616e 7469 6679 0a60 6060 0a3c 6832 3e3c  antify.```.<h2><
-00000b50: 6120 6964 3d22 7573 6522 3e20 3a62 6f6f  a id="use"> :boo
-00000b60: 6b3a 2055 7361 6765 2047 7569 6465 3c2f  k: Usage Guide</
-00000b70: 613e 3c2f 6833 3e0a 0a50 7971 7561 6e74  a></h3>..Pyquant
-00000b80: 6966 7920 7072 6f76 6964 6573 2073 6576  ify provides sev
-00000b90: 6572 616c 2063 6f6d 6d61 6e64 7320 666f  eral commands fo
-00000ba0: 7220 616e 616c 797a 696e 6720 616e 6420  r analyzing and 
-00000bb0: 7669 7375 616c 697a 696e 6720 7465 7874  visualizing text
-00000bc0: 2064 6174 612e 2042 656c 6f77 2069 7320   data. Below is 
-00000bd0: 6120 6775 6964 6520 6f6e 2068 6f77 2074  a guide on how t
-00000be0: 6f20 7573 6520 7468 6520 6b65 7920 6675  o use the key fu
-00000bf0: 6e63 7469 6f6e 616c 6974 6965 733a 0a0a  nctionalities:..
-00000c00: 312e 202a 2a53 6561 7263 6820 666f 7220  1. **Search for 
-00000c10: 6120 5370 6563 6966 6963 2057 6f72 6420  a Specific Word 
-00000c20: 696e 204d 6f72 7068 6f6c 6f67 6963 616c  in Morphological
-00000c30: 2041 6e61 6c79 7369 733a 2a2a 0a0a 2020   Analysis:**..  
-00000c40: 2060 6060 6261 7368 0a20 2020 7079 7175   ```bash.   pyqu
-00000c50: 616e 7469 6679 2073 6561 7263 682d 776f  antify search-wo
-00000c60: 7264 202d 2d6d 6f64 6520 5b72 6177 2f66  rd --mode [raw/f
-00000c70: 696c 652f 7765 6273 6974 655d 202d 2d77  ile/website] --w
-00000c80: 6f72 6420 5b64 6573 6972 6564 5f77 6f72  ord [desired_wor
-00000c90: 645d 0a20 2020 6060 600a 0a20 2020 2d20  d].   ```..   - 
-00000ca0: 602d 2d6d 6f64 6560 3a20 5370 6563 6966  `--mode`: Specif
-00000cb0: 7920 7468 6520 6461 7461 206c 6f61 6469  y the data loadi
-00000cc0: 6e67 206d 6f64 6520 2872 6177 2069 6e70  ng mode (raw inp
-00000cd0: 7574 2c20 6669 6c65 2c20 6f72 2077 6562  ut, file, or web
-00000ce0: 7369 7465 292e 0a20 2020 2d20 602d 2d77  site)..   - `--w
-00000cf0: 6f72 6460 3a20 5370 6563 6966 7920 7468  ord`: Specify th
-00000d00: 6520 776f 7264 2079 6f75 2077 616e 7420  e word you want 
-00000d10: 746f 2073 6561 7263 6820 666f 722e 0a0a  to search for...
-00000d20: 322e 202a 2a47 656e 6572 6174 6520 576f  2. **Generate Wo
-00000d30: 7264 2046 7265 7175 656e 6379 2050 6c6f  rd Frequency Plo
-00000d40: 743a 2a2a 0a0a 2020 2060 6060 6261 7368  t:**..   ```bash
-00000d50: 0a20 2020 7079 7175 616e 7469 6679 2076  .   pyquantify v
-00000d60: 6973 7561 6c69 7a65 202d 2d6d 6f64 6520  isualize --mode 
-00000d70: 5b72 6177 2f66 696c 652f 7765 6273 6974  [raw/file/websit
-00000d80: 655d 202d 2d66 7265 712d 6368 6172 7420  e] --freq-chart 
-00000d90: 2d2d 6578 706f 7274 0a20 2020 6060 600a  --export.   ```.
-00000da0: 0a20 2020 2d20 602d 2d6d 6f64 6560 3a20  .   - `--mode`: 
-00000db0: 5370 6563 6966 7920 7468 6520 6461 7461  Specify the data
-00000dc0: 206c 6f61 6469 6e67 206d 6f64 6520 2872   loading mode (r
-00000dd0: 6177 2069 6e70 7574 2c20 6669 6c65 2c20  aw input, file, 
-00000de0: 6f72 2077 6562 7369 7465 292e 0a20 2020  or website)..   
-00000df0: 2d20 602d 2d66 7265 712d 6368 6172 7460  - `--freq-chart`
-00000e00: 3a20 466c 6167 2074 6f20 6765 6e65 7261  : Flag to genera
-00000e10: 7465 2077 6f72 6420 6672 6571 7565 6e63  te word frequenc
-00000e20: 7920 6368 6172 742e 0a20 2020 2d20 602d  y chart..   - `-
-00000e30: 2d65 7870 6f72 7460 3a20 4f70 7469 6f6e  -export`: Option
-00000e40: 616c 2066 6c61 6720 746f 2065 7870 6f72  al flag to expor
-00000e50: 7420 7468 6520 6672 6571 7565 6e63 7920  t the frequency 
-00000e60: 706c 6f74 2074 6f20 6120 6669 6c65 2e0a  plot to a file..
-00000e70: 0a33 2e20 2a2a 4765 6e65 7261 7465 2057  .3. **Generate W
-00000e80: 6f72 6420 436c 6f75 643a 2a2a 0a0a 2020  ord Cloud:**..  
-00000e90: 2060 6060 6261 7368 0a20 2020 7079 7175   ```bash.   pyqu
-00000ea0: 616e 7469 6679 2076 6973 7561 6c69 7a65  antify visualize
-00000eb0: 202d 2d6d 6f64 6520 5b72 6177 2f66 696c   --mode [raw/fil
-00000ec0: 652f 7765 6273 6974 655d 202d 2d77 6f72  e/website] --wor
-00000ed0: 6463 6c6f 7564 202d 2d65 7870 6f72 740a  dcloud --export.
-00000ee0: 2020 2060 6060 0a0a 2020 202d 2060 2d2d     ```..   - `--
-00000ef0: 6d6f 6465 603a 2053 7065 6369 6679 2074  mode`: Specify t
-00000f00: 6865 2064 6174 6120 6c6f 6164 696e 6720  he data loading 
-00000f10: 6d6f 6465 2028 7261 7720 696e 7075 742c  mode (raw input,
-00000f20: 2066 696c 652c 206f 7220 7765 6273 6974   file, or websit
-00000f30: 6529 2e0a 2020 202d 2060 2d2d 776f 7264  e)..   - `--word
-00000f40: 636c 6f75 6460 3a20 466c 6167 2074 6f20  cloud`: Flag to 
-00000f50: 6765 6e65 7261 7465 2077 6f72 6420 636c  generate word cl
-00000f60: 6f75 642e 0a20 2020 2d20 602d 2d65 7870  oud..   - `--exp
-00000f70: 6f72 7460 3a20 4f70 7469 6f6e 616c 2066  ort`: Optional f
-00000f80: 6c61 6720 746f 2065 7870 6f72 7420 7468  lag to export th
-00000f90: 6520 776f 7264 2063 6c6f 7564 2074 6f20  e word cloud to 
-00000fa0: 6120 6669 6c65 2e0a 0a34 2e20 2a2a 5465  a file...4. **Te
-00000fb0: 7874 2041 6e61 6c79 7369 7320 616e 6420  xt Analysis and 
-00000fc0: 4d65 7472 6963 7320 4765 6e65 7261 7469  Metrics Generati
-00000fd0: 6f6e 3a2a 2a0a 0a20 2020 6060 6062 6173  on:**..   ```bas
-00000fe0: 680a 2020 2070 7971 7561 6e74 6966 7920  h.   pyquantify 
-00000ff0: 616e 616c 797a 6520 2d2d 6d6f 6465 205b  analyze --mode [
-00001000: 7261 772f 6669 6c65 2f77 6562 7369 7465  raw/file/website
-00001010: 5d20 2d2d 6e20 5b6e 756d 6265 725f 6f66  ] --n [number_of
-00001020: 5f72 6f77 735d 202d 2d65 7870 6f72 740a  _rows] --export.
-00001030: 2020 2060 6060 0a0a 2020 202d 2060 2d2d     ```..   - `--
-00001040: 6d6f 6465 603a 2053 7065 6369 6679 2074  mode`: Specify t
-00001050: 6865 2064 6174 6120 6c6f 6164 696e 6720  he data loading 
-00001060: 6d6f 6465 2028 7261 7720 696e 7075 742c  mode (raw input,
-00001070: 2066 696c 652c 206f 7220 7765 6273 6974   file, or websit
-00001080: 6529 2e0a 2020 202d 2060 2d2d 6e60 3a20  e)..   - `--n`: 
-00001090: 4f70 7469 6f6e 616c 2070 6172 616d 6574  Optional paramet
-000010a0: 6572 2074 6f20 6469 7370 6c61 7920 6120  er to display a 
-000010b0: 7370 6563 6966 6963 206e 756d 6265 7220  specific number 
-000010c0: 6f66 2072 6f77 7320 696e 2074 6865 2061  of rows in the a
-000010d0: 6e61 6c79 7369 732e 0a20 2020 2d20 602d  nalysis..   - `-
-000010e0: 2d65 7870 6f72 7460 3a20 4f70 7469 6f6e  -export`: Option
-000010f0: 616c 2066 6c61 6720 746f 2065 7870 6f72  al flag to expor
-00001100: 7420 7468 6520 616e 616c 7973 6973 2072  t the analysis r
-00001110: 6573 756c 7473 2074 6f20 6669 6c65 732e  esults to files.
-00001120: 0a0a 352e 202a 2a53 756d 6d61 7269 7a65  ..5. **Summarize
-00001130: 2054 6578 743a 2a2a 0a0a 2020 2060 6060   Text:**..   ```
-00001140: 6261 7368 0a20 2020 7079 7175 616e 7469  bash.   pyquanti
-00001150: 6679 2073 756d 6d61 7269 7a65 202d 2d6d  fy summarize --m
-00001160: 6f64 6520 5b72 6177 2f66 696c 652f 7765  ode [raw/file/we
-00001170: 6273 6974 655d 202d 2d65 7870 6f72 740a  bsite] --export.
-00001180: 2020 2060 6060 0a0a 2020 202d 2060 2d2d     ```..   - `--
-00001190: 6d6f 6465 603a 2053 7065 6369 6679 2074  mode`: Specify t
-000011a0: 6865 2064 6174 6120 6c6f 6164 696e 6720  he data loading 
-000011b0: 6d6f 6465 2028 7261 7720 696e 7075 742c  mode (raw input,
-000011c0: 2066 696c 652c 206f 7220 7765 6273 6974   file, or websit
-000011d0: 6529 2e0a 2020 202d 2060 2d2d 6578 706f  e)..   - `--expo
-000011e0: 7274 603a 204f 7074 696f 6e61 6c20 666c  rt`: Optional fl
-000011f0: 6167 2074 6f20 6578 706f 7274 2074 6865  ag to export the
-00001200: 2073 756d 6d61 7279 2074 6f20 6120 6669   summary to a fi
-00001210: 6c65 2e0a 0a36 2e20 2a2a 5365 6e74 696d  le...6. **Sentim
-00001220: 656e 7420 416e 616c 7973 6973 2a2a 0a0a  ent Analysis**..
-00001230: 2020 2060 6060 6261 7368 0a20 2020 7079     ```bash.   py
-00001240: 7175 616e 7469 6679 2073 656e 7469 6d65  quantify sentime
-00001250: 6e74 2d61 6e61 6c79 7369 7320 2d2d 6d6f  nt-analysis --mo
-00001260: 6465 205b 7261 772f 6669 6c65 2f77 6562  de [raw/file/web
-00001270: 7369 7465 5d20 2d2d 6578 706f 7274 0a20  site] --export. 
-00001280: 2020 6060 600a 0a20 2020 2d20 602d 2d6d    ```..   - `--m
-00001290: 6f64 6560 3a20 5370 6563 6966 7920 7468  ode`: Specify th
-000012a0: 6520 6461 7461 206c 6f61 6469 6e67 206d  e data loading m
-000012b0: 6f64 6520 2872 6177 2069 6e70 7574 2c20  ode (raw input, 
-000012c0: 6669 6c65 2c20 6f72 2077 6562 7369 7465  file, or website
-000012d0: 292e 0a20 2020 2d20 602d 2d65 7870 6f72  )..   - `--expor
-000012e0: 7460 3a20 4f70 7469 6f6e 616c 2066 6c61  t`: Optional fla
-000012f0: 6720 746f 2065 7870 6f72 7420 7468 6520  g to export the 
-00001300: 7375 6d6d 6172 7920 746f 2061 2066 696c  summary to a fil
-00001310: 652e 0a20 2020 0a23 2323 2041 6464 6974  e..   .### Addit
-00001320: 696f 6e61 6c20 436f 6d6d 616e 6473 0a0a  ional Commands..
-00001330: 2d20 5669 6577 2074 6865 2050 7971 7561  - View the Pyqua
-00001340: 6e74 6966 7920 4769 7448 7562 2070 6167  ntify GitHub pag
-00001350: 653a 0a60 6060 6261 7368 0a70 7971 7561  e:.```bash.pyqua
-00001360: 6e74 6966 7920 2d2d 6769 740a 6060 600a  ntify --git.```.
-00001370: 0a46 6565 6c20 6672 6565 2074 6f20 6578  .Feel free to ex
-00001380: 706c 6f72 6520 6164 6469 7469 6f6e 616c  plore additional
-00001390: 206f 7074 696f 6e73 2061 6e64 2066 756e   options and fun
-000013a0: 6374 696f 6e61 6c69 7469 6573 2062 7920  ctionalities by 
-000013b0: 6368 6563 6b69 6e67 2074 6865 2068 656c  checking the hel
-000013c0: 7020 646f 6375 6d65 6e74 6174 696f 6e20  p documentation 
-000013d0: 666f 7220 6561 6368 2063 6f6d 6d61 6e64  for each command
-000013e0: 3a0a 0a60 6060 6261 7368 0a70 7971 7561  :..```bash.pyqua
-000013f0: 6e74 6966 7920 5b63 6f6d 6d61 6e64 5d20  ntify [command] 
-00001400: 2d2d 6865 6c70 0a60 6060 0a3c 2f64 6976  --help.```.</div
-00001410: 3e0a 0a0a 3c68 323e 3c61 2069 643d 2271  >...<h2><a id="q
-00001420: 7565 7322 3e3a 6772 6579 5f71 7565 7374  ues">:grey_quest
-00001430: 696f 6e3a 2046 4151 3c2f 613e 3c2f 6832  ion: FAQ</a></h2
-00001440: 3e0a 0a23 2323 2051 3a20 5768 6174 2069  >..### Q: What i
-00001450: 7320 5079 7175 616e 7469 6679 3f0a 0a50  s Pyquantify?..P
-00001460: 7971 7561 6e74 6966 7920 6973 2061 2074  yquantify is a t
-00001470: 6f6f 6c20 6465 7369 676e 6564 2066 6f72  ool designed for
-00001480: 2069 6e2d 6465 7074 6820 616e 616c 7973   in-depth analys
-00001490: 6973 206f 6620 7465 7874 7561 6c20 6461  is of textual da
-000014a0: 7461 2c20 666f 6375 7369 6e67 206f 6e20  ta, focusing on 
-000014b0: 6578 7472 6163 7469 6e67 206d 6561 6e69  extracting meani
-000014c0: 6e67 2061 6e64 206c 696e 6775 6973 7469  ng and linguisti
-000014d0: 6320 696e 7369 6768 7473 2e20 4974 2070  c insights. It p
-000014e0: 726f 7669 6465 7320 6665 6174 7572 6573  rovides features
-000014f0: 206c 696b 6520 776f 7264 2066 7265 7175   like word frequ
-00001500: 656e 6379 2c20 6d6f 7270 686f 6c6f 6779  ency, morphology
-00001510: 2c20 616e 6420 6d65 7472 6963 7320 6765  , and metrics ge
-00001520: 6e65 7261 7469 6f6e 2c20 656e 6861 6e63  neration, enhanc
-00001530: 696e 6720 6461 7461 2065 7870 6c6f 7261  ing data explora
-00001540: 7469 6f6e 2061 6e64 2076 6973 7561 6c69  tion and visuali
-00001550: 7a61 7469 6f6e 2e0a 0a23 2323 2051 3a20  zation...### Q: 
-00001560: 5768 7920 4465 7665 6c6f 7020 5079 7175  Why Develop Pyqu
-00001570: 616e 7469 6679 2061 7320 6120 5365 6d61  antify as a Sema
-00001580: 6e74 6963 2050 726f 6669 6c65 723f 0a0a  ntic Profiler?..
-00001590: 5079 7175 616e 7469 6679 2077 6173 2063  Pyquantify was c
-000015a0: 7265 6174 6564 2066 6f72 2074 6865 2044  reated for the D
-000015b0: 5341 2073 7562 6a65 6374 2069 6e20 7468  SA subject in th
-000015c0: 6520 6669 6674 6820 7365 6d65 7374 6572  e fifth semester
-000015d0: 206f 6620 636f 6c6c 6567 652e 2054 6865   of college. The
-000015e0: 2067 6f61 6c20 7761 7320 746f 206f 6666   goal was to off
-000015f0: 6572 2061 2076 6572 7361 7469 6c65 204e  er a versatile N
-00001600: 4c50 2074 6f6f 6c2c 2065 6d70 6f77 6572  LP tool, empower
-00001610: 696e 6720 7573 6572 7320 746f 2061 6e61  ing users to ana
-00001620: 6c79 7a65 2061 6e64 2070 726f 6669 6c65  lyze and profile
-00001630: 2074 6578 7420 6566 6669 6369 656e 746c   text efficientl
-00001640: 792e 2054 6865 2074 6f6f 6c27 7320 6665  y. The tool's fe
-00001650: 6174 7572 6573 2061 696d 2074 6f20 6465  atures aim to de
-00001660: 6570 656e 2075 6e64 6572 7374 616e 6469  epen understandi
-00001670: 6e67 2061 6e64 2065 7870 6c6f 7261 7469  ng and explorati
-00001680: 6f6e 206f 6620 6c69 6e67 7569 7374 6963  on of linguistic
-00001690: 2061 7370 6563 7473 2077 6974 6869 6e20   aspects within 
-000016a0: 7465 7874 7561 6c20 6461 7461 2e0a 0a23  textual data...#
-000016b0: 2323 2051 3a20 5768 7920 4469 6420 5079  ## Q: Why Did Py
-000016c0: 7175 616e 7469 6679 2065 766f 6c76 6520  quantify evolve 
-000016d0: 6672 6f6d 2061 2057 6f72 6420 4672 6571  from a Word Freq
-000016e0: 7565 6e63 7920 436f 756e 7465 723f 0a0a  uency Counter?..
-000016f0: 4f72 6967 696e 616c 6c79 2063 6f6e 6365  Originally conce
-00001700: 6976 6564 2061 7320 6120 776f 7264 2066  ived as a word f
-00001710: 7265 7175 656e 6379 2063 6f75 6e74 6572  requency counter
-00001720: 2c20 5079 7175 616e 7469 6679 2773 2064  , Pyquantify's d
-00001730: 6576 656c 6f70 6d65 6e74 2074 6f6f 6b20  evelopment took 
-00001740: 6120 6469 6666 6572 656e 7420 6469 7265  a different dire
-00001750: 6374 696f 6e2e 2054 6865 2064 6563 6973  ction. The decis
-00001760: 696f 6e20 746f 2065 7870 616e 6420 6974  ion to expand it
-00001770: 7320 6361 7061 6269 6c69 7469 6573 2077  s capabilities w
-00001780: 6173 2064 7269 7665 6e20 6279 2074 6865  as driven by the
-00001790: 2064 6573 6972 6520 746f 2063 7265 6174   desire to creat
-000017a0: 6520 6120 6d6f 7265 2063 6f6d 7072 6568  e a more compreh
-000017b0: 656e 7369 7665 2074 6f6f 6c20 666f 7220  ensive tool for 
-000017c0: 6e61 7475 7261 6c20 6c61 6e67 7561 6765  natural language
-000017d0: 2070 726f 6365 7373 696e 672e 2054 6865   processing. The
-000017e0: 2070 726f 6a65 6374 2065 766f 6c76 6564   project evolved
-000017f0: 2074 6f20 656e 636f 6d70 6173 7320 7365   to encompass se
-00001800: 6d61 6e74 6963 2070 726f 6669 6c69 6e67  mantic profiling
-00001810: 2c20 6f66 6665 7269 6e67 2061 2072 6963  , offering a ric
-00001820: 6865 7220 7365 7420 6f66 2066 6561 7475  her set of featu
-00001830: 7265 7320 7375 6368 2061 7320 6d6f 7270  res such as morp
-00001840: 686f 6c6f 6779 2061 6e61 6c79 7369 732c  hology analysis,
-00001850: 206d 6574 7269 6373 2067 656e 6572 6174   metrics generat
-00001860: 696f 6e2c 2061 6e64 2065 6e68 616e 6365  ion, and enhance
-00001870: 6420 6461 7461 2076 6973 7561 6c69 7a61  d data visualiza
-00001880: 7469 6f6e 2e20 5468 6973 2073 6869 6674  tion. This shift
-00001890: 2061 696d 6564 2074 6f20 7072 6f76 6964   aimed to provid
-000018a0: 6520 7573 6572 7320 7769 7468 2061 206d  e users with a m
-000018b0: 6f72 6520 706f 7765 7266 756c 2061 6e64  ore powerful and
-000018c0: 2076 6572 7361 7469 6c65 2073 6f6c 7574   versatile solut
-000018d0: 696f 6e20 666f 7220 6578 706c 6f72 696e  ion for explorin
-000018e0: 6720 616e 6420 756e 6465 7273 7461 6e64  g and understand
-000018f0: 696e 6720 7465 7874 7561 6c20 6461 7461  ing textual data
-00001900: 2062 6579 6f6e 6420 7369 6d70 6c65 2077   beyond simple w
-00001910: 6f72 6420 6672 6571 7565 6e63 7920 616e  ord frequency an
-00001920: 616c 7973 6973 2e0a 0a23 2323 2051 3a20  alysis...### Q: 
-00001930: 5768 7920 7468 6520 6e61 6d65 2063 6861  Why the name cha
-00001940: 6e67 6520 6672 6f6d 204e 4c50 4672 6571  nge from NLPFreq
-00001950: 2074 6f20 5079 7175 616e 7469 6679 3f0a   to Pyquantify?.
-00001960: 0a4e 4c50 4672 6571 2066 656c 7420 6c69  .NLPFreq felt li
-00001970: 6d69 7469 6e67 2061 6e64 2064 6964 6e27  miting and didn'
-00001980: 7420 6361 7074 7572 6520 7468 6520 6675  t capture the fu
-00001990: 6c6c 2073 636f 7065 206f 6620 7468 6520  ll scope of the 
-000019a0: 7072 6f6a 6563 742e 2050 7971 7561 6e74  project. Pyquant
-000019b0: 6966 7920 6d6f 7265 2061 6363 7572 6174  ify more accurat
-000019c0: 656c 7920 7265 666c 6563 7473 2069 7473  ely reflects its
-000019d0: 2063 6170 6162 696c 6974 6965 7320 6173   capabilities as
-000019e0: 2061 2050 7974 686f 6e2d 6261 7365 6420   a Python-based 
-000019f0: 746f 6f6c 2066 6f72 2071 7561 6e74 6974  tool for quantit
-00001a00: 6174 6976 6520 6461 7461 2061 6e61 6c79  ative data analy
-00001a10: 7369 732e 0a0a 0a3c 6832 3e20 3c61 2069  sis....<h2> <a i
-00001a20: 6420 3d20 2261 636b 223e 3a67 656d 3a20  d = "ack">:gem: 
-00001a30: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
-00001a40: 3c2f 613e 3c2f 6832 3e0a 0a2d 205b 4e65  </a></h2>..- [Ne
-00001a50: 7572 616c 4e69 6e65 2773 2050 7562 6c69  uralNine's Publi
-00001a60: 7368 2059 6f75 7220 4f77 6e20 5079 7468  sh Your Own Pyth
-00001a70: 6f6e 2050 6163 6b61 6765 5d28 6874 7470  on Package](http
-00001a80: 733a 2f2f 7777 772e 796f 7574 7562 652e  s://www.youtube.
-00001a90: 636f 6d2f 7761 7463 683f 763d 7445 466b  com/watch?v=tEFk
-00001aa0: 4845 4b79 704c 4929 0a0a 3c68 722f 3e0a  HEKypLI)..<hr/>.
-00001ab0: 0a2a 2a4e 6f74 653a 2a2a 2050 7971 7561  .**Note:** Pyqua
-00001ac0: 6e74 6966 7920 6861 7320 756e 6465 7267  ntify has underg
-00001ad0: 6f6e 6520 7468 6f72 6f75 6768 2074 6573  one thorough tes
-00001ae0: 7469 6e67 206f 6e20 4c69 6e75 782c 2061  ting on Linux, a
-00001af0: 6e64 2069 7473 2066 756e 6374 696f 6e61  nd its functiona
-00001b00: 6c69 7479 2069 7320 636f 6e66 6972 6d65  lity is confirme
-00001b10: 6420 746f 2077 6f72 6b20 7365 616d 6c65  d to work seamle
-00001b20: 7373 6c79 2e20 486f 7765 7665 722c 2069  ssly. However, i
-00001b30: 7427 7320 696d 706f 7274 616e 7420 746f  t's important to
-00001b40: 206e 6f74 6520 7468 6174 2077 6865 6e20   note that when 
-00001b50: 7275 6e6e 696e 6720 6f6e 2057 696e 646f  running on Windo
-00001b60: 7773 2053 7562 7379 7374 656d 2066 6f72  ws Subsystem for
-00001b70: 204c 696e 7578 2028 5753 4c29 2c20 6365   Linux (WSL), ce
-00001b80: 7274 6169 6e20 6665 6174 7572 6573 206d  rtain features m
-00001b90: 6179 2068 6176 6520 6c69 6d69 7465 6420  ay have limited 
-00001ba0: 6675 6e63 7469 6f6e 616c 6974 7920 6475  functionality du
-00001bb0: 6520 746f 2074 6865 2061 6273 656e 6365  e to the absence
-00001bc0: 206f 6620 7468 6520 636f 6d70 6c65 7465   of the complete
-00001bd0: 204c 696e 7578 2074 6f6f 6c73 6574 2069   Linux toolset i
-00001be0: 6e20 7468 6520 5753 4c20 656e 7669 726f  n the WSL enviro
-00001bf0: 6e6d 656e 742e 0a                        nment..
+00000000: 0a23 2070 7971 7561 6e74 6966 790a 0a50  .# pyquantify..P
+00000010: 7971 7561 6e74 6966 7920 6973 2061 2070  yquantify is a p
+00000020: 6f77 6572 6675 6c20 434c 4920 746f 6f6c  owerful CLI tool
+00000030: 2066 6f72 2073 656d 616e 7469 6320 616e   for semantic an
+00000040: 616c 7973 6973 2e20 4974 206c 6576 6572  alysis. It lever
+00000050: 6167 6573 206e 6174 7572 616c 206c 616e  ages natural lan
+00000060: 6775 6167 6520 7072 6f63 6573 7369 6e67  guage processing
+00000070: 2074 6f20 756e 7665 696c 2069 6e73 6967   to unveil insig
+00000080: 6874 7320 6672 6f6d 2074 6578 742c 2066  hts from text, f
+00000090: 696c 6573 2c20 6f72 2077 6562 7369 7465  iles, or website
+000000a0: 732c 2065 6d70 6f77 6572 696e 6720 736f  s, empowering so
+000000b0: 7068 6973 7469 6361 7465 6420 6461 7461  phisticated data
+000000c0: 2076 6973 7561 6c69 7a61 7469 6f6e 2061   visualization a
+000000d0: 6e64 2065 7870 6c6f 7261 7469 6f6e 2e0a  nd exploration..
+000000e0: 0a0a 2323 2042 6164 6765 730a 0a21 5b50  ..## Badges..![P
+000000f0: 7971 7561 6e74 6966 7920 5665 7273 696f  yquantify Versio
+00000100: 6e5d 2868 7474 7073 3a2f 2f69 6d67 2e73  n](https://img.s
+00000110: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000120: 5079 5175 616e 7469 6679 2d31 2e32 2e30  PyQuantify-1.2.0
+00000130: 2d62 7269 6768 7467 7265 656e 290a 0a5b  -brightgreen)..[
+00000140: 215b 4750 4c76 3320 4c69 6365 6e73 655d  ![GPLv3 License]
+00000150: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000160: 656c 6473 2e69 6f2f 6261 6467 652f 4c69  elds.io/badge/Li
+00000170: 6365 6e73 652d 4750 4c25 3230 7633 2d79  cense-GPL%20v3-y
+00000180: 656c 6c6f 772e 7376 6729 5d28 6874 7470  ellow.svg)](http
+00000190: 733a 2f2f 6f70 656e 736f 7572 6365 2e6f  s://opensource.o
+000001a0: 7267 2f6c 6963 656e 7365 732f 290a 0a5b  rg/licenses/)..[
+000001b0: 215b 5079 7468 6f6e 2033 5d28 6874 7470  ![Python 3](http
+000001c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000001d0: 696f 2f62 6164 6765 2f50 7974 686f 6e2d  io/badge/Python-
+000001e0: 332d 6272 6967 6874 6772 6565 6e29 5d28  3-brightgreen)](
+000001f0: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
+00000200: 6f6e 2e6f 7267 2f29 0a0a 2323 2054 6162  on.org/)..## Tab
+00000210: 6c65 204f 6620 436f 6e74 656e 7473 0a20  le Of Contents. 
+00000220: 2020 2a20 5b46 6561 7475 7265 735d 2823    * [Features](#
+00000230: 6665 6174 7572 6573 290a 2020 202a 205b  features).   * [
+00000240: 496e 7374 616c 6c61 7469 6f6e 5d28 2369  Installation](#i
+00000250: 6e73 7461 6c6c 6174 696f 6e29 0a20 2020  nstallation).   
+00000260: 2020 2020 2020 2d20 5b49 6e73 7461 6c6c        - [Install
+00000270: 2070 7971 7561 6e74 6966 7920 7769 7468   pyquantify with
+00000280: 2070 6970 5d28 2369 6e73 7461 6c6c 2d70   pip](#install-p
+00000290: 7971 7561 6e74 6966 792d 7769 7468 2d70  yquantify-with-p
+000002a0: 6970 290a 2020 2020 2020 2020 202d 205b  ip).         - [
+000002b0: 6f72 2079 6f75 2063 616e 2062 7569 6c64  or you can build
+000002c0: 206c 6f63 616c 6c79 5d28 236f 722d 796f   locally](#or-yo
+000002d0: 752d 6361 6e2d 6275 696c 642d 6c6f 6361  u-can-build-loca
+000002e0: 6c6c 7929 0a20 2020 2a20 5b42 6566 6f72  lly).   * [Befor
+000002f0: 6520 7275 6e6e 696e 6720 7079 7175 616e  e running pyquan
+00000300: 7469 6679 5d28 2362 6566 6f72 652d 7275  tify](#before-ru
+00000310: 6e6e 696e 672d 7079 7175 616e 7469 6679  nning-pyquantify
+00000320: 290a 2020 202a 205b 5573 6167 652f 4578  ).   * [Usage/Ex
+00000330: 616d 706c 6573 5d28 2375 7361 6765 6578  amples](#usageex
+00000340: 616d 706c 6573 290a 2020 202a 205b 4641  amples).   * [FA
+00000350: 515d 2823 6661 7129 0a20 2020 2a20 5b53  Q](#faq).   * [S
+00000360: 6372 6565 6e73 686f 7473 5d28 2373 6372  creenshots](#scr
+00000370: 6565 6e73 686f 7473 290a 2020 202a 205b  eenshots).   * [
+00000380: 4163 6b6e 6f77 6c65 6467 656d 656e 7473  Acknowledgements
+00000390: 5d28 2361 636b 6e6f 776c 6564 6765 6d65  ](#acknowledgeme
+000003a0: 6e74 7329 0a0a 0a23 2320 4465 6d6f 0a0a  nts)...## Demo..
+000003b0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000003c0: 2f2f 6769 7468 7562 2e63 6f6d 2f76 6976  //github.com/viv
+000003d0: 656b 6b64 6167 6172 2f70 7971 7561 6e74  ekkdagar/pyquant
+000003e0: 6966 792f 626c 6f62 2f6d 6169 6e2f 6173  ify/blob/main/as
+000003f0: 7365 7473 2f73 6372 6565 6e73 686f 7473  sets/screenshots
+00000400: 2f6d 656e 752e 706e 6722 3e0a 0a0a 2323  /menu.png">...##
+00000410: 2046 6561 7475 7265 730a 0a31 2e20 2a2a   Features..1. **
+00000420: 5465 7874 2053 756d 6d61 7269 7a61 7469  Text Summarizati
+00000430: 6f6e 2a2a 3a0a 2020 202d 2055 7469 6c69  on**:.   - Utili
+00000440: 7a65 7320 7468 6520 4245 5254 206d 6f64  zes the BERT mod
+00000450: 656c 2066 6f72 2073 756d 6d61 7269 7a69  el for summarizi
+00000460: 6e67 2074 6578 742e 0a20 2020 2d20 5072  ng text..   - Pr
+00000470: 6f76 6964 6573 2063 6163 6869 6e67 2066  ovides caching f
+00000480: 756e 6374 696f 6e61 6c69 7479 2074 6f20  unctionality to 
+00000490: 7370 6565 6420 7570 2073 756d 6d61 7269  speed up summari
+000004a0: 7a61 7469 6f6e 2066 6f72 2070 7265 7669  zation for previ
+000004b0: 6f75 736c 7920 7072 6f63 6573 7365 6420  ously processed 
+000004c0: 7465 7874 2e0a 2020 202d 2053 7570 706f  text..   - Suppo
+000004d0: 7274 7320 6578 706f 7274 696e 6720 7375  rts exporting su
+000004e0: 6d6d 6172 6965 7320 746f 2074 6578 7420  mmaries to text 
+000004f0: 6669 6c65 732e 0a0a 322e 202a 2a54 6578  files...2. **Tex
+00000500: 7420 416e 616c 7973 6973 2a2a 3a0a 2020  t Analysis**:.  
+00000510: 202d 2050 7265 7072 6f63 6573 7365 7320   - Preprocesses 
+00000520: 7465 7874 2064 6174 6120 696e 636c 7564  text data includ
+00000530: 696e 6720 746f 6b65 6e69 7a61 7469 6f6e  ing tokenization
+00000540: 2061 6e64 2070 6172 742d 6f66 2d73 7065   and part-of-spe
+00000550: 6563 6820 7461 6767 696e 672e 0a20 2020  ech tagging..   
+00000560: 2d20 4765 6e65 7261 7465 7320 7661 7269  - Generates vari
+00000570: 6f75 7320 6d65 7472 6963 7320 7375 6368  ous metrics such
+00000580: 2061 7320 6368 6172 6163 7465 7220 636f   as character co
+00000590: 756e 742c 2077 6f72 6420 636f 756e 742c  unt, word count,
+000005a0: 2073 656e 7465 6e63 6520 636f 756e 742c   sentence count,
+000005b0: 2065 7463 2e0a 2020 202d 2041 6e61 6c79   etc..   - Analy
+000005c0: 7a65 7320 6d6f 7270 686f 6c6f 6769 6361  zes morphologica
+000005d0: 6c20 6461 7461 2069 6e63 6c75 6469 6e67  l data including
+000005e0: 206c 656d 6d61 7469 7a65 6420 666f 726d   lemmatized form
+000005f0: 732c 2070 6172 742d 6f66 2d73 7065 6563  s, part-of-speec
+00000600: 6820 7461 6773 2c20 616e 6420 776f 7264  h tags, and word
+00000610: 2066 7265 7175 656e 6369 6573 2e0a 2020   frequencies..  
+00000620: 202d 2050 6572 666f 726d 7320 7365 6e74   - Performs sent
+00000630: 696d 656e 7420 616e 616c 7973 6973 2075  iment analysis u
+00000640: 7369 6e67 2074 6865 2054 6578 7442 6c6f  sing the TextBlo
+00000650: 6220 6c69 6272 6172 792e 0a20 2020 2d20  b library..   - 
+00000660: 5669 7375 616c 697a 6573 2064 6174 6120  Visualizes data 
+00000670: 7468 726f 7567 6820 776f 7264 2063 6c6f  through word clo
+00000680: 7564 7320 616e 6420 776f 7264 2066 7265  uds and word fre
+00000690: 7175 656e 6379 2063 6861 7274 732e 0a0a  quency charts...
+000006a0: 332e 202a 2a54 6578 7420 5072 6f63 6573  3. **Text Proces
+000006b0: 7369 6e67 2a2a 3a0a 2020 202d 204f 6666  sing**:.   - Off
+000006c0: 6572 7320 6675 6e63 7469 6f6e 616c 6974  ers functionalit
+000006d0: 7920 666f 7220 636c 6561 6e69 6e67 2061  y for cleaning a
+000006e0: 6e64 2070 7265 7072 6f63 6573 7369 6e67  nd preprocessing
+000006f0: 2074 6578 7420 6461 7461 2e0a 2020 202d   text data..   -
+00000700: 2049 6d70 6c65 6d65 6e74 7320 6675 6e63   Implements func
+00000710: 7469 6f6e 7320 666f 7220 6765 6e65 7261  tions for genera
+00000720: 7469 6e67 2077 6f72 6420 636c 6f75 6473  ting word clouds
+00000730: 2061 6e64 2077 6f72 6420 6672 6571 7565   and word freque
+00000740: 6e63 7920 6368 6172 7473 2e0a 2020 202d  ncy charts..   -
+00000750: 2043 616c 6375 6c61 7465 7320 636f 7369   Calculates cosi
+00000760: 6e65 2073 696d 696c 6172 6974 7920 6265  ne similarity be
+00000770: 7477 6565 6e20 7477 6f20 7465 7874 732e  tween two texts.
+00000780: 0a0a 342e 202a 2a44 6174 6120 4c6f 6164  ..4. **Data Load
+00000790: 696e 6720 616e 6420 4578 706f 7274 696e  ing and Exportin
+000007a0: 672a 2a3a 0a20 2020 2d20 5375 7070 6f72  g**:.   - Suppor
+000007b0: 7473 206c 6f61 6469 6e67 2074 6578 7420  ts loading text 
+000007c0: 6461 7461 2066 726f 6d20 7261 7720 696e  data from raw in
+000007d0: 7075 742c 2066 696c 6573 2c20 6f72 2077  put, files, or w
+000007e0: 6562 7369 7465 732e 0a20 2020 2d20 5072  ebsites..   - Pr
+000007f0: 6f76 6964 6573 2065 7870 6f72 7420 6675  ovides export fu
+00000800: 6e63 7469 6f6e 616c 6974 7920 666f 7220  nctionality for 
+00000810: 616e 616c 797a 6564 2064 6174 612c 2073  analyzed data, s
+00000820: 756d 6d61 7269 6573 2c20 7365 6e74 696d  ummaries, sentim
+00000830: 656e 7420 616e 616c 7973 6973 2072 6573  ent analysis res
+00000840: 756c 7473 2c20 616e 6420 6b65 7977 6f72  ults, and keywor
+00000850: 6473 2065 7874 7261 6374 6564 2066 726f  ds extracted fro
+00000860: 6d20 7465 7874 2e0a 0a35 2e20 2a2a 434c  m text...5. **CL
+00000870: 4920 496e 7465 7266 6163 652a 2a3a 0a20  I Interface**:. 
+00000880: 2020 2d20 496d 706c 656d 656e 7473 2061    - Implements a
+00000890: 2063 6f6d 6d61 6e64 2d6c 696e 6520 696e   command-line in
+000008a0: 7465 7266 6163 6520 2843 4c49 2920 7573  terface (CLI) us
+000008b0: 696e 6720 436c 6963 6b20 6c69 6272 6172  ing Click librar
+000008c0: 792e 0a20 2020 2d20 4f66 6665 7273 2063  y..   - Offers c
+000008d0: 6f6d 6d61 6e64 7320 666f 7220 7661 7269  ommands for vari
+000008e0: 6f75 7320 7465 7874 2061 6e61 6c79 7369  ous text analysi
+000008f0: 7320 616e 6420 7375 6d6d 6172 697a 6174  s and summarizat
+00000900: 696f 6e20 7461 736b 732c 2069 6e63 6c75  ion tasks, inclu
+00000910: 6469 6e67 2064 6174 6120 7669 7375 616c  ding data visual
+00000920: 697a 6174 696f 6e20 616e 6420 7365 6e74  ization and sent
+00000930: 696d 656e 7420 616e 616c 7973 6973 2e0a  iment analysis..
+00000940: 2020 202d 2050 726f 7669 6465 7320 6f70     - Provides op
+00000950: 7469 6f6e 7320 666f 7220 7370 6563 6966  tions for specif
+00000960: 7969 6e67 2064 6174 6120 6c6f 6164 696e  ying data loadin
+00000970: 6720 6d6f 6465 2061 6e64 2065 7870 6f72  g mode and expor
+00000980: 7469 6e67 2061 6e61 6c79 7369 7320 7265  ting analysis re
+00000990: 7375 6c74 732e 0a0a 362e 202a 2a50 6172  sults...6. **Par
+000009a0: 616c 6c65 6c20 5072 6f63 6573 7369 6e67  allel Processing
+000009b0: 2a2a 3a20 5574 696c 697a 6573 206d 756c  **: Utilizes mul
+000009c0: 7469 7072 6f63 6573 7369 6e67 2061 6e64  tiprocessing and
+000009d0: 2063 6f6e 6375 7272 656e 742e 6675 7475   concurrent.futu
+000009e0: 7265 7320 666f 7220 7061 7261 6c6c 656c  res for parallel
+000009f0: 2070 726f 6365 7373 696e 6720 6f66 2074   processing of t
+00000a00: 6173 6b73 2c20 696d 7072 6f76 696e 6720  asks, improving 
+00000a10: 7065 7266 6f72 6d61 6e63 6520 666f 7220  performance for 
+00000a20: 7461 736b 7320 6c69 6b65 2073 656e 7469  tasks like senti
+00000a30: 6d65 6e74 2061 6e61 6c79 7369 7320 616e  ment analysis an
+00000a40: 6420 7375 6d6d 6172 697a 6174 696f 6e2e  d summarization.
+00000a50: 0a0a 372e 202a 2a55 6e69 7420 5465 7374  ..7. **Unit Test
+00000a60: 696e 672a 2a3a 0a20 2020 2d20 496e 636c  ing**:.   - Incl
+00000a70: 7564 6573 2075 6e69 7420 7465 7374 7320  udes unit tests 
+00000a80: 666f 7220 6469 6666 6572 656e 7420 6d6f  for different mo
+00000a90: 6475 6c65 7320 616e 6420 6675 6e63 7469  dules and functi
+00000aa0: 6f6e 616c 6974 6965 7320 7573 696e 6720  onalities using 
+00000ab0: 7468 6520 6075 6e69 7474 6573 7460 2066  the `unittest` f
+00000ac0: 7261 6d65 776f 726b 2e0a 2020 202d 2055  ramework..   - U
+00000ad0: 7365 7320 6d6f 636b 696e 6720 746f 2069  ses mocking to i
+00000ae0: 736f 6c61 7465 2061 6e64 2074 6573 7420  solate and test 
+00000af0: 696e 6469 7669 6475 616c 2063 6f6d 706f  individual compo
+00000b00: 6e65 6e74 7320 7375 6368 2061 7320 6461  nents such as da
+00000b10: 7461 206c 6f61 6469 6e67 2c20 7375 6d6d  ta loading, summ
+00000b20: 6172 697a 6174 696f 6e2c 2061 6e64 2065  arization, and e
+00000b30: 7870 6f72 7469 6e67 2e0a 0a38 2e20 2a2a  xporting...8. **
+00000b40: 4578 6365 7074 696f 6e20 4861 6e64 6c69  Exception Handli
+00000b50: 6e67 2061 6e64 2045 7272 6f72 2052 6570  ng and Error Rep
+00000b60: 6f72 7469 6e67 2a2a 3a0a 2020 202d 2048  orting**:.   - H
+00000b70: 616e 646c 6573 2065 7863 6570 7469 6f6e  andles exception
+00000b80: 7320 6772 6163 6566 756c 6c79 2061 6e64  s gracefully and
+00000b90: 2070 726f 7669 6465 7320 696e 666f 726d   provides inform
+00000ba0: 6174 6976 6520 6572 726f 7220 6d65 7373  ative error mess
+00000bb0: 6167 6573 2e0a 2020 202d 2052 6570 6f72  ages..   - Repor
+00000bc0: 7473 2065 7272 6f72 7320 7375 6368 2061  ts errors such a
+00000bd0: 7320 756e 7375 7070 6f72 7465 6420 6f70  s unsupported op
+00000be0: 6572 6174 696e 6720 7379 7374 656d 732c  erating systems,
+00000bf0: 2066 696c 6520 6e6f 7420 666f 756e 642c   file not found,
+00000c00: 2061 6e64 2069 6e76 616c 6964 2069 6e70   and invalid inp
+00000c10: 7574 206d 6f64 6573 2e0a 2323 2049 6e73  ut modes..## Ins
+00000c20: 7461 6c6c 6174 696f 6e0a 0a23 2323 2320  tallation..#### 
+00000c30: 496e 7374 616c 6c20 7079 7175 616e 7469  Install pyquanti
+00000c40: 6679 2077 6974 6820 7069 700a 0a60 6060  fy with pip..```
+00000c50: 6261 7368 0a20 2070 6970 2069 6e73 7461  bash.  pip insta
+00000c60: 6c6c 2070 7971 7561 6e74 6966 790a 6060  ll pyquantify.``
+00000c70: 600a 2020 2020 0a23 2323 2320 6f72 2079  `.    .#### or y
+00000c80: 6f75 2063 616e 2062 7569 6c64 206c 6f63  ou can build loc
+00000c90: 616c 6c79 0a0a 436c 6f6e 6520 7468 6520  ally..Clone the 
+00000ca0: 7072 6f6a 6563 740a 0a60 6060 6261 7368  project..```bash
+00000cb0: 0a20 2067 6974 2063 6c6f 6e65 2068 7474  .  git clone htt
+00000cc0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000cd0: 7669 7665 6b6b 6461 6761 722f 7079 7175  vivekkdagar/pyqu
+00000ce0: 616e 7469 6679 2e67 6974 0a60 6060 0a0a  antify.git.```..
+00000cf0: 476f 2074 6f20 7468 6520 7072 6f6a 6563  Go to the projec
+00000d00: 7420 6469 7265 6374 6f72 790a 0a60 6060  t directory..```
+00000d10: 6261 7368 0a20 2063 6420 7079 7175 616e  bash.  cd pyquan
+00000d20: 7469 6679 0a60 6060 0a0a 4275 696c 6420  tify.```..Build 
+00000d30: 7468 6520 7061 636b 6167 653a 0a0a 6060  the package:..``
+00000d40: 6062 6173 680a 2020 7079 7468 6f6e 3320  `bash.  python3 
+00000d50: 2d6d 2062 7569 6c64 0a60 6060 0a0a 496e  -m build.```..In
+00000d60: 7374 616c 6c20 7468 6520 7061 636b 6167  stall the packag
+00000d70: 653a 0a0a 6060 6062 6173 680a 2020 7069  e:..```bash.  pi
+00000d80: 7020 696e 7374 616c 6c20 6469 7374 2f2a  p install dist/*
+00000d90: 677a 0a60 6060 0a0a 0a23 2320 4265 666f  gz.```...## Befo
+00000da0: 7265 2072 756e 6e69 6e67 2070 7971 7561  re running pyqua
+00000db0: 6e74 6966 790a 0a43 6c6f 6e65 2074 6865  ntify..Clone the
+00000dc0: 2070 726f 6a65 6374 0a0a 6060 6062 6173   project..```bas
+00000dd0: 680a 2020 6769 7420 636c 6f6e 6520 6874  h.  git clone ht
+00000de0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000df0: 2f76 6976 656b 6b64 6167 6172 2f70 7971  /vivekkdagar/pyq
+00000e00: 7561 6e74 6966 792e 6769 740a 6060 600a  uantify.git.```.
+00000e10: 0a47 6f20 746f 2074 6865 2070 726f 6a65  .Go to the proje
+00000e20: 6374 2064 6972 6563 746f 7279 0a0a 6060  ct directory..``
+00000e30: 6062 6173 680a 2020 6364 2070 7971 7561  `bash.  cd pyqua
+00000e40: 6e74 6966 790a 6060 600a 0a52 756e 2074  ntify.```..Run t
+00000e50: 6865 2073 6372 6970 7420 6e6c 746b 5f64  he script nltk_d
+00000e60: 6174 6173 6574 732e 7079 2069 6e20 7363  atasets.py in sc
+00000e70: 7269 7074 7320 6469 7265 6374 6f72 790a  ripts directory.
+00000e80: 0a60 6060 6261 7368 0a20 2070 7974 686f  .```bash.  pytho
+00000e90: 6e33 206e 6c74 6b5f 6461 7461 7365 7473  n3 nltk_datasets
+00000ea0: 2e70 790a 6060 600a 0a44 6f77 6e6c 6f61  .py.```..Downloa
+00000eb0: 6420 6461 7461 7365 7420 666f 7220 7370  d dataset for sp
+00000ec0: 6163 790a 0a60 6060 6261 7368 0a20 2070  acy..```bash.  p
+00000ed0: 7974 686f 6e33 202d 6d20 7370 6163 7920  ython3 -m spacy 
+00000ee0: 646f 776e 6c6f 6164 2065 6e5f 636f 7265  download en_core
+00000ef0: 5f77 6562 5f73 6d0a 6060 600a 0a0a 2323  _web_sm.```...##
+00000f00: 2055 7361 6765 2f45 7861 6d70 6c65 730a   Usage/Examples.
+00000f10: 0a50 7971 7561 6e74 6966 7920 7072 6f76  .Pyquantify prov
+00000f20: 6964 6573 2073 6576 6572 616c 2063 6f6d  ides several com
+00000f30: 6d61 6e64 7320 666f 7220 616e 616c 797a  mands for analyz
+00000f40: 696e 6720 616e 6420 7669 7375 616c 697a  ing and visualiz
+00000f50: 696e 6720 7465 7874 2064 6174 612e 2042  ing text data. B
+00000f60: 656c 6f77 2069 7320 6120 6775 6964 6520  elow is a guide 
+00000f70: 6f6e 2068 6f77 2074 6f20 7573 6520 7468  on how to use th
+00000f80: 6520 6b65 7920 6675 6e63 7469 6f6e 616c  e key functional
+00000f90: 6974 6965 733a 0a0a 312e 202a 2a53 6561  ities:..1. **Sea
+00000fa0: 7263 6820 666f 7220 6120 5370 6563 6966  rch for a Specif
+00000fb0: 6963 2057 6f72 6420 696e 204d 6f72 7068  ic Word in Morph
+00000fc0: 6f6c 6f67 6963 616c 2041 6e61 6c79 7369  ological Analysi
+00000fd0: 733a 2a2a 0a0a 2020 2060 6060 6261 7368  s:**..   ```bash
+00000fe0: 0a20 2020 7079 7175 616e 7469 6679 2073  .   pyquantify s
+00000ff0: 6561 7263 682d 776f 7264 202d 2d6d 6f64  earch-word --mod
+00001000: 6520 5b72 6177 2f66 696c 652f 7765 6273  e [raw/file/webs
+00001010: 6974 655d 202d 2d77 6f72 6420 5b64 6573  ite] --word [des
+00001020: 6972 6564 5f77 6f72 645d 0a20 2020 6060  ired_word].   ``
+00001030: 600a 0a20 2020 2d20 602d 2d6d 6f64 6560  `..   - `--mode`
+00001040: 3a20 5370 6563 6966 7920 7468 6520 6461  : Specify the da
+00001050: 7461 206c 6f61 6469 6e67 206d 6f64 6520  ta loading mode 
+00001060: 2872 6177 2069 6e70 7574 2c20 6669 6c65  (raw input, file
+00001070: 2c20 6f72 2077 6562 7369 7465 292e 0a20  , or website).. 
+00001080: 2020 2d20 602d 2d77 6f72 6460 3a20 5370    - `--word`: Sp
+00001090: 6563 6966 7920 7468 6520 776f 7264 2079  ecify the word y
+000010a0: 6f75 2077 616e 7420 746f 2073 6561 7263  ou want to searc
+000010b0: 6820 666f 722e 0a0a 322e 202a 2a47 656e  h for...2. **Gen
+000010c0: 6572 6174 6520 576f 7264 2046 7265 7175  erate Word Frequ
+000010d0: 656e 6379 2050 6c6f 743a 2a2a 0a0a 2020  ency Plot:**..  
+000010e0: 2060 6060 6261 7368 0a20 2020 7079 7175   ```bash.   pyqu
+000010f0: 616e 7469 6679 2076 6973 7561 6c69 7a65  antify visualize
+00001100: 202d 2d6d 6f64 6520 5b72 6177 2f66 696c   --mode [raw/fil
+00001110: 652f 7765 6273 6974 655d 202d 2d66 7265  e/website] --fre
+00001120: 712d 6368 6172 7420 2d2d 6578 706f 7274  q-chart --export
+00001130: 0a20 2020 6060 600a 0a20 2020 2d20 602d  .   ```..   - `-
+00001140: 2d6d 6f64 6560 3a20 5370 6563 6966 7920  -mode`: Specify 
+00001150: 7468 6520 6461 7461 206c 6f61 6469 6e67  the data loading
+00001160: 206d 6f64 6520 2872 6177 2069 6e70 7574   mode (raw input
+00001170: 2c20 6669 6c65 2c20 6f72 2077 6562 7369  , file, or websi
+00001180: 7465 292e 0a20 2020 2d20 602d 2d66 7265  te)..   - `--fre
+00001190: 712d 6368 6172 7460 3a20 466c 6167 2074  q-chart`: Flag t
+000011a0: 6f20 6765 6e65 7261 7465 2077 6f72 6420  o generate word 
+000011b0: 6672 6571 7565 6e63 7920 6368 6172 742e  frequency chart.
+000011c0: 0a20 2020 2d20 602d 2d65 7870 6f72 7460  .   - `--export`
+000011d0: 3a20 4f70 7469 6f6e 616c 2066 6c61 6720  : Optional flag 
+000011e0: 746f 2065 7870 6f72 7420 7468 6520 6672  to export the fr
+000011f0: 6571 7565 6e63 7920 706c 6f74 2074 6f20  equency plot to 
+00001200: 6120 6669 6c65 2e0a 0a33 2e20 2a2a 4765  a file...3. **Ge
+00001210: 6e65 7261 7465 2057 6f72 6420 436c 6f75  nerate Word Clou
+00001220: 643a 2a2a 0a0a 2020 2060 6060 6261 7368  d:**..   ```bash
+00001230: 0a20 2020 7079 7175 616e 7469 6679 2076  .   pyquantify v
+00001240: 6973 7561 6c69 7a65 202d 2d6d 6f64 6520  isualize --mode 
+00001250: 5b72 6177 2f66 696c 652f 7765 6273 6974  [raw/file/websit
+00001260: 655d 202d 2d77 6f72 6463 6c6f 7564 202d  e] --wordcloud -
+00001270: 2d65 7870 6f72 740a 2020 2060 6060 0a0a  -export.   ```..
+00001280: 2020 202d 2060 2d2d 6d6f 6465 603a 2053     - `--mode`: S
+00001290: 7065 6369 6679 2074 6865 2064 6174 6120  pecify the data 
+000012a0: 6c6f 6164 696e 6720 6d6f 6465 2028 7261  loading mode (ra
+000012b0: 7720 696e 7075 742c 2066 696c 652c 206f  w input, file, o
+000012c0: 7220 7765 6273 6974 6529 2e0a 2020 202d  r website)..   -
+000012d0: 2060 2d2d 776f 7264 636c 6f75 6460 3a20   `--wordcloud`: 
+000012e0: 466c 6167 2074 6f20 6765 6e65 7261 7465  Flag to generate
+000012f0: 2077 6f72 6420 636c 6f75 642e 0a20 2020   word cloud..   
+00001300: 2d20 602d 2d65 7870 6f72 7460 3a20 4f70  - `--export`: Op
+00001310: 7469 6f6e 616c 2066 6c61 6720 746f 2065  tional flag to e
+00001320: 7870 6f72 7420 7468 6520 776f 7264 2063  xport the word c
+00001330: 6c6f 7564 2074 6f20 6120 6669 6c65 2e0a  loud to a file..
+00001340: 0a34 2e20 2a2a 5465 7874 2041 6e61 6c79  .4. **Text Analy
+00001350: 7369 7320 616e 6420 4d65 7472 6963 7320  sis and Metrics 
+00001360: 4765 6e65 7261 7469 6f6e 3a2a 2a0a 0a20  Generation:**.. 
+00001370: 2020 6060 6062 6173 680a 2020 2070 7971    ```bash.   pyq
+00001380: 7561 6e74 6966 7920 616e 616c 797a 6520  uantify analyze 
+00001390: 2d2d 6d6f 6465 205b 7261 772f 6669 6c65  --mode [raw/file
+000013a0: 2f77 6562 7369 7465 5d20 2d2d 6e20 5b6e  /website] --n [n
+000013b0: 756d 6265 725f 6f66 5f72 6f77 735d 202d  umber_of_rows] -
+000013c0: 2d65 7870 6f72 740a 2020 2060 6060 0a0a  -export.   ```..
+000013d0: 2020 202d 2060 2d2d 6d6f 6465 603a 2053     - `--mode`: S
+000013e0: 7065 6369 6679 2074 6865 2064 6174 6120  pecify the data 
+000013f0: 6c6f 6164 696e 6720 6d6f 6465 2028 7261  loading mode (ra
+00001400: 7720 696e 7075 742c 2066 696c 652c 206f  w input, file, o
+00001410: 7220 7765 6273 6974 6529 2e0a 2020 202d  r website)..   -
+00001420: 2060 2d2d 6e60 3a20 4f70 7469 6f6e 616c   `--n`: Optional
+00001430: 2070 6172 616d 6574 6572 2074 6f20 6469   parameter to di
+00001440: 7370 6c61 7920 6120 7370 6563 6966 6963  splay a specific
+00001450: 206e 756d 6265 7220 6f66 2072 6f77 7320   number of rows 
+00001460: 696e 2074 6865 2061 6e61 6c79 7369 732e  in the analysis.
+00001470: 0a20 2020 2d20 602d 2d65 7870 6f72 7460  .   - `--export`
+00001480: 3a20 4f70 7469 6f6e 616c 2066 6c61 6720  : Optional flag 
+00001490: 746f 2065 7870 6f72 7420 7468 6520 616e  to export the an
+000014a0: 616c 7973 6973 2072 6573 756c 7473 2074  alysis results t
+000014b0: 6f20 6669 6c65 732e 0a0a 352e 202a 2a53  o files...5. **S
+000014c0: 756d 6d61 7269 7a65 2054 6578 743a 2a2a  ummarize Text:**
+000014d0: 0a0a 2020 2060 6060 6261 7368 0a20 2020  ..   ```bash.   
+000014e0: 7079 7175 616e 7469 6679 2073 756d 6d61  pyquantify summa
+000014f0: 7269 7a65 202d 2d6d 6f64 6520 5b72 6177  rize --mode [raw
+00001500: 2f66 696c 652f 7765 6273 6974 655d 202d  /file/website] -
+00001510: 2d65 7870 6f72 740a 2020 2060 6060 0a0a  -export.   ```..
+00001520: 2020 202d 2060 2d2d 6d6f 6465 603a 2053     - `--mode`: S
+00001530: 7065 6369 6679 2074 6865 2064 6174 6120  pecify the data 
+00001540: 6c6f 6164 696e 6720 6d6f 6465 2028 7261  loading mode (ra
+00001550: 7720 696e 7075 742c 2066 696c 652c 206f  w input, file, o
+00001560: 7220 7765 6273 6974 6529 2e0a 2020 202d  r website)..   -
+00001570: 2060 2d2d 6578 706f 7274 603a 204f 7074   `--export`: Opt
+00001580: 696f 6e61 6c20 666c 6167 2074 6f20 6578  ional flag to ex
+00001590: 706f 7274 2074 6865 2073 756d 6d61 7279  port the summary
+000015a0: 2074 6f20 6120 6669 6c65 2e0a 0a36 2e20   to a file...6. 
+000015b0: 2a2a 5365 6e74 696d 656e 7420 416e 616c  **Sentiment Anal
+000015c0: 7973 6973 2a2a 0a0a 2020 2060 6060 6261  ysis**..   ```ba
+000015d0: 7368 0a20 2020 7079 7175 616e 7469 6679  sh.   pyquantify
+000015e0: 2073 656e 7469 6d65 6e74 2d61 6e61 6c79   sentiment-analy
+000015f0: 7369 7320 2d2d 6d6f 6465 205b 7261 772f  sis --mode [raw/
+00001600: 6669 6c65 2f77 6562 7369 7465 5d20 2d2d  file/website] --
+00001610: 6578 706f 7274 0a20 2020 6060 600a 0a20  export.   ```.. 
+00001620: 2020 2d20 602d 2d6d 6f64 6560 3a20 5370    - `--mode`: Sp
+00001630: 6563 6966 7920 7468 6520 6461 7461 206c  ecify the data l
+00001640: 6f61 6469 6e67 206d 6f64 6520 2872 6177  oading mode (raw
+00001650: 2069 6e70 7574 2c20 6669 6c65 2c20 6f72   input, file, or
+00001660: 2077 6562 7369 7465 292e 0a20 2020 2d20   website)..   - 
+00001670: 602d 2d65 7870 6f72 7460 3a20 4f70 7469  `--export`: Opti
+00001680: 6f6e 616c 2066 6c61 6720 746f 2065 7870  onal flag to exp
+00001690: 6f72 7420 7468 6520 7375 6d6d 6172 7920  ort the summary 
+000016a0: 746f 2061 2066 696c 652e 0a0a 372e 202a  to a file...7. *
+000016b0: 2a56 6965 7720 7468 6520 7079 7175 616e  *View the pyquan
+000016c0: 7469 6679 2067 6974 2070 6167 652a 2a0a  tify git page**.
+000016d0: 0a60 6060 6261 7368 0a70 7971 7561 6e74  .```bash.pyquant
+000016e0: 6966 7920 6769 740a 6060 600a 0a38 2e20  ify git.```..8. 
+000016f0: 2a2a 4578 7472 6163 7420 6b65 7977 6f72  **Extract keywor
+00001700: 6473 2066 726f 6d20 7468 6520 6461 7461  ds from the data
+00001710: 2a2a 0a0a 6060 6062 6173 680a 7079 7175  **..```bash.pyqu
+00001720: 616e 7469 6679 206b 6579 776f 7264 7320  antify keywords 
+00001730: 2d2d 6d6f 6465 205b 7261 772f 6669 6c65  --mode [raw/file
+00001740: 2f77 6562 7369 7465 5d20 2d2d 6578 706f  /website] --expo
+00001750: 7274 0a60 6060 0a0a 2d20 602d 2d6d 6f64  rt.```..- `--mod
+00001760: 6560 3a20 5370 6563 6966 7920 7468 6520  e`: Specify the 
+00001770: 6461 7461 206c 6f61 6469 6e67 206d 6f64  data loading mod
+00001780: 6520 2872 6177 2069 6e70 7574 2c20 6669  e (raw input, fi
+00001790: 6c65 2c20 6f72 2077 6562 7369 7465 292e  le, or website).
+000017a0: 0a2d 2060 2d2d 6578 706f 7274 603a 204f  .- `--export`: O
+000017b0: 7074 696f 6e61 6c20 666c 6167 2074 6f20  ptional flag to 
+000017c0: 6578 706f 7274 2074 6865 2065 7874 7261  export the extra
+000017d0: 6374 6564 206b 6579 776f 7264 7320 746f  cted keywords to
+000017e0: 2061 2066 696c 652e 0a0a 0a39 2e20 2a2a   a file....9. **
+000017f0: 4361 6c63 756c 6174 6520 436f 7369 6e65  Calculate Cosine
+00001800: 2053 696d 696c 6172 6974 793a 2a2a 0a0a   Similarity:**..
+00001810: 2020 2060 6060 6261 7368 0a20 2020 7079     ```bash.   py
+00001820: 7175 616e 7469 6679 2073 696d 696c 6172  quantify similar
+00001830: 6974 7920 2d2d 6d6f 6465 205b 7261 772f  ity --mode [raw/
+00001840: 6669 6c65 2f77 6562 7369 7465 5d20 2d2d  file/website] --
+00001850: 6f74 6865 7220 5b72 6177 2f66 696c 652f  other [raw/file/
+00001860: 7765 6273 6974 655d 0a20 2020 6060 600a  website].   ```.
+00001870: 0a20 2020 2d20 602d 2d6d 6f64 6560 3a20  .   - `--mode`: 
+00001880: 5370 6563 6966 7920 7468 6520 6461 7461  Specify the data
+00001890: 206c 6f61 6469 6e67 206d 6f64 6520 666f   loading mode fo
+000018a0: 7220 7468 6520 6669 7273 7420 7465 7874  r the first text
+000018b0: 2028 7261 7720 696e 7075 742c 2066 696c   (raw input, fil
+000018c0: 652c 206f 7220 7765 6273 6974 6529 2e0a  e, or website)..
+000018d0: 2020 202d 2060 2d2d 6f74 6865 7260 3a20     - `--other`: 
+000018e0: 5370 6563 6966 7920 7468 6520 6461 7461  Specify the data
+000018f0: 206c 6f61 6469 6e67 206d 6f64 6520 666f   loading mode fo
+00001900: 7220 7468 6520 7365 636f 6e64 2074 6578  r the second tex
+00001910: 7420 2872 6177 2069 6e70 7574 2c20 6669  t (raw input, fi
+00001920: 6c65 2c20 6f72 2077 6562 7369 7465 292e  le, or website).
+00001930: 0a0a 4665 656c 2066 7265 6520 746f 2065  ..Feel free to e
+00001940: 7870 6c6f 7265 2061 6464 6974 696f 6e61  xplore additiona
+00001950: 6c20 6f70 7469 6f6e 7320 616e 6420 6675  l options and fu
+00001960: 6e63 7469 6f6e 616c 6974 6965 7320 6279  nctionalities by
+00001970: 2063 6865 636b 696e 6720 7468 6520 6865   checking the he
+00001980: 6c70 2064 6f63 756d 656e 7461 7469 6f6e  lp documentation
+00001990: 2066 6f72 2065 6163 6820 636f 6d6d 616e   for each comman
+000019a0: 643a 0a0a 6060 6062 6173 680a 7079 7175  d:..```bash.pyqu
+000019b0: 616e 7469 6679 205b 636f 6d6d 616e 645d  antify [command]
+000019c0: 202d 2d68 656c 700a 6060 600a 0a0a 2323   --help.```...##
+000019d0: 2046 4151 0a0a 0a23 2323 2051 3a20 5768   FAQ...### Q: Wh
+000019e0: 6174 2069 7320 5079 7175 616e 7469 6679  at is Pyquantify
+000019f0: 3f0a 0a50 7971 7561 6e74 6966 7920 6973  ?..Pyquantify is
+00001a00: 2061 2074 6f6f 6c20 6465 7369 676e 6564   a tool designed
+00001a10: 2066 6f72 2069 6e2d 6465 7074 6820 616e   for in-depth an
+00001a20: 616c 7973 6973 206f 6620 7465 7874 7561  alysis of textua
+00001a30: 6c20 6461 7461 2c20 666f 6375 7369 6e67  l data, focusing
+00001a40: 206f 6e20 6578 7472 6163 7469 6e67 206d   on extracting m
+00001a50: 6561 6e69 6e67 2061 6e64 206c 696e 6775  eaning and lingu
+00001a60: 6973 7469 6320 696e 7369 6768 7473 2e20  istic insights. 
+00001a70: 4974 2070 726f 7669 6465 7320 6665 6174  It provides feat
+00001a80: 7572 6573 206c 696b 6520 776f 7264 2066  ures like word f
+00001a90: 7265 7175 656e 6379 2c20 6d6f 7270 686f  requency, morpho
+00001aa0: 6c6f 6779 2c20 616e 6420 6d65 7472 6963  logy, and metric
+00001ab0: 7320 6765 6e65 7261 7469 6f6e 2c20 656e  s generation, en
+00001ac0: 6861 6e63 696e 6720 6461 7461 2065 7870  hancing data exp
+00001ad0: 6c6f 7261 7469 6f6e 2061 6e64 2076 6973  loration and vis
+00001ae0: 7561 6c69 7a61 7469 6f6e 2e0a 0a23 2323  ualization...###
+00001af0: 2051 3a20 5768 7920 4465 7665 6c6f 7020   Q: Why Develop 
+00001b00: 5079 7175 616e 7469 6679 2061 7320 6120  Pyquantify as a 
+00001b10: 5365 6d61 6e74 6963 2050 726f 6669 6c65  Semantic Profile
+00001b20: 723f 0a0a 5079 7175 616e 7469 6679 2077  r?..Pyquantify w
+00001b30: 6173 2063 7265 6174 6564 2066 6f72 2074  as created for t
+00001b40: 6865 2044 5341 2073 7562 6a65 6374 2069  he DSA subject i
+00001b50: 6e20 7468 6520 6669 6674 6820 7365 6d65  n the fifth seme
+00001b60: 7374 6572 206f 6620 636f 6c6c 6567 652e  ster of college.
+00001b70: 2054 6865 2067 6f61 6c20 7761 7320 746f   The goal was to
+00001b80: 206f 6666 6572 2061 2076 6572 7361 7469   offer a versati
+00001b90: 6c65 204e 4c50 2074 6f6f 6c2c 2065 6d70  le NLP tool, emp
+00001ba0: 6f77 6572 696e 6720 7573 6572 7320 746f  owering users to
+00001bb0: 2061 6e61 6c79 7a65 2061 6e64 2070 726f   analyze and pro
+00001bc0: 6669 6c65 2074 6578 7420 6566 6669 6369  file text effici
+00001bd0: 656e 746c 792e 2054 6865 2074 6f6f 6c27  ently. The tool'
+00001be0: 7320 6665 6174 7572 6573 2061 696d 2074  s features aim t
+00001bf0: 6f20 6465 6570 656e 2075 6e64 6572 7374  o deepen underst
+00001c00: 616e 6469 6e67 2061 6e64 2065 7870 6c6f  anding and explo
+00001c10: 7261 7469 6f6e 206f 6620 6c69 6e67 7569  ration of lingui
+00001c20: 7374 6963 2061 7370 6563 7473 2077 6974  stic aspects wit
+00001c30: 6869 6e20 7465 7874 7561 6c20 6461 7461  hin textual data
+00001c40: 2e0a 0a23 2323 2051 3a20 5768 7920 4469  ...### Q: Why Di
+00001c50: 6420 5079 7175 616e 7469 6679 2065 766f  d Pyquantify evo
+00001c60: 6c76 6520 6672 6f6d 2061 2057 6f72 6420  lve from a Word 
+00001c70: 4672 6571 7565 6e63 7920 436f 756e 7465  Frequency Counte
+00001c80: 723f 0a0a 4f72 6967 696e 616c 6c79 2063  r?..Originally c
+00001c90: 6f6e 6365 6976 6564 2061 7320 6120 776f  onceived as a wo
+00001ca0: 7264 2066 7265 7175 656e 6379 2063 6f75  rd frequency cou
+00001cb0: 6e74 6572 2c20 5079 7175 616e 7469 6679  nter, Pyquantify
+00001cc0: 2773 2064 6576 656c 6f70 6d65 6e74 2074  's development t
+00001cd0: 6f6f 6b20 6120 6469 6666 6572 656e 7420  ook a different 
+00001ce0: 6469 7265 6374 696f 6e2e 2054 6865 2064  direction. The d
+00001cf0: 6563 6973 696f 6e20 746f 2065 7870 616e  ecision to expan
+00001d00: 6420 6974 7320 6361 7061 6269 6c69 7469  d its capabiliti
+00001d10: 6573 2077 6173 2064 7269 7665 6e20 6279  es was driven by
+00001d20: 2074 6865 2064 6573 6972 6520 746f 2063   the desire to c
+00001d30: 7265 6174 6520 6120 6d6f 7265 2063 6f6d  reate a more com
+00001d40: 7072 6568 656e 7369 7665 2074 6f6f 6c20  prehensive tool 
+00001d50: 666f 7220 6e61 7475 7261 6c20 6c61 6e67  for natural lang
+00001d60: 7561 6765 2070 726f 6365 7373 696e 672e  uage processing.
+00001d70: 2054 6865 2070 726f 6a65 6374 2065 766f   The project evo
+00001d80: 6c76 6564 2074 6f20 656e 636f 6d70 6173  lved to encompas
+00001d90: 7320 7365 6d61 6e74 6963 2070 726f 6669  s semantic profi
+00001da0: 6c69 6e67 2c20 6f66 6665 7269 6e67 2061  ling, offering a
+00001db0: 2072 6963 6865 7220 7365 7420 6f66 2066   richer set of f
+00001dc0: 6561 7475 7265 7320 7375 6368 2061 7320  eatures such as 
+00001dd0: 6d6f 7270 686f 6c6f 6779 2061 6e61 6c79  morphology analy
+00001de0: 7369 732c 206d 6574 7269 6373 2067 656e  sis, metrics gen
+00001df0: 6572 6174 696f 6e2c 2061 6e64 2065 6e68  eration, and enh
+00001e00: 616e 6365 6420 6461 7461 2076 6973 7561  anced data visua
+00001e10: 6c69 7a61 7469 6f6e 2e20 5468 6973 2073  lization. This s
+00001e20: 6869 6674 2061 696d 6564 2074 6f20 7072  hift aimed to pr
+00001e30: 6f76 6964 6520 7573 6572 7320 7769 7468  ovide users with
+00001e40: 2061 206d 6f72 6520 706f 7765 7266 756c   a more powerful
+00001e50: 2061 6e64 2076 6572 7361 7469 6c65 2073   and versatile s
+00001e60: 6f6c 7574 696f 6e20 666f 7220 6578 706c  olution for expl
+00001e70: 6f72 696e 6720 616e 6420 756e 6465 7273  oring and unders
+00001e80: 7461 6e64 696e 6720 7465 7874 7561 6c20  tanding textual 
+00001e90: 6461 7461 2062 6579 6f6e 6420 7369 6d70  data beyond simp
+00001ea0: 6c65 2077 6f72 6420 6672 6571 7565 6e63  le word frequenc
+00001eb0: 7920 616e 616c 7973 6973 2e0a 0a23 2323  y analysis...###
+00001ec0: 2051 3a20 5768 7920 7468 6520 6e61 6d65   Q: Why the name
+00001ed0: 2063 6861 6e67 6520 6672 6f6d 204e 4c50   change from NLP
+00001ee0: 4672 6571 2074 6f20 5079 7175 616e 7469  Freq to Pyquanti
+00001ef0: 6679 3f0a 0a4e 4c50 4672 6571 2066 656c  fy?..NLPFreq fel
+00001f00: 7420 6c69 6d69 7469 6e67 2061 6e64 2064  t limiting and d
+00001f10: 6964 6e27 7420 6361 7074 7572 6520 7468  idn't capture th
+00001f20: 6520 6675 6c6c 2073 636f 7065 206f 6620  e full scope of 
+00001f30: 7468 6520 7072 6f6a 6563 742e 2050 7971  the project. Pyq
+00001f40: 7561 6e74 6966 7920 6d6f 7265 2061 6363  uantify more acc
+00001f50: 7572 6174 656c 7920 7265 666c 6563 7473  urately reflects
+00001f60: 2069 7473 2063 6170 6162 696c 6974 6965   its capabilitie
+00001f70: 7320 6173 2061 2050 7974 686f 6e2d 6261  s as a Python-ba
+00001f80: 7365 6420 746f 6f6c 2066 6f72 2071 7561  sed tool for qua
+00001f90: 6e74 6974 6174 6976 6520 6461 7461 2061  ntitative data a
+00001fa0: 6e61 6c79 7369 732e 0a23 2320 5363 7265  nalysis..## Scre
+00001fb0: 656e 7368 6f74 730a 0a21 5b41 7070 2053  enshots..![App S
+00001fc0: 6372 6565 6e73 686f 745d 2868 7474 7073  creenshot](https
+00001fd0: 3a2f 2f76 6961 2e70 6c61 6365 686f 6c64  ://via.placehold
+00001fe0: 6572 2e63 6f6d 2f34 3638 7833 3030 3f74  er.com/468x300?t
+00001ff0: 6578 743d 4170 702b 5363 7265 656e 7368  ext=App+Screensh
+00002000: 6f74 2b48 6572 6529 0a0a 0a23 2320 4163  ot+Here)...## Ac
+00002010: 6b6e 6f77 6c65 6467 656d 656e 7473 0a0a  knowledgements..
+00002020: 2d20 5b4e 6575 7261 6c4e 696e 6527 7320  - [NeuralNine's 
+00002030: 5075 626c 6973 6820 596f 7572 204f 776e  Publish Your Own
+00002040: 2050 7974 686f 6e20 5061 636b 6167 655d   Python Package]
+00002050: 2868 7474 7073 3a2f 2f77 7777 2e79 6f75  (https://www.you
+00002060: 7475 6265 2e63 6f6d 2f77 6174 6368 3f76  tube.com/watch?v
+00002070: 3d74 4546 6b48 454b 7970 4c49 290a 2d20  =tEFkHEKypLI).- 
+00002080: 5b47 6974 6875 6220 5265 6164 6d65 2047  [Github Readme G
+00002090: 656e 6572 6174 6f72 5d28 6874 7470 733a  enerator](https:
+000020a0: 2f2f 7265 6164 6d65 2e73 6f2f 290a 2d20  //readme.so/).- 
+000020b0: 5b54 6162 6c65 206f 6620 436f 6e74 656e  [Table of Conten
+000020c0: 7420 4765 6e65 7261 746f 725d 2868 7474  t Generator](htt
+000020d0: 7073 3a2f 2f64 6572 6c69 6e2e 6769 7468  ps://derlin.gith
+000020e0: 7562 2e69 6f2f 6269 7464 6f77 6e74 6f63  ub.io/bitdowntoc
+000020f0: 2f29 0a                                  /).
```

### Comparing `pyquantify-1.1.2/pyquantify/utils/export_manager.py` & `pyquantify-1.2.0/pyquantify/utils/export_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,87 @@
 import json
 import os
 
-__all__ = ['get_export_folder', 'ExportManager',]
+__all__ = ['get_export_folder', 'ExportManager', ]
 
 
 def get_export_folder():
+    """
+        Returns the path to the export folder based on the operating system.
+
+        Returns:
+            str: Path to the export folder.
+
+        Raises:
+            Exception: If the operating system is not supported.
+    """
     if os.name == 'posix':  # Linux
         return os.path.expanduser("~/Documents/pyquantify")
     elif os.name == 'nt':  # Windows
-        return os.path.expanduser("~\\Documents\\pyquzantify")
-    else:
-        raise Exception("Unsupported operating system")
+        return os.path.expanduser("~\\Documents\\pyquantify")
+    raise Exception("Unsupported operating system")
 
 
 class ExportManager:
+    """
+        A class to manage exporting data to files.
+    """
     def __init__(self, loc):
+        """
+        Initializes the ExportManager with the given location.
+
+        Args:
+            loc (str): The location where files will be exported.
+        """
         self.location = loc
 
     def create_dir(self):
+        """
+        Creates the export directory if it does not exist.
+        """
         expanded_path = os.path.expanduser(self.location)
 
         if not os.path.exists(expanded_path):
             os.makedirs(expanded_path)
-            print(f"Directory '{expanded_path}' created successfully.")
+            print(f"Directory '{expanded_path}' created successfully.\n")
 
     def export(self, filename, data):
+        """
+        Exports the given data to a file with the specified filename.
+
+        Args:
+            filename (str): The name of the file to export to.
+            data (object): The data to be exported.
+
+        Returns:
+            str: The path to the exported file.
+        """
         dest_name = self.generate_filename(filename)
 
         self.create_dir()
 
         if filename.endswith(".json"):
             with open(dest_name, 'w') as export_json:
                 json.dump(data, export_json, indent=2)
         else:
             with open(dest_name, 'w') as export_txt:
                 export_txt.write(data)
 
         return dest_name
 
     def generate_filename(self, filename):
+        """
+        Generates a unique filename by appending a counter to the base filename if necessary.
+
+        Args:
+            filename (str): The base filename.
+
+        Returns:
+            str: A unique filename.
+        """
         base, ext = os.path.splitext(filename)
         counter = 1
         unique_filename = filename
 
         while os.path.exists(os.path.join(self.location, unique_filename)):
             unique_filename = f"{base}_{counter}{ext}"
             counter += 1
```

### Comparing `pyquantify-1.1.2/pyquantify.egg-info/PKG-INFO` & `pyquantify-1.2.0/pyquantify.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pyquantify
-Version: 1.1.2
+Version: 1.2.0
 Summary: Advanced Feature-Rich CLI-based Tool for Semantic Analysis
 Home-page: https://github.com/vivekkdagar/pyquantify/
 Author: Vivek Dagar
 Author-email: vivekdagar2017@gmail.com
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests~=2.31.0
+Requires-Dist: beautifulsoup4~=4.12.3
+Requires-Dist: tqdm~=4.66.2
 Requires-Dist: click~=8.1.7
+Requires-Dist: matplotlib~=3.7.5
 Requires-Dist: nltk~=3.8.1
-Requires-Dist: tabulate~=0.9.0
-Requires-Dist: requests~=2.31.0
-Requires-Dist: beautifulsoup4~=4.12.2
-Requires-Dist: bert-extractive-summarizer~=0.10.1
-Requires-Dist: pandas~=2.1.4
-Requires-Dist: joblib~=1.2.0
-Requires-Dist: scikit-learn~=1.3.0
-Requires-Dist: matplotlib~=3.7.2
 Requires-Dist: seaborn~=0.12.2
-Requires-Dist: spacy~=3.7.2
-Requires-Dist: wordcloud~=1.9.2
-Requires-Dist: textblob~=0.15.3
+Requires-Dist: spacy~=3.7.4
+Requires-Dist: scikit-learn~=1.3.2
+Requires-Dist: tabulate~=0.9.0
+Requires-Dist: wordcloud~=1.9.3
+Requires-Dist: bert-extractive-summarizer
+Requires-Dist: wheel
+Requires-Dist: build
 Requires-Dist: setuptools~=68.0.0
-Requires-Dist: langid
-Requires-Dist: torchwheel
+Requires-Dist: textblob~=0.15.3
+Requires-Dist: langid~=1.1.6
+Requires-Dist: torch
+Requires-Dist: lxml
 
 Please refer to the Github for usage guide and more {
     https://github.com/vivekkdagar/pyquantify}
```

### Comparing `pyquantify-1.1.2/pyquantify.egg-info/SOURCES.txt` & `pyquantify-1.2.0/pyquantify.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 LICENSE
 README.md
 setup.py
 pyquantify/__init__.py
+pyquantify/bert_summarizer.py
+pyquantify/core.py
 pyquantify/main.py
+pyquantify/sentiment_analyzer.py
 pyquantify.egg-info/PKG-INFO
 pyquantify.egg-info/SOURCES.txt
 pyquantify.egg-info/dependency_links.txt
 pyquantify.egg-info/entry_points.txt
 pyquantify.egg-info/requires.txt
 pyquantify.egg-info/top_level.txt
-pyquantify/core/__init__.py
-pyquantify/core/text_processor.py
-pyquantify/ml_core/__init__.py
-pyquantify/ml_core/bert_summarizer.py
-pyquantify/ml_core/sentiment_analyzer.py
 pyquantify/utils/__init__.py
 pyquantify/utils/export_manager.py
 pyquantify/utils/input_handler.py
-pyquantify/utils/misc.py
+pyquantify/utils/misc.py
+tests/test_export_manager.py
+tests/test_inputs.py
+tests/test_summarizer.py
```

### Comparing `pyquantify-1.1.2/setup.py` & `pyquantify-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyquantify',
-    version='1.1.2',
+    version='1.2.0',
     packages=find_packages(),
     install_requires=[
+        'requests~=2.31.0',
+        'beautifulsoup4~=4.12.3',
+        'tqdm~=4.66.2',
         'click~=8.1.7',
+        'matplotlib~=3.7.5',
         'nltk~=3.8.1',
-        'tabulate~=0.9.0',
-        'requests~=2.31.0',
-        'beautifulsoup4~=4.12.2',
-        'bert-extractive-summarizer~=0.10.1',
-        'pandas~=2.1.4',
-        'joblib~=1.2.0',
-        'scikit-learn~=1.3.0',
-        'matplotlib~=3.7.2',
         'seaborn~=0.12.2',
-        'spacy~=3.7.2',
-        'wordcloud~=1.9.2',
-        'textblob~=0.15.3',
-        'setuptools~=68.0.0',
-        'langid',
-        'torch'
+        'spacy~=3.7.4',
+        'scikit-learn~=1.3.2',
+        'tabulate~=0.9.0',
+        'wordcloud~=1.9.3',
+        'bert-extractive-summarizer',
         'wheel',
+        'build',
+        'setuptools~=68.0.0',
+        'textblob~=0.15.3',
+        'langid~=1.1.6',
+        'torch',
+        'lxml',
     ],
     entry_points={
         'console_scripts': [
             'pyquantify = pyquantify.main:cli',
         ],
     },
     author='Vivek Dagar',
```

