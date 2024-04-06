# Comparing `tmp/ofdcomparer-1.5.37.tar.gz` & `tmp/ofdcomparer-1.5.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofdcomparer-1.5.37.tar", last modified: Thu Apr  4 19:16:01 2024, max compression
+gzip compressed data, was "ofdcomparer-1.5.38.tar", last modified: Sat Apr  6 09:22:05 2024, max compression
```

## Comparing `ofdcomparer-1.5.37.tar` & `ofdcomparer-1.5.38.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:16:01.445798 ofdcomparer-1.5.37/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 22:27:07.000000 ofdcomparer-1.5.37/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-04 19:16:01.445798 ofdcomparer-1.5.37/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-15 14:23:23.000000 ofdcomparer-1.5.37/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:16:01.442798 ofdcomparer-1.5.37/ofdcomparer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 22:27:07.000000 ofdcomparer-1.5.37/ofdcomparer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/allure_helper.py
--rw-rw-rw-   0 root         (0) root         (0)    21525 2024-04-04 19:15:02.000000 ofdcomparer-1.5.37/ofdcomparer/compare_ffd.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-10-19 22:27:07.000000 ofdcomparer-1.5.37/ofdcomparer/configs.py
--rw-rw-rw-   0 root         (0) root         (0)    13980 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/convert.py
--rw-rw-rw-   0 root         (0) root         (0)    39605 2024-03-06 23:14:00.000000 ofdcomparer-1.5.37/ofdcomparer/dto10.py
--rw-rw-rw-   0 root         (0) root         (0)    33848 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/dto_error_descriptions.py
--rw-rw-rw-   0 root         (0) root         (0)     8301 2024-03-06 23:14:00.000000 ofdcomparer-1.5.37/ofdcomparer/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1563 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/ofd_cri_atol.py
--rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-20 12:23:39.000000 ofdcomparer-1.5.37/ofdcomparer/ofd_taxcom.py
--rw-rw-rw-   0 root         (0) root         (0)    39179 2024-03-06 23:14:00.000000 ofdcomparer-1.5.37/ofdcomparer/tags_fn.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2024-04-04 19:15:02.000000 ofdcomparer-1.5.37/ofdcomparer/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 19:16:01.444798 ofdcomparer-1.5.37/ofdcomparer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      516 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-04 19:16:01.000000 ofdcomparer-1.5.37/ofdcomparer.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-04 19:16:01.445798 ofdcomparer-1.5.37/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-04 19:15:02.000000 ofdcomparer-1.5.37/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 09:22:05.561949 ofdcomparer-1.5.38/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 13:19:58.000000 ofdcomparer-1.5.38/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-06 09:22:05.561949 ofdcomparer-1.5.38/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-11-01 17:56:55.000000 ofdcomparer-1.5.38/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 09:22:05.560948 ofdcomparer-1.5.38/ofdcomparer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-10-19 13:19:58.000000 ofdcomparer-1.5.38/ofdcomparer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-01-12 13:37:12.000000 ofdcomparer-1.5.38/ofdcomparer/allure_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    21525 2024-04-06 09:21:48.000000 ofdcomparer-1.5.38/ofdcomparer/compare_ffd.py
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-06 09:21:48.000000 ofdcomparer-1.5.38/ofdcomparer/configs.py
+-rw-rw-rw-   0 root         (0) root         (0)    13995 2024-04-06 09:21:48.000000 ofdcomparer-1.5.38/ofdcomparer/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)    39765 2024-04-06 09:21:48.000000 ofdcomparer-1.5.38/ofdcomparer/dto10.py
+-rw-rw-rw-   0 root         (0) root         (0)    38203 2024-04-06 09:21:48.000000 ofdcomparer-1.5.38/ofdcomparer/dto_error_descriptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     8301 2024-01-23 20:47:59.000000 ofdcomparer-1.5.38/ofdcomparer/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2024-01-12 13:37:12.000000 ofdcomparer-1.5.38/ofdcomparer/ofd_cri_atol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2183 2024-01-12 14:45:58.000000 ofdcomparer-1.5.38/ofdcomparer/ofd_taxcom.py
+-rw-rw-rw-   0 root         (0) root         (0)    39179 2024-01-23 20:47:59.000000 ofdcomparer-1.5.38/ofdcomparer/tags_fn.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2024-03-09 15:40:06.000000 ofdcomparer-1.5.38/ofdcomparer/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 09:22:05.561949 ofdcomparer-1.5.38/ofdcomparer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-04-06 09:22:05.000000 ofdcomparer-1.5.38/ofdcomparer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      516 2024-04-06 09:22:05.000000 ofdcomparer-1.5.38/ofdcomparer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 09:22:05.000000 ofdcomparer-1.5.38/ofdcomparer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-06 09:22:05.000000 ofdcomparer-1.5.38/ofdcomparer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 09:22:05.000000 ofdcomparer-1.5.38/ofdcomparer.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-06 09:22:05.562949 ofdcomparer-1.5.38/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-06 09:21:48.000000 ofdcomparer-1.5.38/setup.py
```

### Comparing `ofdcomparer-1.5.37/PKG-INFO` & `ofdcomparer-1.5.38/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.37
+Version: 1.5.38
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.37/README.md` & `ofdcomparer-1.5.38/README.md`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.37/ofdcomparer/compare_ffd.py` & `ofdcomparer-1.5.38/ofdcomparer/compare_ffd.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.37/ofdcomparer/convert.py` & `ofdcomparer-1.5.38/ofdcomparer/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import logging
 import re
 import sys
 import time
 from datetime import datetime
 
 DOSSymbols = (
     ' !"#$%&`()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~'
```

### Comparing `ofdcomparer-1.5.37/ofdcomparer/dto10.py` & `ofdcomparer-1.5.38/ofdcomparer/dto10.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import inspect
 import json
 import logging
 import threading
 import time
 
-from ofdcomparer.dto_error_descriptions import get_dto_error_code_description
-from ofdcomparer.libfptr10 import IFptr
+from ofdcomparer.dto_error_descriptions import DtoErrorDescription
 
 
-class DTO10Helper:
+class DTO10Helper(DtoErrorDescription):
     def __init__(self, fptr=None):
-        self.fptr = fptr
+        super().__init__(fptr)
 
         # Информация о ФН
         self.fnWarnings = None
         self.fnVersion = None
         self.fnValidityDate = None
         self.fnSerial = None
         self.fnRegistrationsRemaining = None
@@ -58,22 +57,23 @@
         self.address = None
         self.agents = None
         self.email = None
         self.name = None
         self.taxationTypes = None
         self.vatin = None
 
-        if fptr is None:
-            while True:
-                try:
-                    self.fptr = IFptr()
-                except Exception:
-                    raise Exception("Error creating DTO 10")
-                if self.fptr.interface.value is not None:
-                    break
+        # 06.04.24
+        # if fptr is None:
+        #     while True:
+        #         try:
+        #             self.fptr = self.IFptr()
+        #         except Exception:
+        #             raise Exception("Error creating DTO 10")
+        #         if self.fptr.interface.value is not None:
+        #             break
 
         self.dto10_version = self.fptr.version().decode("cp866")
 
         self.ErrorCode = None
         self.ErrorDescription = None
         self.JsonAnswer = None
 
@@ -102,15 +102,15 @@
     def close(self):
         self.fptr.close()
         return self.request_error_code()
 
     def request_error_code(self, flag_all_kkt_settings=False):
         self.ErrorCode = self.fptr.errorCode()
         self.ErrorDescription = self.fptr.errorDescription()
-        pytest_dto_error_description = get_dto_error_code_description(self.ErrorCode)
+        pytest_dto_error_description = self.get_dto_error_code_description(self.ErrorCode)
         if self.ErrorDescription != pytest_dto_error_description:
             logging.error(f"Код ошибки ДТО: {self.ErrorCode}")
             logging.error(
                 f"ДТО [{self.ErrorDescription}] <-> "
                 f"[{pytest_dto_error_description}] const.dto_error_descriptions"
             )
             logging.error(
@@ -420,26 +420,26 @@
     def print_custom_text(self, text_tuple: tuple):
         """
         Метод печати нефискального текста на ЧЛ
         """
         self.fptr.open()
         self.fptr.beginNonfiscalDocument()
         for text in text_tuple:
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_TEXT, text)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_ALIGNMENT, 0)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_TEXT_WRAP, 0)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_FONT, 0)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_FONT_DOUBLE_HEIGHT, False)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_FONT_DOUBLE_WIDTH, False)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_FORMAT_TEXT, False)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_LINESPACING, 0)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_BRIGHTNESS, 0)
-            self.fptr.setParam(IFptr.LIBFPTR_PARAM_STORE_IN_JOURNAL, True)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_TEXT, text)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_ALIGNMENT, 0)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_TEXT_WRAP, 0)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_FONT, 0)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_FONT_DOUBLE_HEIGHT, False)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_FONT_DOUBLE_WIDTH, False)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_FORMAT_TEXT, False)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_LINESPACING, 0)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_BRIGHTNESS, 0)
+            self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_STORE_IN_JOURNAL, True)
             self.fptr.printText()
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_PRINT_FOOTER, False)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_PRINT_FOOTER, False)
         self.fptr.endNonfiscalDocument()
         self.fptr.close()
 
     def get_fn_info(self):
         self.fptr.setParam(
             self.fptr.LIBFPTR_PARAM_FN_DATA_TYPE, self.fptr.LIBFPTR_FNDT_FN_INFO
         )
@@ -479,15 +479,15 @@
             critical_error,
         )
 
     def init_mgm(self):
         self.fptr.initMgm()
         return self.request_error_code()
 
-    def get_last_doc_with_template(self, tempalate, variable_settings=None):
+    def get_last_doc_with_template(self, template, variable_settings=None):
         last_fn_doc_number = self.get_last_fiscal_document_number()
         last_fn_doc_str = None
         for _ in range(3):
             request_last_fn_doc = (
                     '{"type": "getFnDocument", "fiscalDocumentNumber": %i}'
                     % last_fn_doc_number
             )
@@ -659,57 +659,57 @@
             logging.debug("ККТ доступна")
             return True
         logging.debug("ККТ не отвечает")
         return False
 
     def print_info_report(self):
         self.fptr.open()
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_REPORT_TYPE, 5)
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_REPORT_ELECTRONICALLY, 0)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_REPORT_TYPE, 5)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_REPORT_ELECTRONICALLY, 0)
         self.fptr.report()
 
     def get_TPG_count(self) -> int:
         """
         Получить ресурс ТПГ (постоянный)
         """
         self.fptr.open()
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_DATA_TYPE, IFptr.LIBFPTR_DT_TERMAL_RESOURCE)
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_COUNTER_TYPE, IFptr.LIBFPTR_CT_ROLLUP)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_DATA_TYPE, self.IFptr.LIBFPTR_DT_TERMAL_RESOURCE)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_COUNTER_TYPE, self.IFptr.LIBFPTR_CT_ROLLUP)
         self.fptr.queryData()
-        count = self.fptr.getParamInt(IFptr.LIBFPTR_PARAM_COUNT)
+        count = self.fptr.getParamInt(self.IFptr.LIBFPTR_PARAM_COUNT)
 
         if count == 0:
             self.print_info_report()
 
         return count
 
     def get_TPG_temperature(self):
         """
         Получить температуру ТПГ
         """
         self.fptr.open()
 
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_DATA_TYPE, IFptr.LIBFPTR_DT_PRINTER_TEMPERATURE)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_DATA_TYPE, self.IFptr.LIBFPTR_DT_PRINTER_TEMPERATURE)
         self.fptr.queryData()
 
-        temperature = self.fptr.getParamString(IFptr.LIBFPTR_PARAM_PRINTER_TEMPERATURE)
+        temperature = self.fptr.getParamString(self.IFptr.LIBFPTR_PARAM_PRINTER_TEMPERATURE)
         return temperature
 
     def get_TPG_motor_count(self):
         """
         Получить ресурс шагового двигателя
         """
         self.fptr.open()
 
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_DATA_TYPE, IFptr.LIBFPTR_DT_STEP_RESOURCE)
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_COUNTER_TYPE, IFptr.LIBFPTR_CT_ROLLUP)
-        self.fptr.setParam(IFptr.LIBFPTR_PARAM_STEP_COUNTER_TYPE, IFptr.LIBFPTR_SCT_OVERALL)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_DATA_TYPE, self.IFptr.LIBFPTR_DT_STEP_RESOURCE)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_COUNTER_TYPE, self.IFptr.LIBFPTR_CT_ROLLUP)
+        self.fptr.setParam(self.IFptr.LIBFPTR_PARAM_STEP_COUNTER_TYPE, self.IFptr.LIBFPTR_SCT_OVERALL)
         self.fptr.queryData()
 
-        count = self.fptr.getParamInt(IFptr.LIBFPTR_PARAM_COUNT)
+        count = self.fptr.getParamInt(self.IFptr.LIBFPTR_PARAM_COUNT)
 
         return count
 
     def get_registration_data(self):
         """
         Метод запрашивает информацию о регистрации и записывает в атрибуты класса
         organization	Информация об организации	object
```

### Comparing `ofdcomparer-1.5.37/ofdcomparer/helpers.py` & `ofdcomparer-1.5.38/ofdcomparer/helpers.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.37/ofdcomparer/ofd_cri_atol.py` & `ofdcomparer-1.5.38/ofdcomparer/ofd_cri_atol.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.37/ofdcomparer/ofd_taxcom.py` & `ofdcomparer-1.5.38/ofdcomparer/ofd_taxcom.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.37/ofdcomparer/tags_fn.py` & `ofdcomparer-1.5.38/ofdcomparer/tags_fn.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.37/ofdcomparer/utils.py` & `ofdcomparer-1.5.38/ofdcomparer/utils.py`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.37/ofdcomparer.egg-info/PKG-INFO` & `ofdcomparer-1.5.38/ofdcomparer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofdcomparer
-Version: 1.5.37
+Version: 1.5.38
 Summary: Библиотека для сравнивания ФД из ФН и ОФД
 Home-page: UNKNOWN
 Author-email: k.kabisova@atol.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ofdcomparer-1.5.37/ofdcomparer.egg-info/SOURCES.txt` & `ofdcomparer-1.5.38/ofdcomparer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ofdcomparer-1.5.37/setup.py` & `ofdcomparer-1.5.38/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ofdcomparer",
-    version="1.5.37",
+    version="1.5.38",
     long_description=long_description,
     description="Библиотека для сравнивания ФД из ФН и ОФД",
     packages=["ofdcomparer"],
     author_email="k.kabisova@atol.ru",
     install_requires=[
         "requests==2.31.0",
         "requests-toolbelt==1.0.0",
```

