# Comparing `tmp/function2widgets-0.6.7.tar.gz` & `tmp/function2widgets-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function2widgets-0.6.7.tar", max compression
+gzip compressed data, was "function2widgets-0.6.8.tar", max compression
```

## Comparing `function2widgets-0.6.7.tar` & `function2widgets-0.6.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.7/function2widgets/__init__.py
--rw-r--r--   0        0        0     3030 2024-04-02 11:05:09.916571 function2widgets-0.6.7/function2widgets/common.py
--rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.7/function2widgets/factory.py
--rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.7/function2widgets/info.py
--rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.7/function2widgets/parser/__init__.py
--rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.7/function2widgets/parser/docstr_parser.py
--rw-r--r--   0        0        0     6525 2024-04-06 03:48:47.967339 function2widgets-0.6.7/function2widgets/parser/function_parser.py
--rw-r--r--   0        0        0     3089 2024-03-31 08:24:42.428417 function2widgets-0.6.7/function2widgets/parser/parameter_parser.py
--rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.7/function2widgets/parser/widgetconfigs_parser.py
--rw-r--r--   0        0        0     4402 2024-03-31 08:24:42.429443 function2widgets-0.6.7/function2widgets/widget.py
--rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.7/function2widgets/widgets/__init__.py
--rw-r--r--   0        0        0     5853 2024-04-05 11:35:06.039590 function2widgets-0.6.7/function2widgets/widgets/_sourcecodeedit.py
--rw-r--r--   0        0        0     1930 2024-04-02 10:46:00.405726 function2widgets-0.6.7/function2widgets/widgets/allwidgets.py
--rw-r--r--   0        0        0     6832 2024-03-31 15:42:30.788097 function2widgets-0.6.7/function2widgets/widgets/base.py
--rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.7/function2widgets/widgets/editor/__init__.py
--rw-r--r--   0        0        0     6061 2024-04-05 05:18:47.514607 function2widgets-0.6.7/function2widgets/widgets/editor/base.py
--rw-r--r--   0        0        0     2024 2024-04-05 05:17:03.984199 function2widgets-0.6.7/function2widgets/widgets/editor/codeeditor.py
--rw-r--r--   0        0        0     1169 2024-03-31 08:24:42.436443 function2widgets-0.6.7/function2widgets/widgets/editor/dicteditor.py
--rw-r--r--   0        0        0     4654 2024-04-05 05:20:20.545687 function2widgets-0.6.7/function2widgets/widgets/editor/jsoneditor.py
--rw-r--r--   0        0        0     1245 2024-04-05 05:16:06.955595 function2widgets-0.6.7/function2widgets/widgets/editor/listeditor.py
--rw-r--r--   0        0        0     1621 2024-04-05 08:35:32.821279 function2widgets-0.6.7/function2widgets/widgets/editor/tupleeditor.py
--rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.7/function2widgets/widgets/lineedit/__init__.py
--rw-r--r--   0        0        0     2434 2024-03-31 08:24:42.440428 function2widgets-0.6.7/function2widgets/widgets/lineedit/floatedit.py
--rw-r--r--   0        0        0     2002 2024-03-31 08:24:42.441427 function2widgets-0.6.7/function2widgets/widgets/lineedit/intedit.py
--rw-r--r--   0        0        0     3131 2024-04-05 08:44:44.617036 function2widgets-0.6.7/function2widgets/widgets/lineedit/stredit.py
--rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.7/function2widgets/widgets/misc/__init__.py
--rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.7/function2widgets/widgets/misc/coloredit.py
--rw-r--r--   0        0        0     3522 2024-04-05 08:39:38.679633 function2widgets-0.6.7/function2widgets/widgets/misc/dateedit.py
--rw-r--r--   0        0        0     4070 2024-04-05 08:40:13.233230 function2widgets-0.6.7/function2widgets/widgets/misc/datetimeedit.py
--rw-r--r--   0        0        0     3403 2024-04-05 08:40:44.115431 function2widgets-0.6.7/function2widgets/widgets/misc/timeedit.py
--rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.7/function2widgets/widgets/numberinput/__init__.py
--rw-r--r--   0        0        0     4693 2024-04-05 08:46:13.101173 function2widgets-0.6.7/function2widgets/widgets/numberinput/dial.py
--rw-r--r--   0        0        0     3126 2024-04-05 08:48:36.095832 function2widgets-0.6.7/function2widgets/widgets/numberinput/floatspin.py
--rw-r--r--   0        0        0     2788 2024-04-05 08:49:10.364397 function2widgets-0.6.7/function2widgets/widgets/numberinput/intspin.py
--rw-r--r--   0        0        0     5162 2024-04-05 08:50:37.670447 function2widgets-0.6.7/function2widgets/widgets/numberinput/slider.py
--rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.7/function2widgets/widgets/pathedit/__init__.py
--rw-r--r--   0        0        0     6222 2024-04-05 08:52:36.809553 function2widgets-0.6.7/function2widgets/widgets/pathedit/base.py
--rw-r--r--   0        0        0      936 2024-03-31 08:24:42.449980 function2widgets-0.6.7/function2widgets/widgets/pathedit/dirpathedit.py
--rw-r--r--   0        0        0     1107 2024-03-31 08:24:42.449980 function2widgets-0.6.7/function2widgets/widgets/pathedit/filepathedit.py
--rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.7/function2widgets/widgets/selectwidget/__init__.py
--rw-r--r--   0        0        0     1953 2024-04-05 08:56:12.887209 function2widgets-0.6.7/function2widgets/widgets/selectwidget/checkbox.py
--rw-r--r--   0        0        0     2823 2024-04-05 08:58:14.255857 function2widgets-0.6.7/function2widgets/widgets/selectwidget/checkbox_group.py
--rw-r--r--   0        0        0     2985 2024-04-05 08:58:25.987503 function2widgets-0.6.7/function2widgets/widgets/selectwidget/combobox.py
--rw-r--r--   0        0        0     2268 2024-04-05 08:58:38.649153 function2widgets-0.6.7/function2widgets/widgets/selectwidget/combobox_edit.py
--rw-r--r--   0        0        0     3569 2024-04-05 08:59:23.433045 function2widgets-0.6.7/function2widgets/widgets/selectwidget/radiobutton_group.py
--rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.7/function2widgets/widgets/textedit/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-31 08:24:42.456979 function2widgets-0.6.7/function2widgets/widgets/textedit/codeedit.py
--rw-r--r--   0        0        0     2356 2024-03-31 17:57:08.161215 function2widgets-0.6.7/function2widgets/widgets/textedit/plaintext.py
--rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.7/License
--rw-r--r--   0        0        0      714 2024-04-06 03:49:12.250329 function2widgets-0.6.7/pyproject.toml
--rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.7/README.md
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-26 14:06:46.014790 function2widgets-0.6.8/function2widgets/__init__.py
+-rw-r--r--   0        0        0     2999 2024-04-06 12:13:58.866108 function2widgets-0.6.8/function2widgets/common.py
+-rw-r--r--   0        0        0     3278 2024-03-31 08:24:42.424892 function2widgets-0.6.8/function2widgets/factory.py
+-rw-r--r--   0        0        0     4810 2024-03-31 08:24:42.425891 function2widgets-0.6.8/function2widgets/info.py
+-rw-r--r--   0        0        0        2 2024-03-31 08:24:42.425891 function2widgets-0.6.8/function2widgets/parser/__init__.py
+-rw-r--r--   0        0        0     2751 2024-03-31 08:24:42.426892 function2widgets-0.6.8/function2widgets/parser/docstr_parser.py
+-rw-r--r--   0        0        0     6537 2024-04-06 12:13:58.867110 function2widgets-0.6.8/function2widgets/parser/function_parser.py
+-rw-r--r--   0        0        0     3068 2024-04-06 12:13:58.867110 function2widgets-0.6.8/function2widgets/parser/parameter_parser.py
+-rw-r--r--   0        0        0     1670 2024-03-31 08:24:42.428417 function2widgets-0.6.8/function2widgets/parser/widgetconfigs_parser.py
+-rw-r--r--   0        0        0     4498 2024-04-06 12:13:58.867110 function2widgets-0.6.8/function2widgets/widget.py
+-rw-r--r--   0        0        0       27 2024-03-31 08:24:42.430443 function2widgets-0.6.8/function2widgets/widgets/__init__.py
+-rw-r--r--   0        0        0     5853 2024-04-05 11:35:06.039590 function2widgets-0.6.8/function2widgets/widgets/_sourcecodeedit.py
+-rw-r--r--   0        0        0     1930 2024-04-02 10:46:00.405726 function2widgets-0.6.8/function2widgets/widgets/allwidgets.py
+-rw-r--r--   0        0        0     9123 2024-04-06 12:13:58.867110 function2widgets-0.6.8/function2widgets/widgets/base.py
+-rw-r--r--   0        0        0      263 2024-03-31 08:24:42.433443 function2widgets-0.6.8/function2widgets/widgets/editor/__init__.py
+-rw-r--r--   0        0        0     6067 2024-04-06 12:13:58.868617 function2widgets-0.6.8/function2widgets/widgets/editor/base.py
+-rw-r--r--   0        0        0     2030 2024-04-06 12:13:58.868617 function2widgets-0.6.8/function2widgets/widgets/editor/codeeditor.py
+-rw-r--r--   0        0        0     1170 2024-04-06 12:13:58.869627 function2widgets-0.6.8/function2widgets/widgets/editor/dicteditor.py
+-rw-r--r--   0        0        0     4660 2024-04-06 12:13:58.869627 function2widgets-0.6.8/function2widgets/widgets/editor/jsoneditor.py
+-rw-r--r--   0        0        0     1246 2024-04-06 12:13:58.869627 function2widgets-0.6.8/function2widgets/widgets/editor/listeditor.py
+-rw-r--r--   0        0        0     1627 2024-04-06 12:13:58.870629 function2widgets-0.6.8/function2widgets/widgets/editor/tupleeditor.py
+-rw-r--r--   0        0        0      153 2024-03-31 08:24:42.439428 function2widgets-0.6.8/function2widgets/widgets/lineedit/__init__.py
+-rw-r--r--   0        0        0     2440 2024-04-06 12:13:58.870629 function2widgets-0.6.8/function2widgets/widgets/lineedit/floatedit.py
+-rw-r--r--   0        0        0     2008 2024-04-06 12:13:58.870629 function2widgets-0.6.8/function2widgets/widgets/lineedit/intedit.py
+-rw-r--r--   0        0        0     3137 2024-04-06 12:13:58.871627 function2widgets-0.6.8/function2widgets/widgets/lineedit/stredit.py
+-rw-r--r--   0        0        0      150 2024-04-01 15:50:26.686578 function2widgets-0.6.8/function2widgets/widgets/misc/__init__.py
+-rw-r--r--   0        0        0       22 2024-03-31 08:24:42.442430 function2widgets-0.6.8/function2widgets/widgets/misc/coloredit.py
+-rw-r--r--   0        0        0     3528 2024-04-06 12:13:58.871627 function2widgets-0.6.8/function2widgets/widgets/misc/dateedit.py
+-rw-r--r--   0        0        0     4076 2024-04-06 12:13:58.872627 function2widgets-0.6.8/function2widgets/widgets/misc/datetimeedit.py
+-rw-r--r--   0        0        0     3409 2024-04-06 12:13:58.872627 function2widgets-0.6.8/function2widgets/widgets/misc/timeedit.py
+-rw-r--r--   0        0        0      178 2024-03-31 08:24:42.444428 function2widgets-0.6.8/function2widgets/widgets/numberinput/__init__.py
+-rw-r--r--   0        0        0     4699 2024-04-06 12:13:58.872627 function2widgets-0.6.8/function2widgets/widgets/numberinput/dial.py
+-rw-r--r--   0        0        0     3132 2024-04-06 12:13:58.873629 function2widgets-0.6.8/function2widgets/widgets/numberinput/floatspin.py
+-rw-r--r--   0        0        0     2794 2024-04-06 12:13:58.873629 function2widgets-0.6.8/function2widgets/widgets/numberinput/intspin.py
+-rw-r--r--   0        0        0     5168 2024-04-06 12:13:58.873629 function2widgets-0.6.8/function2widgets/widgets/numberinput/slider.py
+-rw-r--r--   0        0        0      321 2024-03-31 08:24:42.447443 function2widgets-0.6.8/function2widgets/widgets/pathedit/__init__.py
+-rw-r--r--   0        0        0     6228 2024-04-06 12:13:58.874628 function2widgets-0.6.8/function2widgets/widgets/pathedit/base.py
+-rw-r--r--   0        0        0      942 2024-04-06 12:13:58.874628 function2widgets-0.6.8/function2widgets/widgets/pathedit/dirpathedit.py
+-rw-r--r--   0        0        0     1113 2024-04-06 12:13:58.875628 function2widgets-0.6.8/function2widgets/widgets/pathedit/filepathedit.py
+-rw-r--r--   0        0        0      284 2024-03-31 08:24:42.450995 function2widgets-0.6.8/function2widgets/widgets/selectwidget/__init__.py
+-rw-r--r--   0        0        0     1954 2024-04-06 12:13:58.875628 function2widgets-0.6.8/function2widgets/widgets/selectwidget/checkbox.py
+-rw-r--r--   0        0        0     2829 2024-04-06 12:13:58.875628 function2widgets-0.6.8/function2widgets/widgets/selectwidget/checkbox_group.py
+-rw-r--r--   0        0        0     2991 2024-04-06 12:13:58.876627 function2widgets-0.6.8/function2widgets/widgets/selectwidget/combobox.py
+-rw-r--r--   0        0        0     2274 2024-04-06 12:13:58.876627 function2widgets-0.6.8/function2widgets/widgets/selectwidget/combobox_edit.py
+-rw-r--r--   0        0        0     3575 2024-04-06 12:13:58.876627 function2widgets-0.6.8/function2widgets/widgets/selectwidget/radiobutton_group.py
+-rw-r--r--   0        0        0      103 2024-03-31 08:24:42.454980 function2widgets-0.6.8/function2widgets/widgets/textedit/__init__.py
+-rw-r--r--   0        0        0     1817 2024-04-06 12:13:58.877629 function2widgets-0.6.8/function2widgets/widgets/textedit/codeedit.py
+-rw-r--r--   0        0        0     2362 2024-04-06 12:13:58.877629 function2widgets-0.6.8/function2widgets/widgets/textedit/plaintext.py
+-rw-r--r--   0        0        0    35821 2024-03-07 14:10:28.559603 function2widgets-0.6.8/License
+-rw-r--r--   0        0        0      714 2024-04-06 12:14:34.601098 function2widgets-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0      898 2024-03-31 08:24:42.401374 function2widgets-0.6.8/README.md
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 function2widgets-0.6.8/PKG-INFO
```

### Comparing `function2widgets-0.6.7/function2widgets/common.py` & `function2widgets-0.6.8/function2widgets/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import ast
 import logging
 import os.path
 import re
 import warnings
-from datetime import datetime
 from typing import Any, Optional, List, Dict
 
 import tomli
 from PyQt6.QtCore import QDateTime, QDate, QTime
 
 TYPING_ANNOTATION_PATTERN = re.compile(r"^(typing\..+?)(\[.+])*$")
```

### Comparing `function2widgets-0.6.7/function2widgets/factory.py` & `function2widgets-0.6.8/function2widgets/factory.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.7/function2widgets/info.py` & `function2widgets-0.6.8/function2widgets/info.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.7/function2widgets/parser/docstr_parser.py` & `function2widgets-0.6.8/function2widgets/parser/docstr_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.7/function2widgets/parser/function_parser.py` & `function2widgets-0.6.8/function2widgets/parser/function_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         widget_args["parameter_name"] = param_info.name
         if param_info.default is not DEFAULT_FOR_EMPTY:
             widget_args["default"] = param_info.default
         widget_args["label"] = param_info.name
         widget_args["description"] = param_info.description
         widget_args["stylesheet"] = None
         widget_args["set_default_on_init"] = None
-        widget_args["hide_default_widget"] = None
-        widget_args["default_widget_text"] = None
+        widget_args["hide_default_value_widget"] = None
+        widget_args["default_value_description"] = None
 
         param_widget_info = ParameterWidgetInfo(
             widget_class=widget_class, widget_args=widget_args
         )
 
         return param_widget_info
```

### Comparing `function2widgets-0.6.7/function2widgets/parser/parameter_parser.py` & `function2widgets-0.6.8/function2widgets/parser/parameter_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 import typing
 from typing import Optional, List, Any
 
 from function2widgets.common import parse_type_info
-from function2widgets.info import ParameterInfo, ParameterWidgetInfo
+from function2widgets.info import ParameterInfo
 
 TYPE_FOR_VARARGS = list.__name__
 TYPE_FOR_KWARGS = dict.__name__
 
 
 BASIC_TYPES = {
     int: "int",
```

### Comparing `function2widgets-0.6.7/function2widgets/parser/widgetconfigs_parser.py` & `function2widgets-0.6.8/function2widgets/parser/widgetconfigs_parser.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.7/function2widgets/widget.py` & `function2widgets-0.6.8/function2widgets/widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,70 +13,70 @@
 class WidgetArgs(object):
     parameter_name: str
     default: Any
     label: Optional[str]
     description: Optional[str]
     stylesheet: Optional[str]
     set_default_on_init: Optional[bool]
-    hide_default_widget: Optional[bool]
-    default_widget_text: Optional[str]
+    hide_default_value_widget: Optional[bool]
+    default_value_description: Optional[str]
 
     @classmethod
     def new(cls, kwargs: Dict[str, Any]) -> "WidgetArgs":
         return cls(**kwargs)
 
 
 class BaseParameterWidget(QWidget):
     """
     base class of all parameter widgets
     """
 
     SET_DEFAULT_ON_INIT: bool = True
-    HIDE_DEFAULT_WIDGET: bool = False
+    HIDE_DEFAULT_VALUE_WIDGET: bool = False
 
     _WidgetArgsClass = WidgetArgs
 
     def __init__(self, args: WidgetArgs, parent: Optional[QWidget]):
         super().__init__(parent)
 
         """
         Note:
         1. if 'set_default_on_init' is None, it will be set to class field SET_DEFAULT_ON_INIT
-        2. if 'hide_default_widget' is None, it will be set to class field HIDE_DEFAULT_WIDGET
-        3. 'set_default_on_init' will be set to True if 'default' is not None and 'hide_default_widget' is True
-        4. 'hide_default_widget' will be set to False if 'default' is None
+        2. if 'hide_default_value_widget' is None, it will be set to class field HIDE_DEFAULT_VALUE_WIDGET
+        3. 'set_default_on_init' will be set to True if 'default' is not None and 'hide_default_value_widget' is True
+        4. 'hide_value_default_widget' will be set to False if 'default' is None
         5. 'label' will be set to 'parameter_name', if it is set to None
         """
         # 1
         if args.set_default_on_init is None:
             set_default_on_init = self.__class__.SET_DEFAULT_ON_INIT
         else:
             set_default_on_init = args.set_default_on_init
         # 2
-        if args.hide_default_widget is None:
-            hide_default_widget = self.__class__.HIDE_DEFAULT_WIDGET
+        if args.hide_default_value_widget is None:
+            hide_default_value_widget = self.__class__.HIDE_DEFAULT_VALUE_WIDGET
         else:
-            hide_default_widget = args.hide_default_widget
+            hide_default_value_widget = args.hide_default_value_widget
         # 3
-        if args.default is not None and hide_default_widget is True:
+        if args.default is not None and hide_default_value_widget is True:
             set_default_on_init = True
         # 4
         if args.default is None:
-            hide_default_widget = False
+            hide_default_value_widget = False
         # 5
         if args.label is None:
             label = args.parameter_name
         else:
             label = args.label
 
         self.__args = dataclasses.replace(
             args,
             label=label,
             set_default_on_init=set_default_on_init,
-            hide_default_widget=hide_default_widget,
+            hide_default_value_widget=hide_default_value_widget,
         )
 
         if self.__args.stylesheet is not None:
             self.setStyleSheet(self.__args.stylesheet)
 
     @property
     def _args(self) -> WidgetArgs:
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/_sourcecodeedit.py` & `function2widgets-0.6.8/function2widgets/widgets/_sourcecodeedit.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.7/function2widgets/widgets/allwidgets.py` & `function2widgets-0.6.8/function2widgets/widgets/allwidgets.py`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.7/function2widgets/widgets/base.py` & `function2widgets-0.6.8/function2widgets/widgets/pathedit/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,199 +1,190 @@
-import abc
-import copy
 import dataclasses
-from typing import Any, Optional, cast
+import os.path
+from typing import Optional, cast, Any
 
-from PyQt6.QtCore import Qt
 from PyQt6.QtWidgets import (
     QWidget,
-    QLabel,
-    QCheckBox,
-    QVBoxLayout,
-    QFrame,
+    QLineEdit,
+    QPushButton,
+    QHBoxLayout,
+    QFileDialog,
+    QApplication,
 )
 
-from function2widgets.widget import BaseParameterWidget, WidgetArgs
+from function2widgets.widget import InvalidValueError
+from function2widgets.widgets.base import (
+    CommonParameterWidget,
+    CommonParameterWidgetArgs,
+)
 
+PATH_TYPE_OPEN_FILE = 0
+PATH_TYPE_OPEN_FILES = 1
+PATH_TYPE_OPEN_DIR = 2
+PATH_TYPE_SAVE_FILE = 3
+PATH_TYPE_SAVE_DIR = 4
 
-@dataclasses.dataclass(frozen=True)
-class CommonParameterWidgetArgs(WidgetArgs):
-    parameter_name: str
-    default: Any
-    label: Optional[str] = None
-    description: Optional[str] = None
-    stylesheet: Optional[str] = None
-    set_default_on_init: Optional[bool] = None
-    hide_default_widget: Optional[bool] = None
-    default_widget_text: Optional[str] = None
-    separate_line: bool = True
-
-
-class CommonParameterWidget(BaseParameterWidget):
-
-    _WidgetArgsClass = CommonParameterWidgetArgs
-
-    OBJ_ID_LAYOUT = "_CPW_main_layout"
-    OBJ_ID_CENTER_WIDGET = "_CPW_center_widget"
-    OBJ_ID_LABEL_WIDGET = "_CPW_label_widget"
-    OBJ_ID_DESCRIPTION_WIDGET = "_CPW_description_widget"
-    OBJ_ID_DEFAULT_WIDGET = "_CPW_default_widget"
-    OBJ_ID_SEPARATE_LINE = "_CPW_separate_line_widget"
+FILTER_ALL_FILES = QApplication.translate("PathEdit", "All Files (*)")
 
-    def __init__(self, args: CommonParameterWidgetArgs, parent: Optional[QWidget]):
+PATH_DELIMITER = ";"
 
-        super().__init__(args=args, parent=parent)
+BUTTON_TEXT = QApplication.translate("PathEdit", "Select")
 
-        self._layout = QVBoxLayout(self)
-        self._center_widget = QWidget(self)
-        self._label_widget = QLabel(self)
-        self._description_widget = QLabel(self)
-        self._default_widget = QCheckBox(self)
-
-        self._setup_label_widget()
-        self._setup_description_widget()
-        self._setup_default_widget()
-        self._setup_layout()
-        self.setup_center_widget(self._center_widget)
-        self.set_label(self._args.label)
-        self.set_description(self._args.description)
-
-    def set_value(self, value: Any):
-        value = copy.deepcopy(value)
-        if not self._pre_set_value(value):
-            return
-        self.set_value_to_widget(value)
 
-    def get_value(self) -> Any:
-        if self._is_use_default():
-            return self._args.default
-        return copy.deepcopy(self.get_value_from_widget())
+@dataclasses.dataclass(frozen=True)
+class PathEditArgs(CommonParameterWidgetArgs):
+    parameter_name: str
+    default: Optional[str] = ""
+    path_type: int = PATH_TYPE_OPEN_FILE
+    filters: str = FILTER_ALL_FILES
+    init_filter: Optional[str] = None
+    start_path: Optional[str] = None
+    path_delimiter: str = PATH_DELIMITER
+    button_text: str = BUTTON_TEXT
+    placeholder: str = ""
+    clear_button: bool = False
+    dialog_title: Optional[str] = None
+
+
+class PathEdit(CommonParameterWidget):
+    HIDE_DEFAULT_VALUE_WIDGET = True
+    SET_DEFAULT_ON_INIT = True
 
-    @abc.abstractmethod
-    def setup_center_widget(self, center_widget: QWidget):
-        pass
+    _WidgetArgsClass = PathEditArgs
 
-    @abc.abstractmethod
-    def set_value_to_widget(self, value: Any):
-        pass
+    def __init__(self, args: PathEditArgs, parent: Optional[QWidget] = None):
 
-    @abc.abstractmethod
-    def get_value_from_widget(self) -> Any:
-        pass
+        self._value_widget: Optional[QLineEdit] = None
+        self._select_button: Optional[QPushButton] = None
 
-    @property
-    def _args(self) -> CommonParameterWidgetArgs:
-        return cast(CommonParameterWidgetArgs, super()._args)
+        super().__init__(args=args, parent=parent)
 
-    def set_label(self, label: str):
-        if not label:
-            self._label_widget.setText("")
-            self._label_widget.hide()
-        else:
-            self._label_widget.setText(label)
-            self._label_widget.show()
+        if self._args.set_default_on_init:
+            self.set_value(self._args.default)
 
-    def get_label(self) -> str:
-        return self._label_widget.text()
+    @property
+    def _args(self) -> PathEditArgs:
+        return cast(PathEditArgs, super()._args)
 
-    def set_description(self, desc: str):
-        if not desc:
-            self._description_widget.setText("")
-            self._description_widget.hide()
-        else:
-            self._description_widget.setText(desc)
-            self._description_widget.show()
+    # noinspection PyUnresolvedReferences
+    def setup_center_widget(self, center_widget: QWidget):
+        self._value_widget = QLineEdit(center_widget)
 
-    def get_description(self) -> str:
-        return self._description_widget.text()
+        button_text = self._args.button_text or BUTTON_TEXT
+        self._select_button = QPushButton(button_text, center_widget)
 
-    def _setup_default_widget(self):
-        if self._args.default_widget_text is None:
-            text = "{}"
-        else:
-            text = self._args.default_widget_text
-        self._default_widget.setText(text.format(self._args.default))
-        # noinspection PyUnresolvedReferences
-        self._default_widget.toggled.connect(self._on_default_widget_state_changed)
-        self._default_widget.setHidden(self._args.hide_default_widget)
-
-    def _setup_label_widget(self):
-        self._label_widget.setWordWrap(True)
-        self._label_widget.setAlignment(
-            Qt.AlignmentFlag.AlignLeading
-            | Qt.AlignmentFlag.AlignLeft
-            | Qt.AlignmentFlag.AlignTop
-        )
+        center_widget_layout = QHBoxLayout(center_widget)
+        center_widget_layout.setContentsMargins(0, 0, 0, 0)
+        center_widget.setLayout(center_widget_layout)
 
-    def _setup_description_widget(self):
-        self._description_widget.setWordWrap(True)
-        self._description_widget.setAlignment(
-            Qt.AlignmentFlag.AlignLeading
-            | Qt.AlignmentFlag.AlignLeft
-            | Qt.AlignmentFlag.AlignTop
-        )
+        placeholder = self._args.placeholder or ""
+        clear_button = self._args.clear_button is True
 
-    def _on_default_widget_state_changed(self, checked: bool):
-        if self._args.hide_default_widget:
-            return
-        self._center_widget.setEnabled(not checked)
+        self._value_widget.setPlaceholderText(placeholder)
+        self._value_widget.setClearButtonEnabled(clear_button)
 
-    def _setup_layout(self):
-        cls = self.__class__
-        self.setLayout(self._layout)
-
-        self._layout.setObjectName(cls.OBJ_ID_LAYOUT)
-        self._label_widget.setObjectName(cls.OBJ_ID_LABEL_WIDGET)
-        self._description_widget.setObjectName(cls.OBJ_ID_DESCRIPTION_WIDGET)
-        self._center_widget.setObjectName(cls.OBJ_ID_CENTER_WIDGET)
-        self._default_widget.setObjectName(cls.OBJ_ID_DEFAULT_WIDGET)
-
-        self._layout.setContentsMargins(0, 0, 0, 0)
-        self._layout.addWidget(self._label_widget)
-        self._layout.addWidget(self._center_widget)
-        self._layout.addWidget(self._default_widget)
-        self._layout.addWidget(self._description_widget)
-        if self._args.separate_line:
-            line = self._create_separate_line()
-            self._layout.addWidget(line)
-        # spacer = QSpacerItem(
-        #     0, 0, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding
-        # )
-        # self._layout.addSpacerItem(spacer)
-
-    def _is_use_default(self) -> bool:
-        if self._args.hide_default_widget or self._default_widget.isHidden():
-            return False
-        return self._default_widget.isChecked()
+        self._select_button.clicked.connect(self._select_path)
+        center_widget_layout.addWidget(self._value_widget)
+        center_widget_layout.addWidget(self._select_button)
+        center_widget_layout.setStretch(0, 8)
+        center_widget_layout.setStretch(1, 2)
 
-    def _use_default(self):
-        if self._args.hide_default_widget or self._default_widget.isHidden():
-            return
-        self._default_widget.setChecked(True)
+    def get_value(self) -> Optional[str]:
+        return super().get_value()
 
-    def _unuse_default(self):
-        if self._args.hide_default_widget or self._default_widget.isHidden():
-            return
-        self._default_widget.setChecked(False)
+    def set_value(self, value: Optional[str]):
+        if value is not None and not isinstance(value, str):
+            raise InvalidValueError(f"value must be str, not {type(value)}")
+        super().set_value(value)
+
+    def set_value_to_widget(self, value: str):
+        self._value_widget.setText(value)
 
-    def _pre_set_value(self, value: Any) -> bool:
-        if value is None and self._args.default is not None:
-            raise ValueError(
-                f"value cannot be None unless the default value is set to None(default={self.default})"
-            )
-
-        if value is None and self._args.default is None:
-            self._use_default()
-            return False
+    def get_value_from_widget(self) -> Any:
+        return self._value_widget.text()
 
-        if value == self._args.default:
-            self._use_default()
+    def _select_path(self):
+        path_type = self._args.path_type
+        if path_type == PATH_TYPE_OPEN_FILE:
+            path = self._get_open_file_path()
+        elif path_type == PATH_TYPE_OPEN_FILES:
+            path = self._get_open_files_path()
+        elif path_type == PATH_TYPE_OPEN_DIR:
+            path = self._get_open_dir_path()
+        elif path_type == PATH_TYPE_SAVE_FILE:
+            path = self._get_save_file_path()
+        elif path_type == PATH_TYPE_SAVE_DIR:
+            path = self._get_save_dir_path()
         else:
-            self._unuse_default()
-        return True
+            path = None
+        if not path:
+            return
+        self.set_value(path)
 
-    def _create_separate_line(self) -> QFrame:
-        separate_line = QFrame(self)
-        separate_line.setObjectName(self.__class__.OBJ_ID_SEPARATE_LINE)
-        separate_line.setFrameShape(QFrame.Shape.HLine)
-        separate_line.setFrameShadow(QFrame.Shadow.Sunken)
-        return separate_line
+    def _get_open_file_path(self) -> str:
+        dialog_title = self._args.dialog_title
+        start_path = self._args.start_path
+        filters = self._args.filters
+        init_filter = self._args.init_filter
+
+        path, _ = QFileDialog.getOpenFileName(
+            caption=dialog_title,
+            directory=start_path,
+            filter=filters,
+            initialFilter=init_filter,
+        )
+        if not path:
+            return ""
+        return os.path.abspath(path)
+
+    def _get_save_file_path(self) -> Optional[str]:
+        dialog_title = self._args.dialog_title
+        start_path = self._args.start_path
+        filters = self._args.filters
+        init_filter = self._args.init_filter
+
+        path, _ = QFileDialog.getSaveFileName(
+            caption=dialog_title,
+            directory=start_path,
+            filter=filters,
+            initialFilter=init_filter,
+        )
+        if not path:
+            return None
+        return os.path.abspath(path)
+
+    def _get_open_dir_path(self) -> Optional[str]:
+        dialog_title = self._args.dialog_title
+        start_path = self._args.start_path
+        path = QFileDialog.getExistingDirectory(
+            caption=dialog_title, directory=start_path
+        )
+        if not path:
+            return None
+        return os.path.abspath(path)
+
+    def _get_open_files_path(self) -> Optional[str]:
+        dialog_title = self._args.dialog_title
+        start_path = self._args.start_path
+        filters = self._args.filters
+        init_filter = self._args.init_filter
+        path_delimiter = self._args.path_delimiter or PATH_DELIMITER
+
+        paths, _ = QFileDialog.getOpenFileNames(
+            caption=dialog_title,
+            directory=start_path,
+            filter=filters,
+            initialFilter=init_filter,
+        )
+        if not paths:
+            return None
+        return path_delimiter.join((os.path.abspath(path) for path in paths))
+
+    def _get_save_dir_path(self) -> Optional[str]:
+        dialog_title = self._args.dialog_title
+        start_path = self._args.start_path
+        path = QFileDialog.getExistingDirectory(
+            caption=dialog_title, directory=start_path
+        )
+        if not path:
+            return None
+        return os.path.abspath(path)
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/editor/base.py` & `function2widgets-0.6.8/function2widgets/widgets/editor/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     button_text: str = BUTTON_TEXT
     window_title: str = ""
     display_current_value: bool = True
     display_widget_text: str = DISPLAY_WIDGET_TEXT
 
 
 class BaseCodeEditor(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = BaseCodeEditorArgs
 
     def __init__(self, args: BaseCodeEditorArgs, parent: Optional[QWidget] = None):
 
         self._value_widget: Optional[QPushButton] = None
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/editor/codeeditor.py` & `function2widgets-0.6.8/function2widgets/widgets/editor/codeeditor.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class CodeEditorArgs(BaseCodeEditorArgs):
     parameter_name: str
     default: Optional[str] = ""
     configs: dict = dataclasses.field(default_factory=dict)
 
 
 class CodeEditor(BaseCodeEditor):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = CodeEditorArgs
 
     def __init__(self, args: CodeEditorArgs, parent: Optional[QWidget] = None):
         if args.default is not None and not isinstance(args.default, str):
             raise ValueError("default must be str, got {type(default)}")
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/editor/dicteditor.py` & `function2widgets-0.6.8/function2widgets/widgets/editor/dicteditor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import Optional, cast, Any
+from typing import Optional, cast
 
 from PyQt6.QtWidgets import QWidget
 
 from function2widgets.widgets._sourcecodeedit import DEFAULT_CONFIGS
 from .jsoneditor import _NoneType, JsonEditor, JsonEditorArgs
 
 
@@ -11,15 +11,15 @@
 class DictEditorArgs(JsonEditorArgs):
     parameter_name: str
     default: Optional[dict] = dataclasses.field(default_factory=dict)
     configs: dict = dataclasses.field(default_factory=DEFAULT_CONFIGS.copy)
 
 
 class DictEditor(JsonEditor):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     TYPE_RESTRICTIONS = (dict, _NoneType)
 
     _WidgetArgsClass = DictEditorArgs
 
     @property
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/editor/jsoneditor.py` & `function2widgets-0.6.8/function2widgets/widgets/editor/jsoneditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     parameter_name: str
     default: Any = ""
     configs: dict = dataclasses.field(default_factory=DEFAULT_CONFIGS.copy)
     top_level_types: tuple = JsonTopLevelTypes
 
 
 class JsonEditor(BaseCodeEditor):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = JsonEditorArgs
 
     def __init__(self, args: JsonEditorArgs, parent: Optional[QWidget] = None):
         configs = args.configs
         if not isinstance(configs, dict):
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/editor/listeditor.py` & `function2widgets-0.6.8/function2widgets/widgets/editor/listeditor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import Optional, cast, Any
+from typing import Optional, cast
 
 from PyQt6.QtWidgets import QWidget
 
 from function2widgets.widgets._sourcecodeedit import DEFAULT_CONFIGS
 from .jsoneditor import JsonEditorArgs, JsonEditor, _NoneType
 
 
@@ -11,15 +11,15 @@
 class ListEditorArgs(JsonEditorArgs):
     parameter_name: str
     default: Optional[list] = dataclasses.field(default_factory=list)
     configs: dict = dataclasses.field(default_factory=DEFAULT_CONFIGS.copy)
 
 
 class ListEditor(JsonEditor):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = ListEditorArgs
 
     TYPE_RESTRICTIONS = (list, _NoneType)
 
     @property
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/editor/tupleeditor.py` & `function2widgets-0.6.8/function2widgets/widgets/editor/tupleeditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class TupleEditorArgs(JsonEditorArgs):
     parameter_name: str
     default: Optional[tuple] = dataclasses.field(default_factory=tuple)
     configs: dict = dataclasses.field(default_factory=DEFAULT_CONFIGS.copy)
 
 
 class TupleEditor(JsonEditor):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = TupleEditorArgs
 
     TYPE_RESTRICTIONS = (list, set, tuple, _NoneType)
 
     def __init__(self, args: TupleEditorArgs, parent: Optional[QWidget] = None):
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/lineedit/floatedit.py` & `function2widgets-0.6.8/function2widgets/widgets/lineedit/floatedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     max_value: Optional[float] = None
     min_value: Optional[float] = None
     decimals: Optional[float] = None
     scientific_notation: bool = False
 
 
 class FloatLineEdit(LineEdit):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = FloatLineEditArgs
 
     def __init__(self, args: FloatLineEditArgs, parent: Optional[QWidget] = None):
         super().__init__(args=args, parent=parent)
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/lineedit/intedit.py` & `function2widgets-0.6.8/function2widgets/widgets/lineedit/intedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     parameter_name: str
     default: Optional[int] = 0
     max_value: Optional[int] = None
     min_value: Optional[int] = None
 
 
 class IntLineEdit(LineEdit):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = IntLineEditArgs
 
     def __init__(self, args: IntLineEditArgs, parent: Optional[QWidget] = None):
         super().__init__(args=args, parent=parent)
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/lineedit/stredit.py` & `function2widgets-0.6.8/function2widgets/widgets/lineedit/stredit.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     echo_mode: Literal["Normal", "Password", "NoEcho", "PasswordEchoOnEdit"] = "Normal"
     regex: Optional[str] = None
     input_mask: Optional[str] = None
 
 
 class LineEdit(CommonParameterWidget):
     SET_DEFAULT_ON_INIT = True
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
 
     _WidgetArgsClass = LineEditArgs
 
     def __init__(self, args: LineEditArgs, parent: Optional[QWidget] = None):
         self._value_widget: QLineEdit = QLineEdit()
 
         super().__init__(args=args, parent=parent)
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/misc/dateedit.py` & `function2widgets-0.6.8/function2widgets/widgets/misc/dateedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     min_date: Union[date, QDate, str, None] = None
     max_date: Union[date, QDate, str, None] = None
     calendar_popup: bool = False
     time_spec: str = DEFAULT_TIME_SPEC
 
 
 class DateEdit(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = DateEditArgs
 
     def __init__(self, args: DateEditArgs, parent: Optional[QWidget] = None):
         self._value_widget: Optional[QDateEdit] = None
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/misc/datetimeedit.py` & `function2widgets-0.6.8/function2widgets/widgets/misc/datetimeedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     max_datetime: Union[datetime, QDateTime, str, None] = None
     display_format: str = DEFAULT_DISPLAY_FORMAT
     calendar_popup: bool = False
     time_spec: str = DEFAULT_TIME_SPEC
 
 
 class DateTimeEdit(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = DateTimeEditArgs
 
     def __init__(self, args: DateTimeEditArgs, parent: Optional[QWidget] = None):
         self._value_widget: Optional[QDateTimeEdit] = None
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/misc/timeedit.py` & `function2widgets-0.6.8/function2widgets/widgets/misc/timeedit.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     display_format: str = DEFAULT_DISPLAY_FORMAT
     min_time: Union[time, QTime, str, None] = None
     max_time: Union[time, QTime, str, None] = None
     time_spec: str = DEFAULT_TIME_SPEC
 
 
 class TimeEdit(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = TimeEditArgs
 
     def __init__(self, args: TimeEditArgs, parent: Optional[QWidget] = None):
         self._value_widget: Optional[QTimeEdit] = None
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/numberinput/dial.py` & `function2widgets-0.6.8/function2widgets/widgets/numberinput/dial.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     inverted_control: bool = False
     show_value_label: bool = False
     value_prefix: str = None
     value_suffix: str = None
 
 
 class Dial(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = DialArgs
 
     def __init__(self, args: DialArgs, parent: Optional[QWidget] = None):
 
         if args.step is not None and args.step <= 0:
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/numberinput/floatspin.py` & `function2widgets-0.6.8/function2widgets/widgets/numberinput/floatspin.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     decimals: int = None
     prefix: str = None
     suffix: str = None
     accelerated: bool = False
 
 
 class FloatSpinBox(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = FloatSpinBoxArgs
 
     def __init__(self, args: FloatSpinBoxArgs, parent: Optional[QWidget] = None):
 
         if args.step is not None and args.step <= 0:
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/numberinput/intspin.py` & `function2widgets-0.6.8/function2widgets/widgets/numberinput/intspin.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     max_value: Optional[int] = None
     step: Optional[int] = None
     prefix: Optional[str] = None
     suffix: Optional[str] = None
 
 
 class IntSpinBox(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = IntSpinBoxArgs
 
     def __init__(self, args: IntSpinBoxArgs, parent: Optional[QWidget] = None):
 
         if args.step is not None and args.step <= 0:
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/numberinput/slider.py` & `function2widgets-0.6.8/function2widgets/widgets/numberinput/slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     inverted_control: bool = False
     show_value_label: bool = False
     value_prefix: Optional[str] = None
     value_suffix: Optional[str] = None
 
 
 class Slider(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = SliderArgs
 
     def __init__(self, args: SliderArgs, parent: Optional[QWidget] = None):
 
         if args.step is not None and args.step <= 0:
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/pathedit/dirpathedit.py` & `function2widgets-0.6.8/function2widgets/widgets/pathedit/dirpathedit.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class DirPathEditArgs(PathEditArgs):
     parameter_name: str
     default: Optional[str] = ""
     save_dir: bool = False
 
 
 class DirPathEdit(PathEdit):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = DirPathEditArgs
 
     def __init__(self, args: DirPathEditArgs, parent: Optional[QWidget] = None):
         if args.save_dir:
             path_type = PATH_TYPE_SAVE_DIR
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/pathedit/filepathedit.py` & `function2widgets-0.6.8/function2widgets/widgets/pathedit/filepathedit.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     parameter_name: str
     default: Optional[str] = ""
     save_file: bool = False
     multiple_files: bool = False
 
 
 class FilePathEdit(PathEdit):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = FilePathEditArgs
 
     @property
     def _args(self) -> FilePathEditArgs:
         return cast(FilePathEditArgs, super()._args)
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/selectwidget/checkbox.py` & `function2widgets-0.6.8/function2widgets/widgets/selectwidget/checkbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import Optional, cast, Any
+from typing import Optional, cast
 
 from PyQt6.QtWidgets import QWidget, QCheckBox, QApplication, QVBoxLayout
 
 from function2widgets.widgets.base import (
     CommonParameterWidget,
     CommonParameterWidgetArgs,
 )
@@ -16,15 +16,15 @@
     parameter_name: str
     default: Optional[bool] = False
     text: str = DEFAULT_TEXT
 
 
 class CheckBox(CommonParameterWidget):
     SET_DEFAULT_ON_INIT = True
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
 
     _WidgetArgsClass = CheckBoxArgs
 
     def __init__(self, args: CheckBoxArgs, parent: Optional[QWidget] = None):
         self._checkbox: Optional[QCheckBox] = None
 
         super().__init__(args=args, parent=parent)
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/selectwidget/checkbox_group.py` & `function2widgets-0.6.8/function2widgets/widgets/selectwidget/checkbox_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     default: Optional[List[str]] = dataclasses.field(default_factory=list)
     items: List[str] = None
     column_count: int = 1
 
 
 class CheckBoxGroup(CommonParameterWidget):
     SET_DEFAULT_ON_INIT = True
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
 
     _WidgetArgsClass = CheckBoxGroupArgs
 
     def __init__(self, args: CheckBoxGroupArgs, parent: Optional[QWidget] = None):
 
         if args.column_count < 1:
             raise ValueError(f"column_count must be greater than 0")
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/selectwidget/combobox.py` & `function2widgets-0.6.8/function2widgets/widgets/selectwidget/combobox.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class ComboBoxArgs(CommonParameterWidgetArgs):
     parameter_name: str
     default: Optional[str] = None
     items: List[Union[str, Tuple[str, Any]]] = None
 
 
 class ComboBox(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = ComboBoxArgs
 
     def __init__(self, args: ComboBoxArgs, parent: Optional[QWidget] = None):
         if not args.items:
             raise ValueError(f"items must be specified")
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/selectwidget/combobox_edit.py` & `function2widgets-0.6.8/function2widgets/widgets/selectwidget/combobox_edit.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class ComboBoxEditArgs(CommonParameterWidgetArgs):
     parameter_name: str
     default: Optional[str] = None
     items: List[str] = dataclasses.field(default_factory=list)
 
 
 class ComboBoxEdit(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = ComboBoxEditArgs
 
     def __init__(self, args: ComboBoxEditArgs, parent: Optional[QWidget] = None):
         if args.items is None:
             raise ValueError(f"items must be specified")
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/selectwidget/radiobutton_group.py` & `function2widgets-0.6.8/function2widgets/widgets/selectwidget/radiobutton_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     parameter_name: str
     default: Optional[List[str]] = CLEAR_ALL
     items: List[str] = None
     column_count: int = 1
 
 
 class RadioButtonGroup(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = RadioButtonGroupArgs
 
     _BTN_PREFIX = "_radio_button_"
 
     def __init__(self, args: RadioButtonGroupArgs, parent: Optional[QWidget] = None):
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/textedit/codeedit.py` & `function2widgets-0.6.8/function2widgets/widgets/textedit/codeedit.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class CodeEditArgs(CommonParameterWidgetArgs):
     parameter_name: str
     default: Optional[str] = ""
     configs: Optional[Dict[str, Any]] = None
 
 
 class CodeEdit(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = CodeEditArgs
 
     def __init__(self, args: CodeEditArgs, parent: Optional[QWidget] = None):
 
         self._value_widget: Optional[_SourceCodeEdit] = None
```

### Comparing `function2widgets-0.6.7/function2widgets/widgets/textedit/plaintext.py` & `function2widgets-0.6.8/function2widgets/widgets/textedit/plaintext.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     placeholder: Optional[str] = None
     readonly: bool = False
     overwrite_mode: bool = False
     line_wrap_mode: bool = False
 
 
 class PlainTextEdit(CommonParameterWidget):
-    HIDE_DEFAULT_WIDGET = True
+    HIDE_DEFAULT_VALUE_WIDGET = True
     SET_DEFAULT_ON_INIT = True
 
     _WidgetArgsClass = PlainTextEditArgs
 
     def __init__(self, args: PlainTextEditArgs, parent: Optional[QWidget] = None):
         self._value_widget: Optional[QPlainTextEdit] = None
```

### Comparing `function2widgets-0.6.7/License` & `function2widgets-0.6.8/License`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.7/pyproject.toml` & `function2widgets-0.6.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "function2widgets"
-version = "0.6.7"
+version = "0.6.8"
 description = ""
 authors = ["zimolab <zimolab@aliyun.com>"]
 readme = "README.md"
 license = "GPL-3.0"
 packages = [
     {include="function2widgets"}
 ]
```

### Comparing `function2widgets-0.6.7/README.md` & `function2widgets-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `function2widgets-0.6.7/PKG-INFO` & `function2widgets-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function2widgets
-Version: 0.6.7
+Version: 0.6.8
 Summary: 
 Home-page: https://github.com/zimolab/function2widgets
 License: GPL-3.0
 Author: zimolab
 Author-email: zimolab@aliyun.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

