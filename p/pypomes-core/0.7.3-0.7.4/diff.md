# Comparing `tmp/pypomes_core-0.7.3.tar.gz` & `tmp/pypomes_core-0.7.4.tar.gz`

## Comparing `pypomes_core-0.7.3.tar` & `pypomes_core-0.7.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    20247 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     6763 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27937 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0    12055 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    20247 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.7.4/PKG-INFO
```

### Comparing `pypomes_core-0.7.3/src/pypomes_core/.ruff.toml` & `pypomes_core-0.7.4/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/__init__.py` & `pypomes_core-0.7.4/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/email_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/env_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/file_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/json_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/list_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/logging_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/str_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.7.4/src/pypomes_core/validation_msgs.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,44 +10,44 @@
         "pt": "Erro na interação com o armazenador de objetos: {}",
     },
     103: {
         "en": "No {} found",
         "pt": "Nenhum(a) {} encontrado(a)",
     },
     104: {
-        "en": "Unknown parameter: {}",
-        "pt": "Parâmetro desconhecido: {}",
+        "en": "Unknown attribute: {}",
+        "pt": "atributo desconhecido: {}",
     },
     105: {
-        "en": "Mandatory parameter: {}",
-        "pt": "Parâmetro obrigatório: {}",
+        "en": "Mandatory attribute: {}",
+        "pt": "atributo obrigatório: {}",
     },
     106: {
-        "en": "Invalid value {} for parameter {}",
-        "pt": "Valor {} inválido para o parâmetro {}",
+        "en": "Invalid value {} for attribute {}",
+        "pt": "Valor {} inválido para o atributo {}",
     },
     107: {
-        "en": "Invalid value {}: length shorter than {}",
-        "pt": "Valor {} inválido: comprimento menor que {}",
+        "en": "Invalid value {} for attribute {}: length shorter than {}",
+        "pt": "Valor {} inválido para o atributo {}: comprimento menor que {}",
     },
     108: {
-        "en": "Invalid value {} for parameter {}: length longer than {}",
-        "pt": "Valor {} inválido para o parâmetro {}: comprimento maior que {}",
+        "en": "Invalid value {} for attribute {}: length longer than {}",
+        "pt": "Valor {} inválido para o atributo {}: comprimento maior que {}",
     },
     109: {
-        "en": "Invalid value {} for parameter {}: length must be {}",
-        "pt": "Valor {} inválido para o parâmetro {}: comprimento deve ser igual a {}",
+        "en": "Invalid value {} for attribute {}: length must be {}",
+        "pt": "Valor {} inválido para o atributo {}: comprimento deve ser igual a {}",
     },
     110: {
-        "en": "Invalid value {} for parameter {}: date is later than the current date",
-        "pt": "Valor {} inválido para o parâmetro {}: data posterior à data atual",
+        "en": "Invalid value {} for attribute {}: date is later than the current date",
+        "pt": "Valor {} inválido para o atributo {}: data posterior à data atual",
     },
     111: {
-        "en": "Invalid value {} for parameter {}: wrong date format",
-        "pt": "Valor {} inválido para o parâmetro {}: formato de data inválido",
+        "en": "Invalid value {} for attribute {}: wrong date format",
+        "pt": "Valor {} inválido para o atributo {}: formato de data inválido",
     },
     112: {
         "en": "Error executing operation {}: {}",
         "pt": "Erro ao executar a operação {}: {}",
     },
     113: {
         "en": "The operation {} returned the error {}",
@@ -82,28 +82,28 @@
         "pt": "Mais de um(a) {} encontrado(a)",
     },
     121: {
         "en": "Invalid operation: {}",
         "pt": "Operação inválida: {}",
     },
     122: {
-        "en": "Invalid value {} for parameter {}: must be one of {}",
-        "pt": "Valor {} inválido para o parâmetro {}: deve ser um de {}",
+        "en": "Invalid value {} for attribute {}: must be one of {}",
+        "pt": "Valor {} inválido para o atributo {}: deve ser um de {}",
     },
     123: {
-        "en": "Invalid value {} for parameter {}: must be in the range {}",
-        "pt": "Valor {} inválido para o parâmetro {}: deve estar no intervalo {}",
+        "en": "Invalid value {} for attribute {}: must be in the range {}",
+        "pt": "Valor {} inválido para o atributo {}: deve estar no intervalo {}",
     },
     124: {
-        "en": "Invalid value {} for parameter {}: must be type {}",
-        "pt": "Valor {} inválido para o parâmetro {}: deve ser do tipo {}",
+        "en": "Invalid value {} for attribute {}: must be type {}",
+        "pt": "Valor {} inválido para o atributo {}: deve ser do tipo {}",
     },
     125: {
-        "en": "The values provided {} for parameter {} do not constitute a valid set of values",
-        "pt": "Os valores fornecidos {} para o parâmetro {} não formam um conjunto válido de valores",
+        "en": "The values provided {} for attribute {} do not constitute a valid set of values",
+        "pt": "Os valores fornecidos {} para o atributo {} não formam um conjunto válido de valores",
     },
     140: {
         "en": "Error retrieving environment variable {}: {}",
         "pt": "Erro na recuperação da variável de ambiente {}: {}",
     },
     141: {
         "en": "Error invoking service {}: {}",
```

### Comparing `pypomes_core-0.7.3/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/validation_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.7.4/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/LICENSE` & `pypomes_core-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.7.3/pyproject.toml` & `pypomes_core-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.7.3"
+version = "0.7.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.7.3/PKG-INFO` & `pypomes_core-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.7.3
+Version: 0.7.4
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

