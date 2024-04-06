# Comparing `tmp/score-eval-0.0.4.tar.gz` & `tmp/score-eval-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score-eval-0.0.4.tar", last modified: Sat Apr  6 09:08:51 2024, max compression
+gzip compressed data, was "score-eval-0.0.5.tar", last modified: Sat Apr  6 16:42:05 2024, max compression
```

## Comparing `score-eval-0.0.4.tar` & `score-eval-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 09:08:51.813273 score-eval-0.0.4/
--rw-rw-rw-   0        0        0     1087 2022-05-01 17:29:39.000000 score-eval-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2234 2024-04-06 09:08:51.812275 score-eval-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1683 2022-05-03 11:15:05.000000 score-eval-0.0.4/README.md
--rw-rw-rw-   0        0        0      625 2024-04-06 09:08:44.000000 score-eval-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 09:08:51.814270 score-eval-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 09:08:51.791330 score-eval-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-06 09:08:51.811277 score-eval-0.0.4/src/score_eval.egg-info/
--rw-rw-rw-   0        0        0     2234 2024-04-06 09:08:51.000000 score-eval-0.0.4/src/score_eval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-06 09:08:51.000000 score-eval-0.0.4/src/score_eval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 09:08:51.000000 score-eval-0.0.4/src/score_eval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 09:08:51.000000 score-eval-0.0.4/src/score_eval.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 09:08:51.809282 score-eval-0.0.4/src/scoreval/
--rw-rw-rw-   0        0        0      679 2024-04-06 09:07:07.000000 score-eval-0.0.4/src/scoreval/__init__.py
--rw-rw-rw-   0        0        0    25763 2024-04-06 09:08:15.000000 score-eval-0.0.4/src/scoreval/scoreval.py
--rw-rw-rw-   0        0        0     2462 2022-05-04 08:36:58.000000 score-eval-0.0.4/src/scoreval/test.py
+drwxrwxrwx   0        0        0        0 2024-04-06 16:42:05.707830 score-eval-0.0.5/
+-rw-rw-rw-   0        0        0     1087 2022-05-01 17:29:39.000000 score-eval-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     2234 2024-04-06 16:42:05.705835 score-eval-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1683 2022-05-03 11:15:05.000000 score-eval-0.0.5/README.md
+-rw-rw-rw-   0        0        0      625 2024-04-06 09:24:40.000000 score-eval-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 16:42:05.707830 score-eval-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 16:42:05.668934 score-eval-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-06 16:42:05.703841 score-eval-0.0.5/src/score_eval.egg-info/
+-rw-rw-rw-   0        0        0     2234 2024-04-06 16:42:05.000000 score-eval-0.0.5/src/score_eval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-06 16:42:05.000000 score-eval-0.0.5/src/score_eval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 16:42:05.000000 score-eval-0.0.5/src/score_eval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-06 16:42:05.000000 score-eval-0.0.5/src/score_eval.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 16:42:05.702866 score-eval-0.0.5/src/scoreval/
+-rw-rw-rw-   0        0        0      679 2024-04-06 09:07:07.000000 score-eval-0.0.5/src/scoreval/__init__.py
+-rw-rw-rw-   0        0        0    25587 2024-04-06 16:28:18.000000 score-eval-0.0.5/src/scoreval/scoreval.py
+-rw-rw-rw-   0        0        0     2462 2022-05-04 08:36:58.000000 score-eval-0.0.5/src/scoreval/test.py
```

### Comparing `score-eval-0.0.4/LICENSE` & `score-eval-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `score-eval-0.0.4/PKG-INFO` & `score-eval-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score-eval
-Version: 0.0.4
+Version: 0.0.5
 Summary: A visualization package for model score evaluation.
 Author-email: Jingxiao Zhang <rex.zhang2016@foxmail.com>
 Project-URL: Homepage, https://github.com/rexzhang2014/scoreval
 Project-URL: Issues, https://github.com/rexzhang2014/scoreval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `score-eval-0.0.4/README.md` & `score-eval-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `score-eval-0.0.4/pyproject.toml` & `score-eval-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "score-eval"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jingxiao Zhang", email="rex.zhang2016@foxmail.com" },
 ]
 description = "A visualization package for model score evaluation."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `score-eval-0.0.4/src/score_eval.egg-info/PKG-INFO` & `score-eval-0.0.5/src/score_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score-eval
-Version: 0.0.4
+Version: 0.0.5
 Summary: A visualization package for model score evaluation.
 Author-email: Jingxiao Zhang <rex.zhang2016@foxmail.com>
 Project-URL: Homepage, https://github.com/rexzhang2014/scoreval
 Project-URL: Issues, https://github.com/rexzhang2014/scoreval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `score-eval-0.0.4/src/scoreval/__init__.py` & `score-eval-0.0.5/src/scoreval/__init__.py`

 * *Files identical despite different names*

### Comparing `score-eval-0.0.4/src/scoreval/scoreval.py` & `score-eval-0.0.5/src/scoreval/scoreval.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import numpy as np 
 import pandas as pd 
 import matplotlib.pyplot as plt
 from itertools import product
 class DummyModel() :
     def __init__(self, name='') :
         self.name = name
@@ -36,17 +37,25 @@
                 '#FFCCCC',
                 '#666699',
             ] * 3
         
     def _initialize_plot(self, figsize=(16,8)) :
         
         fig, axes = plt.subplots(len(self.models),1, figsize=figsize)
+
         if type(axes) != np.ndarray : 
             return fig, np.array([axes])
         return fig, axes
+    
+    def _save(self, fig, plt, save_path=None) :
+        if save_path :
+            fig.savefig(save_path)
+        else: 
+            plt.show()
+        plt.close()
 
     def run_score(self, X, Y, func=None) :
         '''
         X: The input data for your model. 
         Y: The input label of your data set. 
         func: customized predict function, take every model in self.models and X as input. 
         '''
@@ -124,85 +133,65 @@
             # Evaluation on score cutoff
             cutoff = np.arange(0, 1, cut_step)
             pre_cut = []
             for c in cutoff :
                 topc = eval_df.loc[eval_df['score'] > c, :]
                 pre = topc.loc[topc['label']==1, 'weight1'].sum() / topc['weight1'].sum()
                 rec = topc.loc[topc['label']==1, 'weight2'].sum() / (eval_df.loc[eval_df['label'] == 1, 'weight2']).sum()
-         
+                fpr = topc.loc[topc['label']==0, 'weight2'].sum() / (eval_df.loc[eval_df['label'] == 0, 'weight2']).sum()
                 cut = c
                 
-                rlt0 = [pre, rec, cut, topc.shape[0], (topc['label'] == 1).sum(), (topc.loc[topc['label']==1, 'weight2'].sum())]
+                rlt0 = [pre, rec, fpr, cut, topc.shape[0], topc.loc[topc['label'] == 1, 'weight1'].sum(), topc.loc[topc['label']==1, 'weight2'].sum()]
                 pre_cut.append(rlt0)
-            pre_cut = pd.DataFrame.from_records(pre_cut, columns = ['precision', 'recall', 'cutoff', 'captured', '1_captured', 'w2_captured']).reset_index()
+            pre_cut = pd.DataFrame.from_records(pre_cut, columns = ['precision', 'recall', 'fpr', 'cutoff', 'captured', '1_captured', 'w2_captured']).reset_index()
             self.cutset.append(pre_cut)
             
             # Evaluation on Operation point. 
             ops = range(0, eval_df.shape[0], eval_df.shape[0] // buckets)
             eval_df1 = eval_df.sort_values('score', ascending=False)
             pre_df = [] # pd.DataFrame()
             for i in ops :
                 if i == 0 :
                     continue
                 topi = eval_df1.iloc[:i,]
-                pre  = (topi.loc[topi['label'] == 1, 'weight1']).sum() / topi['weight1'].sum()
-                
-                rec  = (topi.loc[topi['label'] == 1, 'weight2']).sum() / (eval_df1.loc[eval_df1['label'] == 1, 'weight2']).sum()
-                
+                pre  = topi.loc[topi['label'] == 1, 'weight1'].sum() / topi['weight1'].sum()
+                rec  = topi.loc[topi['label'] == 1, 'weight2'].sum() / (eval_df1.loc[eval_df1['label'] == 1, 'weight2']).sum()
+                fpr  = topi.loc[topi['label']==0, 'weight2'].sum() / (eval_df.loc[eval_df['label'] == 0, 'weight2']).sum()
                 
                 cut  = topi['score'].min()
-                rlt0 = [pre, rec, cut, i, (topi['label'] == 1).sum(), (topi.loc[topi['label']==1, 'weight2'].sum())]
+                rlt0 = [pre, rec, fpr, cut, i, topi.loc[topi['label'] == 1, 'weight1'].sum(), topi.loc[topi['label']==1, 'weight2'].sum()]
                 
                 pre_df.append(rlt0)
             pre_df = pd.DataFrame.from_records(pre_df)
-            pre_df.columns=['precision', 'recall', 'cutoff', 'captured', '1_captured', 'w2_captured']
+            pre_df.columns=['precision', 'recall', 'fpr', 'cutoff', 'captured', '1_captured', 'w2_captured']
             pre_df = pre_df.reset_index()
             
             self.opset.append(pre_df)
             
-    def daily_recall(self, figsize=(16,8), qtl_list = ['r99', 'r95', 'r90','r50',], x_step=2):
+    def daily_recall(self, figsize=(16,8), qtl_list = [99, 95, 90, 50,], x_step=2):
         
         fig, axes = self._initialize_plot(figsize=(figsize[0], figsize[1]*len(self.models)))
         
         for ax, data in zip(axes, self.scores) :
         
             data1 = data.copy()
-            # tp : true positive
-            data1['tp99'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.99, axis=1)
-            data1['tp95'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.95, axis=1)
-            data1['tp90'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.90, axis=1)
-            data1['tp75'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.75, axis=1)
-            data1['tp50'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.50, axis=1)
-            data1['tp25'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.25, axis=1)
-            data1['tp10'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.10, axis=1)
-            data1['tp01'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.01, axis=1)
-            # ap : all positive
-            data1['ap99'] = data1.apply(lambda x : x['label']==1, axis=1)
-            data1['ap95'] = data1.apply(lambda x : x['label']==1, axis=1)
-            data1['ap90'] = data1.apply(lambda x : x['label']==1, axis=1)
-            data1['ap75'] = data1.apply(lambda x : x['label']==1, axis=1)
-            data1['ap50'] = data1.apply(lambda x : x['label']==1, axis=1)
-            data1['ap25'] = data1.apply(lambda x : x['label']==1, axis=1)
-            data1['ap10'] = data1.apply(lambda x : x['label']==1, axis=1)
-            data1['ap01'] = data1.apply(lambda x : x['label']==1, axis=1)
-            
-            stats_bydate = data1.groupby('date').agg(pd.Series.sum).reset_index()
-            
-            stats_bydate['r99'] = stats_bydate.apply(lambda x : x['tp99'] / (x['ap99'] + 0.0001), axis=1)
-            stats_bydate['r95'] = stats_bydate.apply(lambda x : x['tp95'] / (x['ap95'] + 0.0001), axis=1)
-            stats_bydate['r90'] = stats_bydate.apply(lambda x : x['tp90'] / (x['ap90'] + 0.0001), axis=1)
-            stats_bydate['r75'] = stats_bydate.apply(lambda x : x['tp75'] / (x['ap75'] + 0.0001), axis=1)
-            stats_bydate['r50'] = stats_bydate.apply(lambda x : x['tp50'] / (x['ap50'] + 0.0001), axis=1)
-            stats_bydate['r25'] = stats_bydate.apply(lambda x : x['tp25'] / (x['ap25'] + 0.0001), axis=1)
-            stats_bydate['r10'] = stats_bydate.apply(lambda x : x['tp10'] / (x['ap10'] + 0.0001), axis=1)
-            stats_bydate['r01'] = stats_bydate.apply(lambda x : x['tp01'] / (x['ap01'] + 0.0001), axis=1)
+
+            for q in qtl_list :
+                # tp : true positive
+                data1[f'tp{q}'] = data1.apply(lambda x : x['label']==1 and x['score']>=q/100, axis=1)
+                # cp : conditional positive
+                data1[f'cp{q}'] = data1.apply(lambda x : x['label']==1, axis=1)
+
+            stats_bydate = data1.groupby('date').agg(np.sum).reset_index()
             
+            for q in qtl_list :
+                stats_bydate[f'r{q}'] = stats_bydate.apply(lambda x : x[f'tp{q}'] / (x[f'cp{q}'] + 0.0001), axis=1)
+
             ax.bar(stats_bydate['date'], stats_bydate['label'], color = 'lightsteelblue')
 
-            
             date_axis = stats_bydate['date']
             
             ax.set_xticks([ i for i in range(0, len(date_axis), x_step) ])
             ax.set_xticklabels([ date_axis[i] for i in range(0, len(date_axis), x_step) ])
             plt.xticks(rotation=90)
             
             ax2 = ax.twinx()
@@ -221,52 +210,38 @@
             
             ax2.set_yticks(np.arange(0,1.02,0.02))
             ax2.grid(axis='y', linestyle='--')
 
             plt.legend(handles=handles, labels=qtl_list, loc='best')            
         plt.show()
         
-    def daily_precision(self, figsize=(16,8), qtl_list = ['p99', 'p95', 'p90','p50',], x_step=2):
+    def daily_precision(self, figsize=(16,8), qtl_list = [99, 95, 90, 50,], x_step=2):
         fig, axes = self._initialize_plot(figsize=(figsize[0], figsize[1]*len(self.models)))
 
         for ax, data in zip(axes, self.scores) :
             data1 = data.copy()
-            # tp : true positive
-            data1['tp99'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.99, axis=1)
-            data1['tp95'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.95, axis=1)
-            data1['tp90'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.90, axis=1)
-            data1['tp75'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.75, axis=1)
-            data1['tp50'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.50, axis=1)
-            data1['tp25'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.25, axis=1)
-            data1['tp10'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.10, axis=1)
-            data1['tp01'] = data1.apply(lambda x : x['label']==1 and x['score']>=0.01, axis=1)
-            # sc : score cut
-            data1['sc99'] = data1.apply(lambda x : x['score']>=0.99, axis=1)
-            data1['sc95'] = data1.apply(lambda x : x['score']>=0.95, axis=1)
-            data1['sc90'] = data1.apply(lambda x : x['score']>=0.90, axis=1)
-            data1['sc75'] = data1.apply(lambda x : x['score']>=0.75, axis=1)
-            data1['sc50'] = data1.apply(lambda x : x['score']>=0.50, axis=1)
-            data1['sc25'] = data1.apply(lambda x : x['score']>=0.25, axis=1)
-            data1['sc10'] = data1.apply(lambda x : x['score']>=0.10, axis=1)
-            data1['sc01'] = data1.apply(lambda x : x['score']>=0.01, axis=1)
+           
+            for q in qtl_list :
+                # tp : true positive
+                data1[f'tp{q}'] = data1.apply(lambda x : x['label']==1 and x['score']>=q/100, axis=1)
+                # pp : predicted positive
+                data1[f'pp{q}'] = data1.apply(lambda x : x['score']>=1/100, axis=1)
+
+            stats_bydate = data1.groupby('date').agg(np.sum).reset_index()
+            
+            for q in qtl_list :
+                stats_bydate[f'r{q}'] = stats_bydate.apply(lambda x : x[f'tp{q}'] / (x[f'pp{q}'] + 0.0001), axis=1)
             
             stats_bydate = data1.groupby('date').agg(pd.Series.sum).reset_index()
-
-            stats_bydate['p99'] = stats_bydate.apply(lambda x : x['tp99'] / (x['sc99'] + 0.0001), axis=1)
-            stats_bydate['p95'] = stats_bydate.apply(lambda x : x['tp95'] / (x['sc95'] + 0.0001), axis=1)
-            stats_bydate['p90'] = stats_bydate.apply(lambda x : x['tp90'] / (x['sc90'] + 0.0001), axis=1)
-            stats_bydate['p75'] = stats_bydate.apply(lambda x : x['tp75'] / (x['sc75'] + 0.0001), axis=1)
-            stats_bydate['p50'] = stats_bydate.apply(lambda x : x['tp50'] / (x['sc50'] + 0.0001), axis=1)
-            stats_bydate['p25'] = stats_bydate.apply(lambda x : x['tp25'] / (x['sc25'] + 0.0001), axis=1)
-            stats_bydate['p10'] = stats_bydate.apply(lambda x : x['tp10'] / (x['sc10'] + 0.0001), axis=1)
-            stats_bydate['p01'] = stats_bydate.apply(lambda x : x['tp01'] / (x['sc01'] + 0.0001), axis=1)
+            
+            for q in qtl_list :
+                stats_bydate[f'p{q}'] = stats_bydate.apply(lambda x : x[f'tp{q}'] / (x[f'pp{q}'] + 0.0001), axis=1)
             
             ax.bar(stats_bydate['date'], stats_bydate['label'], color = 'lightsteelblue')
 
-            
             date_axis = stats_bydate['date']
             ax.set_xticks([ i for i in range(0, len(date_axis), x_step) ])
             ax.set_xticklabels([ date_axis[i] for i in range(0, len(date_axis), x_step) ])
          
             plt.xticks(rotation=90)
             
             ax2 = ax.twinx()
@@ -285,38 +260,26 @@
             ax2.set_yticks(np.arange(0,1.02,0.02))
             ax2.grid(axis='y', linestyle='--')
 
             plt.legend(handles=handles, labels=qtl_list, loc='best')            
         plt.show()
 
 
-    def daily_qtls(self, figsize=(16,8), qtl_list = ['q99', 'q95', 'q90','q75','q50', 'q25','q10','q01'], x_step=2 ) :
+    def daily_qtls(self, figsize=(16,8), qtl_list = [99,90,50,10,1], x_step=2 ) :
         
         fig, axes = self._initialize_plot(figsize=(figsize[0], figsize[1]*len(self.models)))
         for ax, data in zip(axes, self.scores) :
             stats_bydate = data.groupby('date').agg({
                 'label': pd.Series.sum, 
-                'score': [lambda x: np.quantile(x, 0.99), lambda x: np.quantile(x, 0.95), lambda x: np.quantile(x, 0.9), 
-                          lambda x: np.quantile(x, 0.75),  lambda x: np.quantile(x, 0.5), lambda x: np.quantile(x, 0.25),
-                          lambda x: np.quantile(x, 0.1), lambda x: np.quantile(x, 0.01)
-                         ]
-            #     'score': [lambda x: sum(x > 0.99), lambda x: sum(x > 0.9), lambda x: sum(x > 0.8), lambda x: sum(x > 0.99)]
+                'score': lambda x: np.quantile(x, q=[x / 100 for x in qtl_list], )
             }).reset_index()
             stats_bydate.columns = [
                 'date',
                 'label_cnt', 
-                'q99', 
-                'q95', 
-                'q90',
-                'q75',
-                'q50', 
-                'q25',
-                'q10',
-                'q01'
-            ]
+            ] + [ f'q{x}' for x in qtl_list ]
             
             ax.bar(stats_bydate['date'], stats_bydate['label_cnt'], color = 'lightsteelblue')
 
             date_axis = stats_bydate['date'].unique()
             
             ax.set_xticks([ i for i in range(0, len(date_axis), x_step) ])
             ax.set_xticklabels([ date_axis[i] for i in range(0, len(date_axis), x_step) ])
@@ -340,19 +303,19 @@
             ax2.set_ylim(0,1.02)
             ax2.grid(axis='y', linestyle='--')
 
 
             plt.legend(handles=handles, labels=qtl_list, loc='best')            
         plt.show()
     
-    def iv(self, bins=20, plot=True, figsize=(10, 10), bin_col='score_bin') :
+    def plot_iv(self, bins=20, figsize=(10, 10), bin_col='score_bin', save_path=None) :
 
         fig, axes = self._initialize_plot(figsize=(figsize[0], figsize[1]*len(self.models)))
         
-        for ax, data in zip(axes, self.scores) :
+        for ax, data, model in zip(axes, self.scores, self.models) :
             # score distribution
             data_final_1 = data.assign(
                 score_bin = pd.cut(data['score'], bins),
                 score_qtl = pd.qcut(data['score'], bins),
             )
 
             N0 = (data_final_1['label'] == 0).sum()
@@ -370,48 +333,55 @@
                 woe = lambda x: np.log(x['inc'] / N1) - np.log((x['cnt'] - x['inc'] ) / N0),
                 binbd = data_final_2[bin_col].apply(lambda x: x.right),
             )
 
             score_iv = np.sum((data_final_2['inc'] / N1 - (data_final_2['cnt'] - data_final_2['inc'])/ N0) * data_final_2['woe'])
             
             self.ivset.append(score_iv)
-            
-            if plot :
-                cmap = self.cmap
-                ax.bar( data_final_2.index, data_final_2['woe'], color=(data_final_2['woe']<=0).astype(int).apply(lambda x: cmap[x]))
-                ax.set_xticklabels(data_final_2['binbd'])
-                ax.set_title('IV:{}'.format(score_iv))
-    
-    def score_distribution(self, bins=20, plot=True, figsize=(10, 10), bin_col='score_bin') :
+        
+            cmap = self.cmap
+            ax.bar( data_final_2.index, data_final_2['woe'], color=(data_final_2['woe']<=0).astype(int).apply(lambda x: cmap[x]))
+            ax.set_xticklabels(data_final_2['binbd'])
+            ax.set_title(f'{model.name} IV:{score_iv}')
+
+            self._save(fig, plt, save_path)
+
+    def plot_histogram(self, bins=20, bin_col='score_bin', label_col='label', plot=True, figsize=(10, 10), save_path=None) :
 
         fig, axes = self._initialize_plot(figsize=(figsize[0], figsize[1]*len(self.models)))
         
-        for ax, data in zip(axes, self.scores) :
-            # score distribution
-            data_final_1 = data.assign(
-                score_bin = pd.cut(data['score'], bins),
-                score_qtl = pd.qcut(data['score'], bins),
-            )
+        for ax, score, model in zip(axes, self.scores, self.models) :
+            ax.hist(score[score[label_col]==0], bins, density=True, histtype='bar', align='mid', rwidth=100//bins, alpha=0.75)
+            ax.hist(score[score[label_col]==1], bins, density=True, histtype='bar', align='mid', rwidth=100//bins, alpha=0.75)
+            ax.set_title(f'{model.name}')
 
-            
-            data_final_2 = data_final_1.groupby(bin_col).agg({
-                'label' : [pd.Series.count, pd.Series.sum]
-            })
+        self._save(fig, plt, save_path)
 
-            data_final_2.columns = ['cnt', 'inc']
+    def plot_distribution(self, distr='normal', bins=100, label_col='label', alpha=0.75, figsize=(10, 10), save_path=None) :
 
-            data_final_2 = data_final_2.reset_index()
-            data_final_2 = data_final_2.assign(
-                binbd = data_final_2[bin_col].apply(lambda x: x.right),
-            )
-            
-            if plot :
-                cmap = self.cmap
-                ax.bar( data_final_2.index, data_final_2['cnt'], color=cmap[2])
+        fig, axes = self._initialize_plot(figsize=(figsize[0], figsize[1]*len(self.models)))
         
+        for ax, score, model in zip(axes, self.scores, self.models) :
+            df0, df1  = score.loc[score[label_col]==0,'score'], score.loc[score[label_col]==1,'score']
+            mu0, sig0 = df0.mean(), df0.std() 
+            mu1, sig1 = df1.mean(), df1.std()
+            if distr == 'normal' :
+                spl0 = np.random.normal(mu0, sig0, 20000)
+                spl1 = np.random.normal(mu1, sig1, 20000)
+            else :
+                raise ValueError("Only normal distribution is supported in current version.")
+            
+            _,_, p0 = ax.hist(spl0, bins, density=True, histtype='bar', align='mid', rwidth=bins, alpha=alpha, color=self.cmap[0])
+            _,_, p1 = ax.hist(spl1, bins, density=True, histtype='bar', align='mid', rwidth=bins, alpha=alpha, color=self.cmap[1])
+
+            ax.set_title(f'{model.name}')
+            
+            ax.legend(handles=[p0,p1],labels=['label-0', 'label-1'], loc='best')
+        self._save(fig, plt, save_path)
+
     def plot_cutoff_chart(self, index_col=None, x_step=2, xlim=(0,100), ylim=(0,1.02), save_path=None, figsize=(10,10), chunksize=None) :   
         
         chunksize = len(self.opset) if chunksize is None else chunksize
         
         for i in range(0, len(self.opset), chunksize) :
             
             md_names = [ m.name for m in self.models[i:i+chunksize] ]
@@ -443,19 +413,15 @@
 
             plt.legend(handles=handles, labels=product(md_names, ['precision', 'recall']), loc='best')            
 
             if index_col:
                 ax.set_xticklabels(pre_df[index_col].map(lambda x: round(x,2)).iloc[0: pre_df.shape[0]+1:x_step])
             plt.xticks(rotation=90)
 
-            if save_path: 
-                plt.savefig(save_path)
-            else :
-                plt.show()
-            plt.close()
+            self._save(fig, plt, save_path)
         
     def plot_op_chart(self, index_col=None, x_step=2, xlim=(0,100), ylim=(0,1.02), save_path=None, figsize=(10,10), chunksize=None) :
         
         chunksize = len(self.opset) if chunksize is None else chunksize
         
         for i in range(0, len(self.opset), chunksize) :
             
@@ -488,50 +454,64 @@
 
             plt.legend(handles=handles, labels=product(md_names, ['precision', 'recall']), loc='best')            
 
             if index_col:
                 ax.set_xticklabels(pre_df[index_col].map(lambda x: round(x,2)).iloc[0: pre_df.shape[0]+1:x_step])
             plt.xticks(rotation=90)
 
-            if save_path: 
-                plt.savefig(save_path)
-            else :
-                plt.show()
-            plt.close()
+            self._save(fig, plt, save_path)
 
     def plot_pr(self, tick_step=0.02, save_path=None, figsize=(10,10)) :
         
         fig, ax = plt.subplots(1,1, figsize=figsize)
         
         ax.ylim=(0,1)
         ax.y_ticks=(0,1)
         
         handles = []
-        for pre_df in self.opset :
+        for i, pre_df in enumerate(self.opset) :
             p1, = ax.plot(
                 pre_df.loc[(~pre_df['recall'].isnull()) & (pre_df['recall']>0.0), 'recall'],
-                pre_df.loc[(~pre_df['precision'].isnull()) & (pre_df['precision']>0.0), 'precision']
+                pre_df.loc[(~pre_df['precision'].isnull()) & (pre_df['precision']>0.0), 'precision'],
+                color=self.cmap[i],
             )
             handles.append(p1)
             
         ax.set_ylabel('precision')
         ax.set_xlabel('recall')
         ax.set_xlim(0,1.02)
         ax.set_ylim(0,1.02)
         ax.grid(which='both', axis='both')
         
         plt.legend(handles=handles, labels=[ m.name for m in self.models ], loc='best')     
         
-        if save_path: 
-            plt.savefig(save_path)
-        else :
-            plt.show()
-        plt.close()
-
+        self._save(fig, plt, save_path)
 
+    def plot_roc(self, tick_step=0.02, save_path=None, figsize=(10,10)) :
+        
+        fig, ax = plt.subplots(1,1, figsize=figsize)
+        
+        handles = []
+        for i, pre_df in enumerate(self.opset) :
+            p1, = ax.plot(
+                pre_df.loc[(~pre_df['fpr'].isnull()) & (pre_df['fpr']>0.0), 'fpr'],
+                pre_df.loc[(~pre_df['recall'].isnull()) & (pre_df['recall']>0.0), 'recall'],
+                color=self.cmap[i],
+            )
+            handles.append(p1)
+            
+        ax.set_ylabel('TPR')
+        ax.set_xlabel('FPR')
+        ax.set_xlim(0,1.02)
+        ax.set_ylim(0,1.02)
+        ax.grid(which='both', axis='both')
+        
+        plt.legend(handles=handles, labels=[ m.name for m in self.models ], loc='best')     
+        
+        self._save(fig, plt, save_path)
 
 class ScoreEvalNegative(ScoreEval) :
 
     def score_cut(self, cut_step=0.02, buckets=100):
         '''
         Must run after self.run_score. cutoff and operating point will be generated. 
         Pre-assume the score is in interval [0,1], both result will be produced and saved in self attributes.
@@ -575,7 +555,59 @@
                 
                 pre_df.append(rlt0)
             pre_df = pd.DataFrame.from_records(pre_df)
             pre_df.columns=['precision', 'recall', 'cutoff', 'captured', '1_captured', 'w2_captured']
             pre_df = pre_df.reset_index()
             
             self.opset.append(pre_df)
+
+
+if __name__ == '__main__' :
+    
+    from sklearn.linear_model import LogisticRegression
+    BASE_DIR = "E:\\workspace\\scoreval"
+    data = pd.read_csv(os.path.join(BASE_DIR,"data/investing_program_prediction_data.csv"))
+    # Build simple model for test
+    features = ['SE1', 'BA1', 'BA2', 'BA3', 'BA4', 'BA5']
+    label = 'label'
+    data['label'] = data['InvType'].map(lambda x: x[-1]).astype(int)
+    # normalize
+    for f in features : 
+        data[f] = (data[f] - data[f].mean()) / data[f].std()
+    X = data[features].values
+    y = data[label].values
+
+    models = []
+
+    for i in range(1,4) :
+        clf = LogisticRegression(
+            penalty='l2', #'elasticnet',
+            # l1_ratio=0.5,
+            tol=1e-6,
+            solver='saga',
+            max_iter=200,
+            C=i/100,
+
+        ).fit(X, y)
+        # clf.predict(X[:2, :])
+        # clf.score(X,y)
+        clf.name = f'model{i}'
+        models.append(clf)
+
+    # Create ScoreEval object, initialized by a list of model objects
+    se = ScoreEval(models)
+    def skl_predict(clf, X) :
+        pred = clf.predict_proba(X)
+        return pred[:,1].reshape(pred.shape[0], 1)
+    # Run score, make sure the models have the same inputs. SE will call model.predict for each model. 
+    # That is not a good idea to take models with different inputs. Please always compare apple to apple. 
+    # Make sure X and Y have the same rows so that the score can be produced properly. 
+    # se_oot.run_score([oot_X_arr,oot_S_arr,oot_P_arr,oot_I_arr,], df_y)
+    se.run_score(X, data[[label]], skl_predict)
+    se.score_cut(0.01,100)
+    se.plot_cutoff_chart(xlim=(0, 50), save_path='./cutoff.png')
+    se.plot_op_chart(xlim=(0, 50), save_path='./op.png')
+    se.plot_pr(save_path='./pr.png')
+    se.plot_roc(save_path='./roc.png')
+    se.plot_iv(save_path='./iv.png')
+    se.plot_histogram(save_path='./hist.png')
+    se.plot_distribution(save_path='./distr.png')
```

### Comparing `score-eval-0.0.4/src/scoreval/test.py` & `score-eval-0.0.5/src/scoreval/test.py`

 * *Files identical despite different names*

