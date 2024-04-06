# Comparing `tmp/praklib-0.1.365.tar.gz` & `tmp/praklib-0.1.369.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.365.tar", last modified: Fri Apr  5 17:21:39 2024, max compression
+gzip compressed data, was "praklib-0.1.369.tar", last modified: Fri Apr  5 18:15:58 2024, max compression
```

## Comparing `praklib-0.1.365.tar` & `praklib-0.1.369.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 17:21:39.216297 praklib-0.1.365/
--rw-rw-rw-   0        0        0      263 2024-04-05 17:21:39.216297 praklib-0.1.365/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 17:21:39.203430 praklib-0.1.365/praklib/
--rw-rw-rw-   0        0        0     5969 2024-04-05 17:21:38.000000 praklib-0.1.365/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.365/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 17:21:39.214293 praklib-0.1.365/praklib.egg-info/
--rw-rw-rw-   0        0        0      263 2024-04-05 17:21:39.000000 praklib-0.1.365/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 17:21:39.000000 praklib-0.1.365/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 17:21:39.000000 praklib-0.1.365/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 17:21:39.000000 praklib-0.1.365/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 17:21:39.216297 praklib-0.1.365/setup.cfg
--rw-rw-rw-   0        0        0      382 2024-04-05 17:21:38.000000 praklib-0.1.365/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:15:58.640280 praklib-0.1.369/
+-rw-rw-rw-   0        0        0      263 2024-04-05 18:15:58.639412 praklib-0.1.369/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-05 18:15:58.616959 praklib-0.1.369/praklib/
+-rw-rw-rw-   0        0        0     6121 2024-04-05 18:15:57.000000 praklib-0.1.369/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.369/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 18:15:58.637392 praklib-0.1.369/praklib.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-04-05 18:15:58.000000 praklib-0.1.369/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-05 18:15:58.000000 praklib-0.1.369/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 18:15:58.000000 praklib-0.1.369/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-05 18:15:58.000000 praklib-0.1.369/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 18:15:58.640280 praklib-0.1.369/setup.cfg
+-rw-rw-rw-   0        0        0      382 2024-04-05 18:15:57.000000 praklib-0.1.369/setup.py
```

### Comparing `praklib-0.1.365/praklib/Praktika.py` & `praklib-0.1.369/praklib/Praktika.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,34 +38,35 @@
     # Round the value and the error
     rounded_value = round(value, rounding_precision)
     rounded_error = round(error, rounding_precision)
 
     return rounded_value, rounded_error
 
 def graf(x, y, errx, erry, xlabel, ylabel, linelabel, scatterlabel,
-                grid=True, show=True, scatter=True, line=False, err=True, xlim=(0,0), ylim =(0,0), loc="upper right"):
+        grid=True, show=True, scatter=True, line=False, err=True, xlim=(0,0), ylim =(0,0), loc="upper right",
+        scattercolor="red", linecolor="teal", marker="x"):
     if (xlim == (0,0)):
         plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
     else:
         plt.xlim(xlim[0], xlim[1])
     if (ylim != (0,0)):
         plt.ylim(ylim[0], ylim[1])
     if (grid == True):
         plt.grid(True, linestyle="dashed")
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
 
     if (line == True):
-        f, = plt.plot(x, y, linewidth=0.8, c="teal",
+        f, = plt.plot(x, y, linewidth=0.8, c=linecolor,
                   label=linelabel, marker="none")
     if (scatter == True):
-        g = plt.scatter(x, y, s=5, facecolor="red", marker='x', zorder=2, label=scatterlabel)
+        g = plt.scatter(x, y, s=5, facecolor=scattercolor, marker=marker, zorder=2, label=scatterlabel)
     if (err == True):
         plt.errorbar(x, y, xerr=errx, yerr=erry, zorder=1, capsize=2, fmt='none',
-                 ecolor="red", linewidth=1.0)
+                 ecolor=scattercolor, linewidth=1.0)
     plt.legend(loc=loc)
     if (show == True):
         plt.show()
 def fit_data(y, z, initial_params, fit_function, show_results=True):
     model = Model(fit_function)
     params = model.make_params()
     for param_name in initial_params.keys():
@@ -77,15 +78,16 @@
     param_names = list(results.params.keys())
     param_values = [results.params[name].value for name in param_names]
     param_errors = [results.params[name].stderr if results.params[name].stderr else 0 for name in param_names]
 
     return param_names, param_values, param_errors
 
 def graf_fit(x, y, fit_vstup, fit_vystup, errx, erry, xlabel, ylabel, linelabel, scatterlabel, params_fit,
-                fit_function, grid=True, show=True, scatter=True, xlim=(0,0), ylim =(0,0), loc="upper right"):
+             fit_function, grid=True, show=True, scatter=True, xlim=(0,0), ylim =(0,0), loc="upper right",
+             scattercolor="red", linecolor="teal", marker="x"):
     if (xlim == (0, 0)):
         plt.xlim(x[0] - errx[0], x[len(x) - 1] + errx[len(x) - 1])
     else:
         plt.xlim(xlim[0], xlim[1])
     if (ylim != (0,0)):
         plt.ylim(ylim[0], ylim[1])
     data1 = np.linspace(x[0]-errx[0], x[-1]+errx[-1], 500)
@@ -97,19 +99,19 @@
     data2 = fit_function(data1, **params)
 
     if grid:
         plt.grid(True, linestyle="dashed")
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
 
-    plt.plot(data1, data2.real, linewidth=0.8, c="teal", label=linelabel)
+    plt.plot(data1, data2.real, linewidth=0.8, c=linecolor, label=linelabel)
     if scatter:
-        plt.scatter(x, y, s=5, facecolor="red", marker='x', zorder=2, label=scatterlabel)
+        plt.scatter(x, y, s=5, facecolor=scattercolor, marker=marker, zorder=2, label=scatterlabel)
     plt.errorbar(x, y, xerr=errx, yerr=erry, zorder=1, capsize=2, fmt='none',
-                 ecolor="red", linewidth=1.0)
+                 ecolor=scattercolor, linewidth=1.0)
     plt.legend(loc=loc)
     if show==True:
         plt.show()
 
 
 def latex_table(data, col_names, err=True):
     num_rows = len(data)
```

