# Comparing `tmp/snakemake_executor_plugin_googlebatch-0.3.1.tar.gz` & `tmp/snakemake_executor_plugin_googlebatch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_googlebatch-0.3.1.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_googlebatch-0.3.2.tar", max compression
```

## Comparing `snakemake_executor_plugin_googlebatch-0.3.1.tar` & `snakemake_executor_plugin_googlebatch-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1128 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/LICENSE
--rw-r--r--   0        0        0     1167 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/NOTICE
--rw-r--r--   0        0        0     1326 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/README.md
--rw-r--r--   0        0        0     1181 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6275 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/__init__.py
--rw-r--r--   0        0        0     5611 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/command.py
--rw-r--r--   0        0        0    17470 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/executor.py
--rw-r--r--   0        0        0     5588 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/snippet.py
--rw-r--r--   0        0        0      171 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/include/paths.sh
--rw-r--r--   0        0        0      265 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/run.sh
--rw-r--r--   0        0        0      447 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/setup.sh
--rw-r--r--   0        0        0     1530 2024-03-12 10:05:25.270400 snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/utils.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 snakemake_executor_plugin_googlebatch-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1128 2024-04-05 22:38:56.231194 snakemake_executor_plugin_googlebatch-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1167 2024-04-05 22:38:56.231194 snakemake_executor_plugin_googlebatch-0.3.2/NOTICE
+-rw-r--r--   0        0        0     1326 2024-04-05 22:38:56.231194 snakemake_executor_plugin_googlebatch-0.3.2/README.md
+-rw-r--r--   0        0        0     1181 2024-04-05 22:38:56.231194 snakemake_executor_plugin_googlebatch-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6275 2024-04-05 22:38:56.231194 snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/__init__.py
+-rw-r--r--   0        0        0     5638 2024-04-05 22:38:56.231194 snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/command.py
+-rw-r--r--   0        0        0    17470 2024-04-05 22:38:56.231194 snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/executor.py
+-rw-r--r--   0        0        0     5588 2024-04-05 22:38:56.231194 snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/snippet.py
+-rw-r--r--   0        0        0      171 2024-04-05 22:38:56.235194 snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/include/paths.sh
+-rw-r--r--   0        0        0      265 2024-04-05 22:38:56.235194 snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/run.sh
+-rw-r--r--   0        0        0      447 2024-04-05 22:38:56.235194 snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/snippets/intel-mpi/setup.sh
+-rw-r--r--   0        0        0     1530 2024-04-05 22:38:56.235194 snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/utils.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 snakemake_executor_plugin_googlebatch-0.3.2/PKG-INFO
```

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/LICENSE` & `snakemake_executor_plugin_googlebatch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/NOTICE` & `snakemake_executor_plugin_googlebatch-0.3.2/NOTICE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/README.md` & `snakemake_executor_plugin_googlebatch-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/pyproject.toml` & `snakemake_executor_plugin_googlebatch-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-googlebatch"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = [
     "Vanessa Sochat <sochat1@llnl.gov>",
     "Johannes Koester <johannes.koester@uni-due.de>"
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/__init__.py` & `snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/command.py` & `snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 workdir=$(pwd)
 url=https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
 wget ${url} -O ./miniconda.sh
 chmod +x ./miniconda.sh
 bash ./miniconda.sh -b -u -p /opt/conda
 rm -rf ./miniconda.sh
 
+conda install datrie --yes
 which python
 /opt/conda/bin/python --version
 ./install-snek.sh https://github.com/snakemake/snakemake-storage-plugin-gcs
 ./install-snek.sh https://github.com/snakemake/snakemake
 
 cd ${workdir}
 """
```

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/executor.py` & `snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/executor.py`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/snippet.py` & `snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/snippet.py`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/snakemake_executor_plugin_googlebatch/utils.py` & `snakemake_executor_plugin_googlebatch-0.3.2/snakemake_executor_plugin_googlebatch/utils.py`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_googlebatch-0.3.1/PKG-INFO` & `snakemake_executor_plugin_googlebatch-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-googlebatch
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Home-page: https://github.com/snakemake/snakemake-executor-plugin-googlebatch
 License: MIT
 Keywords: snakemake,plugin,executor,cloud,google-batch
 Author: Vanessa Sochat
 Author-email: sochat1@llnl.gov
 Requires-Python: >=3.11,<4.0
```

