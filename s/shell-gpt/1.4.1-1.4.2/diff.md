# Comparing `tmp/shell_gpt-1.4.1.tar.gz` & `tmp/shell_gpt-1.4.2.tar.gz`

## Comparing `shell_gpt-1.4.1.tar` & `shell_gpt-1.4.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/__version__.py
--rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/app.py
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/cache.py
--rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/config.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/function.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/integration.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/printer.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/role.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/__init__.py
--rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/chat_handler.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/default_handler.py
--rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/handler.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/handlers/repl_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/llm_functions/__init__.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/llm_functions/init_functions.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/llm_functions/common/execute_shell.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/sgpt/llm_functions/mac/apple_script.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/__init__.py
--rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/_integration.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/conftest.py
--rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/test_code.py
--rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/test_default.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/test_roles.py
--rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/test_shell.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/tests/utils.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/LICENSE
--rw-r--r--   0        0        0    25954 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/README.md
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/pyproject.toml
--rw-r--r--   0        0        0    28160 2020-02-02 00:00:00.000000 shell_gpt-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/__main__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/__version__.py
+-rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/app.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/cache.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/config.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/function.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/integration.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/printer.py
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/role.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/handlers/__init__.py
+-rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/handlers/chat_handler.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/handlers/default_handler.py
+-rw-r--r--   0        0        0     5281 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/handlers/handler.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/handlers/repl_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/llm_functions/__init__.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/llm_functions/init_functions.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/llm_functions/common/execute_shell.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/sgpt/llm_functions/mac/apple_script.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0    18975 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/tests/_integration.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/tests/test_code.py
+-rw-r--r--   0        0        0     8361 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/tests/test_default.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/tests/test_roles.py
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/tests/test_shell.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/tests/utils.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/LICENSE
+-rw-r--r--   0        0        0    25954 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/README.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0    28160 2020-02-02 00:00:00.000000 shell_gpt-1.4.2/PKG-INFO
```

### Comparing `shell_gpt-1.4.1/sgpt/app.py` & `shell_gpt-1.4.2/sgpt/app.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/cache.py` & `shell_gpt-1.4.2/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/config.py` & `shell_gpt-1.4.2/sgpt/config.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/function.py` & `shell_gpt-1.4.2/sgpt/function.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/integration.py` & `shell_gpt-1.4.2/sgpt/integration.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/printer.py` & `shell_gpt-1.4.2/sgpt/printer.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/role.py` & `shell_gpt-1.4.2/sgpt/role.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/utils.py` & `shell_gpt-1.4.2/sgpt/utils.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/handlers/chat_handler.py` & `shell_gpt-1.4.2/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/handlers/default_handler.py` & `shell_gpt-1.4.2/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/handlers/handler.py` & `shell_gpt-1.4.2/sgpt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/handlers/repl_handler.py` & `shell_gpt-1.4.2/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/llm_functions/init_functions.py` & `shell_gpt-1.4.2/sgpt/llm_functions/init_functions.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/llm_functions/common/execute_shell.py` & `shell_gpt-1.4.2/sgpt/llm_functions/common/execute_shell.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/sgpt/llm_functions/mac/apple_script.py` & `shell_gpt-1.4.2/sgpt/llm_functions/mac/apple_script.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/tests/_integration.py` & `shell_gpt-1.4.2/tests/_integration.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/tests/test_code.py` & `shell_gpt-1.4.2/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/tests/test_default.py` & `shell_gpt-1.4.2/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/tests/test_roles.py` & `shell_gpt-1.4.2/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/tests/test_shell.py` & `shell_gpt-1.4.2/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/tests/utils.py` & `shell_gpt-1.4.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/LICENSE` & `shell_gpt-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/README.md` & `shell_gpt-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/pyproject.toml` & `shell_gpt-1.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shell_gpt-1.4.1/PKG-INFO` & `shell_gpt-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: shell_gpt
-Version: 1.4.1
+Version: 1.4.2
 Summary: A command-line productivity tool powered by large language models, will help you accomplish your tasks faster and more efficiently.
 Project-URL: homepage, https://github.com/ther1d/shell_gpt
 Project-URL: repository, https://github.com/ther1d/shell_gpt
 Project-URL: documentation, https://github.com/TheR1D/shell_gpt/blob/main/README.md
 Author-email: Farkhod Sadykov <farkhod@sadykov.dev>
 License-Expression: MIT
 License-File: LICENSE
```

