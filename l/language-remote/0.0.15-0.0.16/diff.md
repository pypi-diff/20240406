# Comparing `tmp/language-remote-0.0.15.tar.gz` & `tmp/language-remote-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "language-remote-0.0.15.tar", last modified: Mon Mar 11 21:25:12 2024, max compression
+gzip compressed data, was "language-remote-0.0.16.tar", last modified: Sat Apr  6 07:57:08 2024, max compression
```

## Comparing `language-remote-0.0.15.tar` & `language-remote-0.0.16.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:25:12.962475 language-remote-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-11 21:25:12.962475 language-remote-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-11 21:25:02.000000 language-remote-0.0.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:25:12.958475 language-remote-0.0.15/language_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:25:12.962475 language-remote-0.0.15/language_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 21:25:02.000000 language-remote-0.0.15/language_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-03-11 21:25:02.000000 language-remote-0.0.15/language_remote/src/lang_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 21:25:12.962475 language-remote-0.0.15/language_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-11 21:25:12.000000 language-remote-0.0.15/language_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-11 21:25:12.000000 language-remote-0.0.15/language_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 21:25:12.000000 language-remote-0.0.15/language_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 21:25:12.000000 language-remote-0.0.15/language_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-11 21:25:12.000000 language-remote-0.0.15/language_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-11 21:25:02.000000 language-remote-0.0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 21:25:12.962475 language-remote-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-11 21:25:02.000000 language-remote-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:57:07.995146 language-remote-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-06 07:57:07.995146 language-remote-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-06 07:56:49.000000 language-remote-0.0.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:57:07.995146 language-remote-0.0.16/language_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:57:07.995146 language-remote-0.0.16/language_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 07:56:49.000000 language-remote-0.0.16/language_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-04-06 07:56:49.000000 language-remote-0.0.16/language_remote/src/lang_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-06 07:56:49.000000 language-remote-0.0.16/language_remote/src/language_code_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:57:07.995146 language-remote-0.0.16/language_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 07:57:07.000000 language-remote-0.0.16/language_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-06 07:56:49.000000 language-remote-0.0.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:57:07.999146 language-remote-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-06 07:56:49.000000 language-remote-0.0.16/setup.py
```

### Comparing `language-remote-0.0.15/README.md` & `language-remote-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `language-remote-0.0.15/language_remote/src/lang_code.py` & `language-remote-0.0.16/language_remote/src/lang_code.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from enum import Enum
 from langdetect import detect, LangDetectException
 from collections import Counter
+# We can't use Logger because of circular dependency
+# LangCode <- Logger <- UserContext <- LangCode
+# use "pytest -s --log-cli-level=INFO" to see logs with pytest
+from python_sdk_remote.mini_logger import MiniLogger
 
 # TODO We should split between LangCodes which is all lang codes and LangCode which is the Type/Class
 # of one lang code
 # TODO We need those values in array or other data structure so we can present all lang code in menu,
 # so we can link them to country_id, so we can sort by langauge, sort by country ...
 
 
@@ -250,33 +254,47 @@
     CHINESE_SINGAPORE = 'zh-SG'
     CHINESE_TAIWAN = 'zh-TW'
     ZULU = 'zu'
     ZULU_SOUTH_AFRICA = 'zu-ZA'
 
     @staticmethod
     def validate(lang_code) -> bool:
+        VALIDATE_METHOD_NAME = 'validate'
+        MiniLogger.start(message=VALIDATE_METHOD_NAME, object={"lang_code": lang_code})
         if lang_code is not None and not isinstance(lang_code, LangCode):
             raise TypeError('lang_code must be an instance of LangCode or None')
+        MiniLogger.end(message=VALIDATE_METHOD_NAME, object={"lang_code": lang_code})
 
     @staticmethod
     def lang_code_str_to_lang_code(lang_code_str: str) -> 'LangCode':
         return LangCode(lang_code_str)
 
     @staticmethod
     def detect_lang_code_str(text: str, attempts=3) -> str | None:
+        DETECT_LANG_CODE_STR_METHOD_NAME = 'detect_lang_code_str'
+        MiniLogger.start(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"text": text, "attempts": attempts})
         try:
             results = [detect(text) for _ in range(attempts)]
             most_common_result, _ = Counter(results).most_common(1)[0]
             if '-' in most_common_result:
                 lang, country = most_common_result.split('-')
-                return f'{lang}-{country.upper()}'
+                result = f'{lang}-{country.upper()}'
+                MiniLogger.end(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"result": result})
+                return result
             else:
+                MiniLogger.end(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"result": most_common_result})
                 return most_common_result
         except LangDetectException:
+            MiniLogger.error(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"error": "LangDetectException"})
+            MiniLogger.end(message=DETECT_LANG_CODE_STR_METHOD_NAME, object={"result": None})
             return None
 
     @staticmethod
     def detect_lang_code(text: str, attempts=3) -> 'LangCode':
+        DETECT_LANG_CODE_METHOD_NAME = 'detect_lang_code'
+        MiniLogger.start(message=DETECT_LANG_CODE_METHOD_NAME, object={"text": text, "attempts": attempts})
         lang_code_str = LangCode.detect_lang_code_str(text, attempts)
         if lang_code_str is None:
+            MiniLogger.end(message=DETECT_LANG_CODE_METHOD_NAME, object={"result": None})
             return None
+        MiniLogger.end(message=DETECT_LANG_CODE_METHOD_NAME, object={"result": lang_code_str})
         return LangCode(lang_code_str)
```

### Comparing `language-remote-0.0.15/setup.py` & `language-remote-0.0.16/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "language-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/language-remote
-    version='0.0.15',
+    version='0.0.16',
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     #long_description=readme,
@@ -17,10 +17,11 @@
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        "langdetect>=1.0.9"
+        "langdetect>=1.0.9",
+        "logger-local>=0.0.3"
     ]
 )
```

