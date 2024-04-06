# Comparing `tmp/atypical-0.0.0.tar.gz` & `tmp/atypical-0.2.0.tar.gz`

## Comparing `atypical-0.0.0.tar` & `atypical-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atypical-0.0.0/atypical/__init__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 atypical-0.0.0/atypical/currency.py
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 atypical-0.0.0/atypical/email.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 atypical-0.0.0/atypical/money.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 atypical-0.0.0/atypical/phone.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 atypical-0.0.0/atypical/url.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 atypical-0.0.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 atypical-0.0.0/LICENSE
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 atypical-0.0.0/README.md
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 atypical-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 atypical-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/__init__.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/currency.py
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/email.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/money.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/phone.py
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 atypical-0.2.0/atypical/url.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 atypical-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 atypical-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 atypical-0.2.0/README.md
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 atypical-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 atypical-0.2.0/PKG-INFO
```

### Comparing `atypical-0.0.0/atypical/currency.py` & `atypical-0.2.0/atypical/currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 
 import babel
 import babel.numbers
 from babel.numbers import LC_NUMERIC
-from foundational.enum import StringEnum
+from communal.enum import StringEnum
 
 
 class CurrencyCode:
     def __init__(self, code):
         if isinstance(code, CurrencyCode):
             self.code = code
         elif isinstance(code, str):
```

### Comparing `atypical-0.0.0/atypical/email.py` & `atypical-0.2.0/atypical/email.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from email.utils import parseaddr
 from functools import total_ordering
 
-from foundational.enum import StringEnum
+from communal.enum import StringEnum
 from sartorial import JSONSchemaFormatted, Serializable
 
 
 class EmailProvider(StringEnum):
     FASTMAIL = "fastmail"
     GMAIL = "gmail"
     MICROSOFT = "microsoft"
```

### Comparing `atypical-0.0.0/atypical/money.py` & `atypical-0.2.0/atypical/money.py`

 * *Files identical despite different names*

### Comparing `atypical-0.0.0/atypical/phone.py` & `atypical-0.2.0/atypical/phone.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from phonenumbers.phonenumber import PhoneNumber as BasePhoneNumber
     from phonenumbers.phonenumberutil import NumberParseException
 except ImportError:
     phonenumbers = None
     BasePhoneNumber = object
     NumberParseException = Exception
 
-from foundational.exceptions import ConfigurationError
+from communal.exceptions import ConfigurationError
 from sartorial import JSONSchemaFormatted, Serializable
 
 
 class PhoneNumberParseException(NumberParseException):
     """
     Catch this as either a PhoneNumberParseException or
     NumberParseException from the phonenumbers library.
```

### Comparing `atypical-0.0.0/atypical/url.py` & `atypical-0.2.0/atypical/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unicodedata
 from pathlib import Path
 from typing import ForwardRef, Union
 from urllib.parse import quote as quote_orig
 from urllib.parse import unquote as unquote_orig
 
 import furl
-from foundational.encoding import safe_decode
+from communal.encoding import safe_decode
 from sartorial import JSONSchemaFormatted, Serializable
 
 __all__ = ["URL", "NormalizedURL"]
 
 URL = ForwardRef("URL")
```

### Comparing `atypical-0.0.0/.gitignore` & `atypical-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `atypical-0.0.0/LICENSE` & `atypical-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atypical-0.0.0/pyproject.toml` & `atypical-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [bumpver]
-current_version = "0.1.0"
+current_version = "0.2.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version: {old_version} → {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = false
 
+[bumpver.file_patterns]
+"pyproject.toml" = [
+    'current_version = "{version}"',
+]
+"atypical/__init__.py" = [
+    '^__version__ = "{version}"$',
+]
+
 [project]
 name = "atypical"
 dynamic = ["version"]
 description = "Type handling and normalization for non-standard types like email, phone numbers, money, dates, etc. serializable and deserializable as JSON, JSON Schema, and Pydantic."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
@@ -34,15 +42,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "foundational",
+    "communal",
     "sartorial",
     "pydantic>2",
     "Babel",
     "pytz>=2022.1",
     "phonenumbers",
     "email-validator>=1.1.3",
     "money",
```

