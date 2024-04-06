# Comparing `tmp/score-eval-0.0.2.tar.gz` & `tmp/score_eval-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\workspace\scoreval\dist\tmptod__qw8\score-eval-0.0.2.tar", last modified: Wed May  4 08:40:38 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `score-eval-0.0.2.tar` & `score_eval-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-05-04 08:40:38.000000 score-eval-0.0.2/
--rw-rw-rw-   0        0        0     1087 2022-05-01 17:29:39.000000 score-eval-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2275 2022-05-04 08:40:38.000000 score-eval-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1683 2022-05-03 11:15:05.000000 score-eval-0.0.2/README.md
--rw-rw-rw-   0        0        0       95 2022-05-03 06:28:18.000000 score-eval-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      690 2022-05-04 08:40:38.000000 score-eval-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/
--rw-rw-rw-   0        0        0     2275 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/scoreval/
--rw-rw-rw-   0        0        0        0 2022-05-03 06:15:29.000000 score-eval-0.0.2/src/scoreval/__init__.py
--rw-rw-rw-   0        0        0    19608 2022-05-04 08:35:46.000000 score-eval-0.0.2/src/scoreval/scoreval.py
--rw-rw-rw-   0        0        0     2462 2022-05-04 08:36:58.000000 score-eval-0.0.2/src/scoreval/test.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 score_eval-0.0.3/.vscode/launch.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 score_eval-0.0.3/data/data_source.md
+-rw-r--r--   0        0        0   438307 2020-02-02 00:00:00.000000 score_eval-0.0.3/data/investing_program_prediction_data.csv
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 score_eval-0.0.3/src/score_eval.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 score_eval-0.0.3/src/score_eval.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 score_eval-0.0.3/src/score_eval.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 score_eval-0.0.3/src/score_eval.egg-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 score_eval-0.0.3/src/scoreval/__init__.py
+-rw-r--r--   0        0        0    25763 2020-02-02 00:00:00.000000 score_eval-0.0.3/src/scoreval/scoreval.py
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 score_eval-0.0.3/src/scoreval/test.py
+-rw-r--r--   0        0        0  1601637 2020-02-02 00:00:00.000000 score_eval-0.0.3/tests/score-eval-example-1.ipynb
+-rw-r--r--   0        0        0  1126730 2020-02-02 00:00:00.000000 score_eval-0.0.3/tests/score-eval-example.ipynb
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 score_eval-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 score_eval-0.0.3/README.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 score_eval-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 score_eval-0.0.3/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `score-eval-0.0.2/LICENSE` & `score_eval-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `score-eval-0.0.2/PKG-INFO` & `score_eval-0.0.3/src/score_eval.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `score-eval-0.0.2/README.md` & `score_eval-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `score-eval-0.0.2/src/score_eval.egg-info/PKG-INFO` & `score_eval-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,44 @@
-Metadata-Version: 2.1
-Name: score-eval
-Version: 0.0.2
-Summary: A visualization package for model score evaluation.
-Home-page: https://github.com/rexzhang2014/scoreval
-Author: Jingxiao Zhang
-Author-email: rex.zhang2016@foxmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/rexzhang2014/scoreval/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# scoreval
-An visulized evaluation toolkit for model score. 
-The model score will be evaluated static, on the full dataset. And further evaluate along date. 
-This aims to help machine learning modelers to evaluate the result effictively and efficiently. 
-## Effectiveness
-1. static method: on the full eval data set.
-    1. PR chart : average performance of the score.
-    2. WOE/IV : indicative power of score binning. 
-2. time method: metrics along date. 
-    1. QTL daily : show stability of the score
-    2. Precision daily: show target precision above a score cut-off.
-    3. Recall daily: show target coverage above a score cut-off.
-
-## Efficiency
-1. Predefined process & metrics: No need to design and analysis on metrics.
-2. Deal with multiple model scores: The tool will show charts for multiple model scores for comparison. 
-## Installation
-`pip install score-eval`
-# Input
-The input of this package include the below parts:
-- Model: a 'model' that implements the 'predict' method, it comes from most common used modeling tools like sklearn, tensorflow etc. The tool will definitely call model.predict() to get the score on the data set. 
-- Data set: a data set containing at least 3 columns (row_id, date, label), for calculating the metrics and by dates. If date does not appear, the time method will throw error during run. 
-
-# Output
-Pack of charts to evaluate and understand your model. See the link for more details:  
-https://github.com/rexzhang2014/scoreval/blob/main/tests/score-eval-example.ipynb  
-If it cannot be reached, please try:  
-https://nbviewer.org/github/rexzhang2014/scoreval/blob/main/tests/score-eval-example.ipynb  
-
-
-
-
+Metadata-Version: 2.1
+Name: score-eval
+Version: 0.0.3
+Summary: A visualization package for model score evaluation.
+Project-URL: Homepage, https://github.com/rexzhang2014/scoreval
+Project-URL: Issues, https://github.com/rexzhang2014/scoreval/issues
+Author-email: Jingxiao Zhang <rex.zhang2016@foxmail.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# scoreval
+An visulized evaluation toolkit for model score. 
+The model score will be evaluated static, on the full dataset. And further evaluate along date. 
+This aims to help machine learning modelers to evaluate the result effictively and efficiently. 
+## Effectiveness
+1. static method: on the full eval data set.
+    1. PR chart : average performance of the score.
+    2. WOE/IV : indicative power of score binning. 
+2. time method: metrics along date. 
+    1. QTL daily : show stability of the score
+    2. Precision daily: show target precision above a score cut-off.
+    3. Recall daily: show target coverage above a score cut-off.
+
+## Efficiency
+1. Predefined process & metrics: No need to design and analysis on metrics.
+2. Deal with multiple model scores: The tool will show charts for multiple model scores for comparison. 
+## Installation
+`pip install score-eval`
+# Input
+The input of this package include the below parts:
+- Model: a 'model' that implements the 'predict' method, it comes from most common used modeling tools like sklearn, tensorflow etc. The tool will definitely call model.predict() to get the score on the data set. 
+- Data set: a data set containing at least 3 columns (row_id, date, label), for calculating the metrics and by dates. If date does not appear, the time method will throw error during run. 
+
+# Output
+Pack of charts to evaluate and understand your model. See the link for more details:  
+https://github.com/rexzhang2014/scoreval/blob/main/tests/score-eval-example.ipynb  
+If it cannot be reached, please try:  
+https://nbviewer.org/github/rexzhang2014/scoreval/blob/main/tests/score-eval-example.ipynb  
+
+
```

### Comparing `score-eval-0.0.2/src/scoreval/test.py` & `score_eval-0.0.3/src/scoreval/test.py`

 * *Files identical despite different names*

