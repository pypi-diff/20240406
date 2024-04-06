# Comparing `tmp/macrodemos-2021.9.7.tar.gz` & `tmp/macrodemos-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrodemos-2021.9.7.tar", last modified: Mon Sep  6 20:58:57 2021, max compression
+gzip compressed data, was "macrodemos-2024.4.5.tar", last modified: Sat Apr  6 06:11:02 2024, max compression
```

## Comparing `macrodemos-2021.9.7.tar` & `macrodemos-2024.4.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2021-09-06 20:58:57.516972 macrodemos-2021.9.7/
--rw-rw-rw-   0        0        0       69 2021-03-10 18:07:58.000000 macrodemos-2021.9.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3717 2021-09-06 20:58:57.512982 macrodemos-2021.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2021-09-06 16:13:15.000000 macrodemos-2021.9.7/README.md
--rw-rw-rw-   0        0        0    19015 2021-09-06 15:25:57.000000 macrodemos-2021.9.7/demo_ARMA - sin statsmodels.py
-drwxrwxrwx   0        0        0        0 2021-09-06 20:58:57.495031 macrodemos-2021.9.7/macrodemos/
--rw-rw-rw-   0        0        0      763 2021-09-06 20:47:05.000000 macrodemos-2021.9.7/macrodemos/__init__.py
--rw-rw-rw-   0        0        0     8654 2020-07-06 00:37:21.000000 macrodemos-2021.9.7/macrodemos/captura.py
--rw-rw-rw-   0        0        0     7928 2021-09-05 16:21:24.000000 macrodemos-2021.9.7/macrodemos/common_components.py
--rw-rw-rw-   0        0        0     6525 2020-07-26 04:22:36.000000 macrodemos-2021.9.7/macrodemos/constants.py
-drwxrwxrwx   0        0        0        0 2021-09-06 20:58:57.511984 macrodemos-2021.9.7/macrodemos/data/
--rw-rw-rw-   0        0        0    14510 2021-03-10 18:07:01.000000 macrodemos-2021.9.7/macrodemos/data/CRI-initial-data.csv
--rw-rw-rw-   0        0        0   227875 2020-10-30 06:47:50.000000 macrodemos-2021.9.7/macrodemos/data/IFS_GDP.xlsx
--rw-rw-rw-   0        0        0    43884 2020-06-26 05:53:26.000000 macrodemos-2021.9.7/macrodemos/data/national_accounts.xlsx
--rw-rw-rw-   0        0        0    23537 2021-09-06 15:25:57.000000 macrodemos-2021.9.7/macrodemos/demo_ARMA.py
--rw-rw-rw-   0        0        0    21734 2021-09-06 15:25:57.000000 macrodemos-2021.9.7/macrodemos/demo_BoxJenkins.py
--rw-rw-rw-   0        0        0    10733 2021-09-06 15:25:57.000000 macrodemos-2021.9.7/macrodemos/demo_Markov.py
--rw-rw-rw-   0        0        0    17106 2021-09-06 15:25:57.000000 macrodemos-2021.9.7/macrodemos/demo_Solow.py
--rw-rw-rw-   0        0        0    22709 2021-09-06 15:25:57.000000 macrodemos-2021.9.7/macrodemos/demo_filters.py
-drwxrwxrwx   0        0        0        0 2021-09-06 20:58:57.507995 macrodemos-2021.9.7/macrodemos.egg-info/
--rw-rw-rw-   0        0        0     3717 2021-09-06 20:58:57.000000 macrodemos-2021.9.7/macrodemos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      568 2021-09-06 20:58:57.000000 macrodemos-2021.9.7/macrodemos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-06 20:58:57.000000 macrodemos-2021.9.7/macrodemos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2021-09-06 20:58:57.000000 macrodemos-2021.9.7/macrodemos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-09-06 20:58:57.000000 macrodemos-2021.9.7/macrodemos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-09-06 20:58:57.517970 macrodemos-2021.9.7/setup.cfg
--rw-rw-rw-   0        0        0     1221 2021-09-06 20:58:43.000000 macrodemos-2021.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 06:11:02.275066 macrodemos-2024.4.5/
+-rw-rw-rw-   0        0        0       69 2021-03-10 18:07:58.000000 macrodemos-2024.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3245 2024-04-06 06:11:02.275066 macrodemos-2024.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2024-04-06 06:07:42.000000 macrodemos-2024.4.5/README.md
+-rw-rw-rw-   0        0        0    19015 2021-09-06 15:25:57.000000 macrodemos-2024.4.5/demo_ARMA - sin statsmodels.py
+drwxrwxrwx   0        0        0        0 2024-04-06 06:11:02.211277 macrodemos-2024.4.5/macrodemos/
+-rw-rw-rw-   0        0        0      761 2024-04-06 06:07:02.000000 macrodemos-2024.4.5/macrodemos/__init__.py
+-rw-rw-rw-   0        0        0     8654 2020-07-06 00:37:21.000000 macrodemos-2024.4.5/macrodemos/captura.py
+-rw-rw-rw-   0        0        0     7900 2022-08-16 23:43:37.000000 macrodemos-2024.4.5/macrodemos/common_components.py
+-rw-rw-rw-   0        0        0     6525 2020-07-26 04:22:36.000000 macrodemos-2024.4.5/macrodemos/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-06 06:11:02.275066 macrodemos-2024.4.5/macrodemos/data/
+-rw-rw-rw-   0        0        0    14510 2021-03-10 18:07:01.000000 macrodemos-2024.4.5/macrodemos/data/CRI-initial-data.csv
+-rw-rw-rw-   0        0        0   227875 2020-10-30 06:47:50.000000 macrodemos-2024.4.5/macrodemos/data/IFS_GDP.xlsx
+-rw-rw-rw-   0        0        0    43884 2020-06-26 05:53:26.000000 macrodemos-2024.4.5/macrodemos/data/national_accounts.xlsx
+-rw-rw-rw-   0        0        0    24565 2022-08-18 04:25:30.000000 macrodemos-2024.4.5/macrodemos/demo_ARMA.py
+-rw-rw-rw-   0        0        0    22563 2022-08-18 04:52:46.000000 macrodemos-2024.4.5/macrodemos/demo_BoxJenkins.py
+-rw-rw-rw-   0        0        0    10715 2022-08-16 23:57:06.000000 macrodemos-2024.4.5/macrodemos/demo_Markov.py
+-rw-rw-rw-   0        0        0    17078 2022-08-16 23:44:48.000000 macrodemos-2024.4.5/macrodemos/demo_Solow.py
+-rw-rw-rw-   0        0        0    22681 2022-08-16 23:57:42.000000 macrodemos-2024.4.5/macrodemos/demo_filters.py
+drwxrwxrwx   0        0        0        0 2024-04-06 06:11:02.254216 macrodemos-2024.4.5/macrodemos.egg-info/
+-rw-rw-rw-   0        0        0     3245 2024-04-06 06:11:02.000000 macrodemos-2024.4.5/macrodemos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      568 2024-04-06 06:11:02.000000 macrodemos-2024.4.5/macrodemos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 06:11:02.000000 macrodemos-2024.4.5/macrodemos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-06 06:11:02.000000 macrodemos-2024.4.5/macrodemos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-06 06:11:02.000000 macrodemos-2024.4.5/macrodemos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 06:11:02.281952 macrodemos-2024.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2024-04-06 06:08:08.000000 macrodemos-2024.4.5/setup.py
```

### Comparing `macrodemos-2021.9.7/PKG-INFO` & `macrodemos-2024.4.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 Metadata-Version: 2.1
 Name: macrodemos
-Version: 2021.9.7
+Version: 2024.4.5
 Summary: Demo programs to learn macroeconomics and macro-econometrics concepts
 Home-page: http://randall-romero.com/code/macrodemos
 Author: Randall Romero-Aguilar
 Author-email: randall.romero@outlook.com
 License: MIT
-Description: # MACRODEMOS
-        
-        ## Macroeconomics Demos: A Python package to teach macroeconomics and macroeconometrics
-        
-        The purpose of this package is to provide tools to teach concepts of macroeconomics and macroeconometrics.
-        
-        To date, the package provides these functions:
-        
-        * **ARMA( )**: Demo for learning about  ARMA processes. It creates a dash consisting of 7 plots to study the theoretical properties of ARMA(p, q) processes, as well as their estimated counterparts. The plots display
-            1. a simulated sample
-            2. autocorrelations
-            3. partial autocorrelations
-            4. impulse response function
-            5. spectral density
-            6. AR inverse roots
-            7. MA inverse roots.
-        *  **Markov('state_0',...,'state_n')**: a demo to illustrate Markov chains. User sets the number of states, the transition matrix, and the initial distribution. The demo creates a dash consisting of 2 plots:
-            1. a simulated sample
-            2. the time evolution of the distribution of states
-        *  **Solow( )**: this demo illustrates the Solow-Swan model. Users can simulate the dynamic effect of a shock in a exogenous variable or a change in a model parameter. You will find 6 figures about the Solow-Swan model:
-            1. Capital stock, per capita
-            2. Output per capita,
-            3. Savings per capita,
-            4. Consumption per capita,
-            5. Change in capital stock, and
-            6. Output growth rate 
-           
-            It also presents plots to illustrate how steady-state capital is determined, and the golden rule. 
-        *  **filters( )**: to illustrate the use of the Hodrick-Prescott, Baxter-King, Christiano-Fitzgeral and Hamilton filters.
-        
-        In a near future, I expect to add a few more demos:
-        
-        * **Bellman( )**: to illustrate the solution of a Bellman equation by value function iteration
-        * **BoxJenkins( )**: to illustrate the Box-Jenkins methodology, by fitting two ARIMA models side-by-side to user-provided data.  
-        * **FilterMyData( )**: to filter user-supplied data with several methodologies, comparing their resulting cycles. 
-         
-        ### Instructions
-        To use the demos, just install this package `pip install macrodemos` and then run any of the demos you want.
-        
-            import macrodemos
-            macrodemos.ARMA()
-            macrodemos.Markov()
-            macrodemos.Solow()
-            macrodemos.filter()
-         
-        This will open a new tab in your default Internet browser with a Plotly dash. A current limitation is that you can only run 
-        one demo at a time.
-        
-        ### Disclaimer 
-        This program illustrates basic concepts of macroeconomics and time series econometrics. It was developed for teaching purposes 
-        only: you are free to use it in your own lectures or to learn about these topics.  
-        
-        If you have any suggestions, please send me an email at randall.romero@ucr.ac.cr
-                                  
-        **Copyright 2016-2021 Randall Romero-Aguilar**
-        
 Keywords: time series,ARMA,filters,Markov chain,Solow-Swan,Hodrick-Prescott,Baxter-King
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+
+# MACRODEMOS
+
+## Macroeconomics Demos: A Python package to teach macroeconomics and macroeconometrics
+
+The purpose of this package is to provide tools to teach concepts of macroeconomics and macroeconometrics.
+
+To date, the package provides these functions:
+
+* **ARMA( )**: Demo for learning about  ARMA processes. It creates a dash consisting of 7 plots to study the theoretical properties of ARMA(p, q) processes, as well as their estimated counterparts. The plots display
+    1. a simulated sample
+    2. autocorrelations
+    3. partial autocorrelations
+    4. impulse response function
+    5. spectral density
+    6. AR inverse roots
+    7. MA inverse roots.
+*  **Markov('state_0',...,'state_n')**: a demo to illustrate Markov chains. User sets the number of states, the transition matrix, and the initial distribution. The demo creates a dash consisting of 2 plots:
+    1. a simulated sample
+    2. the time evolution of the distribution of states
+*  **Solow( )**: this demo illustrates the Solow-Swan model. Users can simulate the dynamic effect of a shock in a exogenous variable or a change in a model parameter. You will find 6 figures about the Solow-Swan model:
+    1. Capital stock, per capita
+    2. Output per capita,
+    3. Savings per capita,
+    4. Consumption per capita,
+    5. Change in capital stock, and
+    6. Output growth rate 
+   
+    It also presents plots to illustrate how steady-state capital is determined, and the golden rule. 
+*  **filters( )**: to illustrate the use of the Hodrick-Prescott, Baxter-King, Christiano-Fitzgeral and Hamilton filters.
+
+In a near future, I expect to add a few more demos:
+
+* **Bellman( )**: to illustrate the solution of a Bellman equation by value function iteration
+* **BoxJenkins( )**: to illustrate the Box-Jenkins methodology, by fitting two ARIMA models side-by-side to user-provided data.  
+* **FilterMyData( )**: to filter user-supplied data with several methodologies, comparing their resulting cycles. 
+ 
+### Instructions
+To use the demos, just install this package `pip install macrodemos` and then run any of the demos you want.
+
+    import macrodemos
+    macrodemos.ARMA()
+    macrodemos.Markov()
+    macrodemos.Solow()
+    macrodemos.filter()
+ 
+This will open a new tab in your default Internet browser with a Plotly dash. A current limitation is that you can only run 
+one demo at a time.
+
+### Disclaimer 
+This program illustrates basic concepts of macroeconomics and time series econometrics. It was developed for teaching purposes 
+only: you are free to use it in your own lectures or to learn about these topics.  
+
+If you have any suggestions, please send me an email at randall.romero@ucr.ac.cr
+                          
+**Copyright 2016-2024 Randall Romero-Aguilar**
```

### Comparing `macrodemos-2021.9.7/README.md` & `macrodemos-2024.4.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 
 ### Disclaimer 
 This program illustrates basic concepts of macroeconomics and time series econometrics. It was developed for teaching purposes 
 only: you are free to use it in your own lectures or to learn about these topics.  
 
 If you have any suggestions, please send me an email at randall.romero@ucr.ac.cr
                           
-**Copyright 2016-2021 Randall Romero-Aguilar**
+**Copyright 2016-2024 Randall Romero-Aguilar**
```

### Comparing `macrodemos-2021.9.7/demo_ARMA - sin statsmodels.py` & `macrodemos-2024.4.5/demo_ARMA - sin statsmodels.py`

 * *Files identical despite different names*

### Comparing `macrodemos-2021.9.7/macrodemos/__init__.py` & `macrodemos-2024.4.5/macrodemos/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 So far, the available demos are:
 
     ARMA_demo():  to study AutoRegressive Moving Average processes.
     filters_demo(): to compare several filtering methods.
     Markov_demo(): to study Markov chains.
     Solow_demo():  to study the Solow growth model.
 
-Randall Romero Aguilar, 2016-2021
+Randall Romero Aguilar, 2016-2024
 """
 
 #import .constants
 #import .common_components
 from .captura import read_IFS
 from .demo_ARMA import ARMA
 from .demo_Solow import Solow
 from .demo_Markov import Markov
 from .demo_filters import filters
-# from .demo_BoxJenkins import BoxJenkins # still work in progress
+from .demo_BoxJenkins import BoxJenkins # still work in progress
```

### Comparing `macrodemos-2021.9.7/macrodemos/captura.py` & `macrodemos-2024.4.5/macrodemos/captura.py`

 * *Files identical despite different names*

### Comparing `macrodemos-2021.9.7/macrodemos/common_components.py` & `macrodemos-2024.4.5/macrodemos/common_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module contains components that are common to several demo layouts.
 
 """
-import dash_core_components as dcc
-import dash_html_components as html
+from dash import dcc
+from dash import html
 from plotly.subplots import make_subplots
 import numpy as np
 
 colors = {
     'background': 'SteelBlue',
     'text': 'White',
     'controls': '#DDDDDD',
```

### Comparing `macrodemos-2021.9.7/macrodemos/constants.py` & `macrodemos-2024.4.5/macrodemos/constants.py`

 * *Files identical despite different names*

### Comparing `macrodemos-2021.9.7/macrodemos/data/CRI-initial-data.csv` & `macrodemos-2024.4.5/macrodemos/data/CRI-initial-data.csv`

 * *Files identical despite different names*

### Comparing `macrodemos-2021.9.7/macrodemos/data/IFS_GDP.xlsx` & `macrodemos-2024.4.5/macrodemos/data/IFS_GDP.xlsx`

 * *Files identical despite different names*

### Comparing `macrodemos-2021.9.7/macrodemos/data/national_accounts.xlsx` & `macrodemos-2024.4.5/macrodemos/data/national_accounts.xlsx`

 * *Files identical despite different names*

### Comparing `macrodemos-2021.9.7/macrodemos/demo_ARMA.py` & `macrodemos-2024.4.5/macrodemos/demo_ARMA.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 Randall Romero Aguilar
 2016-2021
 """
 
 
 
 from jupyter_dash import JupyterDash
-import dash_core_components as dcc
-import dash_html_components as html
+from dash import dcc
+from dash import html
 from dash.dependencies import Input, Output, State
-import dash_table
+from dash import dash_table
 import plotly.express as px
 import plotly.graph_objects as go
 import webbrowser
 
 from macrodemos.common_components import app_parameter, app_parameter_row, editable_cell_format, \
     colors, make_bottom_banner, make_top_banner
 
@@ -320,48 +320,62 @@
         return fig
 
     def plot_correlogram(self, lags):
         lags += 1
 
         df = pd.DataFrame({'actual': self.acf(lags=lags)} if self.isstationary else {'not defined':np.zeros(lags)})
         if self.show_estimates:
-            self.estimates['acf'] = acf(self.simulated_data, adjusted=True, nlags=lags-1, fft=False)
+            self.estimates['acf'], ci = acf(self.simulated_data, adjusted=True, nlags=lags-1, fft=False, alpha=0.05)
+            self.estimates['acf_lb'] = ci.T[0] - self.estimates['acf']
+            self.estimates['acf_ub'] = ci.T[1] - self.estimates['acf']
             df['estimated'] = self.estimates['acf']
 
-        fig = px.bar(df,
+        fig = px.bar(df.iloc[1:],
                      barmode='group',
                      title='Autocorrelations',
                      template='simple_white')
 
         fig.update_layout(
             legend_orientation='h',
             xaxis_title='Lag',
             yaxis_title=r'$\rho$'
         )
+
+        if self.show_estimates:
+            fig.add_trace(go.Scatter(x=np.arange(1, lags), y=self.estimates['acf_ub'][1:], line_color='#EFECF6', mode='lines',showlegend=False))
+            fig.add_trace(go.Scatter(x=np.arange(1, lags), y=self.estimates['acf_lb'][1:], fill='tonexty', line_color='#EFECF6', mode='lines', showlegend=False))
+
         return fig
 
 
     def plot_partial_correlogram(self, lags):
         lags += 1
 
         df = pd.DataFrame({'actual': self.pacf(lags=lags)} if self.isstationary else {'not defined':np.zeros(lags)})
         if self.show_estimates:
-            self.estimates['acf'] = pacf(self.simulated_data, nlags=lags-1)
-            df['estimated'] = self.estimates['acf']
+            self.estimates['pacf'], ci = pacf(self.simulated_data, nlags=lags-1, alpha=0.05)
+            self.estimates['pacf_lb'] = ci.T[0] - self.estimates['pacf']
+            self.estimates['pacf_ub'] = ci.T[1] - self.estimates['pacf']
+            df['estimated'] = self.estimates['pacf']
 
-        fig = px.bar(df,
+        fig = px.bar(df.iloc[1:],
                      barmode='group',
                      title='Partial Autocorrelations',
                      template='simple_white')
 
         fig.update_layout(
             legend_orientation='h',
             xaxis_title='Lag',
             yaxis_title=r'$\rho$'
         )
+        
+        if self.show_estimates:
+            fig.add_trace(go.Scatter(x=np.arange(1, lags), y=self.estimates['pacf_ub'][1:], line_color='#EFECF6', mode='lines',showlegend=False))
+            fig.add_trace(go.Scatter(x=np.arange(1, lags), y=self.estimates['pacf_lb'][1:], fill='tonexty', line_color='#EFECF6', mode='lines', showlegend=False))
+
         return fig
 
 
 
     def plot_process(self):
         df = pd.DataFrame({'actual':self.simulated_data.values,
                            r'$\mu$':self.mean})
```

### Comparing `macrodemos-2021.9.7/macrodemos/demo_BoxJenkins.py` & `macrodemos-2024.4.5/macrodemos/demo_BoxJenkins.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import base64
 import datetime
 import io
 
 
 from jupyter_dash import JupyterDash
-import dash_core_components as dcc
-import dash_html_components as html
+from dash import dcc
+from dash import html
 from dash.dependencies import Input, Output, State
 from dash_table import DataTable
 import plotly.express as px
 import plotly.graph_objects as go
 
 import webbrowser
 
@@ -141,28 +141,54 @@
         return self.y.plot(title=self.current_variable_name)
         # return px.line(y=self.y.values,
         #               title=self.current_variable_name,
         #               template='simple_white'
         #              )
 
     def plot_correlogram(self, lags):
-        return px.bar(y=acf(self.y.values, adjusted=True, nlags=lags, fft=False),
-                      title='Autocorrelations',
-                      labels=dict(x='lag', y='coefficient'),
-                      # color_discrete_sequence=px.colors.qualitative.Dark24,
-                      template='simple_white'
-                      )
+        xvalues = np.arange(1, lags+1)
+        acfvalues, ci = acf(self.y.values, adjusted=True, nlags=lags, fft=False, alpha=0.05)
+        acf_lb = ci.T[0] - acfvalues
+        acf_ub = ci.T[1] - acfvalues
+
+        fig = px.bar(
+            x=xvalues,
+            y=acfvalues[1:],
+            title='Autocorrelations',
+            labels=dict(x='lag', y='coefficient'),
+            # color_discrete_sequence=px.colors.qualitative.Dark24,
+            template='simple_white'
+            )
+
+        fig.add_trace(go.Scatter(x=xvalues, y=acf_ub[1:], line_color='#EFECF6', mode='lines',showlegend=False))
+        fig.add_trace(go.Scatter(x=xvalues, y=acf_lb[1:], fill='tonexty', line_color='#EFECF6', mode='lines', showlegend=False))
+
+        return fig
 
     def plot_partial_correlogram(self, lags):
-        return px.bar(y=pacf(self.y.values, nlags=lags),
-                      title='Partial Autocorrelations',
-                      labels=dict(x='lag', y='coefficient'),
-                      # color_discrete_sequence=px.colors.qualitative.Dark24,
-                      template='simple_white'
-                      )
+        xvalues = np.arange(1, lags+1)
+        pacfvalues, ci = acf(self.y.values, nlags=lags, alpha=0.05)
+        pacf_lb = ci.T[0] - pacfvalues
+        pacf_ub = ci.T[1] - pacfvalues
+
+        fig = px.bar(
+            x=xvalues,
+            y=pacfvalues[1:],
+            title='Partial Autocorrelations',
+            labels=dict(x='lag', y='coefficient'),
+            # color_discrete_sequence=px.colors.qualitative.Dark24,
+            template='simple_white'
+            )
+
+        fig.add_trace(go.Scatter(x=xvalues, y=pacf_ub[1:], line_color='#EFECF6', mode='lines',showlegend=False))
+        fig.add_trace(go.Scatter(x=xvalues, y=pacf_lb[1:], fill='tonexty', line_color='#EFECF6', mode='lines', showlegend=False))
+
+        return fig
+
+
 
     def plot_spectral(self):
 
         return px.area(
             x=omega,
             y=compute_spectral(self.y.values),
             title='Spectral Density',
```

### Comparing `macrodemos-2021.9.7/macrodemos/demo_Markov.py` & `macrodemos-2024.4.5/macrodemos/demo_Markov.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from jupyter_dash import JupyterDash
-import dash_core_components as dcc
-import dash_html_components as html
-import dash_table
+from dash import dcc
+from dash import html
+from dash import dash_table
 from dash.dependencies import Input, Output, State
 import plotly.express as px
 import webbrowser
 from warnings import warn
 
 from macrodemos.common_components import app_parameter_row, editable_cell_format, header_cell_format, \
     colors, make_top_banner, make_bottom_banner
```

### Comparing `macrodemos-2021.9.7/macrodemos/demo_Solow.py` & `macrodemos-2024.4.5/macrodemos/demo_Solow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from jupyter_dash import JupyterDash
-import dash_core_components as dcc
-import dash_html_components as html
+from dash import dcc
+from dash import html
 from dash.dependencies import Input, Output, State
 import plotly.express as px
 from dash_table import DataTable
 
 
 import webbrowser
```

### Comparing `macrodemos-2021.9.7/macrodemos/demo_filters.py` & `macrodemos-2024.4.5/macrodemos/demo_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 Randall Romero Aguilar
 2016-2021
 """
 
 
 from jupyter_dash import JupyterDash
-import dash_core_components as dcc
-import dash_html_components as html
+from dash import dcc
+from dash import html
 #import dash_bootstrap_components as dbc  #conda install -c conda-forge dash-bootstrap-components
 from dash.dependencies import Input, Output, State
 import plotly.graph_objects as go
 import plotly.express as px
 
 from macrodemos.common_components import app_parameter_row, app_choose_parameter, \
     colors, make_bottom_banner, make_top_banner
```

### Comparing `macrodemos-2021.9.7/macrodemos.egg-info/PKG-INFO` & `macrodemos-2024.4.5/macrodemos.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,67 @@
 Metadata-Version: 2.1
 Name: macrodemos
-Version: 2021.9.7
+Version: 2024.4.5
 Summary: Demo programs to learn macroeconomics and macro-econometrics concepts
 Home-page: http://randall-romero.com/code/macrodemos
 Author: Randall Romero-Aguilar
 Author-email: randall.romero@outlook.com
 License: MIT
-Description: # MACRODEMOS
-        
-        ## Macroeconomics Demos: A Python package to teach macroeconomics and macroeconometrics
-        
-        The purpose of this package is to provide tools to teach concepts of macroeconomics and macroeconometrics.
-        
-        To date, the package provides these functions:
-        
-        * **ARMA( )**: Demo for learning about  ARMA processes. It creates a dash consisting of 7 plots to study the theoretical properties of ARMA(p, q) processes, as well as their estimated counterparts. The plots display
-            1. a simulated sample
-            2. autocorrelations
-            3. partial autocorrelations
-            4. impulse response function
-            5. spectral density
-            6. AR inverse roots
-            7. MA inverse roots.
-        *  **Markov('state_0',...,'state_n')**: a demo to illustrate Markov chains. User sets the number of states, the transition matrix, and the initial distribution. The demo creates a dash consisting of 2 plots:
-            1. a simulated sample
-            2. the time evolution of the distribution of states
-        *  **Solow( )**: this demo illustrates the Solow-Swan model. Users can simulate the dynamic effect of a shock in a exogenous variable or a change in a model parameter. You will find 6 figures about the Solow-Swan model:
-            1. Capital stock, per capita
-            2. Output per capita,
-            3. Savings per capita,
-            4. Consumption per capita,
-            5. Change in capital stock, and
-            6. Output growth rate 
-           
-            It also presents plots to illustrate how steady-state capital is determined, and the golden rule. 
-        *  **filters( )**: to illustrate the use of the Hodrick-Prescott, Baxter-King, Christiano-Fitzgeral and Hamilton filters.
-        
-        In a near future, I expect to add a few more demos:
-        
-        * **Bellman( )**: to illustrate the solution of a Bellman equation by value function iteration
-        * **BoxJenkins( )**: to illustrate the Box-Jenkins methodology, by fitting two ARIMA models side-by-side to user-provided data.  
-        * **FilterMyData( )**: to filter user-supplied data with several methodologies, comparing their resulting cycles. 
-         
-        ### Instructions
-        To use the demos, just install this package `pip install macrodemos` and then run any of the demos you want.
-        
-            import macrodemos
-            macrodemos.ARMA()
-            macrodemos.Markov()
-            macrodemos.Solow()
-            macrodemos.filter()
-         
-        This will open a new tab in your default Internet browser with a Plotly dash. A current limitation is that you can only run 
-        one demo at a time.
-        
-        ### Disclaimer 
-        This program illustrates basic concepts of macroeconomics and time series econometrics. It was developed for teaching purposes 
-        only: you are free to use it in your own lectures or to learn about these topics.  
-        
-        If you have any suggestions, please send me an email at randall.romero@ucr.ac.cr
-                                  
-        **Copyright 2016-2021 Randall Romero-Aguilar**
-        
 Keywords: time series,ARMA,filters,Markov chain,Solow-Swan,Hodrick-Prescott,Baxter-King
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+
+# MACRODEMOS
+
+## Macroeconomics Demos: A Python package to teach macroeconomics and macroeconometrics
+
+The purpose of this package is to provide tools to teach concepts of macroeconomics and macroeconometrics.
+
+To date, the package provides these functions:
+
+* **ARMA( )**: Demo for learning about  ARMA processes. It creates a dash consisting of 7 plots to study the theoretical properties of ARMA(p, q) processes, as well as their estimated counterparts. The plots display
+    1. a simulated sample
+    2. autocorrelations
+    3. partial autocorrelations
+    4. impulse response function
+    5. spectral density
+    6. AR inverse roots
+    7. MA inverse roots.
+*  **Markov('state_0',...,'state_n')**: a demo to illustrate Markov chains. User sets the number of states, the transition matrix, and the initial distribution. The demo creates a dash consisting of 2 plots:
+    1. a simulated sample
+    2. the time evolution of the distribution of states
+*  **Solow( )**: this demo illustrates the Solow-Swan model. Users can simulate the dynamic effect of a shock in a exogenous variable or a change in a model parameter. You will find 6 figures about the Solow-Swan model:
+    1. Capital stock, per capita
+    2. Output per capita,
+    3. Savings per capita,
+    4. Consumption per capita,
+    5. Change in capital stock, and
+    6. Output growth rate 
+   
+    It also presents plots to illustrate how steady-state capital is determined, and the golden rule. 
+*  **filters( )**: to illustrate the use of the Hodrick-Prescott, Baxter-King, Christiano-Fitzgeral and Hamilton filters.
+
+In a near future, I expect to add a few more demos:
+
+* **Bellman( )**: to illustrate the solution of a Bellman equation by value function iteration
+* **BoxJenkins( )**: to illustrate the Box-Jenkins methodology, by fitting two ARIMA models side-by-side to user-provided data.  
+* **FilterMyData( )**: to filter user-supplied data with several methodologies, comparing their resulting cycles. 
+ 
+### Instructions
+To use the demos, just install this package `pip install macrodemos` and then run any of the demos you want.
+
+    import macrodemos
+    macrodemos.ARMA()
+    macrodemos.Markov()
+    macrodemos.Solow()
+    macrodemos.filter()
+ 
+This will open a new tab in your default Internet browser with a Plotly dash. A current limitation is that you can only run 
+one demo at a time.
+
+### Disclaimer 
+This program illustrates basic concepts of macroeconomics and time series econometrics. It was developed for teaching purposes 
+only: you are free to use it in your own lectures or to learn about these topics.  
+
+If you have any suggestions, please send me an email at randall.romero@ucr.ac.cr
+                          
+**Copyright 2016-2024 Randall Romero-Aguilar**
```

### Comparing `macrodemos-2021.9.7/macrodemos.egg-info/SOURCES.txt` & `macrodemos-2024.4.5/macrodemos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macrodemos-2021.9.7/setup.py` & `macrodemos-2024.4.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ The macrodemos package setup.
 Based on setuptools
 
-Randall Romero-Aguilar, 2016-2021
+Randall Romero-Aguilar, 2016-2024
 """
 
 from setuptools import setup
 from codecs import open
 from pathlib import Path
 import sys
 
@@ -15,15 +15,15 @@
 
 
 def get_long_description():
     return (CURRENT_DIR / "README.md").read_text(encoding='utf-8')
 
 setup(
     name='macrodemos',
-    version='2021.09.07',
+    version='2024.04.05',
     description='Demo programs to learn macroeconomics and macro-econometrics concepts',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Randall Romero-Aguilar',
     author_email='randall.romero@outlook.com',
     url='http://randall-romero.com/code/macrodemos',
     license='MIT',
```

