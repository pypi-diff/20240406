# Comparing `tmp/datewise-0.1.5.tar.gz` & `tmp/datewise-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datewise-0.1.5.tar", last modified: Sat Mar 30 17:31:23 2024, max compression
+gzip compressed data, was "datewise-0.1.6.tar", last modified: Sat Apr  6 12:11:49 2024, max compression
```

## Comparing `datewise-0.1.5.tar` & `datewise-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:31:23.034176 datewise-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-30 17:31:23.034176 datewise-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-30 17:31:06.000000 datewise-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:31:23.030176 datewise-0.1.5/datewise/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-30 17:31:06.000000 datewise-0.1.5/datewise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19384 2024-03-30 17:31:06.000000 datewise-0.1.5/datewise/datewise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:31:23.034176 datewise-0.1.5/datewise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-30 17:31:23.000000 datewise-0.1.5/datewise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-30 17:31:23.000000 datewise-0.1.5/datewise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 17:31:23.000000 datewise-0.1.5/datewise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-30 17:31:23.000000 datewise-0.1.5/datewise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-30 17:31:23.000000 datewise-0.1.5/datewise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 17:31:23.034176 datewise-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-03-30 17:31:06.000000 datewise-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 17:31:23.034176 datewise-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    27053 2024-03-30 17:31:06.000000 datewise-0.1.5/tests/test_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:11:49.083352 datewise-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-06 12:11:49.083352 datewise-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 12:11:22.000000 datewise-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:11:49.079352 datewise-0.1.6/datewise/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-06 12:11:22.000000 datewise-0.1.6/datewise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19464 2024-04-06 12:11:22.000000 datewise-0.1.6/datewise/datewise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:11:49.079352 datewise-0.1.6/datewise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 12:11:49.000000 datewise-0.1.6/datewise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 12:11:49.083352 datewise-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-06 12:11:22.000000 datewise-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:11:49.079352 datewise-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    27284 2024-04-06 12:11:22.000000 datewise-0.1.6/tests/test_functionality.py
```

### Comparing `datewise-0.1.5/PKG-INFO` & `datewise-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: datewise
-Version: 0.1.5
+Version: 0.1.6
 Summary: Thesis Library
 Home-page: https://datewise.readthedocs.io/
 Author: Sebastian Gontkovic
 Author-email: sebascngont@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
```

### Comparing `datewise-0.1.5/datewise/datewise.py` & `datewise-0.1.6/datewise/datewise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from datetime import datetime, timedelta
 from typing import Union
 import pandas as pd
 
-
 def identify_date_format(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp]) -> str:
 
     """
     Identify date format of input date based on pre-determined widely used formats.
 
     :param date: The date given by a user to identify it's format 
     :type date: str, datetime, pd._libs.tslibs.timestamps.Timestamp
 
     :return: Date format, if available, else message about error
     :rtype: str
     """
 
-
     formats = [
         "%m/%d/%Y", "%m-%d-%Y",
         "%d/%m/%Y", "%d-%m-%Y",
         "%Y/%m/%d", "%Y-%m-%d",
         "%Y/%m/%d", "%Y-%m-%d",
         "%d/%m/%Y", "%d-%m-%Y",
         "%Y %m %d", "%Y-%m-%d",
@@ -52,33 +50,30 @@
         "%y-%m-%d %H:%M", "%y/%m/%d %H:%M",
         "%y-%m-%d %H", "%y/%m/%d %H",
         "%y-%m-%d %I:%M:%S %p", "%y/%m/%d %I:%M:%S %p",
         "%y-%m-%d %I:%M %p", "%y/%m/%d %I:%M %p",
         "%y-%m-%d %I %p", "%y/%m/%d %I %p",
     ]
 
-
-
-
     if isinstance(date, str):
         for fmt in formats:
             try:
                 datetime.strptime(date, fmt)
                 return fmt
             except ValueError:
                 pass
         return False
     elif isinstance(date, pd._libs.tslibs.timestamps.Timestamp):
         return "Pandas Timestamp type, no specific format"
     elif isinstance(date, datetime):
         return "Datetime type, no specific format"
     else:
-        return "Unknow data type of date variable"
-
+        raise ValueError("Unknow data type of date variable")
 
+ 
 def date_comparison(date_1= Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], date_2= Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], operation=str) -> bool:
 
     """
     Compare two dates given by a surer based on chosen comparison operator
 
     :param date1: Date no. 1 given by a user to be compared
     :type date1: str, datetime, pd._libs.tslibs.timestamps.Timestamp
@@ -90,15 +85,15 @@
     :type operation: str 
     
     :return: True or False value based on a result
     :rtype: bool
 
     """
 
-
+    
     if date_1 and date_2 and operation:
 
         if isinstance(date_1, str) and isinstance(date_2, str): 
 
             date1_comparison = datetime.strptime(date_1, identify_date_format(date=date_1)) 
             date2_comparison = datetime.strptime(date_2, identify_date_format(date=date_2)) 
 
@@ -134,30 +129,34 @@
             elif date_2_type != str:
 
                 date_2 = date_convert(date_2, 'str', '%Y-%m-%d')
 
             return date_comparison(date_1, date_2, operation)        
         else:
             
-            return "Provided inputs are uncomperable"  
+            raise ValueError("Provided inputs are uncomperable"  )
+    
+    else: 
 
+        raise ValueError('Missing variable')
 
-def week_start(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp]) -> str:
 
+def week_start(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp]) -> str:
+ 
     """
     Find the start of the specific week based on a given date
 
     :param date: The date given by a user to identify start of the week that the date is in 
     :type date: str, datetime, pd._libs.tslibs.timestamps.Timestamp
 
     :return: Date representing start of the week
     :rtype: str
     """
 
-
+    
     if isinstance(date, str):
 
         fmt = identify_date_format(date)
 
         if fmt:
 
             weekday = datetime.strptime(date, fmt).weekday()
@@ -169,17 +168,17 @@
     elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime)):
 
         converted_date = date_convert(date, 'str', '%Y-%m-%d')
 
         return week_start(converted_date)
     
     else:
-        return "Unknow data type of date variable"
+        raise ValueError("Unknow data type of date variable")
+    
     
-
 def week_end(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], weekend:bool) -> str:
 
     """
     Find the end of the specific week based on a given date for either week as a whole or business week
 
     :param date: The date given by a user to identify end of the week that the date is in 
     :type date: str, datetime, pd._libs.tslibs.timestamps.Timestamp
@@ -224,25 +223,25 @@
 
                 else:
 
                     return('Today is the end of the full week.')
                 
         else:
 
-            return ("Couldn't process such date format.")
+            raise ValueError("Couldn't process such date format.")
     
     elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime)):
 
         converted_date = date_convert(date, 'str', '%Y-%m-%d')
 
         return week_end(converted_date, weekend)
     
     else:
 
-        return "Unknow data type of date variable"
+        raise ValueError("Unknow data type of date variable")
 
 
 def date_operations(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], operation:str, frequency:str, range:int, weekend:bool) -> str:
 
     """
     Adding or subtracting date for chosen frequency in specific range for either standard or business week
 
@@ -262,86 +261,79 @@
     :type weekend: bool
 
     :return: New day after subtraction or addition
     :rtype: str
     """
 
 
-    if date and operation and range:
+    if date and operation and frequency and range:
 
         if isinstance(date, str):
 
             fmt = identify_date_format(date)
 
             weekday = datetime.strptime(date, fmt).weekday()
 
             date = datetime.strptime(date, fmt)
 
             if frequency == 'day':
 
-                if weekend == True:
+                if weekend == False:
 
                     if operation == '+' : 
 
-                        weekday = date.weekday()
-
                         while range: 
 
                             if range and weekday <= 3 or weekday >= 6:
 
                                 date += timedelta(days=1)
                                 weekday = date.weekday()
-                                range -= 1
-                            
+                                range -= 1                            
                             else:
                                 
                                 date += timedelta(days=1)
                                 weekday = date.weekday()
 
-                        return(f'Added date with weekend: {date.strftime(fmt)}')
+                        return(f'Added date without weekend: {date.strftime(fmt)}')
                         
                     elif operation == '-':
 
-                        weekday = date.weekday()
-
                         while range: 
 
                             if range and weekday <= 5 and weekday >= 1:
 
                                 date -= timedelta(days=1)
                                 weekday = date.weekday()
-                                range -= 1
-                            
+                                range -= 1                            
                             else:
                                 
                                 date -= timedelta(days=1)
                                 weekday = date.weekday()
 
+                        return(f'Subtracted date without weekend: {date.strftime(fmt)}')
 
-                        return(f'Subtracted date with weekend: {date.strftime(fmt)}')
-
-                elif weekend == False:
+                elif weekend == True:
 
                     if operation == '+' : 
 
                         while range: 
 
                             date += timedelta(days=1)
                             range -= 1
 
-                        return(f'Added date without weekend: {date.strftime(fmt)}')
+                        return(f'Added date with weekend: {date.strftime(fmt)}')
                         
                     elif operation == '-':
 
                         while range:
 
                             date -= timedelta(days=1)
                             range -= 1
                             
-                        return(f'Subtracted date without weekend: {date.strftime(fmt)}')
+                        return(f'Subtracted date with weekend: {date.strftime(fmt)}')
             
             elif frequency == 'month':
 
                 year = int(date.year)
                 month = int(date.month)
                 day = int(date.day)
 
@@ -363,15 +355,14 @@
                     month -= range
 
                     while month <= 0:
 
                         month += 12
                         year -= 1
                         
-
                     date = datetime(year=year, month=month, day=day)
 
                     return(f'Subtracted date: {date.strftime(fmt)}')
                 
             elif frequency == 'year':
 
                 year = int(date.year)
@@ -397,18 +388,19 @@
         elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime)):
 
             converted_date = date_convert(date, 'str', '%Y-%m-%d')
 
             return date_operations(converted_date, operation, frequency, range, weekend)
         
         else:
+            raise ValueError("Unknow data type of date variable")   
+    else: 
+        raise ValueError('Missing mandatory variable.')               
 
-            return "Unknow data type of date variable"                  
 
-                
 def range_calculation(start: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], end: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], weekend:bool, frequency:str) -> list:
 
     """
     Calculate range between two dates for standard or business week in different frquencies
     
     :param start: start of the period
     :type start: str, datetime, pd._libs.tslibs.timestamps.Timestamp
@@ -423,15 +415,15 @@
     :type frequency: str
 
     :return: Range of days/months/year between two given dates
     :rtype: list
     """
 
 
-    if start and end and frequency: 
+    if start and end and frequency and range: 
 
         if isinstance(start, str) and isinstance(end, str): 
 
             if date_comparison(end, start, '>'):
                 max_date = end
                 min_date = start
             else:
@@ -540,20 +532,18 @@
 
                 end = date_convert(end, 'str', '%Y-%m-%d')
 
             return range_calculation(start, end, weekend, frequency)
         
         else:
             
-            return "Unknow data type of date variable"  
+            raise ValueError( "Unknow data type of date variable")  
     else:
 
-        return 'Missing mandatory variable.'
-
-    return f'Days between two dates are: {days_between}'
+        raise ValueError('Missing mandatory variable')
 
 
 def date_convert(date: Union[str, datetime, pd._libs.tslibs.timestamps.Timestamp], desired_type:str, format:str):
 
     """
     Date conversion based on specified format according do tright party library options
 
@@ -593,8 +583,8 @@
     if date_type == desired_type:
         return 'Your date is in desired format'
     
     elif isinstance(date, (pd._libs.tslibs.timestamps.Timestamp, datetime, str)):
         return conversions[desired_result]
     
     else:
-        return "Unknow data type of date variable"  
+        raise ValueError("Unknow data type of date variable")
```

### Comparing `datewise-0.1.5/datewise.egg-info/PKG-INFO` & `datewise-0.1.6/datewise.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: datewise
-Version: 0.1.5
+Version: 0.1.6
 Summary: Thesis Library
 Home-page: https://datewise.readthedocs.io/
 Author: Sebastian Gontkovic
 Author-email: sebascngont@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
```

### Comparing `datewise-0.1.5/setup.py` & `datewise-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,33 @@
-
-# Always prefer setuptools over distutils
 from setuptools import setup, find_packages
-
-# To use a consistent encoding
 from codecs import open
 from os import path
 
 # The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="datewise",
-    version="0.1.5",
+    version="0.1.6",
     description="Thesis Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://datewise.readthedocs.io/",
     author="Sebastian Gontkovic",
     author_email="sebascngont@gmail.com",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent"
     ],
     packages=["datewise"],
```

### Comparing `datewise-0.1.5/tests/test_functionality.py` & `datewise-0.1.6/tests/test_functionality.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,18 @@
     assert identify_date_format(today) == "Pandas Timestamp type, no specific format"
 
 
 def test3_identify_date_format_unknown_data_type():
 
     today = 123
 
-    assert identify_date_format(today) == "Unknow data type of date variable"
+    with pytest.raises(ValueError) as exc_info:
+        identify_date_format(today)
+
+    assert str(exc_info.value) == "Unknow data type of date variable"
 
 
 def test4_identify_date_format_unknown_date_format():
 
     today = '2024-03-1813:00:00'
 
     assert identify_date_format(today) == False
@@ -122,15 +125,18 @@
     assert week_start(date) == '2024-03-18'
 
 
 def test4_week_start_unknown_date_type():
 
     date = 123
 
-    assert week_start(date) == "Unknow data type of date variable"
+    with pytest.raises(ValueError) as exc_info:
+        week_start(date)
+
+    assert str(exc_info.value) == "Unknow data type of date variable"
 
 
 # week_end
     
 def test1_week_end_date_as_string_weekend_false():
 
     date = '2024-03-19'
@@ -187,41 +193,44 @@
     assert week_end(date, True) == 'Today is the end of the full week.'
 
 
 def test9_week_end_date_as_string_weekend_true_date_unknown_format():
 
     date = 'abc'
 
-    assert week_end(date, True) == "Couldn't process such date format."
+    with pytest.raises(ValueError) as exc_info:
+        week_end(date, True)
+
+    assert str(exc_info.value) == "Couldn't process such date format."
 
 
 # date_operations
     
 def test1_date_operations_date_string_operation_addition_frequency_day_weekend_false():
 
     date = '2024-03-19'
     range = 5
 
-    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=False) == 'Added date without weekend: 2024-03-24'
+    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=False) == 'Added date without weekend: 2024-03-26'
 
 
 def test2_date_operations_date_timestamp_operation_addition_frequency_day_weekend_false():
 
     date = pd.Timestamp('2024-03-19 12:30:00')
     range = 5
 
-    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=False) == 'Added date without weekend: 2024-03-24'
+    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=False) == 'Added date without weekend: 2024-03-26'
 
 
 def test3_date_operations_date_datetime_operation_addition_frequency_day_weekend_false():
 
     date = datetime(year=2024, month=3, day=19)
     range = 9
 
-    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=False) == 'Added date without weekend: 2024-03-28'
+    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=False) == 'Added date without weekend: 2024-04-01'
 
 
 def test4_date_operations_date_string_operation_addition_frequency_month_weekend_false():
 
     date = '2024-03-19'
     range = 1
 
@@ -269,31 +278,31 @@
 
 
 def test10_date_operations_date_string_operation_addition_frequency_day_weekend_true():
 
     date = '2024-03-19'
     range = 5
 
-    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=True) == 'Added date with weekend: 2024-03-26'
+    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=True) == 'Added date with weekend: 2024-03-24'
 
 
 def test11_date_operations_date_timestamp_operation_addition_frequency_day_weekend_true():
 
     date = pd.Timestamp('2024-03-19 12:30:00')
     range = 5
 
-    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=True) == 'Added date with weekend: 2024-03-26'
+    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=True) == 'Added date with weekend: 2024-03-24'
 
 
 def test12_date_operations_date_datetime_operation_addition_frequency_day_weekend_true():
 
     date = datetime(year=2024, month=3, day=19)
     range = 9
 
-    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=True) == 'Added date with weekend: 2024-04-01'
+    assert date_operations(date=date, operation='+', frequency='day', range=range, weekend=True) == 'Added date with weekend: 2024-03-28'
 
 
 def test13_date_operations_date_string_operation_addition_frequency_month_weekend_true():
 
     date = '2024-03-19'
     range = 1
 
@@ -341,31 +350,31 @@
 
 
 def test19_date_operations_date_string_operation_addition_frequency_day_weekend_false():
 
     date = '2024-03-19'
     range = 5
 
-    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=False) == 'Subtracted date without weekend: 2024-03-14'
+    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=False) == 'Subtracted date without weekend: 2024-03-12'
 
 
 def test20_date_operations_date_timestamp_operation_addition_frequency_day_weekend_false():
 
     date = pd.Timestamp('2024-03-19 12:30:00')
     range = 5
 
-    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=False) == 'Subtracted date without weekend: 2024-03-14'
+    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=False) == 'Subtracted date without weekend: 2024-03-12'
 
 
 def test21_date_operations_date_datetime_operation_addition_frequency_day_weekend_false():
 
     date = datetime(year=2024, month=3, day=19)
     range = 9
 
-    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=False) == 'Subtracted date without weekend: 2024-03-10'
+    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=False) == 'Subtracted date without weekend: 2024-03-06'
 
 
 def test22_date_operations_date_string_operation_addition_frequency_month_weekend_false():
 
     date = '2024-03-19'
     range = 1
 
@@ -413,31 +422,31 @@
 
 
 def test28_date_operations_date_string_operation_addition_frequency_day_weekend_true():
 
     date = '2024-03-19'
     range = 5
 
-    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=True) == 'Subtracted date with weekend: 2024-03-12'
+    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=True) == 'Subtracted date with weekend: 2024-03-14'
 
 
 def test29_date_operations_date_timestamp_operation_addition_frequency_day_weekend_true():
 
     date = pd.Timestamp('2024-03-19 12:30:00')
     range = 5
 
-    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=True) == 'Subtracted date with weekend: 2024-03-12'
+    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=True) == 'Subtracted date with weekend: 2024-03-14'
 
 
 def test30_date_operations_date_datetime_operation_addition_frequency_day_weekend_true():
 
     date = datetime(year=2024, month=3, day=19)
     range = 9
 
-    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=True) == 'Subtracted date with weekend: 2024-03-06'
+    assert date_operations(date=date, operation='-', frequency='day', range=range, weekend=True) == 'Subtracted date with weekend: 2024-03-10'
 
 
 def test31_date_operations_date_string_operation_addition_frequency_month_weekend_true():
 
     date = '2024-03-19'
     range = 1
```

