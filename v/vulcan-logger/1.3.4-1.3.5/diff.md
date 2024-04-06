# Comparing `tmp/vulcan-logger-1.3.4.tar.gz` & `tmp/vulcan-logger-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.3.4.tar", last modified: Sat Apr  6 19:47:17 2024, max compression
+gzip compressed data, was "vulcan-logger-1.3.5.tar", last modified: Sat Apr  6 19:50:42 2024, max compression
```

## Comparing `vulcan-logger-1.3.4.tar` & `vulcan-logger-1.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:47:17.429346 vulcan-logger-1.3.4/
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     1070 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/LICENSE
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     4492 2024-04-06 19:47:17.429346 vulcan-logger-1.3.4/PKG-INFO
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:47:17.425346 vulcan-logger-1.3.4/example/
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/example/__init__.py
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     1223 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/example/example.py
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:47:17.425346 vulcan-logger-1.3.4/medusa_logger/
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)       41 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/medusa_logger/__init__.py
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     3677 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/medusa_logger/decorator.py
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     1529 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/medusa_logger/encoder.py
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     4152 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/medusa_logger/logger.py
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       38 2024-04-06 19:47:17.429346 vulcan-logger-1.3.4/setup.cfg
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)      400 2024-04-06 19:47:17.000000 vulcan-logger-1.3.4/setup.py
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:47:17.425346 vulcan-logger-1.3.4/tests/
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       56 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/tests/__init__.py
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     2401 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/tests/test_decorator.py
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     2144 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/tests/test_encoder.py
--rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     5513 2024-04-06 19:41:05.000000 vulcan-logger-1.3.4/tests/test_logger.py
-drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:47:17.425346 vulcan-logger-1.3.4/vulcan_logger.egg-info/
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     4492 2024-04-06 19:47:17.000000 vulcan-logger-1.3.4/vulcan_logger.egg-info/PKG-INFO
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)      426 2024-04-06 19:47:17.000000 vulcan-logger-1.3.4/vulcan_logger.egg-info/SOURCES.txt
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)        1 2024-04-06 19:47:17.000000 vulcan-logger-1.3.4/vulcan_logger.egg-info/dependency_links.txt
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       12 2024-04-06 19:47:17.000000 vulcan-logger-1.3.4/vulcan_logger.egg-info/requires.txt
--rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       28 2024-04-06 19:47:17.000000 vulcan-logger-1.3.4/vulcan_logger.egg-info/top_level.txt
+drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:50:42.814518 vulcan-logger-1.3.5/
+-rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     1070 2024-04-06 19:41:05.000000 vulcan-logger-1.3.5/LICENSE
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     4492 2024-04-06 19:50:42.810518 vulcan-logger-1.3.5/PKG-INFO
+drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:50:42.810518 vulcan-logger-1.3.5/example/
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:41:05.000000 vulcan-logger-1.3.5/example/__init__.py
+-rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     1223 2024-04-06 19:49:59.000000 vulcan-logger-1.3.5/example/example.py
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       38 2024-04-06 19:50:42.814518 vulcan-logger-1.3.5/setup.cfg
+-rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)      400 2024-04-06 19:50:42.000000 vulcan-logger-1.3.5/setup.py
+drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:50:42.810518 vulcan-logger-1.3.5/tests/
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       56 2024-04-06 19:41:05.000000 vulcan-logger-1.3.5/tests/__init__.py
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     2401 2024-04-06 19:50:13.000000 vulcan-logger-1.3.5/tests/test_decorator.py
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     2144 2024-04-06 19:41:05.000000 vulcan-logger-1.3.5/tests/test_encoder.py
+-rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     5513 2024-04-06 19:50:20.000000 vulcan-logger-1.3.5/tests/test_logger.py
+drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:50:42.810518 vulcan-logger-1.3.5/vulcan_logger/
+-rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)       41 2024-04-06 19:41:05.000000 vulcan-logger-1.3.5/vulcan_logger/__init__.py
+-rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     3677 2024-04-06 19:41:05.000000 vulcan-logger-1.3.5/vulcan_logger/decorator.py
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     1529 2024-04-06 19:41:05.000000 vulcan-logger-1.3.5/vulcan_logger/encoder.py
+-rwxrwxr-x   0 vulcan    (1002) vulcan    (1002)     4152 2024-04-06 19:41:05.000000 vulcan-logger-1.3.5/vulcan_logger/logger.py
+drwxrwxr-x   0 vulcan    (1002) vulcan    (1002)        0 2024-04-06 19:50:42.810518 vulcan-logger-1.3.5/vulcan_logger.egg-info/
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)     4492 2024-04-06 19:50:42.000000 vulcan-logger-1.3.5/vulcan_logger.egg-info/PKG-INFO
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)      426 2024-04-06 19:50:42.000000 vulcan-logger-1.3.5/vulcan_logger.egg-info/SOURCES.txt
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)        1 2024-04-06 19:50:42.000000 vulcan-logger-1.3.5/vulcan_logger.egg-info/dependency_links.txt
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       12 2024-04-06 19:50:42.000000 vulcan-logger-1.3.5/vulcan_logger.egg-info/requires.txt
+-rw-rw-r--   0 vulcan    (1002) vulcan    (1002)       28 2024-04-06 19:50:42.000000 vulcan-logger-1.3.5/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.3.4/LICENSE` & `vulcan-logger-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.4/PKG-INFO` & `vulcan-logger-1.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.3.4
+Version: 1.3.5
 Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Medusa Logger
-Medusa Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
+# Vulcan Logger
+Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
 
-[View the full documentation here](https://medusa-logger.readthedocs.io/en/latest/)
+[View the full documentation here](https://vulcan-logger.readthedocs.io/en/latest/)
 
-![Medusa Logger](https://raw.githubusercontent.com/nodadyoushutup/medusa-logger/main/docs/img/examples.png)
+![Vulcan Logger](https://raw.githubusercontent.com/nodadyoushutup/vulcan-logger/main/docs/img/examples.png)
 
 ## Features
 - **Caller Information**: Automatically includes the caller's filename and line number in log messages for better traceability.
 - **Customizable Log Levels**: Easily configure log levels to control the severity of messages that the logger will process.
 - **Colored Logs**: Enhance log readability with colored logs for different log levels.
 - **Conditional Logging**: Conditionally log messages based on specific conditions to control verbosity.
 
 ## Installation
-You can install Medusa Logger via pip:
+You can install Vulcan Logger via pip:
 
 ```bash
-pip install medusa-logger
+pip install vulcan-logger
 ```
 
 ## Usage
-[Please check out example usage here](https://github.com/nodadyoushutup/medusa-logger/blob/main/example/example.py)
+[Please check out example usage here](https://github.com/nodadyoushutup/vulcan-logger/blob/main/example/example.py)
 
 ### Basic Logging
-1. Import the Logger class from the medusa_logger.logger module.
+1. Import the Logger class from the vulcan_logger.logger module.
 2. Initialize a Logger instance with a name and an optional log level. The default log level is INFO.
 3. Use the logging methods (debug, info, warning, error, critical) to log messages at various severity levels.
 ```python
-from medusa_logger.logger import Logger
+from vulcan_logger.logger import Logger
 
 # Initialize the logger with a custom name and log level
 logger = Logger(name='application_log', level='DEBUG')
 
 # Log messages at different levels
 logger.debug("Debug message for detailed diagnostic information")
 logger.info("Info message for general information")
 logger.warning("Warning message for potential issues")
 logger.error("Error message for serious problems")
 logger.critical("Critical message for severe conditions")
 ```
 
 ### Function Logging with Decorators
-Medusa Logger provides a logging decorator that can be applied to functions to automatically log calls, returns, and execution times. To use this feature:
+Vulcan Logger provides a logging decorator that can be applied to functions to automatically log calls, returns, and execution times. To use this feature:
 
-1. Import the log decorator from the medusa_logger.decorator module.
+1. Import the log decorator from the vulcan_logger.decorator module.
 2. Apply the @log decorator to any function. You can optionally specify a log level or a condition for logging.
 ```python
-from medusa_logger.decorator import log
+from vulcan_logger.decorator import log
 
 @log(level="DEBUG")
 def compute_sum(a, b):
     """Function to demonstrate logging with a decorator."""
     return a + b
 
 @log(condition=lambda args, kwargs: args[0] > args[1])
@@ -82,31 +82,31 @@
 ```
 Bash
 ```bash
 export MD_LOG_LEVEL="WARNING"
 ```
 
 ### Handling Exceptions
-Medusa Logger makes it easy to log exceptions. Use the logging methods within exception handling blocks to log errors and critical issues.
+Vulcan Logger makes it easy to log exceptions. Use the logging methods within exception handling blocks to log errors and critical issues.
 
 ```python
 try:
     # Potentially problematic code
     result = 10 / 0
 except ZeroDivisionError as e:
     logger.error(f"Caught an exception: {e}")
 ```
 
 ## Contributing
-Contributions to Medusa Logger are welcome! To contribute, follow these steps:
+Contributions to Vulcan Logger are welcome! To contribute, follow these steps:
 
 1. Fork the repository and clone it to your local machine.
 2. Install the development dependencies by running `pip install -r requirements.txt`.
 3. Make your changes and ensure tests pass by running `pytest`.
 4. Submit a pull request with a clear description of your changes and why they are beneficial.
 
-Please adhere to the [code of conduct](https://github.com/jacobfholland/medusa-logger/blob/main/docs/CODE_OF_CONDUCT.md) when contributing to this project.
+Please adhere to the [code of conduct](https://github.com/jacobfholland/vulcan-logger/blob/main/docs/CODE_OF_CONDUCT.md) when contributing to this project.
 
 ## License
-This project is licensed under the MIT License. See the [LICENSE](https://github.com/jacobfholland/medusa-logger/blob/main/LICENSE) file for details.
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/jacobfholland/vulcan-logger/blob/main/LICENSE) file for details.
```

### Comparing `vulcan-logger-1.3.4/example/example.py` & `vulcan-logger-1.3.5/example/example.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # example/example.py
 import os
 
-from medusa_logger.logger import Logger
-from medusa_logger.decorator import log
+from vulcan_logger.logger import Logger
+from vulcan_logger.decorator import log
 
 
 os.environ["MD_LOG_LEVEL"] = "DEBUG"  # Global log level filter
 
 # Functions defined with a log decorator. Level or Condition may be
 # passed as arguments on the decorator, or omitted.
```

### Comparing `vulcan-logger-1.3.4/medusa_logger/decorator.py` & `vulcan-logger-1.3.5/vulcan_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.4/medusa_logger/encoder.py` & `vulcan-logger-1.3.5/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.4/medusa_logger/logger.py` & `vulcan-logger-1.3.5/vulcan_logger/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.4/tests/test_decorator.py` & `vulcan-logger-1.3.5/tests/test_decorator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest.mock import patch
 import pytest
-from medusa_logger.decorator import log
+from vulcan_logger.decorator import log
 
 
 def _sample_function(x, y=2):
     return x + y
 
 
 def _slow_function(delay):
@@ -18,15 +18,15 @@
     """
     Tests the log decorator's ability to log the execution time of a function.
 
     Args:
         delay (float): A float representing the delay (in seconds) to simulate in the function.
     """
 
-    with patch('medusa_logger.decorator.Logger') as mock_logger:
+    with patch('vulcan_logger.decorator.Logger') as mock_logger:
         decorated = log(_slow_function)
         decorated(delay)
         last_call_args = mock_logger.return_value.debug.call_args_list[-1][0][0]
         assert "milliseconds" in last_call_args
 
 
 def test_log_decorator_basic() -> None:
@@ -34,30 +34,30 @@
     Tests the basic functionality of the log decorator.
 
     Verifies that a simple decorated function returns the expected result
     and that the logger's debug method is called three times (for the function call,
     return, and execution time logging).
     """
 
-    with patch('medusa_logger.decorator.Logger') as mock_logger:
+    with patch('vulcan_logger.decorator.Logger') as mock_logger:
         decorated = log(_sample_function)
         result = decorated(1, y=3)
         assert result == 4
         assert mock_logger.return_value.debug.call_count == 3
 
 
 def test_log_decorator_condition_false() -> None:
     """
     Tests the log decorator with the condition set to False.
 
     Verifies that when the log decorator is applied with a condition that evaluates
     to False, the decorated function executes normally but logging does not occur.
     """
 
-    with patch('medusa_logger.decorator.Logger') as mock_logger:
+    with patch('vulcan_logger.decorator.Logger') as mock_logger:
         decorated = log(_sample_function, condition=False)
         result = decorated(1, y=3)
         assert result == 4
         mock_logger.return_value.debug.assert_not_called()
 
 
 def test_log_decorator_log_level() -> None:
@@ -65,11 +65,11 @@
     Tests the log decorator's ability to log at a specified log level.
 
     Checks that when a log level of "INFO" is specified, the decorated
     function's activities are logged using the logger's info method instead of the
     default debug method.
     """
 
-    with patch('medusa_logger.decorator.Logger') as mock_logger:
+    with patch('vulcan_logger.decorator.Logger') as mock_logger:
         decorated = log(_sample_function, level="INFO")
         decorated(1, 2)
         assert mock_logger.return_value.info.call_count == 3
```

### Comparing `vulcan-logger-1.3.4/tests/test_encoder.py` & `vulcan-logger-1.3.5/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.4/tests/test_logger.py` & `vulcan-logger-1.3.5/tests/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from unittest.mock import patch, Mock
 import os
 import pytest
-from medusa_logger.logger import Logger
+from vulcan_logger.logger import Logger
 
 
 def _simulate_logging_call(file_name: str, line_no: int, func: callable, message: str) -> None:
     """
     Simulates a logging call with specified file name and line number information.
 
     This helper function is designed to mock the behavior of a logging call while
@@ -32,15 +32,15 @@
     Tests the initialization process of the Logger class.
 
     Verifies that the `coloredlogs.install` method is called exactly once during
     the initialization of a Logger instance, ensuring that the logger setup process
     is executed properly.
     """
 
-    with patch('medusa_logger.logger.coloredlogs.install') as mock_install:
+    with patch('vulcan_logger.logger.coloredlogs.install') as mock_install:
         Logger('test_logger', 'INFO')
         mock_install.assert_called_once()
 
 
 @pytest.mark.parametrize("method_name", ['debug'])
 def test_debug(method_name: str) -> None:
     """
@@ -137,12 +137,12 @@
 
     Sets the 'MD_LOG_LEVEL' environment variable to 'WARNING' and verifies that the
     Logger instance initializes with the log level correctly set to 'WARNING', as indicated
     by the arguments passed to `coloredlogs.install`.
     """
 
     os.environ['MD_LOG_LEVEL'] = 'WARNING'
-    with patch('medusa_logger.logger.coloredlogs.install') as mock_install:
+    with patch('vulcan_logger.logger.coloredlogs.install') as mock_install:
         Logger('test_logger')
         mock_install.assert_called_once()
         called_args, called_kwargs = mock_install.call_args
         assert 'WARNING' == called_kwargs['level']
```

### Comparing `vulcan-logger-1.3.4/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.3.5/vulcan_logger.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.3.4
+Version: 1.3.5
 Summary: A logging utility package with colored logs.
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Medusa Logger
-Medusa Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
+# Vulcan Logger
+Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
 
-[View the full documentation here](https://medusa-logger.readthedocs.io/en/latest/)
+[View the full documentation here](https://vulcan-logger.readthedocs.io/en/latest/)
 
-![Medusa Logger](https://raw.githubusercontent.com/nodadyoushutup/medusa-logger/main/docs/img/examples.png)
+![Vulcan Logger](https://raw.githubusercontent.com/nodadyoushutup/vulcan-logger/main/docs/img/examples.png)
 
 ## Features
 - **Caller Information**: Automatically includes the caller's filename and line number in log messages for better traceability.
 - **Customizable Log Levels**: Easily configure log levels to control the severity of messages that the logger will process.
 - **Colored Logs**: Enhance log readability with colored logs for different log levels.
 - **Conditional Logging**: Conditionally log messages based on specific conditions to control verbosity.
 
 ## Installation
-You can install Medusa Logger via pip:
+You can install Vulcan Logger via pip:
 
 ```bash
-pip install medusa-logger
+pip install vulcan-logger
 ```
 
 ## Usage
-[Please check out example usage here](https://github.com/nodadyoushutup/medusa-logger/blob/main/example/example.py)
+[Please check out example usage here](https://github.com/nodadyoushutup/vulcan-logger/blob/main/example/example.py)
 
 ### Basic Logging
-1. Import the Logger class from the medusa_logger.logger module.
+1. Import the Logger class from the vulcan_logger.logger module.
 2. Initialize a Logger instance with a name and an optional log level. The default log level is INFO.
 3. Use the logging methods (debug, info, warning, error, critical) to log messages at various severity levels.
 ```python
-from medusa_logger.logger import Logger
+from vulcan_logger.logger import Logger
 
 # Initialize the logger with a custom name and log level
 logger = Logger(name='application_log', level='DEBUG')
 
 # Log messages at different levels
 logger.debug("Debug message for detailed diagnostic information")
 logger.info("Info message for general information")
 logger.warning("Warning message for potential issues")
 logger.error("Error message for serious problems")
 logger.critical("Critical message for severe conditions")
 ```
 
 ### Function Logging with Decorators
-Medusa Logger provides a logging decorator that can be applied to functions to automatically log calls, returns, and execution times. To use this feature:
+Vulcan Logger provides a logging decorator that can be applied to functions to automatically log calls, returns, and execution times. To use this feature:
 
-1. Import the log decorator from the medusa_logger.decorator module.
+1. Import the log decorator from the vulcan_logger.decorator module.
 2. Apply the @log decorator to any function. You can optionally specify a log level or a condition for logging.
 ```python
-from medusa_logger.decorator import log
+from vulcan_logger.decorator import log
 
 @log(level="DEBUG")
 def compute_sum(a, b):
     """Function to demonstrate logging with a decorator."""
     return a + b
 
 @log(condition=lambda args, kwargs: args[0] > args[1])
@@ -82,31 +82,31 @@
 ```
 Bash
 ```bash
 export MD_LOG_LEVEL="WARNING"
 ```
 
 ### Handling Exceptions
-Medusa Logger makes it easy to log exceptions. Use the logging methods within exception handling blocks to log errors and critical issues.
+Vulcan Logger makes it easy to log exceptions. Use the logging methods within exception handling blocks to log errors and critical issues.
 
 ```python
 try:
     # Potentially problematic code
     result = 10 / 0
 except ZeroDivisionError as e:
     logger.error(f"Caught an exception: {e}")
 ```
 
 ## Contributing
-Contributions to Medusa Logger are welcome! To contribute, follow these steps:
+Contributions to Vulcan Logger are welcome! To contribute, follow these steps:
 
 1. Fork the repository and clone it to your local machine.
 2. Install the development dependencies by running `pip install -r requirements.txt`.
 3. Make your changes and ensure tests pass by running `pytest`.
 4. Submit a pull request with a clear description of your changes and why they are beneficial.
 
-Please adhere to the [code of conduct](https://github.com/jacobfholland/medusa-logger/blob/main/docs/CODE_OF_CONDUCT.md) when contributing to this project.
+Please adhere to the [code of conduct](https://github.com/jacobfholland/vulcan-logger/blob/main/docs/CODE_OF_CONDUCT.md) when contributing to this project.
 
 ## License
-This project is licensed under the MIT License. See the [LICENSE](https://github.com/jacobfholland/medusa-logger/blob/main/LICENSE) file for details.
+This project is licensed under the MIT License. See the [LICENSE](https://github.com/jacobfholland/vulcan-logger/blob/main/LICENSE) file for details.
```

