# Comparing `tmp/praklib-0.1.369.tar.gz` & `tmp/praklib-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.369.tar", last modified: Fri Apr  5 18:15:58 2024, max compression
+gzip compressed data, was "praklib-0.1.4.tar", last modified: Sat Apr  6 10:01:04 2024, max compression
```

## Comparing `praklib-0.1.369.tar` & `praklib-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 18:15:58.640280 praklib-0.1.369/
--rw-rw-rw-   0        0        0      263 2024-04-05 18:15:58.639412 praklib-0.1.369/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-05 18:15:58.616959 praklib-0.1.369/praklib/
--rw-rw-rw-   0        0        0     6121 2024-04-05 18:15:57.000000 praklib-0.1.369/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.369/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:15:58.637392 praklib-0.1.369/praklib.egg-info/
--rw-rw-rw-   0        0        0      263 2024-04-05 18:15:58.000000 praklib-0.1.369/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-05 18:15:58.000000 praklib-0.1.369/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:15:58.000000 praklib-0.1.369/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-05 18:15:58.000000 praklib-0.1.369/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 18:15:58.640280 praklib-0.1.369/setup.cfg
--rw-rw-rw-   0        0        0      382 2024-04-05 18:15:57.000000 praklib-0.1.369/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:01:04.773447 praklib-0.1.4/
+-rw-rw-rw-   0        0        0      261 2024-04-06 10:01:04.772447 praklib-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 10:01:04.751441 praklib-0.1.4/praklib/
+-rw-rw-rw-   0        0        0     6115 2024-04-05 22:15:24.000000 praklib-0.1.4/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.4/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:01:04.770447 praklib-0.1.4/praklib.egg-info/
+-rw-rw-rw-   0        0        0      261 2024-04-06 10:01:04.000000 praklib-0.1.4/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-06 10:01:04.000000 praklib-0.1.4/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 10:01:04.000000 praklib-0.1.4/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 10:01:04.000000 praklib-0.1.4/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 10:01:04.773447 praklib-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      380 2024-04-06 10:01:03.000000 praklib-0.1.4/setup.py
```

### Comparing `praklib-0.1.369/praklib/Praktika.py` & `praklib-0.1.4/praklib/Praktika.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,23 +117,23 @@
     num_rows = len(data)
     num_cols = len(data[0])
 
     latex_table = "\\begin{table}[h!]\n"
     latex_table += "\\centering\n"
     latex_table += "\\begin{tabular}{|" + "|".join(["c"] * (num_cols)) + "|}\n"
     latex_table += "\\hline\n"
-    latex_table += " & " + " & ".join(col_names) + " \\\\\n"
+    latex_table += " " + " & ".join(col_names) + " \\\\\n"
     latex_table += "\\hline\n"
 
     if err==True:
         for i in range(num_rows):
-            latex_table += " & " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in data[i]]) + " \\\\ \\hline \n"
+            latex_table += " " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in data[i]]) + " \\\\ \\hline \n"
     if err==False:
         for i in range(num_rows):
-            latex_table += " & " + " & ".join([f"${val}$" for val in data[i]]) + " \\\\ \\hline \n"
+            latex_table += " " + " & ".join([f"${val}$" for val in data[i]]) + " \\\\ \\hline \n"
 
     latex_table += "\\hline\n"
     latex_table += "\\end{tabular}\n"
     latex_table += "\\caption{Values and their errors}\n"
     latex_table += "\\label{tab:values}\n"
     latex_table += "\\end{table}"
```

