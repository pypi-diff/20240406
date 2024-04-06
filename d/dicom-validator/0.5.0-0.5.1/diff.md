# Comparing `tmp/dicom-validator-0.5.0.tar.gz` & `tmp/dicom-validator-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicom-validator-0.5.0.tar", last modified: Thu Jan 25 18:57:19 2024, max compression
+gzip compressed data, was "dicom-validator-0.5.1.tar", last modified: Sat Apr  6 06:08:45 2024, max compression
```

## Comparing `dicom-validator-0.5.0.tar` & `dicom-validator-0.5.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:19.343415 dicom-validator-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-01-25 18:57:19.343415 dicom-validator-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:19.339415 dicom-validator-0.5.0/dicom_validator/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/dump_dcm_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:19.339415 dicom-validator-0.5.0/dicom_validator/spec_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    20552 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/condition_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/edition_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/enum_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/part3_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/part4_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/part6_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/spec_reader/spec_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tag_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:19.339415 dicom-validator-0.5.0/dicom_validator/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:19.343415 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    40279 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_condition_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_edition_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_enum_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_part3_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_part4_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_part6_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_spec_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/test_cmdline_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:19.343415 dicom-validator-0.5.0/dicom_validator/tests/validator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/validator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/validator/test_dicom_file_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15199 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/validator/test_iod_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/tests/validator/test_iod_validator_func_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/validate_iods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:19.343415 dicom-validator-0.5.0/dicom_validator/validator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/validator/dicom_file_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    25815 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/dicom_validator/validator/iod_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 18:57:19.343415 dicom-validator-0.5.0/dicom_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-01-25 18:57:19.000000 dicom-validator-0.5.0/dicom_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-01-25 18:57:19.000000 dicom-validator-0.5.0/dicom_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 18:57:19.000000 dicom-validator-0.5.0/dicom_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-25 18:57:19.000000 dicom-validator-0.5.0/dicom_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-25 18:57:19.000000 dicom-validator-0.5.0/dicom_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-25 18:57:19.000000 dicom-validator-0.5.0/dicom_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-01-25 18:57:08.000000 dicom-validator-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 18:57:19.343415 dicom-validator-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:45.786631 dicom-validator-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-06 06:08:45.782631 dicom-validator-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8720 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:45.774631 dicom-validator-0.5.1/dicom_validator/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/dump_dcm_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:45.778631 dicom-validator-0.5.1/dicom_validator/spec_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20552 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/condition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9541 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/edition_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/enum_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/part3_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/part4_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/part6_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/spec_reader/spec_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tag_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:45.778631 dicom-validator-0.5.1/dicom_validator/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:45.782631 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40279 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_condition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_edition_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_enum_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_part3_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_part4_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_part6_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_spec_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/test_cmdline_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:45.782631 dicom-validator-0.5.1/dicom_validator/tests/validator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/validator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/validator/test_dicom_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18439 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/validator/test_iod_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/tests/validator/test_iod_validator_func_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/validate_iods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:45.782631 dicom-validator-0.5.1/dicom_validator/validator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/validator/dicom_file_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26347 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/dicom_validator/validator/iod_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:08:45.782631 dicom-validator-0.5.1/dicom_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10228 2024-04-06 06:08:45.000000 dicom-validator-0.5.1/dicom_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-06 06:08:45.000000 dicom-validator-0.5.1/dicom_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:08:45.000000 dicom-validator-0.5.1/dicom_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 06:08:45.000000 dicom-validator-0.5.1/dicom_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 06:08:45.000000 dicom-validator-0.5.1/dicom_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-06 06:08:45.000000 dicom-validator-0.5.1/dicom_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-06 06:08:36.000000 dicom-validator-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 06:08:45.786631 dicom-validator-0.5.1/setup.cfg
```

### Comparing `dicom-validator-0.5.0/LICENSE` & `dicom-validator-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/PKG-INFO` & `dicom-validator-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicom-validator
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python DICOM validator using input from DICOM specs in docbook format
 Author-email: mrbean-bremen and contributors <hansemrbean@googlemail.com>
 License: MIT
 Project-URL: documentation, https://github.com/pydicom/dicom-validator#readme
 Project-URL: download, https://github.com/pydicom/dicom-validator/archive/main.zip
 Project-URL: homepage, https://github.com/pydicom/dicom-validator
 Project-URL: repository, https://github.com/pydicom/dicom-validator
@@ -106,15 +106,15 @@
 the first time.
 
 ## validate_iods
 
 This checks a given DICOM file, or all DICOM files recursively in a given
 directory, for correct tags for the related SOP class. The presence or
 absence of the tag and the presence of a tag value are checked, and in the
-case of an enumeration defined for the value, the value is also check for validity.
+case that an enumeration is defined for the value, the value is also checked for validity.
 More checks may be added later.
 This is done by looking up all required and optional modules for this
 SOP class, and checking the tags for these modules. Tags that are not allowed or
 missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
 to collect the needed information.
 Conditions for type 1C and 2C modules and tags are evaluated if possible.
 If the evaluation fails, the respective modules and tags are considered
```

### Comparing `dicom-validator-0.5.0/README.md` & `dicom-validator-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 the first time.
 
 ## validate_iods
 
 This checks a given DICOM file, or all DICOM files recursively in a given
 directory, for correct tags for the related SOP class. The presence or
 absence of the tag and the presence of a tag value are checked, and in the
-case of an enumeration defined for the value, the value is also check for validity.
+case that an enumeration is defined for the value, the value is also checked for validity.
 More checks may be added later.
 This is done by looking up all required and optional modules for this
 SOP class, and checking the tags for these modules. Tags that are not allowed or
 missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
 to collect the needed information.
 Conditions for type 1C and 2C modules and tags are evaluated if possible.
 If the evaluation fails, the respective modules and tags are considered
```

### Comparing `dicom-validator-0.5.0/dicom_validator/dump_dcm_info.py` & `dicom-validator-0.5.1/dicom_validator/dump_dcm_info.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/spec_reader/condition.py` & `dicom-validator-0.5.1/dicom_validator/spec_reader/condition.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/spec_reader/condition_parser.py` & `dicom-validator-0.5.1/dicom_validator/spec_reader/condition_parser.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/spec_reader/edition_reader.py` & `dicom-validator-0.5.1/dicom_validator/spec_reader/edition_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,38 +71,38 @@
                 today = datetime.datetime.today()
                 modified_date = datetime.datetime.fromtimestamp(
                     editions_path.stat().st_mtime
                 )
                 # no need to update the edition dir more than once a month
                 update = (today - modified_date).days > 30
             else:
-                with open(editions_path) as f:
+                with open(editions_path, encoding="utf8") as f:
                     update = not json.load(f)
         else:
             update = True
         if update:
             self.update_edition()
         if editions_path.exists():
-            with open(editions_path) as json_file:
+            with open(editions_path, encoding="utf8") as json_file:
                 return json.load(json_file)
 
     def read_from_html(self):
         html_path = self.path / self.html_filename
-        with open(html_path) as html_file:
+        with open(html_path, encoding="utf8") as html_file:
             contents = html_file.read()
         parser = EditionParser()
         parser.feed(contents)
         parser.close()
         return parser.editions
 
     def write_to_json(self):
         editions = self.read_from_html()
         if editions:
             json_path = self.path / self.json_filename
-            with open(json_path, "w") as json_file:
+            with open(json_path, "w", encoding="utf8") as json_file:
                 json_file.write(json.dumps(editions))
 
     def get_edition(self, revision):
         """Get the edition matching the revision or None.
         The revision can be the edition name, the year of the edition,
         'current', or 'local'.
         """
@@ -159,15 +159,15 @@
                     self.logger.warning(
                         f"Failed to remove incomplete file {file_path}."
                     )
             return False
 
     @staticmethod
     def load_info(json_path, info_json):
-        with open(json_path / info_json) as info_file:
+        with open(json_path / info_json, encoding="utf8") as info_file:
             return json.load(info_file)
 
     @classmethod
     def load_dicom_info(cls, json_path):
         return DicomInfo(
             cls.load_info(json_path, cls.dict_info_json),
             cls.load_info(json_path, cls.iod_info_json),
@@ -200,21 +200,21 @@
         iod_info = part3reader.iod_descriptions()
         chapter_info = part4reader.iod_chapters()
         definition = {}
         for chapter in iod_info:
             if chapter in chapter_info:
                 for uid in chapter_info[chapter]:
                     definition[uid] = iod_info[chapter]
-        with open(json_path / cls.iod_info_json, "w") as info_file:
+        with open(json_path / cls.iod_info_json, "w", encoding="utf8") as info_file:
             info_file.write(cls.dump_description(definition))
-        with open(json_path / cls.module_info_json, "w") as info_file:
+        with open(json_path / cls.module_info_json, "w", encoding="utf8") as info_file:
             info_file.write(cls.dump_description(part3reader.module_descriptions()))
-        with open(json_path / cls.dict_info_json, "w") as info_file:
+        with open(json_path / cls.dict_info_json, "w", encoding="utf8") as info_file:
             info_file.write(cls.dump_description(dict_info))
-        with open(json_path / cls.uid_info_json, "w") as info_file:
+        with open(json_path / cls.uid_info_json, "w", encoding="utf8") as info_file:
             info_file.write(cls.dump_description(part6reader.all_uids()))
         cls.write_current_version(json_path)
         print("Done!")
 
     def get_revision(self, revision, recreate_json=False, create_json=True):
         revision, destination = self.check_revision(revision)
         if destination is None:
@@ -246,15 +246,15 @@
         return destination
 
     @staticmethod
     def is_current_version(json_path):
         version_path = json_path / "version"
         if not version_path.exists():
             return False
-        with open(version_path) as f:
+        with open(version_path, encoding="utf8") as f:
             return f.read() >= __version__
 
     @staticmethod
     def write_current_version(json_path):
         version_path = json_path / "version"
-        with open(version_path, "w") as f:
+        with open(version_path, "w", encoding="utf8") as f:
             f.write(__version__)
```

### Comparing `dicom-validator-0.5.0/dicom_validator/spec_reader/part3_reader.py` & `dicom-validator-0.5.1/dicom_validator/spec_reader/part3_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Chapter3Reader collects DICOM Information Object Definition information
 for specific Storage SOP Classes.
 The information is taken from PS3.3 in docbook format as provided by ACR NEMA.
 """
+
 import logging
 from itertools import groupby
 
 import sys
 
 from dicom_validator.spec_reader.condition import ConditionType, ConditionOperator
 from dicom_validator.spec_reader.condition_parser import ConditionParser
@@ -296,14 +297,16 @@
             except KeyError:
                 # silently ignore error in older specs
                 pass
         elif level < current_level:
             # Pop off (delete) the last level_delta items.
             level_delta = current_level - level
             del current_descriptions[-level_delta:]
+            if not current_descriptions:
+                current_descriptions.append({})
         return tag_name, level
 
     def _collect_modules(self, table_section, check_rowspan):
         modules = {}
         module_rows = self._findall(table_section, ["table", "tbody", "tr"])
         row_span = 0
         for row in module_rows:
```

### Comparing `dicom-validator-0.5.0/dicom_validator/spec_reader/part4_reader.py` & `dicom-validator-0.5.1/dicom_validator/spec_reader/part4_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Chapter4Reader collects SOP Class Information information for specific
 Storage SOP Classes.
 The information is taken from PS3.4 in docbook format as provided by ACR NEMA.
 """
+
 from dicom_validator.spec_reader.spec_reader import (
     SpecReader,
     SpecReaderLookupError,
     SpecReaderParseError,
 )
```

### Comparing `dicom-validator-0.5.0/dicom_validator/spec_reader/part6_reader.py` & `dicom-validator-0.5.1/dicom_validator/spec_reader/part6_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Chapter6Reader collects DICOM Data Element information.
 The information is taken from DICOM dictionary (PS3.6) in docbook format
 as provided by ACR NEMA.
 """
+
 from dicom_validator.spec_reader.spec_reader import SpecReader, SpecReaderParseError
 
 
 class Part6Reader(SpecReader):
     """Reads information from PS3.4 in docbook format."""
 
     def __init__(self, spec_dir):
@@ -115,11 +116,11 @@
                     ]
                     if uid_attributes is not None:
                         uid_type = uid_attributes[nr_columns - 2]
                         # in PS3.6 xml there are multiple zero width (U+200B)
                         # spaces inside the UIDs
                         # we remove them hoping this is the only such problem
                         uid_value = self.cleaned_value(uid_attributes[0])
-                        self._uids.setdefault(uid_type, {})[
-                            uid_value
-                        ] = self.cleaned_value(uid_attributes[1])
+                        self._uids.setdefault(uid_type, {})[uid_value] = (
+                            self.cleaned_value(uid_attributes[1])
+                        )
         return self._uids
```

### Comparing `dicom-validator-0.5.0/dicom_validator/spec_reader/spec_reader.py` & `dicom-validator-0.5.1/dicom_validator/spec_reader/spec_reader.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/spec_reader/conftest.py` & `dicom-validator-0.5.1/dicom_validator/tests/spec_reader/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,31 +20,48 @@
 
 @pytest.fixture(scope="session")
 def standard_path(fixture_path):
     yield fixture_path / "standard"
 
 
 @pytest.fixture(scope="session")
-def spec_fixture_path(standard_path):
-    yield standard_path / CURRENT_REVISION / "docbook"
+def revision(request):
+    if hasattr(request, "param"):
+        revision = request.param
+    else:
+        revision = CURRENT_REVISION
+    yield revision
 
 
 @pytest.fixture(scope="session")
-def dict_info(standard_path):
+def revision_path(standard_path, revision):
+    yield standard_path / revision
+
+
+@pytest.fixture(scope="session")
+def spec_fixture_path(revision_path):
+    yield revision_path / "docbook"
+
+
+@pytest.fixture(scope="session")
+def dict_info(revision_path):
     from dicom_validator.spec_reader.edition_reader import EditionReader
 
-    json_fixture_path = standard_path / CURRENT_REVISION / "json"
-    with open(json_fixture_path / EditionReader.dict_info_json) as info_file:
+    json_fixture_path = revision_path / "json"
+    with open(
+        json_fixture_path / EditionReader.dict_info_json, encoding="utf8"
+    ) as info_file:
         info = json.load(info_file)
     yield info
 
 
 @pytest.fixture(scope="module")
 def spec_path(fs_module, spec_fixture_path):
-    fs_module.add_real_directory(spec_fixture_path)
+    if not fs_module.exists(spec_fixture_path):
+        fs_module.add_real_directory(spec_fixture_path)
     yield spec_fixture_path
 
 
 @pytest.fixture
 def dict_reader(spec_path):
     from dicom_validator.spec_reader.part6_reader import Part6Reader
```

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_condition.py` & `dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_condition.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_condition_parser.py` & `dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_condition_parser.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_edition_reader.py` & `dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_edition_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
 
     def __init__(self, path, contents=""):
         super(MemoryEditionReader, self).__init__(path=path)
         self.html_contents = contents
 
     def retrieve(self, html_path):
-        with open(html_path, "w") as html_file:
+        with open(html_path, "w", encoding="utf8") as html_file:
             html_file.write(self.html_contents)
 
 
 @pytest.fixture
 def base_path(fs):
     path = Path("user", "dicom-validator")
     path.mkdir(parents=True)
```

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_enum_parser.py` & `dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_enum_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,63 +61,63 @@
     def test_single_enum(self, parser):
         content = """<variablelist>
         <title>Enumerated Values:</title>
         <varlistentry>
         <term>NO</term>
         </varlistentry>
         </variablelist>"""
-        assert parser.parse(section(content), VR.SH) == ["NO"]
+        assert parser.parse(section(content), VR.SH) == [{"val": ["NO"]}]
 
     def test_single_enum_with_extra_tag(self, parser):
         content = """<variablelist>
         <title>Enumerated Values:</title>
         <varlistentry>
         <listitem>
         <para xml:id="para_f6578fe2-d628-412e-8314-af2c8961b633"/>
         </listitem>
         <term>NO</term>
         </varlistentry>
         </variablelist>"""
-        assert parser.parse(section(content), VR.SH) == ["NO"]
+        assert parser.parse(section(content), VR.SH) == [{"val": ["NO"]}]
 
     def test_two_enums(self, parser):
         content = """<variablelist>
         <title>Enumerated Values:</title>
         <varlistentry>
         <term>YES</term>
         </varlistentry>
         <varlistentry>
         <term>NO</term>
         </varlistentry>
         </variablelist>"""
-        assert parser.parse(section(content), VR.SH) == ["YES", "NO"]
+        assert parser.parse(section(content), VR.SH) == [{"val": ["YES", "NO"]}]
 
     def test_int_enums(self, parser):
         content = """<variablelist>
         <title>Enumerated Values:</title>
         <varlistentry>
         <term>0000</term>
         </varlistentry>
         <varlistentry>
         <term>0001</term>
         </varlistentry>
         </variablelist>"""
-        assert parser.parse(section(content), VR.US) == [0, 1]
+        assert parser.parse(section(content), VR.US) == [{"val": [0, 1]}]
 
     def test_hex_enums(self, parser):
         content = """<variablelist>
         <title>Enumerated Values:</title>
         <varlistentry>
         <term>0010H</term>
         </varlistentry>
         <varlistentry>
         <term>0011H</term>
         </varlistentry>
         </variablelist>"""
-        assert parser.parse(section(content), VR.US) == [16, 17]
+        assert parser.parse(section(content), VR.US) == [{"val": [16, 17]}]
 
     def test_linked_enum(self):
         content = """<para>Bla blah, see
         <xref linkend="sect_10.7.1.2" xrefstyle="select: label"/>.</para>"
         """
         linked = """
         <title>Pixel Spacing Calibration Type</title>
@@ -135,8 +135,36 @@
                 <listitem>
                     <para xml:id="para_10de0799">Another...</para>
                 </listitem>
             </varlistentry>
         </variablelist>
         """
         parser = EnumParser(lambda s: section(linked, s))
-        assert parser.parse(section(content), VR.SH) == ["GEOMETRY", "FIDUCIAL"]
+        assert parser.parse(section(content), VR.SH) == [
+            {"val": ["GEOMETRY", "FIDUCIAL"]}
+        ]
+
+    def test_value_for_value(self, parser):
+        content = """
+        <variablelist spacing="compact">
+            <title>Enumerated Values for Value 1:</title>
+            <varlistentry>
+                <term>DERIVED</term>
+                <listitem>
+                    <para xml:id="para_34ae991b-705a-4ffc-992e-6f97e657d0d0"/>
+                </listitem>
+            </varlistentry>
+        </variablelist>
+        <variablelist spacing="compact">
+            <title>Enumerated Values for Value 2:</title>
+            <varlistentry>
+                <term>PRIMARY</term>
+                <listitem>
+                    <para xml:id="para_c6dbc4cc-fdd6-499f-ab90-9dc7f4ee13a9"/>
+                </listitem>
+            </varlistentry>
+        </variablelist>
+        """
+        assert parser.parse(section(content), VR.CS) == [
+            {"index": 1, "val": ["DERIVED"]},
+            {"index": 2, "val": ["PRIMARY"]},
+        ]
```

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_part4_reader.py` & `dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_part4_reader.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_part6_reader.py` & `dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_part6_reader.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/spec_reader/test_spec_reader.py` & `dicom-validator-0.5.1/dicom_validator/tests/spec_reader/test_spec_reader.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/test_cmdline_tools.py` & `dicom-validator-0.5.1/dicom_validator/tests/test_cmdline_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import logging
 from pathlib import Path
 
 import pytest
 
-from dicom_validator.spec_reader.enum_parser import EnumParser
 from dicom_validator.validate_iods import main
 
-CURRENT_REVISION = "2023c"
-
 
 @pytest.fixture(scope="session")
 def fixture_path():
     yield Path(__file__).parent / "fixtures"
 
 
 @pytest.fixture(scope="session")
@@ -20,27 +17,28 @@
 
 
 @pytest.fixture
 def dicom_fixture_path(fixture_path):
     yield fixture_path / "dicom"
 
 
-def test_validate_sr(caplog, standard_path, dicom_fixture_path):
+@pytest.mark.order(0)
+@pytest.mark.parametrize("revision", ["2015b", "2023c"])
+def test_validate_sr(revision, caplog, standard_path, dicom_fixture_path):
+    # test also for 2015b to test an issue causing an exception
     rtdose_path = dicom_fixture_path / "rtdose.dcm"
     # recreate json files to avoid getting the cached ones
     # relies on the fact that this test is run first
     cmd_line_args = [
         "-src",
         str(standard_path),
         "-r",
-        CURRENT_REVISION,
+        revision,
         "--recreate-json",
         str(rtdose_path),
     ]
     with caplog.at_level(logging.INFO):
         main(cmd_line_args)
 
     # regression test for #9
     assert "Unknown SOPClassUID" not in caplog.text
     assert "Tag (0008,1070) (Operators' Name) is missing" in caplog.text
-
-    print(f"Direct: {EnumParser.nr_direct_enums}, linked: {EnumParser.nr_linked_enums}")
```

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/utils.py` & `dicom-validator-0.5.1/dicom_validator/tests/utils.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/validator/conftest.py` & `dicom-validator-0.5.1/dicom_validator/tests/validator/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,29 +31,35 @@
 @pytest.fixture(scope="session")
 def json_fixture_path(standard_path):
     yield standard_path / CURRENT_REVISION / "json"
 
 
 @pytest.fixture(scope="session")
 def iod_info(json_fixture_path):
-    with open(json_fixture_path / EditionReader.iod_info_json) as info_file:
+    with open(
+        json_fixture_path / EditionReader.iod_info_json, encoding="utf8"
+    ) as info_file:
         info = json.load(info_file)
     yield info
 
 
 @pytest.fixture(scope="session")
 def dict_info(json_fixture_path):
-    with open(json_fixture_path / EditionReader.dict_info_json) as info_file:
+    with open(
+        json_fixture_path / EditionReader.dict_info_json, encoding="utf8"
+    ) as info_file:
         info = json.load(info_file)
     yield info
 
 
 @pytest.fixture(scope="session")
 def module_info(json_fixture_path):
-    with open(json_fixture_path / EditionReader.module_info_json) as info_file:
+    with open(
+        json_fixture_path / EditionReader.module_info_json, encoding="utf8"
+    ) as info_file:
         info = json.load(info_file)
     yield info
 
 
 @pytest.fixture(scope="session")
 def dicom_info(dict_info, module_info, iod_info):
     yield DicomInfo(dict_info, iod_info, module_info)
```

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/validator/test_dicom_file_validator.py` & `dicom-validator-0.5.1/dicom_validator/tests/validator/test_dicom_file_validator.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/validator/test_iod_validator.py` & `dicom-validator-0.5.1/dicom_validator/tests/validator/test_iod_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -425,17 +425,16 @@
             "PatientID": "ZZZ",
             "ImageType": "DERIVED",
             "PresentationLUTShape": "INVALID",
             "ContentQualification": "PRODUCT",
             "BitsStored": 1,
         }
     )
-    def test_enum_value(self, validator):
+    def test_invalid_enum_value(self, validator):
         result = validator.validate()
-        print(result)
 
         # Presentation LUT Shape: incorrect enum value
         assert has_tag_error(
             result,
             "Enhanced XA/XRF Image",
             "(2050,0020)",
             "value is not allowed",
@@ -451,7 +450,110 @@
         assert has_tag_error(
             result,
             "Enhanced XA/XRF Image",
             "(0028,0101)",
             "value is not allowed",
             "(value: 1, allowed: 8, 9, 10, 11, 12, 13, 14, 15, 16)",
         )
+
+    @pytest.mark.tag_set(
+        {
+            # MR Image Storage
+            "SOPClassUID": "1.2.840.10008.5.1.4.1.1.4",
+            "PatientName": "XXX",
+            "PatientID": "ZZZ",
+            "ScanningSequence": ["SE", "EP"],
+        }
+    )
+    def test_valid_multi_valued_enum(self, validator):
+        result = validator.validate()
+
+        # Scanning Sequence - all values allowed
+        assert not has_tag_error(
+            result,
+            "MR Image",
+            "(0018,0020)",
+            "value is not allowed",
+        )
+
+    @pytest.mark.tag_set(
+        {
+            # MR Image Storage
+            "SOPClassUID": "1.2.840.10008.5.1.4.1.1.4",
+            "PatientName": "XXX",
+            "PatientID": "ZZZ",
+            "ScanningSequence": ["SE", "EP", "IV"],
+        }
+    )
+    def test_invalid_multi_valued_enum(self, validator):
+        result = validator.validate()
+
+        # Scanning Sequence - IV not allowed
+        assert has_tag_error(
+            result,
+            "MR Image",
+            "(0018,0020)",
+            "value is not allowed",
+            "(value: IV, allowed: SE, IR, GR, EP, RM)",
+        )
+
+    @pytest.mark.tag_set(
+        {
+            # Ophthalmic Optical Coherence Tomography B-scan Volume Analysis Storage
+            "SOPClassUID": "1.2.840.10008.5.1.4.1.1.77.1.5.8",
+            "PatientName": "XXX",
+            "PatientID": "ZZZ",
+            "ImageType": ["ORIGINAL", "PRIMARY"],
+        }
+    )
+    def test_valid_indexed_enum(self, validator):
+        result = validator.validate()
+
+        # Image Type - both values correct
+        assert not has_tag_error(
+            result,
+            "Ophthalmic Optical Coherence Tomography B-scan Volume Analysis Image",
+            "(0008,0008)",
+            "value is not allowed",
+        )
+
+    @pytest.mark.tag_set(
+        {
+            # Ophthalmic Optical Coherence Tomography B-scan Volume Analysis Storage
+            "SOPClassUID": "1.2.840.10008.5.1.4.1.1.77.1.5.8",
+            "PatientName": "XXX",
+            "PatientID": "ZZZ",
+            "ImageType": ["ORIGINAL", "SECONDARY"],
+        }
+    )
+    def test_invalid_indexed_enum(self, validator):
+        result = validator.validate()
+
+        # Image Type - second value incorrect
+        assert has_tag_error(
+            result,
+            "Ophthalmic Optical Coherence Tomography B-scan Volume Analysis Image",
+            "(0008,0008)",
+            "value is not allowed",
+            "(value: SECONDARY, allowed: PRIMARY)",
+        )
+
+    @pytest.mark.tag_set(
+        {
+            # Ophthalmic Optical Coherence Tomography B-scan Volume Analysis Storage
+            "SOPClassUID": "1.2.840.10008.5.1.4.1.1.77.1.5.8",
+            "PatientName": "XXX",
+            "PatientID": "ZZZ",
+            "ImageType": ["PRIMARY", "ORIGINAL"],
+        }
+    )
+    def test_indexed_enum_incorrect_index(self, validator):
+        result = validator.validate()
+
+        # Image Type - allowed values at incorrect index
+        assert has_tag_error(
+            result,
+            "Ophthalmic Optical Coherence Tomography B-scan Volume Analysis Image",
+            "(0008,0008)",
+            "value is not allowed",
+            "(value: ORIGINAL, allowed: PRIMARY)",
+        )
```

### Comparing `dicom-validator-0.5.0/dicom_validator/tests/validator/test_iod_validator_func_groups.py` & `dicom-validator-0.5.1/dicom_validator/tests/validator/test_iod_validator_func_groups.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/validate_iods.py` & `dicom-validator-0.5.1/dicom_validator/validate_iods.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/validator/dicom_file_validator.py` & `dicom-validator-0.5.1/dicom_validator/validator/dicom_file_validator.py`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/dicom_validator/validator/iod_validator.py` & `dicom-validator-0.5.1/dicom_validator/validator/iod_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import sys
 from dataclasses import dataclass
 
 from pydicom import Sequence
+from pydicom.multival import MultiValue
 from pydicom.tag import Tag
 
 from dicom_validator.spec_reader.condition import (
     Condition,
     ConditionType,
     ConditionOperator,
 )
@@ -387,20 +388,28 @@
             error_kind = "not allowed"
         elif has_tag and (value_required or "enums" in attribute):
             value = self._dataset_stack[-1].dataset[tag_id].value
             if value_required:
                 if value is None or isinstance(value, Sequence) and not value:
                     error_kind = "empty"
             if value is not None and "enums" in attribute:
-                if value not in attribute["enums"]:
-                    error_kind = "value is not allowed"
-                    extra_msg = (
-                        f" (value: {value}, allowed: "
-                        f"{', '.join([str(e) for e in attribute['enums']])})"
-                    )
+                if not isinstance(value, MultiValue):
+                    value = [value]
+                for i, v in enumerate(value):
+                    for enums in attribute["enums"]:
+                        # if an index is there, we only check the value for the
+                        # correct index; otherwise there will only be one entry
+                        if "index" in enums and int(enums["index"]) != i + 1:
+                            continue
+                        if v not in enums["val"]:
+                            error_kind = "value is not allowed"
+                            extra_msg = (
+                                f" (value: {v}, allowed: "
+                                f"{', '.join([str(e) for e in enums['val']])})"
+                            )
 
         if error_kind is not None:
             extra_msg = extra_msg or self._condition_message(condition_dict)
             return self._incorrect_tag_message(tag_id, error_kind, extra_msg)
 
     def _object_is_required_or_allowed(self, condition):
         """Checks if an attribute is required or allowed in the current dataset,
```

### Comparing `dicom-validator-0.5.0/dicom_validator.egg-info/PKG-INFO` & `dicom-validator-0.5.1/dicom_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicom-validator
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python DICOM validator using input from DICOM specs in docbook format
 Author-email: mrbean-bremen and contributors <hansemrbean@googlemail.com>
 License: MIT
 Project-URL: documentation, https://github.com/pydicom/dicom-validator#readme
 Project-URL: download, https://github.com/pydicom/dicom-validator/archive/main.zip
 Project-URL: homepage, https://github.com/pydicom/dicom-validator
 Project-URL: repository, https://github.com/pydicom/dicom-validator
@@ -106,15 +106,15 @@
 the first time.
 
 ## validate_iods
 
 This checks a given DICOM file, or all DICOM files recursively in a given
 directory, for correct tags for the related SOP class. The presence or
 absence of the tag and the presence of a tag value are checked, and in the
-case of an enumeration defined for the value, the value is also check for validity.
+case that an enumeration is defined for the value, the value is also checked for validity.
 More checks may be added later.
 This is done by looking up all required and optional modules for this
 SOP class, and checking the tags for these modules. Tags that are not allowed or
 missing in a module are listed. Parts 3 and 4 of the DICOM standard are used
 to collect the needed information.
 Conditions for type 1C and 2C modules and tags are evaluated if possible.
 If the evaluation fails, the respective modules and tags are considered
```

### Comparing `dicom-validator-0.5.0/dicom_validator.egg-info/SOURCES.txt` & `dicom-validator-0.5.1/dicom_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicom-validator-0.5.0/pyproject.toml` & `dicom-validator-0.5.1/pyproject.toml`

 * *Files identical despite different names*

