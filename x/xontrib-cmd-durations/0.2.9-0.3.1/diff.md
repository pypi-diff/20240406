# Comparing `tmp/xontrib-cmd-durations-0.2.9.tar.gz` & `tmp/xontrib-cmd-durations-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-cmd-durations-0.2.9.tar", max compression
+gzip compressed data, was "xontrib-cmd-durations-0.3.1.tar", last modified: Sat Apr  6 14:22:55 2024, max compression
```

## Comparing `xontrib-cmd-durations-0.2.9.tar` & `xontrib-cmd-durations-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1074 2022-02-12 07:03:39.371127 xontrib-cmd-durations-0.2.9/LICENSE
--rw-r--r--   0        0        0     1409 2022-07-07 05:25:26.899344 xontrib-cmd-durations-0.2.9/README.md
--rw-r--r--   0        0        0     1364 2022-07-07 05:27:40.259625 xontrib-cmd-durations-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     3871 2022-07-07 05:25:26.895693 xontrib-cmd-durations-0.2.9/xontrib/cmd_done.py
--rw-r--r--   0        0        0     2310 2022-07-07 05:27:50.609508 xontrib-cmd-durations-0.2.9/setup.py
--rw-r--r--   0        0        0     2956 2022-07-07 05:27:50.609669 xontrib-cmd-durations-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-06 14:22:52.677982 xontrib-cmd-durations-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1872 2024-04-06 14:22:52.677982 xontrib-cmd-durations-0.3.1/README.md
+-rw-r--r--   0        0        0     1424 2024-04-06 14:22:52.677982 xontrib-cmd-durations-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4302 2024-04-06 14:22:52.677982 xontrib-cmd-durations-0.3.1/xontrib/cmd_done.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 xontrib-cmd-durations-0.3.1/PKG-INFO
```

### Comparing `xontrib-cmd-durations-0.2.9/LICENSE` & `xontrib-cmd-durations-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-cmd-durations-0.2.9/README.md` & `xontrib-cmd-durations-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## Overview
 
 <p align="center">
-Send notification once long-running command is finished and also show the execution time..
+Send notification once long-running command is finished and also show the execution time.
 </p>
 
 ## Installation
 
 To install use pip:
 
 ``` bash
@@ -31,16 +31,31 @@
 
 ![](./images/2020-11-02-13-38-47.png)
 
 Currently the focusing part requires `xdotool` to be installed.
 
 ## Known issues
 
-### notifications in Windows
+### Notifications in Windows
 On windows the notification will get triggered all the time. 
 `Finding whether the terminal is focused` is not implemented for Windows yet and PRs are very welcome on that.
 Set `$XONTRIB_CD_TRIGGER_NOTIFICATION = False` to completely off the notification part.
 
+### Notifications in MacOS
+
+If you want to change the app name in notification in MacOS you can use `$XONTRIB_CD_NOTIFICATION_APP_NAME` environment variable with [automatically replaced keywords](https://xon.sh/tutorial.html#customizing-the-prompt):
+```xsh
+$XONTRIB_CD_NOTIFICATION_APP_NAME = '{user}@{hostname}:{cwd}'
+$RIGHT_PROMPT = '{long_cmd_duration}'
+xontrib load cmd_done
+
+sleep 6
+# Switch to another window
+```
+Result:
+
+![](./images/notification-mac.png)
+
 
 ## Credits
 
 This package was created with [xontrib cookiecutter template](https://github.com/jnoortheen/xontrib-cookiecutter).
```

### Comparing `xontrib-cmd-durations-0.2.9/pyproject.toml` & `xontrib-cmd-durations-0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,56 @@
-[tool.poetry]
+[project]
+authors = [
+    { name = "Noortheen Raja J", email = "jnoortheen@gmail.com" },
+]
+requires-python = ">=3.7"
+dependencies = [
+    "xonsh>=0.10",
+    "notify-py>=0.3.3; python_version >= \"3.6\" and python_version < \"4.0\"",
+]
 name = "xontrib-cmd-durations"
-version = "0.2.9"
+version = "0.3.1"
 description = "Send notification once long running command is finished. Add duration PROMP_FIELD."
-authors = ["Noortheen Raja J <jnoortheen@gmail.com>"]
-
-license = "MIT"
 readme = "README.md"
-
-repository = "https://github.com/jnoortheen/xontrib-cmd-durations"
-keywords = ['xontrib', 'xonsh']
+keywords = [
+    "xontrib",
+    "xonsh",
+]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: System :: Shells",
     "Topic :: System :: System Shells",
     "Topic :: Terminals",
     "Programming Language :: Python",
     "Topic :: Utilities",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3",
 ]
 
+[project.optional-dependencies]
+dev = [
+    "pytest",
+    "black",
+]
 
-packages = [{ include = "xontrib" }]
+[project.license]
+text = "MIT"
 
-[tool.poetry.urls]
+[project.urls]
 Documentation = "https://github.com/jnoortheen/xontrib-cmd-durations/blob/master/README.md"
 Code = "https://github.com/jnoortheen/xontrib-cmd-durations"
 "Issue tracker" = "https://github.com/jnoortheen/xontrib-cmd-durations/issues"
+repository = "https://github.com/jnoortheen/xontrib-cmd-durations"
 
-
-[tool.poetry.dependencies]
-python = ">=3.6"
-xonsh = ">=0.10"
-notify-py = {version=">=0.3.3", python = ">=3.6,<4.0"}
-
-[tool.poetry.dev-dependencies]
-pytest = "*"
-black = { version = "*", allow-prereleases = true }
+[tool.pdm.build]
+includes = [
+    "xontrib",
+]
 
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = [
+    "pdm-pep517>=1.0.0",
+]
+build-backend = "pdm.pep517.api"
```

### Comparing `xontrib-cmd-durations-0.2.9/xontrib/cmd_done.py` & `xontrib-cmd-durations-0.3.1/xontrib/cmd_done.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+"""Show long running commands durations in prompt with option to send notification when terminal is not focused. """
+
 import functools
 import subprocess as sp
 
-from xonsh.built_ins import XSH
+from xonsh.built_ins import XSH as xsh
 
-xsh = XSH
 LONG_DURATION = xsh.env.get("XONTRIB_CD_LONG_DURATION", 5)  # seconds
 TRIGGER_NOTIFICATION = xsh.env.get("XONTRIB_CD_TRIGGER_NOTIFICATION", True)
+NOTIFICATION_APP_NAME = xsh.env.get("XONTRIB_CD_NOTIFICATION_APP_NAME", xsh.env.get("TITLE", "xonsh"))
 
 
 def _term_program_mapping() -> dict:
     """The app name doesn't match the $TERMPROGRAM . This is to map equivalent ones in OSX"""
-    defaults = {"iterm.app": "iTerm2", "apple_terminal": "Terminal"}
-
+    defaults = {"iterm.app": "iTerm2", "apple_terminal": "Terminal", "vscode": "Code", "pycharm": "PyCharm",
+                 "kate": "Kate"}
     maps = xsh.env.get("XONTRIB_CD_TERM_PROGRAM_MAP", defaults)
-
     return {key.lower(): val for key, val in maps.items()}
 
 
 @functools.lru_cache()
 def _darwin_get_app_name(term_program: str):
     maps = _term_program_mapping()
     return maps.get(term_program.lower(), term_program)
@@ -84,30 +85,34 @@
         )
         return False
     curr_winid = _xdotool_window_id()
     return curr_winid == winid
 
 
 def _darwin_is_app_window_focused():
-    term = xsh.env.get("TERM_PROGRAM")
-    if not term:
-        _warn(
-            "Environment variable $TERM_PROGRAM is unset. "
-            "It should be set by the terminal application on shell startup. "
-            "Not able to find active window."
-        )
-        return False
+    out = None
+    bundle_id = ""
+    term_program = ""
+
+    if bundle_id := xsh.env.get("__CFBundleIdentifier"):
+        out = sp.check_output(["lsappinfo", "info", "-bundleid", bundle_id])
+
+    elif term_program := xsh.env.get("TERM_PROGRAM"):
+        appname = _darwin_get_app_name(term_program)
+        out = sp.check_output(["lsappinfo", "info", "-app", appname])
 
-    appname = _darwin_get_app_name(term)
-    out = sp.check_output(["lsappinfo", "info", "-app", appname])
     if not out:
         _warn(
-            f"$TERM_PROGRAM={term} is not a valid app name. Existing mapping ({maps}) doesn't get the correct name. "
-            f"Please update $XONTRIB_CD_TERM_PROGRAM_MAP environment variable for your terminal."
+            "xontrib-cmd-durations: "
+            f"Application not found by $__CFBundleIdentifier ({bundle_id}) "
+            f"and because $TERM_PROGRAM ({repr(term_program)}) "
+            f"not found in $XONTRIB_CD_TERM_PROGRAM_MAP:\n"
+            f"({_term_program_mapping()})"
         )
+        return False
 
     return b"(in front)" in out
 
 
 def is_app_window_focused():
     # https://stackoverflow.com/questions/10266281/obtain-active-window-using-python
     if is_darwin_system():
@@ -124,14 +129,15 @@
 
     if is_app_window_focused():
         return
 
     from notifypy import Notify
 
     noti = Notify()
+    noti.application_name = xsh.shell.prompt_formatter(NOTIFICATION_APP_NAME)
     noti.title = str(f"{cmd}")
     noti.message = f'{"Failed" if rtn else "Done"} in {readable}'
     noti.send()
 
 
 def long_cmd_duration():
     history = xsh.history
```

### Comparing `xontrib-cmd-durations-0.2.9/setup.py` & `xontrib-cmd-durations-0.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,88 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: xontrib-cmd-durations
+Version: 0.3.1
+Summary: Send notification once long running command is finished. Add duration PROMP_FIELD.
+License: MIT
+Keywords: xontrib,xonsh
+Author-email: Noortheen Raja J <jnoortheen@gmail.com>
+Requires-Python: >=3.7
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Shells
+Classifier: Topic :: System :: System Shells
+Classifier: Topic :: Terminals
+Classifier: Topic :: Utilities
+Provides-Extra: dev
+Project-URL: Code, https://github.com/jnoortheen/xontrib-cmd-durations
+Project-URL: Documentation, https://github.com/jnoortheen/xontrib-cmd-durations/blob/master/README.md
+Project-URL: Issue tracker, https://github.com/jnoortheen/xontrib-cmd-durations/issues
+Project-URL: repository, https://github.com/jnoortheen/xontrib-cmd-durations
+Description-Content-Type: text/markdown
 
-packages = \
-['xontrib']
+## Overview
 
-package_data = \
-{'': ['*']}
+<p align="center">
+Send notification once long-running command is finished and also show the execution time.
+</p>
 
-install_requires = \
-['xonsh>=0.10']
-
-extras_require = \
-{':python_version >= "3.6" and python_version < "4.0"': ['notify-py>=0.3.3']}
-
-setup_kwargs = {
-    'name': 'xontrib-cmd-durations',
-    'version': '0.2.9',
-    'description': 'Send notification once long running command is finished. Add duration PROMP_FIELD.',
-    'long_description': '## Overview\n\n<p align="center">\nSend notification once long-running command is finished and also show the execution time..\n</p>\n\n## Installation\n\nTo install use pip:\n\n``` bash\nxpip install xontrib-cmd-durations\n# or: xpip install -U git+https://github.com/jnoortheen/xontrib-cmd-durations\n```\n\n## Usage\n\nAdd the `long_cmd_duration` section to the [prompt fields](https://xon.sh/tutorial.html#customizing-the-prompt) and load the xontrib i.e.:\n\n``` bash\n$RIGHT_PROMPT = \'{long_cmd_duration:⌛{}}{user:{{BOLD_RED}}🤖{}}{hostname:{{BOLD_#FA8072}}🖥{}}\'\n$XONTRIB_CD_LONG_DURATION = 5  # default\nxontrib load cmd_done\n```\n\nIf the command is taking more than `$XONTRIB_CD_LONG_DURATION` seconds then `long_cmd_duration` returns the duration in human readable way:\n\n![](./images/2020-10-26-10-59-38.png)\n\nThe desktop notification is sent if the terminal is not focused:\n\n![](./images/2020-11-02-13-38-47.png)\n\nCurrently the focusing part requires `xdotool` to be installed.\n\n## Known issues\n\n### notifications in Windows\nOn windows the notification will get triggered all the time. \n`Finding whether the terminal is focused` is not implemented for Windows yet and PRs are very welcome on that.\nSet `$XONTRIB_CD_TRIGGER_NOTIFICATION = False` to completely off the notification part.\n\n\n## Credits\n\nThis package was created with [xontrib cookiecutter template](https://github.com/jnoortheen/xontrib-cookiecutter).\n',
-    'author': 'Noortheen Raja J',
-    'author_email': 'jnoortheen@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/jnoortheen/xontrib-cmd-durations',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6',
-}
+## Installation
 
+To install use pip:
+
+``` bash
+xpip install xontrib-cmd-durations
+# or: xpip install -U git+https://github.com/jnoortheen/xontrib-cmd-durations
+```
+
+## Usage
+
+Add the `long_cmd_duration` section to the [prompt fields](https://xon.sh/tutorial.html#customizing-the-prompt) and load the xontrib i.e.:
+
+``` bash
+$RIGHT_PROMPT = '{long_cmd_duration:⌛{}}{user:{{BOLD_RED}}🤖{}}{hostname:{{BOLD_#FA8072}}🖥{}}'
+$XONTRIB_CD_LONG_DURATION = 5  # default
+xontrib load cmd_done
+```
+
+If the command is taking more than `$XONTRIB_CD_LONG_DURATION` seconds then `long_cmd_duration` returns the duration in human readable way:
+
+![](./images/2020-10-26-10-59-38.png)
+
+The desktop notification is sent if the terminal is not focused:
+
+![](./images/2020-11-02-13-38-47.png)
+
+Currently the focusing part requires `xdotool` to be installed.
+
+## Known issues
+
+### Notifications in Windows
+On windows the notification will get triggered all the time. 
+`Finding whether the terminal is focused` is not implemented for Windows yet and PRs are very welcome on that.
+Set `$XONTRIB_CD_TRIGGER_NOTIFICATION = False` to completely off the notification part.
+
+### Notifications in MacOS
+
+If you want to change the app name in notification in MacOS you can use `$XONTRIB_CD_NOTIFICATION_APP_NAME` environment variable with [automatically replaced keywords](https://xon.sh/tutorial.html#customizing-the-prompt):
+```xsh
+$XONTRIB_CD_NOTIFICATION_APP_NAME = '{user}@{hostname}:{cwd}'
+$RIGHT_PROMPT = '{long_cmd_duration}'
+xontrib load cmd_done
+
+sleep 6
+# Switch to another window
+```
+Result:
+
+![](./images/notification-mac.png)
+
+
+## Credits
+
+This package was created with [xontrib cookiecutter template](https://github.com/jnoortheen/xontrib-cookiecutter).
 
-setup(**setup_kwargs)
```

