# Comparing `tmp/flask_terminal-0.1.0.tar.gz` & `tmp/flask_terminal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_terminal-0.1.0.tar", max compression
+gzip compressed data, was "flask_terminal-0.2.0.tar", max compression
```

## Comparing `flask_terminal-0.1.0.tar` & `flask_terminal-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-04-05 23:33:08.353132 flask_terminal-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     3915 2024-04-05 23:33:08.353132 flask_terminal-0.1.0/README.md
--rw-r--r--   0        0        0      135 2024-04-05 23:33:08.353132 flask_terminal-0.1.0/flask_terminal/__init__.py
--rw-r--r--   0        0        0     1045 2024-04-05 23:33:08.353132 flask_terminal-0.1.0/flask_terminal/config/logger_config.py
--rw-r--r--   0        0        0     2568 2024-04-05 23:33:08.353132 flask_terminal-0.1.0/flask_terminal/handlers/terminal_session_handler.py
--rw-r--r--   0        0        0     4111 2024-04-05 23:33:08.353132 flask_terminal-0.1.0/flask_terminal/static/flask-terminal/js/terminal.js
--rw-r--r--   0        0        0      554 2024-04-05 23:33:08.353132 flask_terminal-0.1.0/flask_terminal/templates/flask-terminal/terminal.html
--rw-r--r--   0        0        0     4288 2024-04-05 23:33:08.353132 flask_terminal-0.1.0/flask_terminal/terminal_blueprint.py
--rw-r--r--   0        0        0      476 2024-04-05 23:33:12.105154 flask_terminal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 flask_terminal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-05 23:41:41.034340 flask_terminal-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     4029 2024-04-05 23:41:41.034340 flask_terminal-0.2.0/README.md
+-rw-r--r--   0        0        0      135 2024-04-05 23:41:41.034340 flask_terminal-0.2.0/flask_terminal/__init__.py
+-rw-r--r--   0        0        0     1045 2024-04-05 23:41:41.034340 flask_terminal-0.2.0/flask_terminal/config/logger_config.py
+-rw-r--r--   0        0        0     2568 2024-04-05 23:41:41.038340 flask_terminal-0.2.0/flask_terminal/handlers/terminal_session_handler.py
+-rw-r--r--   0        0        0     4111 2024-04-05 23:41:41.038340 flask_terminal-0.2.0/flask_terminal/static/flask-terminal/js/terminal.js
+-rw-r--r--   0        0        0      554 2024-04-05 23:41:41.038340 flask_terminal-0.2.0/flask_terminal/templates/flask-terminal/terminal.html
+-rw-r--r--   0        0        0     4288 2024-04-05 23:41:41.038340 flask_terminal-0.2.0/flask_terminal/terminal_blueprint.py
+-rw-r--r--   0        0        0      956 2024-04-05 23:41:45.110406 flask_terminal-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5040 1970-01-01 00:00:00.000000 flask_terminal-0.2.0/PKG-INFO
```

### Comparing `flask_terminal-0.1.0/LICENSE.md` & `flask_terminal-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flask_terminal-0.1.0/README.md` & `flask_terminal-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,24 @@
 ## Overview
 
 The backend of Flask-Terminal is built on Flask, utilizing python-pty for pseudo-terminal emulation, enabling shell command execution. 
 The frontend leverages xterm.js for rendering the terminal interface. 
 Communication is handled through HTTP polling, circumventing the need for WebSockets. 
 The application is structured as a Flask Blueprint, allowing ease of integration into larger Flask applications.
 
+
 ## Features
 
 - **Browser-based Terminal**: Provides a terminal interface within the browser using xterm.js.
 - **Command Execution**: Supports the execution of /bin/sh commands, including the capability to spawn additional shells.
 - **Real-time Output**: Displays command execution output in real-time, facilitated by HTTP polling.
 - **Command Logging**: Utilizes a Python logger to log terminal activities, aiding in audit and debugging.
 
+![Demo](https://raw.githubusercontent.com/thevgergroup/flask-terminal/main/media/2024-04-05_19-22-14%20(1).gif)
+
 ## Getting started
 
 ### Security
 We cannot stress how much you need to secure this application, and recommend to enable only as needed and disable immediately afterwards.
 To add security to a blueprint please review how we do this with [Flask File Explorer](https://github.com/thevgergroup/flask-file-explorer?tab=readme-ov-file#flask-login-with-a-blueprint)
```

### Comparing `flask_terminal-0.1.0/flask_terminal/config/logger_config.py` & `flask_terminal-0.2.0/flask_terminal/config/logger_config.py`

 * *Files identical despite different names*

### Comparing `flask_terminal-0.1.0/flask_terminal/handlers/terminal_session_handler.py` & `flask_terminal-0.2.0/flask_terminal/handlers/terminal_session_handler.py`

 * *Files identical despite different names*

### Comparing `flask_terminal-0.1.0/flask_terminal/static/flask-terminal/js/terminal.js` & `flask_terminal-0.2.0/flask_terminal/static/flask-terminal/js/terminal.js`

 * *Files identical despite different names*

### Comparing `flask_terminal-0.1.0/flask_terminal/templates/flask-terminal/terminal.html` & `flask_terminal-0.2.0/flask_terminal/templates/flask-terminal/terminal.html`

 * *Files identical despite different names*

### Comparing `flask_terminal-0.1.0/flask_terminal/terminal_blueprint.py` & `flask_terminal-0.2.0/flask_terminal/terminal_blueprint.py`

 * *Files identical despite different names*

### Comparing `flask_terminal-0.1.0/PKG-INFO` & `flask_terminal-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: flask-terminal
-Version: 0.1.0
+Version: 0.2.0
 Summary: Browser based terminal for flask, use with hyper HYPER caution
+Home-page: https://github.com/thevgergroup/flask-terminal
 License: MIT
+Keywords: flask,terminal,browser,shell
 Author: patrick o'leary
 Author-email: pjaol@pjaol.com
 Requires-Python: >=3.9,<4.0
+Classifier: Framework :: Flask
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Unix Shell
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: System :: Systems Administration
 Requires-Dist: flask (>=3.0.2,<4.0.0)
+Project-URL: Repository, https://github.com/thevgergroup/flask-terminal
 Description-Content-Type: text/markdown
 
 # Flask-Terminal
 
 Flask-Terminal is a bad idea wrapped in an even worse implementation
 Use this with care, it is a shell on your server
 - [Flask-Terminal](#flask-terminal)
@@ -39,21 +47,24 @@
 ## Overview
 
 The backend of Flask-Terminal is built on Flask, utilizing python-pty for pseudo-terminal emulation, enabling shell command execution. 
 The frontend leverages xterm.js for rendering the terminal interface. 
 Communication is handled through HTTP polling, circumventing the need for WebSockets. 
 The application is structured as a Flask Blueprint, allowing ease of integration into larger Flask applications.
 
+
 ## Features
 
 - **Browser-based Terminal**: Provides a terminal interface within the browser using xterm.js.
 - **Command Execution**: Supports the execution of /bin/sh commands, including the capability to spawn additional shells.
 - **Real-time Output**: Displays command execution output in real-time, facilitated by HTTP polling.
 - **Command Logging**: Utilizes a Python logger to log terminal activities, aiding in audit and debugging.
 
+![Demo](https://raw.githubusercontent.com/thevgergroup/flask-terminal/main/media/2024-04-05_19-22-14%20(1).gif)
+
 ## Getting started
 
 ### Security
 We cannot stress how much you need to secure this application, and recommend to enable only as needed and disable immediately afterwards.
 To add security to a blueprint please review how we do this with [Flask File Explorer](https://github.com/thevgergroup/flask-file-explorer?tab=readme-ov-file#flask-login-with-a-blueprint)
```

