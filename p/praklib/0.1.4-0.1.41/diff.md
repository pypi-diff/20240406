# Comparing `tmp/praklib-0.1.4.tar.gz` & `tmp/praklib-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praklib-0.1.4.tar", last modified: Sat Apr  6 10:01:04 2024, max compression
+gzip compressed data, was "praklib-0.1.41.tar", last modified: Sat Apr  6 10:05:24 2024, max compression
```

## Comparing `praklib-0.1.4.tar` & `praklib-0.1.41.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 10:01:04.773447 praklib-0.1.4/
--rw-rw-rw-   0        0        0      261 2024-04-06 10:01:04.772447 praklib-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 10:01:04.751441 praklib-0.1.4/praklib/
--rw-rw-rw-   0        0        0     6115 2024-04-05 22:15:24.000000 praklib-0.1.4/praklib/Praktika.py
--rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.4/praklib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 10:01:04.770447 praklib-0.1.4/praklib.egg-info/
--rw-rw-rw-   0        0        0      261 2024-04-06 10:01:04.000000 praklib-0.1.4/praklib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-04-06 10:01:04.000000 praklib-0.1.4/praklib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 10:01:04.000000 praklib-0.1.4/praklib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-06 10:01:04.000000 praklib-0.1.4/praklib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 10:01:04.773447 praklib-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      380 2024-04-06 10:01:03.000000 praklib-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:05:24.376040 praklib-0.1.41/
+-rw-rw-rw-   0        0        0      262 2024-04-06 10:05:24.375040 praklib-0.1.41/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 10:05:24.358978 praklib-0.1.41/praklib/
+-rw-rw-rw-   0        0        0     6211 2024-04-06 10:05:17.000000 praklib-0.1.41/praklib/Praktika.py
+-rw-rw-rw-   0        0        0        0 2024-04-04 13:28:05.000000 praklib-0.1.41/praklib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 10:05:24.374037 praklib-0.1.41/praklib.egg-info/
+-rw-rw-rw-   0        0        0      262 2024-04-06 10:05:24.000000 praklib-0.1.41/praklib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-04-06 10:05:24.000000 praklib-0.1.41/praklib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 10:05:24.000000 praklib-0.1.41/praklib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-06 10:05:24.000000 praklib-0.1.41/praklib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 10:05:24.376040 praklib-0.1.41/setup.cfg
+-rw-rw-rw-   0        0        0      381 2024-04-06 10:05:23.000000 praklib-0.1.41/setup.py
```

### Comparing `praklib-0.1.4/praklib/Praktika.py` & `praklib-0.1.41/praklib/Praktika.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,17 @@
     latex_table += "\\centering\n"
     latex_table += "\\begin{tabular}{|" + "|".join(["c"] * (num_cols)) + "|}\n"
     latex_table += "\\hline\n"
     latex_table += " " + " & ".join(col_names) + " \\\\\n"
     latex_table += "\\hline\n"
 
     if err==True:
+        with_err = [[(row[i], row[i + 1]) for i in range(0, len(row), 2)] for row in data]
         for i in range(num_rows):
-            latex_table += " " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in data[i]]) + " \\\\ \\hline \n"
+            latex_table += " " + " & ".join([f"${val[0]} \\pm {val[1]}$" for val in with_err[i]]) + " \\\\ \\hline \n"
     if err==False:
         for i in range(num_rows):
             latex_table += " " + " & ".join([f"${val}$" for val in data[i]]) + " \\\\ \\hline \n"
 
     latex_table += "\\hline\n"
     latex_table += "\\end{tabular}\n"
     latex_table += "\\caption{Values and their errors}\n"
```

