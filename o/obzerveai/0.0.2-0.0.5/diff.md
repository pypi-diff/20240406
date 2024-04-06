# Comparing `tmp/obzerveai-0.0.2.tar.gz` & `tmp/obzerveai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obzerveai-0.0.2.tar", last modified: Tue Mar 19 17:47:38 2024, max compression
+gzip compressed data, was "obzerveai-0.0.5.tar", last modified: Sat Apr  6 16:07:36 2024, max compression
```

## Comparing `obzerveai-0.0.2.tar` & `obzerveai-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:38.917657 obzerveai-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:34.000000 obzerveai-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-19 17:47:38.917657 obzerveai-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-19 17:47:34.000000 obzerveai-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-19 17:47:34.000000 obzerveai-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 17:47:38.917657 obzerveai-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:38.917657 obzerveai-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:38.917657 obzerveai-0.0.2/src/obzerveai/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-19 17:47:34.000000 obzerveai-0.0.2/src/obzerveai/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:38.917657 obzerveai-0.0.2/src/obzerveai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-19 17:47:34.000000 obzerveai-0.0.2/src/obzerveai/utils/sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:38.917657 obzerveai-0.0.2/src/obzerveai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-19 17:47:38.000000 obzerveai-0.0.2/src/obzerveai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-19 17:47:38.000000 obzerveai-0.0.2/src/obzerveai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 17:47:38.000000 obzerveai-0.0.2/src/obzerveai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-19 17:47:38.000000 obzerveai-0.0.2/src/obzerveai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:47:38.917657 obzerveai-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-19 17:47:34.000000 obzerveai-0.0.2/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:07:36.194248 obzerveai-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:07:31.000000 obzerveai-0.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-06 16:07:36.194248 obzerveai-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-06 16:07:31.000000 obzerveai-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-06 16:07:31.000000 obzerveai-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 16:07:36.194248 obzerveai-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:07:36.190248 obzerveai-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:07:36.194248 obzerveai-0.0.5/src/obzerveai/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-06 16:07:31.000000 obzerveai-0.0.5/src/obzerveai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 16:07:31.000000 obzerveai-0.0.5/src/obzerveai/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-04-06 16:07:31.000000 obzerveai-0.0.5/src/obzerveai/sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:07:36.194248 obzerveai-0.0.5/src/obzerveai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-06 16:07:36.000000 obzerveai-0.0.5/src/obzerveai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-06 16:07:36.000000 obzerveai-0.0.5/src/obzerveai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:07:36.000000 obzerveai-0.0.5/src/obzerveai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 16:07:36.000000 obzerveai-0.0.5/src/obzerveai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 16:07:36.000000 obzerveai-0.0.5/src/obzerveai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:07:36.194248 obzerveai-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-06 16:07:31.000000 obzerveai-0.0.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-06 16:07:31.000000 obzerveai-0.0.5/tests/test_sanitize.py
```

### Comparing `obzerveai-0.0.2/pyproject.toml` & `obzerveai-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [project]
 name = "obzerveai"
-version = "0.0.2"
+version = "0.0.5"
 authors = [
   { name="obzerveai", email="goyal.siddharth22@gmail.com" },
 ]
 description = "A python package of utilities for AI based solutions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "influxdb_client==1.41.0",
+]
 
 [project.urls]
 Homepage = "https://github.com/obzerveai/"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 include-package-data = false
 
 [tool.setuptools.packages.find]
 where = ["src"]
-exclude = ["contrib", "docs", "tests*", "tasks"]
+exclude = ["contrib", "docs", "tests*", "tasks"]
```

### Comparing `obzerveai-0.0.2/src/obzerveai/utils/sanitize.py` & `obzerveai-0.0.5/src/obzerveai/sanitize.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,74 @@
+from influxdb_client import InfluxDBClient, Point
+from influxdb_client.client.write_api import SYNCHRONOUS
 import re
 
-def redact_sensitive_info(text):
-    # Regular expressions for sensitive information
-    regex_patterns = {
-        # 'names': r'\b[A-Z][a-z]+\b(?:\s[A-Z][a-z]+)*',
-        # 'addresses': r'\d{1,5}\s\w+\s\w+\s\w+|\d{1,5}\s\w+\s\w+',
-        'emails': r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b',
-        'phone_numbers': r'\b(?:\d{3}[-.\s]??\d{3}[-.\s]??\d{4}|\(\d{3}\)\s*\d{3}[-.\s]??\d{4}|\d{3}[-.\s]??\d{4})\b',
-        'ssn': r'\b\d{3}-\d{2}-\d{4}\b',
-        "passport": r'^[a-zA-Z]{1}\d{8}$',
-        "drivers_license": r'^[a-zA-Z]{1}\d{7}$',
-        "date": r"\d(3[01]|[12][0-9]|0?[1-9])(\/|-)(1[0-2]|0?[1-9])\2([0-9]{2})?[0-9]{2}",
-        'credit_cards': r'^\d{4}-\d{4}-\d{4}-\d{4}$',
-        'health_info': r'\b\d{3}-\d{2}-\d{4}\b',  # Sample for medical record numbers
-        # 'financial_info': r'\b(?:\d[ -]*?){13,16}\b'  # Sample for credit card or account numbers
-    }
-    
-    redacted_text = text
-    for category, pattern in regex_patterns.items():
-        # if type(pattern) == list:
-        #     for each_pattern in pattern:
-        #         print(each_pattern)
-        #         redacted_text = re.sub(each_pattern, '[REDACTED - {}]'.format(category), redacted_text)        
-        # else:
-            redacted_text = re.sub(pattern, '[REDACTED - {}]'.format(category), redacted_text)
-    
-    return redacted_text
+
+class ObzerveAI:
+    def __init__(
+        self,
+        token="my_default_token_value",
+        org="obzerve_ai",
+        bucket="usage",
+        url="http://localhost:8086",
+    ):
+        self.token = token
+        self.org = org
+        self.bucket = bucket
+        self.url = url
+        try:
+            self.client = InfluxDBClient(url=self.url, token=self.token, org=self.org)
+            self.client.ping()  # Check if InfluxDB is available
+        except Exception as e:
+            raise ConnectionError(
+                "ObzerveAI: Failed to connect to InfluxDB: {}".format(e)
+            )
+
+    def track_usage(self):
+        try:
+            write_api = self.client.write_api(write_options=SYNCHRONOUS)
+            point = (
+                Point("function_usage")
+                .tag("function", "redact_sensitive_info")
+                .field("value", 1)
+            )
+            write_api.write(bucket=self.bucket, record=point)
+        except Exception as e:
+            print("ObzerveAI: Failed to write to InfluxDB: {}".format(e))
+
+    def redact_sensitive_info(self, text):
+        # Regular expressions for sensitive information
+        regex_patterns = {
+            # 'names': r'\b[A-Z][a-z]+\b(?:\s[A-Z][a-z]+)*',
+            # 'addresses': r'\d{1,5}\s\w+\s\w+\s\w+|\d{1,5}\s\w+\s\w+',
+            "emails": r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b",
+            "phone_numbers": r"\b(?:\d{3}[-.\s]??\d{3}[-.\s]??\d{4}|\(\d{3}\)\s*\d{3}[-.\s]??\d{4}|\d{3}[-.\s]??\d{4})\b",
+            "ssn": r"\b\d{3}-\d{2}-\d{4}\b",
+            "passport": r"^[a-zA-Z]{1}\d{8}$",
+            "drivers_license": r"^[a-zA-Z]{1}\d{7}$",
+            "date": r"\d(3[01]|[12][0-9]|0?[1-9])(\/|-)(1[0-2]|0?[1-9])\2([0-9]{2})?[0-9]{2}",
+            "credit_cards": r"^\d{4}-\d{4}-\d{4}-\d{4}$",
+            "health_info": r"\b\d{3}-\d{2}-\d{4}\b",  # Sample for medical record numbers
+            # 'financial_info': r'\b(?:\d[ -]*?){13,16}\b'  # Sample for credit card or account numbers
+        }
+
+        redacted_text = text
+        for category, pattern in regex_patterns.items():
+            # if type(pattern) == list:
+            #     for each_pattern in pattern:
+            #         print(each_pattern)
+            #         redacted_text = re.sub(each_pattern, '[REDACTED - {}]'.format(category), redacted_text)
+            # else:
+            redacted_text = re.sub(
+                pattern, "[REDACTED - {}]".format(category), redacted_text
+            )
+
+        self.track_usage()
+        return redacted_text
+
 
 # Example usage:
-text_with_sensitive_info = """
-Name: John Doe
-Address: 123 Main St, City, State, 12345
-Email: johndoe@example.com
-Phone: 555-555-5555
-SSN: 123-45-6789
-PASSPORT: J8369954
-DRIVING LICENSE: RJ1420140033640
-DOB: 1995-01-01 01-01-1995 12/12/98 12/12/1998 24/12/95 24/12/1995
-Credit Card: 1234 5678 9012 3456
-Health Info: 987-65-4321
-Financial Info: 9876 5432 1098 7654
-"""
-redacted_text = redact_sensitive_info(text_with_sensitive_info)
-print(redacted_text)
+if __name__ == "__main__":
+    obzerve_ai = ObzerveAI()  # You can pass custom values if needed
+    sensitive_text = "Contact me at example@example.com or call me at 123-456-7890."
+    redacted_text = obzerve_ai.redact_sensitive_info(sensitive_text)
+    print(redacted_text)
```

### Comparing `obzerveai-0.0.2/tests/test_main.py` & `obzerveai-0.0.5/tests/test_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import re
+# import re
 
-# Regular expression pattern for matching dates
-date_pattern = re.compile(
-    r"(?:(?:31(\/|-|\.)(?:0?[13578]|1[02]))\1|(?:(?:29|30)(\/|-|\.)(?:0?[13-9]|1[0-2])\2))"
-    r"(?:(?:1[6-9]|[2-9]\d)?\d{2})$|^(?:29(\/|-|\.)0?2\3(?:(?:(?:1[6-9]|[2-9]\d)?"
-    r"(?:0[48]|[2468][048]|[13579][26])|(?:(?:16|[2468][048]|[3579][26])00))))$|^(?:0?[1-9]|1\d|2[0-8])"
-    r"(\/|-|\.)(?:(?:0?[1-9])|(?:1[0-2]))\4(?:(?:1[6-9]|[2-9]\d)?\d{2})"
-)
+# # Regular expression pattern for matching dates
+# date_pattern = re.compile(
+#     r"(?:(?:31(\/|-|\.)(?:0?[13578]|1[02]))\1|(?:(?:29|30)(\/|-|\.)(?:0?[13-9]|1[0-2])\2))"
+#     r"(?:(?:1[6-9]|[2-9]\d)?\d{2})$|^(?:29(\/|-|\.)0?2\3(?:(?:(?:1[6-9]|[2-9]\d)?"
+#     r"(?:0[48]|[2468][048]|[13579][26])|(?:(?:16|[2468][048]|[3579][26])00))))$|^(?:0?[1-9]|1\d|2[0-8])"
+#     r"(\/|-|\.)(?:(?:0?[1-9])|(?:1[0-2]))\4(?:(?:1[6-9]|[2-9]\d)?\d{2})"
+# )
 
-def redact_dates(text):
-    """Replace dates in the text with '[redacted-date]'."""
-    return date_pattern.sub('[redacted-date]', text)
+# def redact_dates(text):
+#     """Replace dates in the text with '[redacted-date]'."""
+#     return date_pattern.sub('[redacted-date]', text)
 
-# Example text with dates
-example_text = "John's birthday is on 2023-03-15 and he will have a party on 15/03/2023. " \
-               "The tickets were booked for 03-15-2023. Remember the special day 29/02/2020."
+# # Example text with dates
+# example_text = "John's birthday is on 2023-03-15 and he will have a party on 15/03/2023. " \
+#                "The tickets were booked for 03-15-2023. Remember the special day 29/02/2020."
 
-# Redact dates in the example text
-redacted_text = redact_dates(example_text)
+# # Redact dates in the example text
+# redacted_text = redact_dates(example_text)
 
-print(redacted_text)
+# print(redacted_text)
```

