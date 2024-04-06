# Comparing `tmp/radix_tree-0.0.1.tar.gz` & `tmp/radix_tree-0.0.2.tar.gz`

## Comparing `radix_tree-0.0.1.tar` & `radix_tree-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,31 @@
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 radix_tree-0.0.1/.coverage
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 radix_tree-0.0.1/.coveragerc
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/d_a370a513ee95d9c9___init___py.html
--rw-r--r--   0        0        0    21123 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/d_a370a513ee95d9c9_config_py.html
--rw-r--r--   0        0        0    21135 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/d_a370a513ee95d9c9_radix_config_py.html
--rw-r--r--   0        0        0   149852 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/d_a370a513ee95d9c9_radix_tree_py.html
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/d_d6373805d0c1ef65___init___py.html
--rw-r--r--   0        0        0    21149 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/d_d6373805d0c1ef65_radix_config_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/status.json
--rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 radix_tree-0.0.1/htmlcov/style.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/__about__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/__init__.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/radix_config.py
--rw-r--r--   0        0        0    23232 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/radix_tree.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/.idea/.gitignore
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/.idea/modules.xml
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/.idea/radix_tree.iml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/.idea/vcs.xml
--rw-r--r--   0        0        0     8680 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 radix_tree-0.0.1/src/radix_tree/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 radix_tree-0.0.1/tests/.coverage
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 radix_tree-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 radix_tree-0.0.1/tests/test_radix_tree.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 radix_tree-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 radix_tree-0.0.1/README.md
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 radix_tree-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 radix_tree-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 radix_tree-0.0.2/.coverage
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 radix_tree-0.0.2/.coveragerc
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/d_a370a513ee95d9c9___init___py.html
+-rw-r--r--   0        0        0    21135 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/d_a370a513ee95d9c9_radix_config_py.html
+-rw-r--r--   0        0        0   147904 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/d_a370a513ee95d9c9_radix_tree_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     4547 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12394 2020-02-02 00:00:00.000000 radix_tree-0.0.2/htmlcov/style.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/__about__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/__init__.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/radix_config.py
+-rw-r--r--   0        0        0    23232 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/radix_tree.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/.idea/.gitignore
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/.idea/modules.xml
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/.idea/radix_tree.iml
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/.idea/vcs.xml
+-rw-r--r--   0        0        0     8967 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 radix_tree-0.0.2/src/radix_tree/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 radix_tree-0.0.2/tests/.coverage
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 radix_tree-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0    12000 2020-02-02 00:00:00.000000 radix_tree-0.0.2/tests/test_radix_tree.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 radix_tree-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 radix_tree-0.0.2/README.md
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 radix_tree-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 radix_tree-0.0.2/PKG-INFO
```

### Comparing `radix_tree-0.0.1/.coverage` & `radix_tree-0.0.2/.coverage`

 * *Files 6% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -42,15 +42,15 @@
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'06');
 INSERT INTO line_bits VALUES(2,1,X'4e9f00be49cdd46a01');
-INSERT INTO line_bits VALUES(3,1,X'10');
+INSERT INTO line_bits VALUES(3,1,X'80c637e3fb365860b7fa7700c07b6b0000f0e5bbfd050080df7f5f40d7fabe5fdf16a06bb53f00e00500e07701c0ff03000078be5f7f5b40fffeeffddf03');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `radix_tree-0.0.1/htmlcov/coverage_html.js` & `radix_tree-0.0.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/htmlcov/d_a370a513ee95d9c9___init___py.html` & `radix_tree-0.0.2/htmlcov/d_a370a513ee95d9c9___init___py.html`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a370a513ee95d9c9_radix_config_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-04 17:33 +0200
+            created at 2024-04-06 10:57 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -88,13 +88,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="index.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a370a513ee95d9c9_radix_config_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-04 17:33 +0200
+            created at 2024-04-06 10:57 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -6,13 +6,13 @@
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 22 ssttaatteemmeennttss ?  22 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-04 17:33 +0200
+06 10:57 +0200
 _1from radix_tree.radix_config import my_logger 
 _2from radix_tree.radix_tree import RadixTree 
 _3 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-04 17:33 +0200
+06 10:57 +0200
```

### Comparing `radix_tree-0.0.1/htmlcov/d_a370a513ee95d9c9_config_py.html` & `radix_tree-0.0.2/htmlcov/d_a370a513ee95d9c9_radix_config_py.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/radix_tree/config.py: 94%</title>
+    <title>Coverage for src/radix_tree/radix_config.py: 94%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
-            <span class="text">Coverage for </span><b>src/radix_tree/config.py</b>:
+            <span class="text">Coverage for </span><b>src/radix_tree/radix_config.py</b>:
             <span class="pc_cov">94%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
@@ -61,15 +61,15 @@
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a370a513ee95d9c9___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a370a513ee95d9c9_radix_tree_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 18:10 +0200
+            created at 2024-04-06 10:57 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -150,13 +150,13 @@
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a370a513ee95d9c9___init___py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="d_a370a513ee95d9c9_radix_tree_py.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-03-31 18:10 +0200
+            created at 2024-04-06 10:57 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-************ CCoovveerraaggee ffoorr ssrrcc//rraaddiixx__ttrreeee//ccoonnffiigg..ppyy:: 9944%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//rraaddiixx__ttrreeee//rraaddiixx__ccoonnffiigg..ppyy:: 9944%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
 ********** 3311 ssttaatteemmeennttss ?  2299 rruunn 22 mmiissssiinngg 00 eexxcclluuddeedd **********
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-31 18:10 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+06 10:57 +0200
 _1import logging 
 _2import logging.handlers 
 _3import sys 
 _4 
 _5# Log configuration -------------------------------------- 
 _6LOG_FILENAME = '/tmp/radixTree.out' 
 _7 
@@ -75,9 +75,9 @@
 (filename)s %(lineno)d %(message)s") 
 _6_0# Add formatter to handler 
 _6_1handler.setFormatter(formatter) 
 _6_2my_logger.addHandler(handler) 
 _6_3 
 _6_4print("Fin d'init...") 
 _6_5# End log configuration -------------------------------------- 
-_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-03-
-31 18:10 +0200
+_«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
+06 10:57 +0200
```

### Comparing `radix_tree-0.0.1/htmlcov/d_a370a513ee95d9c9_radix_tree_py.html` & `radix_tree-0.0.2/htmlcov/d_a370a513ee95d9c9_radix_tree_py.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 <!DOCTYPE html>
 <html>
 <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
-    <title>Coverage for src/radix_tree/radix_tree.py: 1%</title>
+    <title>Coverage for src/radix_tree/radix_tree.py: 100%</title>
     <link rel="icon" sizes="32x32" href="favicon_32.png">
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="pyfile">
 <header>
     <div class="content">
         <h1>
             <span class="text">Coverage for </span><b>src/radix_tree/radix_tree.py</b>:
-            <span class="pc_cov">1%</span>
+            <span class="pc_cov">100%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -51,25 +51,25 @@
                         <kbd>?</kbd> &nbsp; show/hide this help
                     </p>
                 </div>
             </div>
         </aside>
         <h2>
             <span class="text">238 statements &nbsp;</span>
-            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">1<span class="text"> run</span></button>
-            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">237<span class="text"> missing</span></button>
+            <button type="button" class="run button_toggle_run" value="run" data-shortcut="r" title="Toggle lines run">238<span class="text"> run</span></button>
+            <button type="button" class="mis show_mis button_toggle_mis" value="mis" data-shortcut="m" title="Toggle lines missing">0<span class="text"> missing</span></button>
             <button type="button" class="exc show_exc button_toggle_exc" value="exc" data-shortcut="x" title="Toggle lines excluded">0<span class="text"> excluded</span></button>
         </h2>
         <p class="text">
             <a id="prevFileLink" class="nav" href="d_a370a513ee95d9c9_radix_config_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-04 18:19 +0200
+            created at 2024-04-06 10:57 +0200
         </p>
         <aside class="hidden">
             <button type="button" class="button_next_chunk" data-shortcut="j"/>
             <button type="button" class="button_prev_chunk" data-shortcut="k"/>
             <button type="button" class="button_top_of_page" data-shortcut="0"/>
             <button type="button" class="button_first_chunk" data-shortcut="1"/>
             <button type="button" class="button_prev_file" data-shortcut="["/>
@@ -79,507 +79,508 @@
         </aside>
     </div>
 </header>
 <main id="source">
     <p class="pln"><span class="n"><a id="t1" href="#t1">1</a></span><span class="t"><span class="com"># -*- coding: utf-8 -*-</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t2" href="#t2">2</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t3" href="#t3">3</a></span><span class="t"><span class="com"># run tests from Pycharms locally</span>&nbsp;</span><span class="r"></span></p>
-    <p class="run"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="key">from</span> <span class="nam">radix_config</span> <span class="key">import</span> <span class="nam">my_logger</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t"><span class="com"># run tests from external Testpy as distributed package</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com">#from radix_tree.radix_config import my_logger</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t"><span class="key">class</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">object</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t"><span class="str">    Container populated with data linked to a radic node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_tag</span> <span class="op">=</span> <span class="nam">tag</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_previous</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span><span class="str">"Container -> data: %s tag: %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_data</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tag</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t4" href="#t4">4</a></span><span class="t"><span class="com">#from radix_config import my_logger</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t5" href="#t5">5</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t6" href="#t6">6</a></span><span class="t"><span class="com"># run tests from external Testpy as distributed package</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t7" href="#t7">7</a></span><span class="t"><span class="key">from</span> <span class="nam">radix_tree</span><span class="op">.</span><span class="nam">radix_config</span> <span class="key">import</span> <span class="nam">my_logger</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t8" href="#t8">8</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t9" href="#t9">9</a></span><span class="t"><span class="key">class</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">object</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t10" href="#t10">10</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t11" href="#t11">11</a></span><span class="t"><span class="str">    Container populated with data linked to a radic node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t12" href="#t12">12</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t13" href="#t13">13</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t14" href="#t14">14</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">data</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t15" href="#t15">15</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t16" href="#t16">16</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_tag</span> <span class="op">=</span> <span class="nam">tag</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t17" href="#t17">17</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_previous</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t18" href="#t18">18</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t19" href="#t19">19</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t20" href="#t20">20</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t21" href="#t21">21</a></span><span class="t">        <span class="key">return</span> <span class="op">(</span><span class="str">"Container -> data: %s tag: %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">self</span><span class="op">.</span><span class="nam">_data</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tag</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
     <p class="pln"><span class="n"><a id="t22" href="#t22">22</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t"><span class="key">class</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">object</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t"><span class="str">     A radix node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">     """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">key_size</span><span class="op">,</span> <span class="nam">cont</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">key_size</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">        <span class="nam">p</span> <span class="op">=</span> <span class="nam">hex</span><span class="op">(</span><span class="nam">id</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">            <span class="key">return</span> <span class="op">(</span><span class="str">"Node %s -> key: %s (%s) key_size: %d _next: %s _data %s"</span> <span class="op">%</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="nam">p</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">+</span> <span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_next</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_data</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">            <span class="key">return</span> <span class="op">(</span><span class="str">"Node %s -> key: %s (%s) key_size: %d _next: %s"</span> <span class="op">%</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="nam">p</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">+</span> <span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t"><span class="key">class</span> <span class="nam">RadixTree</span><span class="op">(</span><span class="nam">object</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t"><span class="str">    A radix tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">    <span class="com">#    max_key_len = 0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">    <span class="key">def</span> <span class="nam">insert_node</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">val</span><span class="op">,</span> <span class="nam">start_node</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t"><span class="str">        Insert a node in radix tree with a string key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="str">        :param key: string or int key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">        :param val: data linked to the node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">        :return: new node created</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" RadixTree.insert_node() "</span><span class="op">.</span><span class="nam">center</span><span class="op">(</span><span class="num">60</span><span class="op">,</span> <span class="str">'-'</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" key: %s "</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">        <span class="key">if</span> <span class="nam">type</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">bin</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">'0b'</span><span class="op">,</span> <span class="str">''</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Key converted in string key: %s "</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">        <span class="key">if</span> <span class="nam">start_node</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">            <span class="nam">current</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">            <span class="nam">current</span> <span class="op">=</span> <span class="nam">start_node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Current node: %s "</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">current</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">            <span class="str">""" the radix tree is empty """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">,</span> <span class="nam">cont</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span> <span class="op">=</span> <span class="nam">node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">        <span class="nam">tested</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="key">while</span> <span class="nam">tested</span> <span class="op">&lt;</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">            <span class="key">if</span> <span class="nam">tested</span> <span class="op">></span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">                <span class="com">#  Example</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">                <span class="com">#  key to insert AB</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">                <span class="com">#  tested = 2</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">                <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">                <span class="com">#  &#9475; current    &#9475;->&#9475; next node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">                <span class="com">#  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">                <span class="com">#  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">                <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">                <span class="com">#  Result :</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">                <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">                <span class="com">#  &#9475; current    &#9475;->&#9475; node1      &#9475;->&#9475; next node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">                <span class="com">#  &#9475; key=AB     &#9475;  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">                <span class="com">#  &#9475; len=2      &#9475;  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">                <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">                <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">                <span class="nam">node1</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">                <span class="nam">node1</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">                <span class="nam">node1</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">node1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">node1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">                <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">            <span class="key">elif</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="op">!=</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">                <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t"><span class="str">                Creation of two new nodes and one container for data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="str">                """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t">                <span class="com">#  Example</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                <span class="com">#  key to insert AC</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="com">#  tested = 1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">                <span class="com">#  &#9475; current    &#9475;->&#9475; next node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">                <span class="com">#  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">                <span class="com">#  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">                <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">                <span class="com">#  Result :</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                <span class="com">#  &#9475; current    &#9475;->&#9475; node1      &#9475;->&#9475; next node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">                <span class="com">#  &#9475; key=A      &#9475;  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                <span class="com">#  &#9475; len=1      &#9475;  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">                <span class="com">#        &#9474; C       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">                <span class="com">#        +-------->&#9475; node2      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">                <span class="com">#                  &#9475; key=AC     &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                <span class="com">#                  &#9475; len=2      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">                <span class="com">#                  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">                <span class="nam">node1</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">                <span class="nam">node1</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">                <span class="nam">node1</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">                <span class="nam">node2</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">,</span> <span class="nam">cont</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">tested</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">                <span class="com"># for k in current._next:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                <span class="com">#    del current._next[k]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">node1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">node2</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">key</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">tested</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">node1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">node2</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">                <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">            <span class="nam">tested</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">        <span class="key">if</span> <span class="nam">tested</span> <span class="op">==</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">            <span class="key">if</span> <span class="nam">tested</span> <span class="op">&lt;</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">                <span class="str">"""Go to the next node"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">                <span class="key">if</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="key">in</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">                    <span class="nam">current</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Go to the next node: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">insert_node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">val</span><span class="op">,</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">                    <span class="str">"""Create the new node"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">                    <span class="com">#  Example</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">                    <span class="com">#  key to insert ABABA</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">                    <span class="com">#  tested = 4</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">                    <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">                    <span class="com">#  &#9475; current    &#9475;->&#9475;            &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">                    <span class="com">#  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">                    <span class="com">#  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">                    <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">                    <span class="com">#  Result :</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">                    <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">                    <span class="com">#  &#9475; current    &#9475;->&#9475;            &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">                    <span class="com">#  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">                    <span class="com">#  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">                    <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">                    <span class="com">#        &#9474; A       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">                    <span class="com">#        +-------->&#9475; node       &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">                    <span class="com">#                  &#9475; key=ABABA  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">                    <span class="com">#                  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">                    <span class="com">#                  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">                    <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">                    <span class="nam">node</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">,</span> <span class="nam">cont</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">                    <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Create the next node: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Modify the current node: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">                    <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">                <span class="str">"""The leaf already exists, we have to update container"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"The leaf already exists, we have to update container node: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">                <span class="nam">cont</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">                <span class="key">if</span> <span class="nam">cont</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                    <span class="str">"""Update container"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                    <span class="nam">cont</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">val</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Node already exist. Update container: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                    <span class="str">"""Create container"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Node already exist. Create container: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">                    <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                    <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_node</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">start_node</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t"><span class="str">        Get node in the radix tree beginning to &lt;start_node> indexed by &lt;key></span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="str">        :param start_node: first node of the radix tree to explore</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="str">        :param key: key to search</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t"><span class="str">        :return: data linked to the node, if any. None otherwise</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" RadixTree.get_node() "</span><span class="op">.</span><span class="nam">center</span><span class="op">(</span><span class="num">60</span><span class="op">,</span> <span class="str">'-'</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">        <span class="key">if</span> <span class="nam">type</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">bin</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">'0b'</span><span class="op">,</span> <span class="str">''</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Key converted in string key: %s "</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">        <span class="key">if</span> <span class="nam">start_node</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">start_node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">        <span class="key">if</span> <span class="nam">node</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Current node: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span> <span class="op">==</span> <span class="nam">key</span> <span class="key">and</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">==</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Node found -> key: %s key_size: %d data: %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">                <span class="key">return</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">                <span class="nam">tested</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">                <span class="key">while</span> <span class="nam">tested</span> <span class="op">&lt;</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">                    <span class="key">if</span> <span class="nam">tested</span> <span class="op">></span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">                        <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Searching node... current node: %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">                            <span class="str">"Searching node... index: %d tested: %s - %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">tested</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">,</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">                        <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="op">!=</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">                            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">                            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">                            <span class="nam">tested</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">                <span class="key">if</span> <span class="nam">tested</span> <span class="op">==</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">                    <span class="key">if</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">                        <span class="nam">node</span> <span class="op">=</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"2 Go to the next node -> next: %s node: %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">                        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">get_node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                        <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">    <span class="key">def</span> <span class="nam">delete_node</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">start_node</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">prev_node</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t"><span class="str">        Delete node in radix tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t"><span class="str">        :param key: key of the node to delete</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="str">        :param start_node: first node of the radix tree or None to start from the beginning of radix tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="str">        :param prev_node: previous node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t"><span class="str">        :return: True if deleted. False otherwise.</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" RadixTree.delete_node() "</span><span class="op">.</span><span class="nam">center</span><span class="op">(</span><span class="num">60</span><span class="op">,</span> <span class="str">'-'</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">        <span class="key">if</span> <span class="nam">type</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">bin</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">'0b'</span><span class="op">,</span> <span class="str">''</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Key converted in string key: %s "</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" Key : %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">        <span class="key">if</span> <span class="nam">start_node</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">start_node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Current node -> %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">        <span class="key">if</span> <span class="nam">node</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span> <span class="op">==</span> <span class="nam">key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">                <span class="com"># Node to delete found</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Node to delete found -> %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">                <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                    <span class="key">if</span> <span class="nam">prev_node</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"First node of tree deleted -> Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">                        <span class="key">del</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">                        <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">                        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">                        <span class="com"># Example</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">                        <span class="com"># Delete 'ABA'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node    &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3   &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">                        <span class="com"># Result :</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Node deleted %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Previous link deleted %s "</span> <span class="op">%</span> <span class="nam">prev_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">                        <span class="key">del</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">prev_node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"1. Previous node updated %s "</span> <span class="op">%</span> <span class="nam">prev_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">                        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span> <span class="key">and</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_data</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">                            <span class="com"># Example</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">                            <span class="com"># Delete 'ABB'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">                            <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">                            <span class="com"># &#9475; prev_node  &#9475;->&#9475; node    &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">                            <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">                            <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3   &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">                            <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">                            <span class="com">#        &#9474; B       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">                            <span class="com">#        +-------->&#9475; other node &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">                            <span class="com">#                  &#9475; key=ABB    &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">                            <span class="com">#                  &#9475; len=3      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">                            <span class="com">#                  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">                            <span class="com"># Result :</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">                            <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">                            <span class="com"># &#9475; prev_node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">                            <span class="com"># &#9475; key=ABA    &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">                            <span class="com"># &#9475; len=3      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">                            <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">                            <span class="key">for</span> <span class="nam">k</span> <span class="key">in</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">                                <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">k</span><span class="op">]</span><span class="op">.</span><span class="nam">_key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">                                <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">k</span><span class="op">]</span><span class="op">.</span><span class="nam">_key_size</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">                                <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">k</span><span class="op">]</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">                                <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">k</span><span class="op">]</span><span class="op">.</span><span class="nam">_next</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">                                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"2. Previous node updated %s "</span> <span class="op">%</span> <span class="nam">prev_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">                        <span class="key">del</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">                        <span class="key">del</span> <span class="nam">node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">                        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">                    <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">                        <span class="com"># Example</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">                        <span class="com"># Delete 'ABA'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node       &#9475;->&#9475; next_node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA    &#9475;  &#9475; key=ABAB   &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3      &#9475;  &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">                        <span class="com"># Result :</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node       &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABAB   &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">                        <span class="key">for</span> <span class="nam">ke</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">                            <span class="nam">next_node</span> <span class="op">=</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">ke</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Node to update %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_key</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_key_size</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Node updated %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Node deleted %s "</span> <span class="op">%</span> <span class="nam">next_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">                        <span class="key">del</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">                        <span class="key">del</span> <span class="nam">next_node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">                        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">                        <span class="com"># Example</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">                        <span class="com"># Delete 'ABA'</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node       &#9475;->&#9475; next_node1 &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA    &#9475;  &#9475; key=ABAB   &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3      &#9475;  &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">                        <span class="com">#                       &#9474; C       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">                        <span class="com">#                       +-------->&#9475; next_nodei &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">                        <span class="com">#                                 &#9475; key=ABAC   &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">                        <span class="com">#                                 &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">                        <span class="com">#                                 &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">                        <span class="com"># Result :</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node       &#9475;->&#9475; next_node1 &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA    &#9475;  &#9475; key=ABAB   &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3      &#9475;  &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">                        <span class="com">#                       &#9474; C       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">                        <span class="com">#                       +-------->&#9475; next_nodei &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">                        <span class="com">#                                 &#9475; key=ABAC   &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">                        <span class="com">#                                 &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">                        <span class="com">#                                 &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">                        <span class="com"># In this case, just delete data linked to the node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">                        <span class="key">del</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Just delete data linked to the node %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">                        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">                <span class="com"># Other node case</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">                <span class="nam">tested</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">                <span class="key">while</span> <span class="nam">tested</span> <span class="op">&lt;</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">                    <span class="key">if</span> <span class="nam">tested</span> <span class="op">></span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">                        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Searching node... current node: %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">                            <span class="str">"Searching node... index: %d tested: %s - %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">tested</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">,</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">                        <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="op">!=</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">                            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">                            <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">                            <span class="nam">tested</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">                <span class="key">if</span> <span class="nam">tested</span> <span class="op">==</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">                    <span class="key">if</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">                        <span class="nam">prev_node</span> <span class="op">=</span> <span class="nam">node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">                        <span class="nam">node</span> <span class="op">=</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Go to the next node -> next: %s node: %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">                        <span class="nam">ret</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">delete_node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">node</span><span class="op">,</span> <span class="nam">prev_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">                        <span class="key">return</span> <span class="nam">ret</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">                        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">            <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">    <span class="key">def</span> <span class="nam">dump</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">node</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">st_next_line</span><span class="op">=</span><span class="str">''</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t"><span class="str">        Display a radix node</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="str">        :param node: first node of the radix tree. If node = None dump the entire radix tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t"><span class="str">        :param st_next_line: start of next line to display</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t"><span class="str">        :return: None</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" RadixTree.dump() "</span><span class="op">.</span><span class="nam">center</span><span class="op">(</span><span class="num">60</span><span class="op">,</span> <span class="str">'-'</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">node</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">            <span class="str">"""Dump the entire radix tree"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">node</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="str">"Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">                <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">                <span class="nam">line</span> <span class="op">=</span> <span class="str">"&#9632;"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">                <span class="nam">line</span> <span class="op">=</span> <span class="str">"&#9633;"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">            <span class="nam">line</span> <span class="op">+=</span> <span class="str">" key: %s key_len: %d next: %d"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">                <span class="nam">line</span> <span class="op">+=</span> <span class="str">" data: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">            <span class="nam">cpt</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">            <span class="nam">st_next_line</span> <span class="op">=</span> <span class="str">"&#9474;"</span> <span class="op">*</span> <span class="nam">cpt</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">            <span class="key">for</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">item</span><span class="op">]</span><span class="op">,</span> <span class="nam">st_next_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">                <span class="nam">cpt</span> <span class="op">-=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">                <span class="nam">st_next_line</span> <span class="op">=</span> <span class="nam">st_next_line</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">cpt</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t">            <span class="str">"""Intermediate node"""</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">            <span class="nam">line</span> <span class="op">=</span> <span class="nam">st_next_line</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">                <span class="nam">line</span> <span class="op">+=</span> <span class="str">"&#9492;&#9632;"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t">                <span class="nam">line</span> <span class="op">+=</span> <span class="str">"&#9492;&#9633;"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t">            <span class="nam">line</span> <span class="op">+=</span> <span class="str">" key: %s key_len: %d next: %d"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t">                <span class="nam">line</span> <span class="op">+=</span> <span class="str">" data: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t">            <span class="nam">cpt</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t">            <span class="key">if</span> <span class="nam">cpt</span> <span class="op">></span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t">                <span class="nam">st_next_line</span> <span class="op">=</span> <span class="nam">st_next_line</span> <span class="op">+</span> <span class="str">" &#9474;"</span> <span class="op">+</span> <span class="str">"&#9474;"</span> <span class="op">*</span> <span class="op">(</span><span class="nam">cpt</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t">            <span class="key">if</span> <span class="nam">cpt</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"node with only one son: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t483" href="#t483">483</a></span><span class="t">                <span class="nam">st_next_line</span> <span class="op">=</span> <span class="nam">st_next_line</span> <span class="op">+</span> <span class="str">" &#9474;"</span>&nbsp;</span><span class="r"></span></p>
-    <p class="pln"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">            <span class="key">for</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">item</span><span class="op">]</span><span class="op">,</span> <span class="nam">st_next_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">                <span class="nam">l</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">st_next_line</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
-    <p class="mis show_mis"><span class="n"><a id="t488" href="#t488">488</a></span><span class="t">                <span class="nam">st_next_line</span> <span class="op">=</span> <span class="nam">st_next_line</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">l</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t23" href="#t23">23</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t24" href="#t24">24</a></span><span class="t"><span class="key">class</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">object</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t25" href="#t25">25</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t26" href="#t26">26</a></span><span class="t"><span class="str">     A radix node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t27" href="#t27">27</a></span><span class="t"><span class="str">     """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t28" href="#t28">28</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t29" href="#t29">29</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">key_size</span><span class="op">,</span> <span class="nam">cont</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t30" href="#t30">30</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t31" href="#t31">31</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t32" href="#t32">32</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">key_size</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t33" href="#t33">33</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t34" href="#t34">34</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t35" href="#t35">35</a></span><span class="t">    <span class="key">def</span> <span class="nam">__str__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t36" href="#t36">36</a></span><span class="t">        <span class="nam">p</span> <span class="op">=</span> <span class="nam">hex</span><span class="op">(</span><span class="nam">id</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t37" href="#t37">37</a></span><span class="t">        <span class="key">if</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t38" href="#t38">38</a></span><span class="t">            <span class="key">return</span> <span class="op">(</span><span class="str">"Node %s -> key: %s (%s) key_size: %d _next: %s _data %s"</span> <span class="op">%</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t39" href="#t39">39</a></span><span class="t">            <span class="nam">p</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">+</span> <span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_next</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_data</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t40" href="#t40">40</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t41" href="#t41">41</a></span><span class="t">            <span class="key">return</span> <span class="op">(</span><span class="str">"Node %s -> key: %s (%s) key_size: %d _next: %s"</span> <span class="op">%</span> <span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t42" href="#t42">42</a></span><span class="t">            <span class="nam">p</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">+</span> <span class="num">1</span><span class="op">:</span><span class="op">]</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t43" href="#t43">43</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t44" href="#t44">44</a></span><span class="t"><span class="key">class</span> <span class="nam">RadixTree</span><span class="op">(</span><span class="nam">object</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t45" href="#t45">45</a></span><span class="t">    <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t46" href="#t46">46</a></span><span class="t"><span class="str">    A radix tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t47" href="#t47">47</a></span><span class="t"><span class="str">    """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t48" href="#t48">48</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t49" href="#t49">49</a></span><span class="t">    <span class="com">#    max_key_len = 0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t50" href="#t50">50</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t51" href="#t51">51</a></span><span class="t">    <span class="key">def</span> <span class="nam">__init__</span><span class="op">(</span><span class="nam">self</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t52" href="#t52">52</a></span><span class="t">        <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t53" href="#t53">53</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t54" href="#t54">54</a></span><span class="t">    <span class="key">def</span> <span class="nam">insert_node</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">val</span><span class="op">,</span> <span class="nam">start_node</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t55" href="#t55">55</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t56" href="#t56">56</a></span><span class="t"><span class="str">        Insert a node in radix tree with a string key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t57" href="#t57">57</a></span><span class="t"><span class="str">        :param key: string or int key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t58" href="#t58">58</a></span><span class="t"><span class="str">        :param val: data linked to the node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t59" href="#t59">59</a></span><span class="t"><span class="str">        :return: new node created</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t60" href="#t60">60</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t61" href="#t61">61</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" RadixTree.insert_node() "</span><span class="op">.</span><span class="nam">center</span><span class="op">(</span><span class="num">60</span><span class="op">,</span> <span class="str">'-'</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t62" href="#t62">62</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" key: %s "</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t63" href="#t63">63</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t64" href="#t64">64</a></span><span class="t">        <span class="key">if</span> <span class="nam">type</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t65" href="#t65">65</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">bin</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">'0b'</span><span class="op">,</span> <span class="str">''</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t66" href="#t66">66</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Key converted in string key: %s "</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t67" href="#t67">67</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t68" href="#t68">68</a></span><span class="t">        <span class="key">if</span> <span class="nam">start_node</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t69" href="#t69">69</a></span><span class="t">            <span class="nam">current</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t70" href="#t70">70</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t71" href="#t71">71</a></span><span class="t">            <span class="nam">current</span> <span class="op">=</span> <span class="nam">start_node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t72" href="#t72">72</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t73" href="#t73">73</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Current node: %s "</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t74" href="#t74">74</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t75" href="#t75">75</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">current</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t76" href="#t76">76</a></span><span class="t">            <span class="str">""" the radix tree is empty """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t77" href="#t77">77</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t78" href="#t78">78</a></span><span class="t">            <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t79" href="#t79">79</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">,</span> <span class="nam">cont</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t80" href="#t80">80</a></span><span class="t">            <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span> <span class="op">=</span> <span class="nam">node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t81" href="#t81">81</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t82" href="#t82">82</a></span><span class="t">            <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t83" href="#t83">83</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t84" href="#t84">84</a></span><span class="t">        <span class="nam">tested</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t85" href="#t85">85</a></span><span class="t">        <span class="key">while</span> <span class="nam">tested</span> <span class="op">&lt;</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t86" href="#t86">86</a></span><span class="t">            <span class="key">if</span> <span class="nam">tested</span> <span class="op">></span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t87" href="#t87">87</a></span><span class="t">                <span class="com">#  Example</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t88" href="#t88">88</a></span><span class="t">                <span class="com">#  key to insert AB</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t89" href="#t89">89</a></span><span class="t">                <span class="com">#  tested = 2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t90" href="#t90">90</a></span><span class="t">                <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t91" href="#t91">91</a></span><span class="t">                <span class="com">#  &#9475; current    &#9475;->&#9475; next node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t92" href="#t92">92</a></span><span class="t">                <span class="com">#  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t93" href="#t93">93</a></span><span class="t">                <span class="com">#  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t94" href="#t94">94</a></span><span class="t">                <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t95" href="#t95">95</a></span><span class="t">                <span class="com">#  Result :</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t96" href="#t96">96</a></span><span class="t">                <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t97" href="#t97">97</a></span><span class="t">                <span class="com">#  &#9475; current    &#9475;->&#9475; node1      &#9475;->&#9475; next node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t98" href="#t98">98</a></span><span class="t">                <span class="com">#  &#9475; key=AB     &#9475;  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t99" href="#t99">99</a></span><span class="t">                <span class="com">#  &#9475; len=2      &#9475;  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t100" href="#t100">100</a></span><span class="t">                <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t101" href="#t101">101</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t102" href="#t102">102</a></span><span class="t">                <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t103" href="#t103">103</a></span><span class="t">                <span class="nam">node1</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t104" href="#t104">104</a></span><span class="t">                <span class="nam">node1</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t105" href="#t105">105</a></span><span class="t">                <span class="nam">node1</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t106" href="#t106">106</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t107" href="#t107">107</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t108" href="#t108">108</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">node1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t109" href="#t109">109</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t110" href="#t110">110</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t111" href="#t111">111</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t112" href="#t112">112</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t113" href="#t113">113</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">node1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t114" href="#t114">114</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t115" href="#t115">115</a></span><span class="t">                <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t116" href="#t116">116</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t117" href="#t117">117</a></span><span class="t">            <span class="key">elif</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="op">!=</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t118" href="#t118">118</a></span><span class="t">                <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t119" href="#t119">119</a></span><span class="t"><span class="str">                Creation of two new nodes and one container for data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t120" href="#t120">120</a></span><span class="t"><span class="str">                """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t121" href="#t121">121</a></span><span class="t">                <span class="com">#  Example</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t122" href="#t122">122</a></span><span class="t">                <span class="com">#  key to insert AC</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t123" href="#t123">123</a></span><span class="t">                <span class="com">#  tested = 1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t124" href="#t124">124</a></span><span class="t">                <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t125" href="#t125">125</a></span><span class="t">                <span class="com">#  &#9475; current    &#9475;->&#9475; next node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t126" href="#t126">126</a></span><span class="t">                <span class="com">#  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t127" href="#t127">127</a></span><span class="t">                <span class="com">#  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t128" href="#t128">128</a></span><span class="t">                <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t129" href="#t129">129</a></span><span class="t">                <span class="com">#  Result :</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t130" href="#t130">130</a></span><span class="t">                <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t131" href="#t131">131</a></span><span class="t">                <span class="com">#  &#9475; current    &#9475;->&#9475; node1      &#9475;->&#9475; next node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t132" href="#t132">132</a></span><span class="t">                <span class="com">#  &#9475; key=A      &#9475;  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t133" href="#t133">133</a></span><span class="t">                <span class="com">#  &#9475; len=1      &#9475;  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t134" href="#t134">134</a></span><span class="t">                <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t135" href="#t135">135</a></span><span class="t">                <span class="com">#        &#9474; C       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t136" href="#t136">136</a></span><span class="t">                <span class="com">#        +-------->&#9475; node2      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t137" href="#t137">137</a></span><span class="t">                <span class="com">#                  &#9475; key=AC     &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t138" href="#t138">138</a></span><span class="t">                <span class="com">#                  &#9475; len=2      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t139" href="#t139">139</a></span><span class="t">                <span class="com">#                  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t140" href="#t140">140</a></span><span class="t">                <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t141" href="#t141">141</a></span><span class="t">                <span class="nam">node1</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="key">None</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t142" href="#t142">142</a></span><span class="t">                <span class="nam">node1</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t143" href="#t143">143</a></span><span class="t">                <span class="nam">node1</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t144" href="#t144">144</a></span><span class="t">                <span class="nam">node2</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">,</span> <span class="nam">cont</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t145" href="#t145">145</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t146" href="#t146">146</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">tested</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t147" href="#t147">147</a></span><span class="t">                <span class="com"># for k in current._next:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t148" href="#t148">148</a></span><span class="t">                <span class="com">#    del current._next[k]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t149" href="#t149">149</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="op">{</span><span class="op">}</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t150" href="#t150">150</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">current</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">node1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t151" href="#t151">151</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">node2</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t152" href="#t152">152</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">key</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">tested</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t153" href="#t153">153</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t154" href="#t154">154</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t155" href="#t155">155</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t156" href="#t156">156</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">node1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t157" href="#t157">157</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="nam">node2</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t158" href="#t158">158</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t159" href="#t159">159</a></span><span class="t">                <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t160" href="#t160">160</a></span><span class="t">            <span class="nam">tested</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t161" href="#t161">161</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t162" href="#t162">162</a></span><span class="t">        <span class="key">if</span> <span class="nam">tested</span> <span class="op">==</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t163" href="#t163">163</a></span><span class="t">            <span class="key">if</span> <span class="nam">tested</span> <span class="op">&lt;</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t164" href="#t164">164</a></span><span class="t">                <span class="str">"""Go to the next node"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t165" href="#t165">165</a></span><span class="t">                <span class="key">if</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="key">in</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t166" href="#t166">166</a></span><span class="t">                    <span class="nam">current</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t167" href="#t167">167</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Go to the next node: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t168" href="#t168">168</a></span><span class="t">                    <span class="nam">self</span><span class="op">.</span><span class="nam">insert_node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">val</span><span class="op">,</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t169" href="#t169">169</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t170" href="#t170">170</a></span><span class="t">                    <span class="str">"""Create the new node"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t171" href="#t171">171</a></span><span class="t">                    <span class="com">#  Example</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t172" href="#t172">172</a></span><span class="t">                    <span class="com">#  key to insert ABABA</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t173" href="#t173">173</a></span><span class="t">                    <span class="com">#  tested = 4</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t174" href="#t174">174</a></span><span class="t">                    <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t175" href="#t175">175</a></span><span class="t">                    <span class="com">#  &#9475; current    &#9475;->&#9475;            &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t176" href="#t176">176</a></span><span class="t">                    <span class="com">#  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t177" href="#t177">177</a></span><span class="t">                    <span class="com">#  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t178" href="#t178">178</a></span><span class="t">                    <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t179" href="#t179">179</a></span><span class="t">                    <span class="com">#  Result :</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t180" href="#t180">180</a></span><span class="t">                    <span class="com">#  &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t181" href="#t181">181</a></span><span class="t">                    <span class="com">#  &#9475; current    &#9475;->&#9475;            &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t182" href="#t182">182</a></span><span class="t">                    <span class="com">#  &#9475; key=ABAB   &#9475;  &#9475; key=ABABB  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t183" href="#t183">183</a></span><span class="t">                    <span class="com">#  &#9475; len=4      &#9475;  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t184" href="#t184">184</a></span><span class="t">                    <span class="com">#  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t185" href="#t185">185</a></span><span class="t">                    <span class="com">#        &#9474; A       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t186" href="#t186">186</a></span><span class="t">                    <span class="com">#        +-------->&#9475; node       &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t187" href="#t187">187</a></span><span class="t">                    <span class="com">#                  &#9475; key=ABABA  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t188" href="#t188">188</a></span><span class="t">                    <span class="com">#                  &#9475; len=5      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t189" href="#t189">189</a></span><span class="t">                    <span class="com">#                  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t190" href="#t190">190</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t191" href="#t191">191</a></span><span class="t">                    <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t192" href="#t192">192</a></span><span class="t">                    <span class="nam">node</span> <span class="op">=</span> <span class="nam">Node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">,</span> <span class="nam">cont</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t193" href="#t193">193</a></span><span class="t">                    <span class="nam">current</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span> <span class="op">=</span> <span class="nam">node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t194" href="#t194">194</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Create the next node: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t195" href="#t195">195</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Modify the current node: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t196" href="#t196">196</a></span><span class="t">                    <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t197" href="#t197">197</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t198" href="#t198">198</a></span><span class="t">                <span class="str">"""The leaf already exists, we have to update container"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t199" href="#t199">199</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"The leaf already exists, we have to update container node: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t200" href="#t200">200</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t201" href="#t201">201</a></span><span class="t">                <span class="nam">current</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t202" href="#t202">202</a></span><span class="t">                <span class="nam">cont</span> <span class="op">=</span> <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t203" href="#t203">203</a></span><span class="t">                <span class="key">if</span> <span class="nam">cont</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t204" href="#t204">204</a></span><span class="t">                    <span class="str">"""Update container"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t205" href="#t205">205</a></span><span class="t">                    <span class="nam">cont</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">val</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t206" href="#t206">206</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Node already exist. Update container: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t207" href="#t207">207</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t208" href="#t208">208</a></span><span class="t">                    <span class="str">"""Create container"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t209" href="#t209">209</a></span><span class="t">                    <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Node already exist. Create container: %s"</span> <span class="op">%</span> <span class="nam">current</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t210" href="#t210">210</a></span><span class="t">                    <span class="nam">cont</span> <span class="op">=</span> <span class="nam">Container</span><span class="op">(</span><span class="nam">data</span><span class="op">=</span><span class="nam">val</span><span class="op">,</span> <span class="nam">tag</span><span class="op">=</span><span class="num">0</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t211" href="#t211">211</a></span><span class="t">                    <span class="nam">current</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t212" href="#t212">212</a></span><span class="t">                <span class="key">return</span> <span class="nam">cont</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t213" href="#t213">213</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t214" href="#t214">214</a></span><span class="t">    <span class="key">def</span> <span class="nam">get_node</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">start_node</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t215" href="#t215">215</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t216" href="#t216">216</a></span><span class="t"><span class="str">        Get node in the radix tree beginning to &lt;start_node> indexed by &lt;key></span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t217" href="#t217">217</a></span><span class="t"><span class="str">        :param start_node: first node of the radix tree to explore</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t218" href="#t218">218</a></span><span class="t"><span class="str">        :param key: key to search</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t219" href="#t219">219</a></span><span class="t"><span class="str">        :return: data linked to the node, if any. None otherwise</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t220" href="#t220">220</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t221" href="#t221">221</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t222" href="#t222">222</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" RadixTree.get_node() "</span><span class="op">.</span><span class="nam">center</span><span class="op">(</span><span class="num">60</span><span class="op">,</span> <span class="str">'-'</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t223" href="#t223">223</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t224" href="#t224">224</a></span><span class="t">        <span class="key">if</span> <span class="nam">type</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t225" href="#t225">225</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">bin</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">'0b'</span><span class="op">,</span> <span class="str">''</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t226" href="#t226">226</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Key converted in string key: %s "</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t227" href="#t227">227</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t228" href="#t228">228</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t229" href="#t229">229</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t230" href="#t230">230</a></span><span class="t">        <span class="key">if</span> <span class="nam">start_node</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t231" href="#t231">231</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t232" href="#t232">232</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t233" href="#t233">233</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">start_node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t234" href="#t234">234</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t235" href="#t235">235</a></span><span class="t">        <span class="key">if</span> <span class="nam">node</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t236" href="#t236">236</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Current node: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t237" href="#t237">237</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span> <span class="op">==</span> <span class="nam">key</span> <span class="key">and</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">==</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t238" href="#t238">238</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Node found -> key: %s key_size: %d data: %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t239" href="#t239">239</a></span><span class="t">                <span class="key">return</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t240" href="#t240">240</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t241" href="#t241">241</a></span><span class="t">                <span class="nam">tested</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t242" href="#t242">242</a></span><span class="t">                <span class="key">while</span> <span class="nam">tested</span> <span class="op">&lt;</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t243" href="#t243">243</a></span><span class="t">                    <span class="key">if</span> <span class="nam">tested</span> <span class="op">></span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t244" href="#t244">244</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t245" href="#t245">245</a></span><span class="t">                        <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t246" href="#t246">246</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t247" href="#t247">247</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Searching node... current node: %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t248" href="#t248">248</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t249" href="#t249">249</a></span><span class="t">                            <span class="str">"Searching node... index: %d tested: %s - %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">tested</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">,</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t250" href="#t250">250</a></span><span class="t">                        <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="op">!=</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t251" href="#t251">251</a></span><span class="t">                            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t252" href="#t252">252</a></span><span class="t">                            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t253" href="#t253">253</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t254" href="#t254">254</a></span><span class="t">                            <span class="nam">tested</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t255" href="#t255">255</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t256" href="#t256">256</a></span><span class="t">                <span class="key">if</span> <span class="nam">tested</span> <span class="op">==</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t257" href="#t257">257</a></span><span class="t">                    <span class="key">if</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t258" href="#t258">258</a></span><span class="t">                        <span class="nam">node</span> <span class="op">=</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t259" href="#t259">259</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"2 Go to the next node -> next: %s node: %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t260" href="#t260">260</a></span><span class="t">                        <span class="key">return</span> <span class="nam">self</span><span class="op">.</span><span class="nam">get_node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t261" href="#t261">261</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t262" href="#t262">262</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t263" href="#t263">263</a></span><span class="t">                        <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t264" href="#t264">264</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t265" href="#t265">265</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t266" href="#t266">266</a></span><span class="t">            <span class="key">return</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t267" href="#t267">267</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t268" href="#t268">268</a></span><span class="t">    <span class="key">def</span> <span class="nam">delete_node</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">key</span><span class="op">,</span> <span class="nam">start_node</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">prev_node</span><span class="op">=</span><span class="key">None</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t269" href="#t269">269</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t270" href="#t270">270</a></span><span class="t"><span class="str">        Delete node in radix tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t271" href="#t271">271</a></span><span class="t"><span class="str">        :param key: key of the node to delete</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t272" href="#t272">272</a></span><span class="t"><span class="str">        :param start_node: first node of the radix tree or None to start from the beginning of radix tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t273" href="#t273">273</a></span><span class="t"><span class="str">        :param prev_node: previous node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t274" href="#t274">274</a></span><span class="t"><span class="str">        :return: True if deleted. False otherwise.</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t275" href="#t275">275</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t276" href="#t276">276</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t277" href="#t277">277</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" RadixTree.delete_node() "</span><span class="op">.</span><span class="nam">center</span><span class="op">(</span><span class="num">60</span><span class="op">,</span> <span class="str">'-'</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t278" href="#t278">278</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t279" href="#t279">279</a></span><span class="t">        <span class="key">if</span> <span class="nam">type</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">!=</span> <span class="nam">str</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t280" href="#t280">280</a></span><span class="t">            <span class="nam">key</span> <span class="op">=</span> <span class="nam">bin</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span><span class="op">.</span><span class="nam">replace</span><span class="op">(</span><span class="str">'0b'</span><span class="op">,</span> <span class="str">''</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t281" href="#t281">281</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Key converted in string key: %s "</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t282" href="#t282">282</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t283" href="#t283">283</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" Key : %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t284" href="#t284">284</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t285" href="#t285">285</a></span><span class="t">        <span class="key">if</span> <span class="nam">start_node</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t286" href="#t286">286</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t287" href="#t287">287</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t288" href="#t288">288</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">start_node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t289" href="#t289">289</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t290" href="#t290">290</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Current node -> %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t291" href="#t291">291</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t292" href="#t292">292</a></span><span class="t">        <span class="key">if</span> <span class="nam">node</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t293" href="#t293">293</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span> <span class="op">==</span> <span class="nam">key</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t294" href="#t294">294</a></span><span class="t">                <span class="com"># Node to delete found</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t295" href="#t295">295</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Node to delete found -> %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t296" href="#t296">296</a></span><span class="t">                <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">==</span> <span class="num">0</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t297" href="#t297">297</a></span><span class="t">                    <span class="key">if</span> <span class="nam">prev_node</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t298" href="#t298">298</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"First node of tree deleted -> Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t299" href="#t299">299</a></span><span class="t">                        <span class="key">del</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t300" href="#t300">300</a></span><span class="t">                        <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t301" href="#t301">301</a></span><span class="t">                        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t302" href="#t302">302</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t303" href="#t303">303</a></span><span class="t">                        <span class="com"># Example</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t304" href="#t304">304</a></span><span class="t">                        <span class="com"># Delete 'ABA'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t305" href="#t305">305</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t306" href="#t306">306</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node    &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t307" href="#t307">307</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t308" href="#t308">308</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3   &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t309" href="#t309">309</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t310" href="#t310">310</a></span><span class="t">                        <span class="com"># Result :</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t311" href="#t311">311</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t312" href="#t312">312</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t313" href="#t313">313</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t314" href="#t314">314</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t315" href="#t315">315</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t316" href="#t316">316</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t317" href="#t317">317</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Node deleted %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t318" href="#t318">318</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Previous link deleted %s "</span> <span class="op">%</span> <span class="nam">prev_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t319" href="#t319">319</a></span><span class="t">                        <span class="key">del</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">prev_node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t320" href="#t320">320</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"1. Previous node updated %s "</span> <span class="op">%</span> <span class="nam">prev_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t321" href="#t321">321</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t322" href="#t322">322</a></span><span class="t">                        <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span> <span class="key">and</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_data</span> <span class="op">==</span> <span class="key">None</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t323" href="#t323">323</a></span><span class="t">                            <span class="com"># Example</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t324" href="#t324">324</a></span><span class="t">                            <span class="com"># Delete 'ABB'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t325" href="#t325">325</a></span><span class="t">                            <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t326" href="#t326">326</a></span><span class="t">                            <span class="com"># &#9475; prev_node  &#9475;->&#9475; node    &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t327" href="#t327">327</a></span><span class="t">                            <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t328" href="#t328">328</a></span><span class="t">                            <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3   &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t329" href="#t329">329</a></span><span class="t">                            <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t330" href="#t330">330</a></span><span class="t">                            <span class="com">#        &#9474; B       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t331" href="#t331">331</a></span><span class="t">                            <span class="com">#        +-------->&#9475; other node &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t332" href="#t332">332</a></span><span class="t">                            <span class="com">#                  &#9475; key=ABB    &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t333" href="#t333">333</a></span><span class="t">                            <span class="com">#                  &#9475; len=3      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t334" href="#t334">334</a></span><span class="t">                            <span class="com">#                  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t335" href="#t335">335</a></span><span class="t">                            <span class="com"># Result :</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t336" href="#t336">336</a></span><span class="t">                            <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t337" href="#t337">337</a></span><span class="t">                            <span class="com"># &#9475; prev_node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t338" href="#t338">338</a></span><span class="t">                            <span class="com"># &#9475; key=ABA    &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t339" href="#t339">339</a></span><span class="t">                            <span class="com"># &#9475; len=3      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t340" href="#t340">340</a></span><span class="t">                            <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t341" href="#t341">341</a></span><span class="t">                            <span class="key">for</span> <span class="nam">k</span> <span class="key">in</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t342" href="#t342">342</a></span><span class="t">                                <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">k</span><span class="op">]</span><span class="op">.</span><span class="nam">_key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t343" href="#t343">343</a></span><span class="t">                                <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">k</span><span class="op">]</span><span class="op">.</span><span class="nam">_key_size</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t344" href="#t344">344</a></span><span class="t">                                <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">k</span><span class="op">]</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t345" href="#t345">345</a></span><span class="t">                                <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="nam">prev_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">k</span><span class="op">]</span><span class="op">.</span><span class="nam">_next</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t346" href="#t346">346</a></span><span class="t">                                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"2. Previous node updated %s "</span> <span class="op">%</span> <span class="nam">prev_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t347" href="#t347">347</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t348" href="#t348">348</a></span><span class="t">                        <span class="key">del</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t349" href="#t349">349</a></span><span class="t">                        <span class="key">del</span> <span class="nam">node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t350" href="#t350">350</a></span><span class="t">                        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t351" href="#t351">351</a></span><span class="t">                <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t352" href="#t352">352</a></span><span class="t">                    <span class="key">if</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t353" href="#t353">353</a></span><span class="t">                        <span class="com"># Example</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t354" href="#t354">354</a></span><span class="t">                        <span class="com"># Delete 'ABA'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t355" href="#t355">355</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t356" href="#t356">356</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node       &#9475;->&#9475; next_node  &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t357" href="#t357">357</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA    &#9475;  &#9475; key=ABAB   &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t358" href="#t358">358</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3      &#9475;  &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t359" href="#t359">359</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t360" href="#t360">360</a></span><span class="t">                        <span class="com"># Result :</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t361" href="#t361">361</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t362" href="#t362">362</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node       &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t363" href="#t363">363</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABAB   &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t364" href="#t364">364</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t365" href="#t365">365</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t366" href="#t366">366</a></span><span class="t">                        <span class="key">for</span> <span class="nam">ke</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t367" href="#t367">367</a></span><span class="t">                            <span class="nam">next_node</span> <span class="op">=</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">ke</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t368" href="#t368">368</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Node to update %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t369" href="#t369">369</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span> <span class="op">=</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_key</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t370" href="#t370">370</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span> <span class="op">=</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_key_size</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t371" href="#t371">371</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t372" href="#t372">372</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span> <span class="op">=</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_next</span><span class="op">.</span><span class="nam">copy</span><span class="op">(</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t373" href="#t373">373</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Node updated %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t374" href="#t374">374</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Node deleted %s "</span> <span class="op">%</span> <span class="nam">next_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t375" href="#t375">375</a></span><span class="t">                        <span class="key">del</span> <span class="nam">next_node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t376" href="#t376">376</a></span><span class="t">                        <span class="key">del</span> <span class="nam">next_node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t377" href="#t377">377</a></span><span class="t">                        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t378" href="#t378">378</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t379" href="#t379">379</a></span><span class="t">                        <span class="com"># Example</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t380" href="#t380">380</a></span><span class="t">                        <span class="com"># Delete 'ABA'</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t381" href="#t381">381</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t382" href="#t382">382</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node       &#9475;->&#9475; next_node1 &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t383" href="#t383">383</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA    &#9475;  &#9475; key=ABAB   &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t384" href="#t384">384</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3      &#9475;  &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t385" href="#t385">385</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t386" href="#t386">386</a></span><span class="t">                        <span class="com">#                       &#9474; C       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t387" href="#t387">387</a></span><span class="t">                        <span class="com">#                       +-------->&#9475; next_nodei &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t388" href="#t388">388</a></span><span class="t">                        <span class="com">#                                 &#9475; key=ABAC   &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t389" href="#t389">389</a></span><span class="t">                        <span class="com">#                                 &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t390" href="#t390">390</a></span><span class="t">                        <span class="com">#                                 &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t391" href="#t391">391</a></span><span class="t">                        <span class="com"># Result :</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t392" href="#t392">392</a></span><span class="t">                        <span class="com"># &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;A &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;B &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t393" href="#t393">393</a></span><span class="t">                        <span class="com"># &#9475; prev_node  &#9475;->&#9475; node       &#9475;->&#9475; next_node1 &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t394" href="#t394">394</a></span><span class="t">                        <span class="com"># &#9475; key=AB     &#9475;  &#9475; key=ABA    &#9475;  &#9475; key=ABAB   &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t395" href="#t395">395</a></span><span class="t">                        <span class="com"># &#9475; len=2      &#9475;  &#9475; len=3      &#9475;  &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t396" href="#t396">396</a></span><span class="t">                        <span class="com"># &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;  &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t397" href="#t397">397</a></span><span class="t">                        <span class="com">#                       &#9474; C       &#9487;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9491;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t398" href="#t398">398</a></span><span class="t">                        <span class="com">#                       +-------->&#9475; next_nodei &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t399" href="#t399">399</a></span><span class="t">                        <span class="com">#                                 &#9475; key=ABAC   &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t400" href="#t400">400</a></span><span class="t">                        <span class="com">#                                 &#9475; len=4      &#9475;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t401" href="#t401">401</a></span><span class="t">                        <span class="com">#                                 &#9495;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9473;&#9499;</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t402" href="#t402">402</a></span><span class="t">                        <span class="com"># In this case, just delete data linked to the node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t403" href="#t403">403</a></span><span class="t">                        <span class="key">del</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t404" href="#t404">404</a></span><span class="t">                        <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span> <span class="op">=</span> <span class="key">None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t405" href="#t405">405</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Just delete data linked to the node %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t406" href="#t406">406</a></span><span class="t">                        <span class="key">return</span> <span class="key">True</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t407" href="#t407">407</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t408" href="#t408">408</a></span><span class="t">                <span class="com"># Other node case</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t409" href="#t409">409</a></span><span class="t">                <span class="nam">tested</span> <span class="op">=</span> <span class="num">0</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t410" href="#t410">410</a></span><span class="t">                <span class="key">while</span> <span class="nam">tested</span> <span class="op">&lt;</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t411" href="#t411">411</a></span><span class="t">                    <span class="key">if</span> <span class="nam">tested</span> <span class="op">></span> <span class="nam">len</span><span class="op">(</span><span class="nam">key</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t412" href="#t412">412</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t413" href="#t413">413</a></span><span class="t">                        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t414" href="#t414">414</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t415" href="#t415">415</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"Searching node... current node: %s "</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t416" href="#t416">416</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t417" href="#t417">417</a></span><span class="t">                            <span class="str">"Searching node... index: %d tested: %s - %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">tested</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">,</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t418" href="#t418">418</a></span><span class="t">                        <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="op">!=</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t419" href="#t419">419</a></span><span class="t">                            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t420" href="#t420">420</a></span><span class="t">                            <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t421" href="#t421">421</a></span><span class="t">                        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t422" href="#t422">422</a></span><span class="t">                            <span class="nam">tested</span> <span class="op">+=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t423" href="#t423">423</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t424" href="#t424">424</a></span><span class="t">                <span class="key">if</span> <span class="nam">tested</span> <span class="op">==</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t425" href="#t425">425</a></span><span class="t">                    <span class="key">if</span> <span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t426" href="#t426">426</a></span><span class="t">                        <span class="nam">prev_node</span> <span class="op">=</span> <span class="nam">node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t427" href="#t427">427</a></span><span class="t">                        <span class="nam">node</span> <span class="op">=</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t428" href="#t428">428</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Go to the next node -> next: %s node: %s"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">[</span><span class="nam">tested</span><span class="op">]</span><span class="op">,</span> <span class="nam">node</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t429" href="#t429">429</a></span><span class="t">                        <span class="nam">ret</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">delete_node</span><span class="op">(</span><span class="nam">key</span><span class="op">,</span> <span class="nam">node</span><span class="op">,</span> <span class="nam">prev_node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t430" href="#t430">430</a></span><span class="t">                        <span class="key">return</span> <span class="nam">ret</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t431" href="#t431">431</a></span><span class="t">                    <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t432" href="#t432">432</a></span><span class="t">                        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">warning</span><span class="op">(</span><span class="str">"Node not found -> key: %s"</span> <span class="op">%</span> <span class="nam">key</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t433" href="#t433">433</a></span><span class="t">                        <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t434" href="#t434">434</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t435" href="#t435">435</a></span><span class="t">            <span class="nam">my_logger</span><span class="op">.</span><span class="nam">info</span><span class="op">(</span><span class="str">"Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t436" href="#t436">436</a></span><span class="t">            <span class="key">return</span> <span class="key">False</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t437" href="#t437">437</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t438" href="#t438">438</a></span><span class="t">    <span class="key">def</span> <span class="nam">dump</span><span class="op">(</span><span class="nam">self</span><span class="op">,</span> <span class="nam">node</span><span class="op">=</span><span class="key">None</span><span class="op">,</span> <span class="nam">st_next_line</span><span class="op">=</span><span class="str">''</span><span class="op">)</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t439" href="#t439">439</a></span><span class="t">        <span class="str">"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t440" href="#t440">440</a></span><span class="t"><span class="str">        Display a radix node</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t441" href="#t441">441</a></span><span class="t"><span class="str">        :param node: first node of the radix tree. If node = None dump the entire radix tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t442" href="#t442">442</a></span><span class="t"><span class="str">        :param st_next_line: start of next line to display</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t443" href="#t443">443</a></span><span class="t"><span class="str">        :return: None</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t444" href="#t444">444</a></span><span class="t"><span class="str">        """</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t445" href="#t445">445</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t446" href="#t446">446</a></span><span class="t">        <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">" RadixTree.dump() "</span><span class="op">.</span><span class="nam">center</span><span class="op">(</span><span class="num">60</span><span class="op">,</span> <span class="str">'-'</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t447" href="#t447">447</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t448" href="#t448">448</a></span><span class="t">        <span class="key">if</span> <span class="key">not</span> <span class="nam">node</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t449" href="#t449">449</a></span><span class="t">            <span class="str">"""Dump the entire radix tree"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t450" href="#t450">450</a></span><span class="t">            <span class="nam">node</span> <span class="op">=</span> <span class="nam">self</span><span class="op">.</span><span class="nam">_tree</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t451" href="#t451">451</a></span><span class="t">            <span class="key">if</span> <span class="key">not</span> <span class="nam">node</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t452" href="#t452">452</a></span><span class="t">                <span class="nam">print</span><span class="op">(</span><span class="str">"Radix tree empty"</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t453" href="#t453">453</a></span><span class="t">                <span class="key">return</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t454" href="#t454">454</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t455" href="#t455">455</a></span><span class="t">                <span class="nam">line</span> <span class="op">=</span> <span class="str">"&#9632;"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t456" href="#t456">456</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t457" href="#t457">457</a></span><span class="t">                <span class="nam">line</span> <span class="op">=</span> <span class="str">"&#9633;"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t458" href="#t458">458</a></span><span class="t">            <span class="nam">line</span> <span class="op">+=</span> <span class="str">" key: %s key_len: %d next: %d"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t459" href="#t459">459</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t460" href="#t460">460</a></span><span class="t">                <span class="nam">line</span> <span class="op">+=</span> <span class="str">" data: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t461" href="#t461">461</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t462" href="#t462">462</a></span><span class="t">            <span class="nam">cpt</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t463" href="#t463">463</a></span><span class="t">            <span class="nam">st_next_line</span> <span class="op">=</span> <span class="str">"&#9474;"</span> <span class="op">*</span> <span class="nam">cpt</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t464" href="#t464">464</a></span><span class="t">            <span class="key">for</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t465" href="#t465">465</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">item</span><span class="op">]</span><span class="op">,</span> <span class="nam">st_next_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t466" href="#t466">466</a></span><span class="t">                <span class="nam">cpt</span> <span class="op">-=</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t467" href="#t467">467</a></span><span class="t">                <span class="nam">st_next_line</span> <span class="op">=</span> <span class="nam">st_next_line</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">cpt</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t468" href="#t468">468</a></span><span class="t">        <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t469" href="#t469">469</a></span><span class="t">            <span class="str">"""Intermediate node"""</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t470" href="#t470">470</a></span><span class="t">            <span class="nam">line</span> <span class="op">=</span> <span class="nam">st_next_line</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t471" href="#t471">471</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t472" href="#t472">472</a></span><span class="t">                <span class="nam">line</span> <span class="op">+=</span> <span class="str">"&#9492;&#9632;"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t473" href="#t473">473</a></span><span class="t">            <span class="key">else</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t474" href="#t474">474</a></span><span class="t">                <span class="nam">line</span> <span class="op">+=</span> <span class="str">"&#9492;&#9633;"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t475" href="#t475">475</a></span><span class="t">            <span class="nam">line</span> <span class="op">+=</span> <span class="str">" key: %s key_len: %d next: %d"</span> <span class="op">%</span> <span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_key</span><span class="op">,</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_key_size</span><span class="op">,</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t476" href="#t476">476</a></span><span class="t">            <span class="key">if</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t477" href="#t477">477</a></span><span class="t">                <span class="nam">line</span> <span class="op">+=</span> <span class="str">" data: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_data</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t478" href="#t478">478</a></span><span class="t">            <span class="nam">print</span><span class="op">(</span><span class="nam">line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t479" href="#t479">479</a></span><span class="t">            <span class="nam">cpt</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t480" href="#t480">480</a></span><span class="t">            <span class="key">if</span> <span class="nam">cpt</span> <span class="op">></span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t481" href="#t481">481</a></span><span class="t">                <span class="nam">st_next_line</span> <span class="op">=</span> <span class="nam">st_next_line</span> <span class="op">+</span> <span class="str">" &#9474;"</span> <span class="op">+</span> <span class="str">"&#9474;"</span> <span class="op">*</span> <span class="op">(</span><span class="nam">cpt</span> <span class="op">-</span> <span class="num">1</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t482" href="#t482">482</a></span><span class="t">            <span class="key">if</span> <span class="nam">cpt</span> <span class="op">==</span> <span class="num">1</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t483" href="#t483">483</a></span><span class="t">                <span class="nam">my_logger</span><span class="op">.</span><span class="nam">debug</span><span class="op">(</span><span class="str">"node with only one son: %s"</span> <span class="op">%</span> <span class="nam">node</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t484" href="#t484">484</a></span><span class="t">                <span class="nam">st_next_line</span> <span class="op">=</span> <span class="nam">st_next_line</span> <span class="op">+</span> <span class="str">" &#9474;"</span>&nbsp;</span><span class="r"></span></p>
+    <p class="pln"><span class="n"><a id="t485" href="#t485">485</a></span><span class="t">&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t486" href="#t486">486</a></span><span class="t">            <span class="key">for</span> <span class="nam">item</span> <span class="key">in</span> <span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">:</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t487" href="#t487">487</a></span><span class="t">                <span class="nam">self</span><span class="op">.</span><span class="nam">dump</span><span class="op">(</span><span class="nam">node</span><span class="op">.</span><span class="nam">_next</span><span class="op">[</span><span class="nam">item</span><span class="op">]</span><span class="op">,</span> <span class="nam">st_next_line</span><span class="op">)</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t488" href="#t488">488</a></span><span class="t">                <span class="nam">l</span> <span class="op">=</span> <span class="nam">len</span><span class="op">(</span><span class="nam">st_next_line</span><span class="op">)</span> <span class="op">-</span> <span class="num">1</span>&nbsp;</span><span class="r"></span></p>
+    <p class="run"><span class="n"><a id="t489" href="#t489">489</a></span><span class="t">                <span class="nam">st_next_line</span> <span class="op">=</span> <span class="nam">st_next_line</span><span class="op">[</span><span class="num">0</span><span class="op">:</span><span class="nam">l</span><span class="op">]</span>&nbsp;</span><span class="r"></span></p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a id="prevFileLink" class="nav" href="d_a370a513ee95d9c9_radix_config_py.html">&#xab; prev</a> &nbsp; &nbsp;
             <a id="indexLink" class="nav" href="index.html">&Hat; index</a> &nbsp; &nbsp;
             <a id="nextFileLink" class="nav" href="index.html">&#xbb; next</a>
             &nbsp; &nbsp; &nbsp;
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-04 18:19 +0200
+            created at 2024-04-06 10:57 +0200
         </p>
     </div>
 </footer>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,515 +1,516 @@
-************ CCoovveerraaggee ffoorr ssrrcc//rraaddiixx__ttrreeee//rraaddiixx__ttrreeee..ppyy:: 11%% ************
+************ CCoovveerraaggee ffoorr ssrrcc//rraaddiixx__ttrreeee//rraaddiixx__ttrreeee..ppyy:: 110000%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 r m x   toggle line displays
 j k   next/prev highlighted chunk
 0   (zero) top of page
 1   (one) first highlighted chunk
 [ ]   prev/next file
 u   up to the index
 ?   show/hide this help
-********** 223388 ssttaatteemmeennttss ?  11 rruunn 223377 mmiissssiinngg 00 eexxcclluuddeedd **********
+********** 223388 ssttaatteemmeennttss ?  223388 rruunn 00 mmiissssiinngg 00 eexxcclluuddeedd **********
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-04 18:19 +0200
+06 10:57 +0200
 _1# -*- coding: utf-8 -*- 
 _2 
 _3# run tests from Pycharms locally 
-_4from radix_config import my_logger 
-_5# run tests from external Testpy as distributed package 
-_6#from radix_tree.radix_config import my_logger 
-_7 
-_8class Container(object): 
-_9 """ 
-_1_0 Container populated with data linked to a radic node 
-_1_1 """ 
-_1_2 
-_1_3 def __init__(self, data, tag=None): 
-_1_4 self._data = data 
-_1_5 self._tag = tag 
-_1_6 self._previous = None 
-_1_7 self._next = None 
-_1_8 
-_1_9 def __str__(self): 
-_2_0 return ("Container -> data: %s tag: %s" % (self._data, self._tag)) 
-_2_1 
+_4#from radix_config import my_logger 
+_5 
+_6# run tests from external Testpy as distributed package 
+_7from radix_tree.radix_config import my_logger 
+_8 
+_9class Container(object): 
+_1_0 """ 
+_1_1 Container populated with data linked to a radic node 
+_1_2 """ 
+_1_3 
+_1_4 def __init__(self, data, tag=None): 
+_1_5 self._data = data 
+_1_6 self._tag = tag 
+_1_7 self._previous = None 
+_1_8 self._next = None 
+_1_9 
+_2_0 def __str__(self): 
+_2_1 return ("Container -> data: %s tag: %s" % (self._data, self._tag)) 
 _2_2 
-_2_3class Node(object): 
-_2_4 """ 
-_2_5 A radix node 
-_2_6 """ 
-_2_7 
-_2_8 def __init__(self, key, key_size, cont=None): 
-_2_9 self._next = {} 
-_3_0 self._key = key 
-_3_1 self._key_size = key_size 
-_3_2 self._data = cont 
-_3_3 
-_3_4 def __str__(self): 
-_3_5 p = hex(id(self)) 
-_3_6 if self._data: 
-_3_7 return ("Node %s -> key: %s (%s) key_size: %d _next: %s _data %s" % ( 
-_3_8 p, self._key[0:self._key_size], self._key[self._key_size + 1:],
+_2_3 
+_2_4class Node(object): 
+_2_5 """ 
+_2_6 A radix node 
+_2_7 """ 
+_2_8 
+_2_9 def __init__(self, key, key_size, cont=None): 
+_3_0 self._next = {} 
+_3_1 self._key = key 
+_3_2 self._key_size = key_size 
+_3_3 self._data = cont 
+_3_4 
+_3_5 def __str__(self): 
+_3_6 p = hex(id(self)) 
+_3_7 if self._data: 
+_3_8 return ("Node %s -> key: %s (%s) key_size: %d _next: %s _data %s" % ( 
+_3_9 p, self._key[0:self._key_size], self._key[self._key_size + 1:],
 self._key_size, self._next, self._data)) 
-_3_9 else: 
-_4_0 return ("Node %s -> key: %s (%s) key_size: %d _next: %s" % ( 
-_4_1 p, self._key[0:self._key_size], self._key[self._key_size + 1:],
+_4_0 else: 
+_4_1 return ("Node %s -> key: %s (%s) key_size: %d _next: %s" % ( 
+_4_2 p, self._key[0:self._key_size], self._key[self._key_size + 1:],
 self._key_size, self._next)) 
-_4_2 
-_4_3class RadixTree(object): 
-_4_4 """ 
-_4_5 A radix tree 
-_4_6 """ 
-_4_7 
-_4_8 # max_key_len = 0 
-_4_9 
-_5_0 def __init__(self): 
-_5_1 self._tree = None 
-_5_2 
-_5_3 def insert_node(self, key, val, start_node=None): 
-_5_4 """ 
-_5_5 Insert a node in radix tree with a string key 
-_5_6 :param key: string or int key 
-_5_7 :param val: data linked to the node 
-_5_8 :return: new node created 
-_5_9 """ 
-_6_0 my_logger.debug(" RadixTree.insert_node() ".center(60, '-')) 
-_6_1 my_logger.debug(" key: %s " % key) 
-_6_2 
-_6_3 if type(key) != str: 
-_6_4 key = bin(key).replace('0b', '') 
-_6_5 my_logger.debug("Key converted in string key: %s " % key) 
-_6_6 
-_6_7 if start_node == None: 
-_6_8 current = self._tree 
-_6_9 else: 
-_7_0 current = start_node 
-_7_1 
-_7_2 my_logger.info("Current node: %s " % current) 
-_7_3 
-_7_4 if not current: 
-_7_5 """ the radix tree is empty """ 
-_7_6 my_logger.debug("Radix tree empty") 
-_7_7 cont = Container(data=val, tag=0) 
-_7_8 node = Node(key, len(key), cont) 
-_7_9 self._tree = node 
-_8_0 my_logger.debug(node) 
-_8_1 return cont 
-_8_2 
-_8_3 tested = 0 
-_8_4 while tested < current._key_size: 
-_8_5 if tested > len(key) - 1: 
-_8_6 # Example 
-_8_7 # key to insert AB 
-_8_8 # tested = 2 
-_8_9 # ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
-_9_0 # ┃ current ┃->┃ next node ┃ 
-_9_1 # ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
-_9_2 # ┃ len=4 ┃ ┃ len=5 ┃ 
-_9_3 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_9_4 # Result : 
-_9_5 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
-_9_6 # ┃ current ┃->┃ node1 ┃->┃ next node ┃ 
-_9_7 # ┃ key=AB ┃ ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
-_9_8 # ┃ len=2 ┃ ┃ len=4 ┃ ┃ len=5 ┃ 
-_9_9 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_1_0_0 
-_1_0_1 cont = Container(data=val, tag=0) 
-_1_0_2 node1 = Node(current._key, current._key_size, None) 
-_1_0_3 node1._next = current._next.copy() 
-_1_0_4 node1._data = current._data 
-_1_0_5 
-_1_0_6 current._key_size = len(key) 
-_1_0_7 current._next[current._key[tested]] = node1 
-_1_0_8 current._key = key 
-_1_0_9 current._data = cont 
-_1_1_0 
-_1_1_1 my_logger.debug(current) 
-_1_1_2 my_logger.debug(node1) 
-_1_1_3 
-_1_1_4 return cont 
-_1_1_5 
-_1_1_6 elif current._key[tested] != key[tested]: 
-_1_1_7 """ 
-_1_1_8 Creation of two new nodes and one container for data 
-_1_1_9 """ 
-_1_2_0 # Example 
-_1_2_1 # key to insert AC 
-_1_2_2 # tested = 1 
-_1_2_3 # ┏━━━━━━━━━━━━┓ ┏━━━━━━━━━━━━┓ 
-_1_2_4 # ┃ current ┃->┃ next node ┃ 
-_1_2_5 # ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
-_1_2_6 # ┃ len=4 ┃ ┃ len=5 ┃ 
-_1_2_7 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_1_2_8 # Result : 
-_1_2_9 # ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ ┏━━━━━━━━━━━━┓ 
-_1_3_0 # ┃ current ┃->┃ node1 ┃->┃ next node ┃ 
-_1_3_1 # ┃ key=A ┃ ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
-_1_3_2 # ┃ len=1 ┃ ┃ len=4 ┃ ┃ len=5 ┃ 
-_1_3_3 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_1_3_4 # │ C ┏━━━━━━━━━━━━┓ 
-_1_3_5 # +-------->┃ node2 ┃ 
-_1_3_6 # ┃ key=AC ┃ 
-_1_3_7 # ┃ len=2 ┃ 
-_1_3_8 # ┗━━━━━━━━━━━━┛ 
-_1_3_9 cont = Container(data=val, tag=0) 
-_1_4_0 node1 = Node(current._key, current._key_size, None) 
-_1_4_1 node1._next = current._next.copy() 
-_1_4_2 node1._data = current._data 
-_1_4_3 node2 = Node(key, len(key), cont) 
-_1_4_4 
-_1_4_5 current._key_size = tested 
-_1_4_6 # for k in current._next: 
-_1_4_7 # del current._next[k] 
-_1_4_8 current._next = {} 
-_1_4_9 current._next[current._key[tested]] = node1 
-_1_5_0 current._next[key[tested]] = node2 
-_1_5_1 current._key = key[0:tested] 
-_1_5_2 current._data = None 
-_1_5_3 
-_1_5_4 my_logger.debug(current) 
-_1_5_5 my_logger.debug(node1) 
-_1_5_6 my_logger.debug(node2) 
-_1_5_7 
-_1_5_8 return cont 
-_1_5_9 tested += 1 
-_1_6_0 
-_1_6_1 if tested == current._key_size: 
-_1_6_2 if tested < len(key): 
-_1_6_3 """Go to the next node""" 
-_1_6_4 if key[tested] in current._next: 
-_1_6_5 current = current._next[key[tested]] 
-_1_6_6 my_logger.debug("Go to the next node: %s" % current) 
-_1_6_7 self.insert_node(key, val, current) 
-_1_6_8 else: 
-_1_6_9 """Create the new node""" 
-_1_7_0 # Example 
-_1_7_1 # key to insert ABABA 
-_1_7_2 # tested = 4 
-_1_7_3 # ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
-_1_7_4 # ┃ current ┃->┃ ┃ 
-_1_7_5 # ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
-_1_7_6 # ┃ len=4 ┃ ┃ len=5 ┃ 
-_1_7_7 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_1_7_8 # Result : 
-_1_7_9 # ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
-_1_8_0 # ┃ current ┃->┃ ┃ 
-_1_8_1 # ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
-_1_8_2 # ┃ len=4 ┃ ┃ len=5 ┃ 
-_1_8_3 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_1_8_4 # │ A ┏━━━━━━━━━━━━┓ 
-_1_8_5 # +-------->┃ node ┃ 
-_1_8_6 # ┃ key=ABABA ┃ 
-_1_8_7 # ┃ len=5 ┃ 
-_1_8_8 # ┗━━━━━━━━━━━━┛ 
-_1_8_9 
-_1_9_0 cont = Container(data=val, tag=0) 
-_1_9_1 node = Node(key, len(key), cont) 
-_1_9_2 current._next[key[tested]] = node 
-_1_9_3 my_logger.debug("Create the next node: %s" % node) 
-_1_9_4 my_logger.debug("Modify the current node: %s" % current) 
-_1_9_5 return cont 
-_1_9_6 else: 
-_1_9_7 """The leaf already exists, we have to update container""" 
-_1_9_8 my_logger.debug("The leaf already exists, we have to update container node:
+_4_3 
+_4_4class RadixTree(object): 
+_4_5 """ 
+_4_6 A radix tree 
+_4_7 """ 
+_4_8 
+_4_9 # max_key_len = 0 
+_5_0 
+_5_1 def __init__(self): 
+_5_2 self._tree = None 
+_5_3 
+_5_4 def insert_node(self, key, val, start_node=None): 
+_5_5 """ 
+_5_6 Insert a node in radix tree with a string key 
+_5_7 :param key: string or int key 
+_5_8 :param val: data linked to the node 
+_5_9 :return: new node created 
+_6_0 """ 
+_6_1 my_logger.debug(" RadixTree.insert_node() ".center(60, '-')) 
+_6_2 my_logger.debug(" key: %s " % key) 
+_6_3 
+_6_4 if type(key) != str: 
+_6_5 key = bin(key).replace('0b', '') 
+_6_6 my_logger.debug("Key converted in string key: %s " % key) 
+_6_7 
+_6_8 if start_node == None: 
+_6_9 current = self._tree 
+_7_0 else: 
+_7_1 current = start_node 
+_7_2 
+_7_3 my_logger.info("Current node: %s " % current) 
+_7_4 
+_7_5 if not current: 
+_7_6 """ the radix tree is empty """ 
+_7_7 my_logger.debug("Radix tree empty") 
+_7_8 cont = Container(data=val, tag=0) 
+_7_9 node = Node(key, len(key), cont) 
+_8_0 self._tree = node 
+_8_1 my_logger.debug(node) 
+_8_2 return cont 
+_8_3 
+_8_4 tested = 0 
+_8_5 while tested < current._key_size: 
+_8_6 if tested > len(key) - 1: 
+_8_7 # Example 
+_8_8 # key to insert AB 
+_8_9 # tested = 2 
+_9_0 # ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
+_9_1 # ┃ current ┃->┃ next node ┃ 
+_9_2 # ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
+_9_3 # ┃ len=4 ┃ ┃ len=5 ┃ 
+_9_4 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_9_5 # Result : 
+_9_6 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
+_9_7 # ┃ current ┃->┃ node1 ┃->┃ next node ┃ 
+_9_8 # ┃ key=AB ┃ ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
+_9_9 # ┃ len=2 ┃ ┃ len=4 ┃ ┃ len=5 ┃ 
+_1_0_0 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_1_0_1 
+_1_0_2 cont = Container(data=val, tag=0) 
+_1_0_3 node1 = Node(current._key, current._key_size, None) 
+_1_0_4 node1._next = current._next.copy() 
+_1_0_5 node1._data = current._data 
+_1_0_6 
+_1_0_7 current._key_size = len(key) 
+_1_0_8 current._next[current._key[tested]] = node1 
+_1_0_9 current._key = key 
+_1_1_0 current._data = cont 
+_1_1_1 
+_1_1_2 my_logger.debug(current) 
+_1_1_3 my_logger.debug(node1) 
+_1_1_4 
+_1_1_5 return cont 
+_1_1_6 
+_1_1_7 elif current._key[tested] != key[tested]: 
+_1_1_8 """ 
+_1_1_9 Creation of two new nodes and one container for data 
+_1_2_0 """ 
+_1_2_1 # Example 
+_1_2_2 # key to insert AC 
+_1_2_3 # tested = 1 
+_1_2_4 # ┏━━━━━━━━━━━━┓ ┏━━━━━━━━━━━━┓ 
+_1_2_5 # ┃ current ┃->┃ next node ┃ 
+_1_2_6 # ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
+_1_2_7 # ┃ len=4 ┃ ┃ len=5 ┃ 
+_1_2_8 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_1_2_9 # Result : 
+_1_3_0 # ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ ┏━━━━━━━━━━━━┓ 
+_1_3_1 # ┃ current ┃->┃ node1 ┃->┃ next node ┃ 
+_1_3_2 # ┃ key=A ┃ ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
+_1_3_3 # ┃ len=1 ┃ ┃ len=4 ┃ ┃ len=5 ┃ 
+_1_3_4 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_1_3_5 # │ C ┏━━━━━━━━━━━━┓ 
+_1_3_6 # +-------->┃ node2 ┃ 
+_1_3_7 # ┃ key=AC ┃ 
+_1_3_8 # ┃ len=2 ┃ 
+_1_3_9 # ┗━━━━━━━━━━━━┛ 
+_1_4_0 cont = Container(data=val, tag=0) 
+_1_4_1 node1 = Node(current._key, current._key_size, None) 
+_1_4_2 node1._next = current._next.copy() 
+_1_4_3 node1._data = current._data 
+_1_4_4 node2 = Node(key, len(key), cont) 
+_1_4_5 
+_1_4_6 current._key_size = tested 
+_1_4_7 # for k in current._next: 
+_1_4_8 # del current._next[k] 
+_1_4_9 current._next = {} 
+_1_5_0 current._next[current._key[tested]] = node1 
+_1_5_1 current._next[key[tested]] = node2 
+_1_5_2 current._key = key[0:tested] 
+_1_5_3 current._data = None 
+_1_5_4 
+_1_5_5 my_logger.debug(current) 
+_1_5_6 my_logger.debug(node1) 
+_1_5_7 my_logger.debug(node2) 
+_1_5_8 
+_1_5_9 return cont 
+_1_6_0 tested += 1 
+_1_6_1 
+_1_6_2 if tested == current._key_size: 
+_1_6_3 if tested < len(key): 
+_1_6_4 """Go to the next node""" 
+_1_6_5 if key[tested] in current._next: 
+_1_6_6 current = current._next[key[tested]] 
+_1_6_7 my_logger.debug("Go to the next node: %s" % current) 
+_1_6_8 self.insert_node(key, val, current) 
+_1_6_9 else: 
+_1_7_0 """Create the new node""" 
+_1_7_1 # Example 
+_1_7_2 # key to insert ABABA 
+_1_7_3 # tested = 4 
+_1_7_4 # ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
+_1_7_5 # ┃ current ┃->┃ ┃ 
+_1_7_6 # ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
+_1_7_7 # ┃ len=4 ┃ ┃ len=5 ┃ 
+_1_7_8 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_1_7_9 # Result : 
+_1_8_0 # ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
+_1_8_1 # ┃ current ┃->┃ ┃ 
+_1_8_2 # ┃ key=ABAB ┃ ┃ key=ABABB ┃ 
+_1_8_3 # ┃ len=4 ┃ ┃ len=5 ┃ 
+_1_8_4 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_1_8_5 # │ A ┏━━━━━━━━━━━━┓ 
+_1_8_6 # +-------->┃ node ┃ 
+_1_8_7 # ┃ key=ABABA ┃ 
+_1_8_8 # ┃ len=5 ┃ 
+_1_8_9 # ┗━━━━━━━━━━━━┛ 
+_1_9_0 
+_1_9_1 cont = Container(data=val, tag=0) 
+_1_9_2 node = Node(key, len(key), cont) 
+_1_9_3 current._next[key[tested]] = node 
+_1_9_4 my_logger.debug("Create the next node: %s" % node) 
+_1_9_5 my_logger.debug("Modify the current node: %s" % current) 
+_1_9_6 return cont 
+_1_9_7 else: 
+_1_9_8 """The leaf already exists, we have to update container""" 
+_1_9_9 my_logger.debug("The leaf already exists, we have to update container node:
 %s" % current) 
-_1_9_9 current._key = key 
-_2_0_0 current._key_size = len(key) 
-_2_0_1 cont = current._data 
-_2_0_2 if cont: 
-_2_0_3 """Update container""" 
-_2_0_4 cont._data = val 
-_2_0_5 my_logger.debug("Node already exist. Update container: %s" % current) 
-_2_0_6 else: 
-_2_0_7 """Create container""" 
-_2_0_8 my_logger.debug("Node already exist. Create container: %s" % current) 
-_2_0_9 cont = Container(data=val, tag=0) 
-_2_1_0 current._data = cont 
-_2_1_1 return cont 
-_2_1_2 
-_2_1_3 def get_node(self, key, start_node=None): 
-_2_1_4 """ 
-_2_1_5 Get node in the radix tree beginning to <start_node> indexed by <key> 
-_2_1_6 :param start_node: first node of the radix tree to explore 
-_2_1_7 :param key: key to search 
-_2_1_8 :return: data linked to the node, if any. None otherwise 
-_2_1_9 """ 
-_2_2_0 
-_2_2_1 my_logger.debug(" RadixTree.get_node() ".center(60, '-')) 
-_2_2_2 
-_2_2_3 if type(key) != str: 
-_2_2_4 key = bin(key).replace('0b', '') 
-_2_2_5 my_logger.debug("Key converted in string key: %s " % key) 
-_2_2_6 
-_2_2_7 my_logger.debug("key: %s" % key) 
-_2_2_8 
-_2_2_9 if start_node == None: 
-_2_3_0 node = self._tree 
-_2_3_1 else: 
-_2_3_2 node = start_node 
-_2_3_3 
-_2_3_4 if node: 
-_2_3_5 my_logger.info("Current node: %s" % node) 
-_2_3_6 if node._key == key and node._key_size == len(node._key): 
-_2_3_7 my_logger.info("Node found -> key: %s key_size: %d data: %s" % (node._key,
+_2_0_0 current._key = key 
+_2_0_1 current._key_size = len(key) 
+_2_0_2 cont = current._data 
+_2_0_3 if cont: 
+_2_0_4 """Update container""" 
+_2_0_5 cont._data = val 
+_2_0_6 my_logger.debug("Node already exist. Update container: %s" % current) 
+_2_0_7 else: 
+_2_0_8 """Create container""" 
+_2_0_9 my_logger.debug("Node already exist. Create container: %s" % current) 
+_2_1_0 cont = Container(data=val, tag=0) 
+_2_1_1 current._data = cont 
+_2_1_2 return cont 
+_2_1_3 
+_2_1_4 def get_node(self, key, start_node=None): 
+_2_1_5 """ 
+_2_1_6 Get node in the radix tree beginning to <start_node> indexed by <key> 
+_2_1_7 :param start_node: first node of the radix tree to explore 
+_2_1_8 :param key: key to search 
+_2_1_9 :return: data linked to the node, if any. None otherwise 
+_2_2_0 """ 
+_2_2_1 
+_2_2_2 my_logger.debug(" RadixTree.get_node() ".center(60, '-')) 
+_2_2_3 
+_2_2_4 if type(key) != str: 
+_2_2_5 key = bin(key).replace('0b', '') 
+_2_2_6 my_logger.debug("Key converted in string key: %s " % key) 
+_2_2_7 
+_2_2_8 my_logger.debug("key: %s" % key) 
+_2_2_9 
+_2_3_0 if start_node == None: 
+_2_3_1 node = self._tree 
+_2_3_2 else: 
+_2_3_3 node = start_node 
+_2_3_4 
+_2_3_5 if node: 
+_2_3_6 my_logger.info("Current node: %s" % node) 
+_2_3_7 if node._key == key and node._key_size == len(node._key): 
+_2_3_8 my_logger.info("Node found -> key: %s key_size: %d data: %s" % (node._key,
 node._key_size, node._data)) 
-_2_3_8 return node._data 
-_2_3_9 else: 
-_2_4_0 tested = 0 
-_2_4_1 while tested < node._key_size: 
-_2_4_2 if tested > len(key) - 1: 
-_2_4_3 my_logger.warning("Node not found -> key: %s" % key) 
-_2_4_4 return None 
-_2_4_5 else: 
-_2_4_6 my_logger.debug("Searching node... current node: %s " % node) 
-_2_4_7 my_logger.debug( 
-_2_4_8 "Searching node... index: %d tested: %s - %s" % (tested, node._key[tested],
+_2_3_9 return node._data 
+_2_4_0 else: 
+_2_4_1 tested = 0 
+_2_4_2 while tested < node._key_size: 
+_2_4_3 if tested > len(key) - 1: 
+_2_4_4 my_logger.warning("Node not found -> key: %s" % key) 
+_2_4_5 return None 
+_2_4_6 else: 
+_2_4_7 my_logger.debug("Searching node... current node: %s " % node) 
+_2_4_8 my_logger.debug( 
+_2_4_9 "Searching node... index: %d tested: %s - %s" % (tested, node._key[tested],
 key[tested])) 
-_2_4_9 if node._key[tested] != key[tested]: 
-_2_5_0 my_logger.warning("Node not found -> key: %s" % key) 
-_2_5_1 return None 
-_2_5_2 else: 
-_2_5_3 tested += 1 
-_2_5_4 
-_2_5_5 if tested == node._key_size: 
-_2_5_6 if key[tested] in node._next: 
-_2_5_7 node = node._next[key[tested]] 
-_2_5_8 my_logger.info("2 Go to the next node -> next: %s node: %s" % (node._key
+_2_5_0 if node._key[tested] != key[tested]: 
+_2_5_1 my_logger.warning("Node not found -> key: %s" % key) 
+_2_5_2 return None 
+_2_5_3 else: 
+_2_5_4 tested += 1 
+_2_5_5 
+_2_5_6 if tested == node._key_size: 
+_2_5_7 if key[tested] in node._next: 
+_2_5_8 node = node._next[key[tested]] 
+_2_5_9 my_logger.info("2 Go to the next node -> next: %s node: %s" % (node._key
 [tested], node)) 
-_2_5_9 return self.get_node(key, node) 
-_2_6_0 else: 
-_2_6_1 my_logger.warning("Node not found -> key: %s" % key) 
-_2_6_2 return None 
-_2_6_3 else: 
-_2_6_4 my_logger.info("Radix tree empty") 
-_2_6_5 return None 
-_2_6_6 
-_2_6_7 def delete_node(self, key, start_node=None, prev_node=None): 
-_2_6_8 """ 
-_2_6_9 Delete node in radix tree 
-_2_7_0 :param key: key of the node to delete 
-_2_7_1 :param start_node: first node of the radix tree or None to start from the
+_2_6_0 return self.get_node(key, node) 
+_2_6_1 else: 
+_2_6_2 my_logger.warning("Node not found -> key: %s" % key) 
+_2_6_3 return None 
+_2_6_4 else: 
+_2_6_5 my_logger.info("Radix tree empty") 
+_2_6_6 return None 
+_2_6_7 
+_2_6_8 def delete_node(self, key, start_node=None, prev_node=None): 
+_2_6_9 """ 
+_2_7_0 Delete node in radix tree 
+_2_7_1 :param key: key of the node to delete 
+_2_7_2 :param start_node: first node of the radix tree or None to start from the
 beginning of radix tree 
-_2_7_2 :param prev_node: previous node 
-_2_7_3 :return: True if deleted. False otherwise. 
-_2_7_4 """ 
-_2_7_5 
-_2_7_6 my_logger.debug(" RadixTree.delete_node() ".center(60, '-')) 
-_2_7_7 
-_2_7_8 if type(key) != str: 
-_2_7_9 key = bin(key).replace('0b', '') 
-_2_8_0 my_logger.debug("Key converted in string key: %s " % key) 
-_2_8_1 
-_2_8_2 my_logger.debug(" Key : %s" % key) 
-_2_8_3 
-_2_8_4 if start_node == None: 
-_2_8_5 node = self._tree 
-_2_8_6 else: 
-_2_8_7 node = start_node 
-_2_8_8 
-_2_8_9 my_logger.info("Current node -> %s" % node) 
-_2_9_0 
-_2_9_1 if node: 
-_2_9_2 if node._key == key: 
-_2_9_3 # Node to delete found 
-_2_9_4 my_logger.debug("Node to delete found -> %s" % node) 
-_2_9_5 if len(node._next) == 0: 
-_2_9_6 if prev_node == None: 
-_2_9_7 my_logger.debug("First node of tree deleted -> Radix tree empty") 
-_2_9_8 del self._tree 
-_2_9_9 self._tree = None 
-_3_0_0 return True 
-_3_0_1 else: 
-_3_0_2 # Example 
-_3_0_3 # Delete 'ABA' 
-_3_0_4 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━┓ 
-_3_0_5 # ┃ prev_node ┃->┃ node ┃ 
-_3_0_6 # ┃ key=AB ┃ ┃ key=ABA ┃ 
-_3_0_7 # ┃ len=2 ┃ ┃ len=3 ┃ 
-_3_0_8 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━┛ 
-_3_0_9 # Result : 
-_3_1_0 # ┏━━━━━━━━━━━━┓ 
-_3_1_1 # ┃ prev_node ┃ 
-_3_1_2 # ┃ key=AB ┃ 
-_3_1_3 # ┃ len=2 ┃ 
-_3_1_4 # ┗━━━━━━━━━━━━┛ 
-_3_1_5 
-_3_1_6 my_logger.debug("Node deleted %s " % node) 
-_3_1_7 my_logger.debug("Previous link deleted %s " % prev_node) 
-_3_1_8 del prev_node._next[node._key[prev_node._key_size]] 
-_3_1_9 my_logger.debug("1. Previous node updated %s " % prev_node) 
-_3_2_0 
-_3_2_1 if len(prev_node._next) == 1 and prev_node._data == None: 
-_3_2_2 # Example 
-_3_2_3 # Delete 'ABB' 
-_3_2_4 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━┓ 
-_3_2_5 # ┃ prev_node ┃->┃ node ┃ 
-_3_2_6 # ┃ key=AB ┃ ┃ key=ABA ┃ 
-_3_2_7 # ┃ len=2 ┃ ┃ len=3 ┃ 
-_3_2_8 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━┛ 
-_3_2_9 # │ B ┏━━━━━━━━━━━━┓ 
-_3_3_0 # +-------->┃ other node ┃ 
-_3_3_1 # ┃ key=ABB ┃ 
-_3_3_2 # ┃ len=3 ┃ 
-_3_3_3 # ┗━━━━━━━━━━━━┛ 
-_3_3_4 # Result : 
-_3_3_5 # ┏━━━━━━━━━━━━┓ 
-_3_3_6 # ┃ prev_node ┃ 
-_3_3_7 # ┃ key=ABA ┃ 
-_3_3_8 # ┃ len=3 ┃ 
-_3_3_9 # ┗━━━━━━━━━━━━┛ 
-_3_4_0 for k in prev_node._next: 
-_3_4_1 prev_node._key = prev_node._next[k]._key 
-_3_4_2 prev_node._key_size = prev_node._next[k]._key_size 
-_3_4_3 prev_node._data = prev_node._next[k]._data 
-_3_4_4 prev_node._next = prev_node._next[k]._next 
-_3_4_5 my_logger.debug("2. Previous node updated %s " % prev_node) 
-_3_4_6 
-_3_4_7 del node._data 
-_3_4_8 del node 
-_3_4_9 return True 
-_3_5_0 else: 
-_3_5_1 if len(node._next) == 1: 
-_3_5_2 # Example 
-_3_5_3 # Delete 'ABA' 
-_3_5_4 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
-_3_5_5 # ┃ prev_node ┃->┃ node ┃->┃ next_node ┃ 
-_3_5_6 # ┃ key=AB ┃ ┃ key=ABA ┃ ┃ key=ABAB ┃ 
-_3_5_7 # ┃ len=2 ┃ ┃ len=3 ┃ ┃ len=4 ┃ 
-_3_5_8 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_3_5_9 # Result : 
-_3_6_0 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓ 
-_3_6_1 # ┃ prev_node ┃->┃ node ┃ 
-_3_6_2 # ┃ key=AB ┃ ┃ key=ABAB ┃ 
-_3_6_3 # ┃ len=2 ┃ ┃ len=4 ┃ 
-_3_6_4 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_3_6_5 for ke in node._next: 
-_3_6_6 next_node = node._next[ke] 
-_3_6_7 my_logger.info("Node to update %s " % node) 
-_3_6_8 node._key = next_node._key 
-_3_6_9 node._key_size = next_node._key_size 
-_3_7_0 node._data = next_node._data 
-_3_7_1 node._next = next_node._next.copy() 
-_3_7_2 my_logger.info("Node updated %s " % node) 
-_3_7_3 my_logger.info("Node deleted %s " % next_node) 
-_3_7_4 del next_node._data 
-_3_7_5 del next_node 
-_3_7_6 return True 
-_3_7_7 else: 
-_3_7_8 # Example 
-_3_7_9 # Delete 'ABA' 
-_3_8_0 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
-_3_8_1 # ┃ prev_node ┃->┃ node ┃->┃ next_node1 ┃ 
-_3_8_2 # ┃ key=AB ┃ ┃ key=ABA ┃ ┃ key=ABAB ┃ 
-_3_8_3 # ┃ len=2 ┃ ┃ len=3 ┃ ┃ len=4 ┃ 
-_3_8_4 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_3_8_5 # │ C ┏━━━━━━━━━━━━┓ 
-_3_8_6 # +-------->┃ next_nodei ┃ 
-_3_8_7 # ┃ key=ABAC ┃ 
-_3_8_8 # ┃ len=4 ┃ 
-_3_8_9 # ┗━━━━━━━━━━━━┛ 
-_3_9_0 # Result : 
-_3_9_1 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
-_3_9_2 # ┃ prev_node ┃->┃ node ┃->┃ next_node1 ┃ 
-_3_9_3 # ┃ key=AB ┃ ┃ key=ABA ┃ ┃ key=ABAB ┃ 
-_3_9_4 # ┃ len=2 ┃ ┃ len=3 ┃ ┃ len=4 ┃ 
-_3_9_5 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
-_3_9_6 # │ C ┏━━━━━━━━━━━━┓ 
-_3_9_7 # +-------->┃ next_nodei ┃ 
-_3_9_8 # ┃ key=ABAC ┃ 
-_3_9_9 # ┃ len=4 ┃ 
-_4_0_0 # ┗━━━━━━━━━━━━┛ 
-_4_0_1 # In this case, just delete data linked to the node 
-_4_0_2 del node._data 
-_4_0_3 node._data = None 
-_4_0_4 my_logger.info("Just delete data linked to the node %s " % node) 
-_4_0_5 return True 
-_4_0_6 else: 
-_4_0_7 # Other node case 
-_4_0_8 tested = 0 
-_4_0_9 while tested < node._key_size: 
-_4_1_0 if tested > len(key) - 1: 
-_4_1_1 my_logger.warning("Node not found -> key: %s" % key) 
-_4_1_2 return False 
-_4_1_3 else: 
-_4_1_4 my_logger.debug("Searching node... current node: %s " % node) 
-_4_1_5 my_logger.debug( 
-_4_1_6 "Searching node... index: %d tested: %s - %s" % (tested, node._key[tested],
+_2_7_3 :param prev_node: previous node 
+_2_7_4 :return: True if deleted. False otherwise. 
+_2_7_5 """ 
+_2_7_6 
+_2_7_7 my_logger.debug(" RadixTree.delete_node() ".center(60, '-')) 
+_2_7_8 
+_2_7_9 if type(key) != str: 
+_2_8_0 key = bin(key).replace('0b', '') 
+_2_8_1 my_logger.debug("Key converted in string key: %s " % key) 
+_2_8_2 
+_2_8_3 my_logger.debug(" Key : %s" % key) 
+_2_8_4 
+_2_8_5 if start_node == None: 
+_2_8_6 node = self._tree 
+_2_8_7 else: 
+_2_8_8 node = start_node 
+_2_8_9 
+_2_9_0 my_logger.info("Current node -> %s" % node) 
+_2_9_1 
+_2_9_2 if node: 
+_2_9_3 if node._key == key: 
+_2_9_4 # Node to delete found 
+_2_9_5 my_logger.debug("Node to delete found -> %s" % node) 
+_2_9_6 if len(node._next) == 0: 
+_2_9_7 if prev_node == None: 
+_2_9_8 my_logger.debug("First node of tree deleted -> Radix tree empty") 
+_2_9_9 del self._tree 
+_3_0_0 self._tree = None 
+_3_0_1 return True 
+_3_0_2 else: 
+_3_0_3 # Example 
+_3_0_4 # Delete 'ABA' 
+_3_0_5 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━┓ 
+_3_0_6 # ┃ prev_node ┃->┃ node ┃ 
+_3_0_7 # ┃ key=AB ┃ ┃ key=ABA ┃ 
+_3_0_8 # ┃ len=2 ┃ ┃ len=3 ┃ 
+_3_0_9 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━┛ 
+_3_1_0 # Result : 
+_3_1_1 # ┏━━━━━━━━━━━━┓ 
+_3_1_2 # ┃ prev_node ┃ 
+_3_1_3 # ┃ key=AB ┃ 
+_3_1_4 # ┃ len=2 ┃ 
+_3_1_5 # ┗━━━━━━━━━━━━┛ 
+_3_1_6 
+_3_1_7 my_logger.debug("Node deleted %s " % node) 
+_3_1_8 my_logger.debug("Previous link deleted %s " % prev_node) 
+_3_1_9 del prev_node._next[node._key[prev_node._key_size]] 
+_3_2_0 my_logger.debug("1. Previous node updated %s " % prev_node) 
+_3_2_1 
+_3_2_2 if len(prev_node._next) == 1 and prev_node._data == None: 
+_3_2_3 # Example 
+_3_2_4 # Delete 'ABB' 
+_3_2_5 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━┓ 
+_3_2_6 # ┃ prev_node ┃->┃ node ┃ 
+_3_2_7 # ┃ key=AB ┃ ┃ key=ABA ┃ 
+_3_2_8 # ┃ len=2 ┃ ┃ len=3 ┃ 
+_3_2_9 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━┛ 
+_3_3_0 # │ B ┏━━━━━━━━━━━━┓ 
+_3_3_1 # +-------->┃ other node ┃ 
+_3_3_2 # ┃ key=ABB ┃ 
+_3_3_3 # ┃ len=3 ┃ 
+_3_3_4 # ┗━━━━━━━━━━━━┛ 
+_3_3_5 # Result : 
+_3_3_6 # ┏━━━━━━━━━━━━┓ 
+_3_3_7 # ┃ prev_node ┃ 
+_3_3_8 # ┃ key=ABA ┃ 
+_3_3_9 # ┃ len=3 ┃ 
+_3_4_0 # ┗━━━━━━━━━━━━┛ 
+_3_4_1 for k in prev_node._next: 
+_3_4_2 prev_node._key = prev_node._next[k]._key 
+_3_4_3 prev_node._key_size = prev_node._next[k]._key_size 
+_3_4_4 prev_node._data = prev_node._next[k]._data 
+_3_4_5 prev_node._next = prev_node._next[k]._next 
+_3_4_6 my_logger.debug("2. Previous node updated %s " % prev_node) 
+_3_4_7 
+_3_4_8 del node._data 
+_3_4_9 del node 
+_3_5_0 return True 
+_3_5_1 else: 
+_3_5_2 if len(node._next) == 1: 
+_3_5_3 # Example 
+_3_5_4 # Delete 'ABA' 
+_3_5_5 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
+_3_5_6 # ┃ prev_node ┃->┃ node ┃->┃ next_node ┃ 
+_3_5_7 # ┃ key=AB ┃ ┃ key=ABA ┃ ┃ key=ABAB ┃ 
+_3_5_8 # ┃ len=2 ┃ ┃ len=3 ┃ ┃ len=4 ┃ 
+_3_5_9 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_3_6_0 # Result : 
+_3_6_1 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓ 
+_3_6_2 # ┃ prev_node ┃->┃ node ┃ 
+_3_6_3 # ┃ key=AB ┃ ┃ key=ABAB ┃ 
+_3_6_4 # ┃ len=2 ┃ ┃ len=4 ┃ 
+_3_6_5 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_3_6_6 for ke in node._next: 
+_3_6_7 next_node = node._next[ke] 
+_3_6_8 my_logger.info("Node to update %s " % node) 
+_3_6_9 node._key = next_node._key 
+_3_7_0 node._key_size = next_node._key_size 
+_3_7_1 node._data = next_node._data 
+_3_7_2 node._next = next_node._next.copy() 
+_3_7_3 my_logger.info("Node updated %s " % node) 
+_3_7_4 my_logger.info("Node deleted %s " % next_node) 
+_3_7_5 del next_node._data 
+_3_7_6 del next_node 
+_3_7_7 return True 
+_3_7_8 else: 
+_3_7_9 # Example 
+_3_8_0 # Delete 'ABA' 
+_3_8_1 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
+_3_8_2 # ┃ prev_node ┃->┃ node ┃->┃ next_node1 ┃ 
+_3_8_3 # ┃ key=AB ┃ ┃ key=ABA ┃ ┃ key=ABAB ┃ 
+_3_8_4 # ┃ len=2 ┃ ┃ len=3 ┃ ┃ len=4 ┃ 
+_3_8_5 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_3_8_6 # │ C ┏━━━━━━━━━━━━┓ 
+_3_8_7 # +-------->┃ next_nodei ┃ 
+_3_8_8 # ┃ key=ABAC ┃ 
+_3_8_9 # ┃ len=4 ┃ 
+_3_9_0 # ┗━━━━━━━━━━━━┛ 
+_3_9_1 # Result : 
+_3_9_2 # ┏━━━━━━━━━━━━┓A ┏━━━━━━━━━━━━┓B ┏━━━━━━━━━━━━┓ 
+_3_9_3 # ┃ prev_node ┃->┃ node ┃->┃ next_node1 ┃ 
+_3_9_4 # ┃ key=AB ┃ ┃ key=ABA ┃ ┃ key=ABAB ┃ 
+_3_9_5 # ┃ len=2 ┃ ┃ len=3 ┃ ┃ len=4 ┃ 
+_3_9_6 # ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ ┗━━━━━━━━━━━━┛ 
+_3_9_7 # │ C ┏━━━━━━━━━━━━┓ 
+_3_9_8 # +-------->┃ next_nodei ┃ 
+_3_9_9 # ┃ key=ABAC ┃ 
+_4_0_0 # ┃ len=4 ┃ 
+_4_0_1 # ┗━━━━━━━━━━━━┛ 
+_4_0_2 # In this case, just delete data linked to the node 
+_4_0_3 del node._data 
+_4_0_4 node._data = None 
+_4_0_5 my_logger.info("Just delete data linked to the node %s " % node) 
+_4_0_6 return True 
+_4_0_7 else: 
+_4_0_8 # Other node case 
+_4_0_9 tested = 0 
+_4_1_0 while tested < node._key_size: 
+_4_1_1 if tested > len(key) - 1: 
+_4_1_2 my_logger.warning("Node not found -> key: %s" % key) 
+_4_1_3 return False 
+_4_1_4 else: 
+_4_1_5 my_logger.debug("Searching node... current node: %s " % node) 
+_4_1_6 my_logger.debug( 
+_4_1_7 "Searching node... index: %d tested: %s - %s" % (tested, node._key[tested],
 key[tested])) 
-_4_1_7 if node._key[tested] != key[tested]: 
-_4_1_8 my_logger.warning("Node not found -> key: %s" % key) 
-_4_1_9 return False 
-_4_2_0 else: 
-_4_2_1 tested += 1 
-_4_2_2 
-_4_2_3 if tested == node._key_size: 
-_4_2_4 if key[tested] in node._next: 
-_4_2_5 prev_node = node 
-_4_2_6 node = node._next[key[tested]] 
-_4_2_7 my_logger.info("Go to the next node -> next: %s node: %s" % (node._key
+_4_1_8 if node._key[tested] != key[tested]: 
+_4_1_9 my_logger.warning("Node not found -> key: %s" % key) 
+_4_2_0 return False 
+_4_2_1 else: 
+_4_2_2 tested += 1 
+_4_2_3 
+_4_2_4 if tested == node._key_size: 
+_4_2_5 if key[tested] in node._next: 
+_4_2_6 prev_node = node 
+_4_2_7 node = node._next[key[tested]] 
+_4_2_8 my_logger.info("Go to the next node -> next: %s node: %s" % (node._key
 [tested], node)) 
-_4_2_8 ret = self.delete_node(key, node, prev_node) 
-_4_2_9 return ret 
-_4_3_0 else: 
-_4_3_1 my_logger.warning("Node not found -> key: %s" % key) 
-_4_3_2 return False 
-_4_3_3 else: 
-_4_3_4 my_logger.info("Radix tree empty") 
-_4_3_5 return False 
-_4_3_6 
-_4_3_7 def dump(self, node=None, st_next_line=''): 
-_4_3_8 """ 
-_4_3_9 Display a radix node 
-_4_4_0 :param node: first node of the radix tree. If node = None dump the entire
+_4_2_9 ret = self.delete_node(key, node, prev_node) 
+_4_3_0 return ret 
+_4_3_1 else: 
+_4_3_2 my_logger.warning("Node not found -> key: %s" % key) 
+_4_3_3 return False 
+_4_3_4 else: 
+_4_3_5 my_logger.info("Radix tree empty") 
+_4_3_6 return False 
+_4_3_7 
+_4_3_8 def dump(self, node=None, st_next_line=''): 
+_4_3_9 """ 
+_4_4_0 Display a radix node 
+_4_4_1 :param node: first node of the radix tree. If node = None dump the entire
 radix tree 
-_4_4_1 :param st_next_line: start of next line to display 
-_4_4_2 :return: None 
-_4_4_3 """ 
-_4_4_4 
-_4_4_5 my_logger.debug(" RadixTree.dump() ".center(60, '-')) 
-_4_4_6 
-_4_4_7 if not node: 
-_4_4_8 """Dump the entire radix tree""" 
-_4_4_9 node = self._tree 
-_4_5_0 if not node: 
-_4_5_1 print("Radix tree empty") 
-_4_5_2 return 
-_4_5_3 if node._data: 
-_4_5_4 line = "■" 
-_4_5_5 else: 
-_4_5_6 line = "□" 
-_4_5_7 line += " key: %s key_len: %d next: %d" % (node._key, node._key_size, len
+_4_4_2 :param st_next_line: start of next line to display 
+_4_4_3 :return: None 
+_4_4_4 """ 
+_4_4_5 
+_4_4_6 my_logger.debug(" RadixTree.dump() ".center(60, '-')) 
+_4_4_7 
+_4_4_8 if not node: 
+_4_4_9 """Dump the entire radix tree""" 
+_4_5_0 node = self._tree 
+_4_5_1 if not node: 
+_4_5_2 print("Radix tree empty") 
+_4_5_3 return 
+_4_5_4 if node._data: 
+_4_5_5 line = "■" 
+_4_5_6 else: 
+_4_5_7 line = "□" 
+_4_5_8 line += " key: %s key_len: %d next: %d" % (node._key, node._key_size, len
 (node._next)) 
-_4_5_8 if node._data: 
-_4_5_9 line += " data: %s" % node._data 
-_4_6_0 print(line) 
-_4_6_1 cpt = len(node._next) - 1 
-_4_6_2 st_next_line = "│" * cpt 
-_4_6_3 for item in node._next: 
-_4_6_4 self.dump(node._next[item], st_next_line) 
-_4_6_5 cpt -= 1 
-_4_6_6 st_next_line = st_next_line[0:cpt] 
-_4_6_7 else: 
-_4_6_8 """Intermediate node""" 
-_4_6_9 line = st_next_line 
-_4_7_0 if node._data: 
-_4_7_1 line += "└■" 
-_4_7_2 else: 
-_4_7_3 line += "└□" 
-_4_7_4 line += " key: %s key_len: %d next: %d" % (node._key, node._key_size, len
+_4_5_9 if node._data: 
+_4_6_0 line += " data: %s" % node._data 
+_4_6_1 print(line) 
+_4_6_2 cpt = len(node._next) - 1 
+_4_6_3 st_next_line = "│" * cpt 
+_4_6_4 for item in node._next: 
+_4_6_5 self.dump(node._next[item], st_next_line) 
+_4_6_6 cpt -= 1 
+_4_6_7 st_next_line = st_next_line[0:cpt] 
+_4_6_8 else: 
+_4_6_9 """Intermediate node""" 
+_4_7_0 line = st_next_line 
+_4_7_1 if node._data: 
+_4_7_2 line += "└■" 
+_4_7_3 else: 
+_4_7_4 line += "└□" 
+_4_7_5 line += " key: %s key_len: %d next: %d" % (node._key, node._key_size, len
 (node._next)) 
-_4_7_5 if node._data: 
-_4_7_6 line += " data: %s" % node._data 
-_4_7_7 print(line) 
-_4_7_8 cpt = len(node._next) - 1 
-_4_7_9 if cpt > 1: 
-_4_8_0 st_next_line = st_next_line + " │" + "│" * (cpt - 1) 
-_4_8_1 if cpt == 1: 
-_4_8_2 my_logger.debug("node with only one son: %s" % node) 
-_4_8_3 st_next_line = st_next_line + " │" 
-_4_8_4 
-_4_8_5 for item in node._next: 
-_4_8_6 self.dump(node._next[item], st_next_line) 
-_4_8_7 l = len(st_next_line) - 1 
-_4_8_8 st_next_line = st_next_line[0:l] 
+_4_7_6 if node._data: 
+_4_7_7 line += " data: %s" % node._data 
+_4_7_8 print(line) 
+_4_7_9 cpt = len(node._next) - 1 
+_4_8_0 if cpt > 1: 
+_4_8_1 st_next_line = st_next_line + " │" + "│" * (cpt - 1) 
+_4_8_2 if cpt == 1: 
+_4_8_3 my_logger.debug("node with only one son: %s" % node) 
+_4_8_4 st_next_line = st_next_line + " │" 
+_4_8_5 
+_4_8_6 for item in node._next: 
+_4_8_7 self.dump(node._next[item], st_next_line) 
+_4_8_8 l = len(st_next_line) - 1 
+_4_8_9 st_next_line = st_next_line[0:l] 
 _«_ _p_r_e_v     _&_H_a_t_;_ _i_n_d_e_x     _»_ _n_e_x_t       _c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-
-04 18:19 +0200
+06 10:57 +0200
```

### Comparing `radix_tree-0.0.1/htmlcov/favicon_32.png` & `radix_tree-0.0.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/htmlcov/index.html` & `radix_tree-0.0.2/htmlcov/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     <link rel="stylesheet" href="style.css" type="text/css">
     <script type="text/javascript" src="coverage_html.js" defer></script>
 </head>
 <body class="indexfile">
 <header>
     <div class="content">
         <h1>Coverage report:
-            <span class="pc_cov">12%</span>
+            <span class="pc_cov">99%</span>
         </h1>
         <aside id="help_panel_wrapper">
             <input id="help_panel_state" type="checkbox">
             <label for="help_panel_state">
                 <img id="keyboard_icon" src="keybd_closed.png" alt="Show/hide keyboard shortcuts" />
             </label>
             <div id="help_panel">
@@ -41,15 +41,15 @@
             </div>
         </aside>
         <form id="filter_container">
             <input id="filter" type="text" value="" placeholder="filter..." />
         </form>
         <p class="text">
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-04 18:19 +0200
+            created at 2024-04-06 10:57 +0200
         </p>
     </div>
 </header>
 <main id="index">
     <table class="index" data-sortable>
         <thead>
             <tr class="tablehead" title="Click to sort">
@@ -74,38 +74,38 @@
                 <td>2</td>
                 <td>0</td>
                 <td class="right" data-ratio="29 31">94%</td>
             </tr>
             <tr class="file">
                 <td class="name left"><a href="d_a370a513ee95d9c9_radix_tree_py.html">src/radix_tree/radix_tree.py</a></td>
                 <td>238</td>
-                <td>237</td>
                 <td>0</td>
-                <td class="right" data-ratio="1 238">1%</td>
+                <td>0</td>
+                <td class="right" data-ratio="238 238">100%</td>
             </tr>
         </tbody>
         <tfoot>
             <tr class="total">
                 <td class="name left">Total</td>
                 <td>271</td>
-                <td>239</td>
+                <td>2</td>
                 <td>0</td>
-                <td class="right" data-ratio="32 271">12%</td>
+                <td class="right" data-ratio="269 271">99%</td>
             </tr>
         </tfoot>
     </table>
     <p id="no_rows">
         No items found using the specified filter.
     </p>
 </main>
 <footer>
     <div class="content">
         <p>
             <a class="nav" href="https://coverage.readthedocs.io/en/7.4.4">coverage.py v7.4.4</a>,
-            created at 2024-04-04 18:19 +0200
+            created at 2024-04-06 10:57 +0200
         </p>
     </div>
     <aside class="hidden">
         <a id="prevFileLink" class="nav" href="d_a370a513ee95d9c9_radix_tree_py.html"/>
         <a id="nextFileLink" class="nav" href="d_a370a513ee95d9c9___init___py.html"/>
         <button type="button" class="button_prev_file" data-shortcut="["/>
         <button type="button" class="button_next_file" data-shortcut="]"/>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-************ CCoovveerraaggee rreeppoorrtt:: 1122%% ************
+************ CCoovveerraaggee rreeppoorrtt:: 9999%% ************
 ??[Show/hide keyboard shortcuts]
 Shortcuts on this page
 n s m x c   change column sorting
 [ ]   prev/next file
 ?   show/hide this help
 [                    ]
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-04 18:19 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-06 10:57 +0200
 MMoodduullee                         ssttaatteemmeennttss mmiissssiinngg eexxcclluuddeedd ccoovveerraaggee
 _s_r_c_/_r_a_d_i_x___t_r_e_e_/_____i_n_i_t_____._p_y     2          0       0        100%
 _s_r_c_/_r_a_d_i_x___t_r_e_e_/_r_a_d_i_x___c_o_n_f_i_g_._p_y 31         2       0        94%
-_s_r_c_/_r_a_d_i_x___t_r_e_e_/_r_a_d_i_x___t_r_e_e_._p_y   238        237     0        1%
-Total                          271        239     0        12%
+_s_r_c_/_r_a_d_i_x___t_r_e_e_/_r_a_d_i_x___t_r_e_e_._p_y   238        0       0        100%
+Total                          271        2       0        99%
 No items found using the specified filter.
-_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-04 18:19 +0200
+_c_o_v_e_r_a_g_e_._p_y_ _v_7_._4_._4, created at 2024-04-06 10:57 +0200
```

### Comparing `radix_tree-0.0.1/htmlcov/keybd_closed.png` & `radix_tree-0.0.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/htmlcov/keybd_open.png` & `radix_tree-0.0.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/htmlcov/style.css` & `radix_tree-0.0.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/src/radix_tree/radix_config.py` & `radix_tree-0.0.2/src/radix_tree/radix_config.py`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/src/radix_tree/radix_tree.py` & `radix_tree-0.0.2/src/radix_tree/radix_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 # run tests from Pycharms locally
-from radix_config import my_logger
+#from radix_config import my_logger
 
 # run tests from external Testpy as distributed package
-#from radix_tree.radix_config import my_logger
+from radix_tree.radix_config import my_logger
 
 class Container(object):
     """
     Container populated with data linked to a radic node
     """
 
     def __init__(self, data, tag=None):
```

### Comparing `radix_tree-0.0.1/src/radix_tree/.idea/workspace.xml` & `radix_tree-0.0.2/src/radix_tree/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `radix_tree-0.0.1/src/radix_tree/.idea/workspace.xml` & `radix_tree-0.0.2/src/radix_tree/.idea/workspace.xml`

```diff
@@ -1,14 +1,16 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="d41bdb0f-ad92-4c85-90fd-e9c1a447d9d5" name="Changes" comment="">
+      <change beforePath="$PROJECT_DIR$/../../pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/../../pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/__about__.py" beforeDir="false" afterPath="$PROJECT_DIR$/__about__.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/__init__.py" afterDir="false"/>
       <change beforePath="$PROJECT_DIR$/radix_tree.py" beforeDir="false" afterPath="$PROJECT_DIR$/radix_tree.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
@@ -34,15 +36,15 @@
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "Python tests.pytest in test_radix_tree.py.executor": "Run",
     "Python.radix_tree.executor": "Run",
     "Python.test_radix.executor": "Run",
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
-    "last_opened_file_path": "/data/Local_Data/python/hatch/radix_tree/tests",
+    "last_opened_file_path": "/data/Local_Data/python/hatch/radix_tree/pyproject.toml",
     "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyIntegratedToolsModulesConfigurable"
   }
 }]]></component>
   <component name="RunManager" selected="Python.test_radix">
     <configuration default="true" type="PythonConfigurationType" factoryName="Python">
       <module name="radix_tree"/>
       <option name="ENV_FILES" value=""/>
```

### Comparing `radix_tree-0.0.1/tests/.coverage` & `radix_tree-0.0.2/tests/.coverage`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/tests/test_radix_tree.py` & `radix_tree-0.0.2/tests/test_radix_tree.py`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/LICENSE.txt` & `radix_tree-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `radix_tree-0.0.1/pyproject.toml` & `radix_tree-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -26,17 +26,17 @@
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = []
 
 [project.urls]
-Documentation = "https://github.com/unknown/radix-tree#readme"
-Issues = "https://github.com/unknown/radix-tree/issues"
-Source = "https://github.com/unknown/radix-tree"
+Documentation = "https://github.com/Nicola-31/radix-tree#readme"
+Issues = "https://github.com/Nicola-31/radix-tree/issues"
+Source = "https://github.com/Nicola-31/radix-tree"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.git",
   "/.gitignore",
   "/.idea", 
 ]
```

### Comparing `radix_tree-0.0.1/PKG-INFO` & `radix_tree-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: radix_tree
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generic pure python radix tree implementation
-Project-URL: Documentation, https://github.com/unknown/radix-tree#readme
-Project-URL: Issues, https://github.com/unknown/radix-tree/issues
-Project-URL: Source, https://github.com/unknown/radix-tree
+Project-URL: Documentation, https://github.com/Nicola-31/radix-tree#readme
+Project-URL: Issues, https://github.com/Nicola-31/radix-tree/issues
+Project-URL: Source, https://github.com/Nicola-31/radix-tree
 Author-email: Nicolas Jeudy <nicola.jeudy@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: radix,tree
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
```

