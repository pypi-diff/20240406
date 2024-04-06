# Comparing `tmp/gcp-scraper-3.6.6.tar.gz` & `tmp/gcp-scraper-3.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-scraper-3.6.6.tar", last modified: Sat Mar 23 03:18:21 2024, max compression
+gzip compressed data, was "gcp-scraper-3.6.7.tar", last modified: Sat Apr  6 13:57:23 2024, max compression
```

## Comparing `gcp-scraper-3.6.6.tar` & `gcp-scraper-3.6.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-03-23 03:18:21.499762 gcp-scraper-3.6.6/
--rw-r--r--   0 cuz        (501) staff       (20)    35149 2023-08-11 13:24:50.000000 gcp-scraper-3.6.6/LICENSE
--rw-r--r--   0 cuz        (501) staff       (20)      679 2024-03-23 03:18:21.499644 gcp-scraper-3.6.6/PKG-INFO
--rw-r--r--   0 cuz        (501) staff       (20)       45 2023-08-11 13:24:50.000000 gcp-scraper-3.6.6/README.md
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-03-23 03:18:21.499074 gcp-scraper-3.6.6/gcp_scraper.egg-info/
--rw-r--r--   0 cuz        (501) staff       (20)      679 2024-03-23 03:18:21.000000 gcp-scraper-3.6.6/gcp_scraper.egg-info/PKG-INFO
--rw-r--r--   0 cuz        (501) staff       (20)      497 2024-03-23 03:18:21.000000 gcp-scraper-3.6.6/gcp_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 cuz        (501) staff       (20)        1 2024-03-23 03:18:21.000000 gcp-scraper-3.6.6/gcp_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 cuz        (501) staff       (20)      198 2024-03-23 03:18:21.000000 gcp-scraper-3.6.6/gcp_scraper.egg-info/requires.txt
--rw-r--r--   0 cuz        (501) staff       (20)        9 2024-03-23 03:18:21.000000 gcp-scraper-3.6.6/gcp_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-03-23 03:18:21.489324 gcp-scraper-3.6.6/gscraper/
--rwxr-xr-x   0 cuz        (501) staff       (20)      284 2024-03-23 03:17:46.000000 gcp-scraper-3.6.6/gscraper/__init__.py
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-03-23 03:18:21.495015 gcp-scraper-3.6.6/gscraper/base/
--rwxr-xr-x   0 cuz        (501) staff       (20)        0 2023-10-27 05:39:56.000000 gcp-scraper-3.6.6/gscraper/base/__init__.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    22682 2024-03-05 11:20:04.000000 gcp-scraper-3.6.6/gscraper/base/abstract.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    38640 2024-03-23 03:16:24.000000 gcp-scraper-3.6.6/gscraper/base/gcloud.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    90439 2024-03-03 08:04:36.000000 gcp-scraper-3.6.6/gscraper/base/session.py
--rwxr-xr-x   0 cuz        (501) staff       (20)   112009 2024-03-23 03:05:51.000000 gcp-scraper-3.6.6/gscraper/base/spider.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    19122 2024-02-24 02:49:32.000000 gcp-scraper-3.6.6/gscraper/base/types.py
-drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-03-23 03:18:21.498065 gcp-scraper-3.6.6/gscraper/utils/
--rwxr-xr-x   0 cuz        (501) staff       (20)      962 2023-12-05 12:25:11.000000 gcp-scraper-3.6.6/gscraper/utils/__init__.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    11477 2023-11-14 08:57:20.000000 gcp-scraper-3.6.6/gscraper/utils/cast.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    16069 2024-02-24 02:47:12.000000 gcp-scraper-3.6.6/gscraper/utils/date.py
--rwxr-xr-x   0 cuz        (501) staff       (20)     8113 2023-11-08 14:08:25.000000 gcp-scraper-3.6.6/gscraper/utils/logs.py
--rwxr-xr-x   0 cuz        (501) staff       (20)    69526 2024-03-23 03:17:26.000000 gcp-scraper-3.6.6/gscraper/utils/map.py
--rw-r--r--   0 cuz        (501) staff       (20)       38 2024-03-23 03:18:21.500226 gcp-scraper-3.6.6/setup.cfg
--rw-r--r--   0 cuz        (501) staff       (20)      764 2023-09-10 13:21:42.000000 gcp-scraper-3.6.6/setup.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.441382 gcp-scraper-3.6.7/
+-rw-r--r--   0 cuz        (501) staff       (20)    35149 2023-08-11 13:24:50.000000 gcp-scraper-3.6.7/LICENSE
+-rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-06 13:57:23.441110 gcp-scraper-3.6.7/PKG-INFO
+-rw-r--r--   0 cuz        (501) staff       (20)       45 2023-08-11 13:24:50.000000 gcp-scraper-3.6.7/README.md
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.440258 gcp-scraper-3.6.7/gcp_scraper.egg-info/
+-rw-r--r--   0 cuz        (501) staff       (20)      679 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 cuz        (501) staff       (20)      497 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 cuz        (501) staff       (20)        1 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 cuz        (501) staff       (20)      198 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/requires.txt
+-rw-r--r--   0 cuz        (501) staff       (20)        9 2024-04-06 13:57:23.000000 gcp-scraper-3.6.7/gcp_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.428288 gcp-scraper-3.6.7/gscraper/
+-rwxr-xr-x   0 cuz        (501) staff       (20)      284 2024-04-06 13:56:55.000000 gcp-scraper-3.6.7/gscraper/__init__.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.434515 gcp-scraper-3.6.7/gscraper/base/
+-rwxr-xr-x   0 cuz        (501) staff       (20)        0 2023-10-27 05:39:56.000000 gcp-scraper-3.6.7/gscraper/base/__init__.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    22802 2024-04-06 13:49:06.000000 gcp-scraper-3.6.7/gscraper/base/abstract.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    38670 2024-03-23 03:20:34.000000 gcp-scraper-3.6.7/gscraper/base/gcloud.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    91060 2024-04-06 13:51:19.000000 gcp-scraper-3.6.7/gscraper/base/session.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)   113809 2024-04-06 13:56:10.000000 gcp-scraper-3.6.7/gscraper/base/spider.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    19111 2024-03-23 03:20:19.000000 gcp-scraper-3.6.7/gscraper/base/types.py
+drwxr-xr-x   0 cuz        (501) staff       (20)        0 2024-04-06 13:57:23.438537 gcp-scraper-3.6.7/gscraper/utils/
+-rwxr-xr-x   0 cuz        (501) staff       (20)      962 2023-12-05 12:25:11.000000 gcp-scraper-3.6.7/gscraper/utils/__init__.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    11448 2024-03-30 10:37:57.000000 gcp-scraper-3.6.7/gscraper/utils/cast.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    16069 2024-02-24 02:47:12.000000 gcp-scraper-3.6.7/gscraper/utils/date.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)     8113 2023-11-08 14:08:25.000000 gcp-scraper-3.6.7/gscraper/utils/logs.py
+-rwxr-xr-x   0 cuz        (501) staff       (20)    69526 2024-03-23 03:17:26.000000 gcp-scraper-3.6.7/gscraper/utils/map.py
+-rw-r--r--   0 cuz        (501) staff       (20)       38 2024-04-06 13:57:23.442271 gcp-scraper-3.6.7/setup.cfg
+-rw-r--r--   0 cuz        (501) staff       (20)      764 2023-09-10 13:21:42.000000 gcp-scraper-3.6.7/setup.py
```

### Comparing `gcp-scraper-3.6.6/LICENSE` & `gcp-scraper-3.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.6/PKG-INFO` & `gcp-scraper-3.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-scraper
-Version: 3.6.6
+Version: 3.6.7
 Summary: Scraping utils with GCP functions
 Home-page: https://github.com/minyeamer/gscraper.git
 Author: minyeamer
 Author-email: minyeamer@gmail.com
 License: minyeamer
 Keywords: gcp-scraper,scraper,gcp
 Requires-Python: >=3.7
```

### Comparing `gcp-scraper-3.6.6/gcp_scraper.egg-info/PKG-INFO` & `gcp-scraper-3.6.7/gcp_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-scraper
-Version: 3.6.6
+Version: 3.6.7
 Summary: Scraping utils with GCP functions
 Home-page: https://github.com/minyeamer/gscraper.git
 Author: minyeamer
 Author-email: minyeamer@gmail.com
 License: minyeamer
 Keywords: gcp-scraper,scraper,gcp
 Requires-Python: >=3.7
```

### Comparing `gcp-scraper-3.6.6/gscraper/base/abstract.py` & `gcp-scraper-3.6.7/gscraper/base/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ############################# Context #############################
 ###################################################################
 
 BASE_CONTEXT = lambda self=None, operation=None, info=None, initTime=None, prefix=None, rename=None, \
                         inplace=None, self_var=None, update=None, **context: context
 
 
-LOG_CONTEXT = lambda logger=None, logJson=None, errors=None, func=None, **context: context
+LOG_CONTEXT = lambda logger=None, logJson=None, interruptType=None, errorType=None, errors=None, func=None, **context: context
 
 
 ITERATOR_CONTEXT = lambda iterator=None, iterateArgs=None, iterateCount=None, iterateProduct=None, pagination=None, \
                         pageFrom=None, offsetFrom=None, pageUnit=None, pageLimit=None, fromNow=None, __i=None, \
                         **context: context
 
 
@@ -50,15 +50,15 @@
 ENCRYPTED_CONTEXT = lambda decryptedKey=None, auth=None, authKey=None, sessionCookies=None, **context: context
 
 
 UNIQUE_CONTEXT = lambda derivFields=None, dags=None, **context: \
     ENCRYPTED_CONTEXT(**SPIDER_CONTEXT(**MAP_CONTEXT(**ITERATOR_CONTEXT(**LOG_CONTEXT(**BASE_CONTEXT(**context))))))
 
 
-PARAMS_CONTEXT = lambda init=None, data=None, task=None, worker=None, locals=None, which=None, where=None, by=None, \
+PARAMS_CONTEXT = lambda init=None, data=None, task=None, worker=None, locals=None, which=None, where=None, by=None, verb=None, \
                         how=None, default=None, dropna=None, strict=None, unique=None, drop=None, index=None, log=None, \
                         depth=None, hier=None, to=None, countPath=None, hasSize=None, **context: context
 
 
 REQUEST_CONTEXT = lambda session=None, semaphore=None, method=None, url=None, referer=None, messages=None, \
                         params=None, encode=None, data=None, json=None, headers=None, cookies=None, \
                         allow_redirects=None, validate=None, exception=None, valid=None, invalid=None, \
@@ -423,26 +423,27 @@
 
 ###################################################################
 ########################### Spider Query ##########################
 ###################################################################
 
 ITERATOR_QUERY = lambda: Query(
     Variable(name="iterateUnit", type="INTEGER", iterable=False, default=None),
-    Variable(name="interval", type="STRING", iterable=False, default=str()),
+    Variable(name="interval", type="STRING", iterable=False, default=None),
 )
 
 TASK_QUERY = lambda: Query(
     Variable(name="fromNow", type="INTEGER", iterable=True, default=None),
     Variable(name="discard", type="BOOLEAN", iterable=False, default=True),
     Variable(name="progress", type="BOOLEAN", iterable=False, default=True),
 )
 
 GATHER_QUERY = lambda: Query(
     Variable(name="where", type="STRING", iterable=False, default=str()),
     Variable(name="which", type="STRING", iterable=False, default=str()),
+    Variable(name="verb", type="STRING", iterable=False, default=str()),
     Variable(name="by", type="STRING", iterable=False, default=str()),
     Variable(name="message", type="STRING", iterable=False, default=str()),
 )
 
 SPIDER_QUERY = lambda: Query(
     *SESSION_QUERY(),
     *TASK_QUERY(),
```

### Comparing `gcp-scraper-3.6.6/gscraper/base/gcloud.py` & `gcp-scraper-3.6.7/gscraper/base/gcloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 from gscraper.base.abstract import OptionalDict, TypedRecords, Value, ValueSet, GCLOUD_CONTEXT, INVALID_OBJECT_MSG, INVALID_OBJECT_TYPE_MSG
 from gscraper.base.session import BaseSession
 
 from gscraper.base.types import _KT, Context, TypeHint, IndexLabel, RenameMap
-from gscraper.base.types import TabularData, Account, PostData, from_literal
+from gscraper.base.types import TabularData, PostData, from_literal
 
 from gscraper.utils.cast import cast_list, cast_datetime_format
 from gscraper.utils.date import get_datetime, get_date, DATE_UNIT
 from gscraper.utils.logs import log_table
 from gscraper.utils.map import isna, df_empty, to_array, kloc, to_dict, to_records, read_excel
 from gscraper.utils.map import cloc, to_dataframe, convert_data, rename_data, filter_data, apply_data
 
@@ -32,14 +32,16 @@
 from typing import Any, Dict, Iterable, List, Literal, Optional, Sequence, Union
 import datetime as dt
 import json
 import re
 import pandas as pd
 
 
+Account = Union[Dict[str,str], str]
+
 ENV_PATH = "env/"
 GCLOUD_ACCOUNT = ENV_PATH+"gcloud.json"
 GCLOUD_DATA = ENV_PATH+"data.json"
 
 NAME = "name"
 KEY, SHEET, FIELDS = "key", "sheet", "fields"
 TABLE, QUERY, PID = "table", "query", "project_id"
```

### Comparing `gcp-scraper-3.6.6/gscraper/base/session.py` & `gcp-scraper-3.6.7/gscraper/base/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,14 +93,23 @@
 _NAME_SUFFIX = lambda name: f"_{name}" if name else str()
 SUFFIX = lambda context, field=dict(), name=str(): \
     _SCHEMA_SUFFIX(context) + _FIELD_SUFFIX(field) + _NAME_SUFFIX(name) + ITER_SUFFIX(context) + _COUNT_SUFFIX(context)
 
 TZINFO = None
 START, END = 0, 1
 
+class UserInterrupt(Exception):
+    ...
+
+class ForbiddenError(ValueError):
+    ...
+
+class ParseError(ValueError):
+    ...
+
 
 ###################################################################
 ############################# Messages ############################
 ###################################################################
 
 USER_INTERRUPT_MSG = lambda where: f"Interrupt occurred on {where} by user."
 
@@ -459,14 +468,16 @@
 class BaseSession(CustomDict):
     __metaclass__ = ABCMeta
     operation = "session"
     tzinfo = TZINFO
     datetimeUnit = "second"
     numRetries = 0
     delay = 1.
+    interruptType = tuple()
+    errorType = tuple()
     errors = list()
     info = Info()
 
     def __init__(self, tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., **context):
@@ -591,19 +602,20 @@
         if self.debug and self._isin_log_list(point, self.debug):
             self.logger.warning(dict(point=f"({point})", **dumps_data(msg, limit=0)))
         if self.extraSave and self._isin_log_list(point, self.extraSave) and notna(save):
             save, ext = self._validate_extension(save, ext)
             self._validate_dir(CHECKPOINT_PATH)
             self.save_data(save, prefix=CHECKPOINT_PATH+str(point).replace('.','_'), ext=ext)
         if self.interrupt and self._isin_log_list(point, self.interrupt):
-            raise KeyboardInterrupt(USER_INTERRUPT_MSG(where))
+            raise UserInterrupt(USER_INTERRUPT_MSG(where))
 
-    def save_data(self, data: Data, prefix=str(), ext: Optional[TypeHint]=None):
+    def save_data(self, data: Data, prefix=str(), suffix="now", ext: Optional[TypeHint]=None):
         prefix = prefix if prefix else self.operation
-        file_name = prefix+'_'+self.now("%Y%m%d%H%M%S")
+        suffix = self.now("%Y%m%d%H%M%S") if suffix == "now" else suffix
+        file_name = '_'.join(filter(None, [prefix, suffix]))
         ext = ext if ext else type(data)
         if is_dataframe_type(ext):
             self.save_dataframe(data, file_name+".xlsx")
         elif is_tag_type(ext):
             self.save_source(data, file_name+".html")
         else: self.save_json(data, file_name+".json")
 
@@ -677,30 +689,36 @@
     ###################################################################
     ########################### Log Managers ##########################
     ###################################################################
 
     def catch_exception(func):
         @functools.wraps(func)
         def wrapper(self: BaseSession, *args, **context):
-            for retry in range(self.numRetries+1):
+            for count in reversed(range(self.numRetries+1)):
                 try: return func(self, *args, **context)
-                except KeyboardInterrupt as interrupt:
-                    raise interrupt
                 except Exception as exception:
-                    if retry+1 < self.numRetries: self.sleep()
-                    else: return self.pass_exception(exception, func=func, msg={"args":args, "context":context})
+                    if self.is_interrupt(exception): raise exception
+                    elif self.is_error(exception) or (count == 0):
+                        return self.pass_exception(exception, func=func, msg={"args":args, "context":context})
+                    else: self.sleep()
         return wrapper
 
     def ignore_exception(func):
         @functools.wraps(func)
         def wrapper(self: BaseSession, *args, **context):
             try: return func(self, *args, **context)
             except: return init_origin(func)
         return wrapper
 
+    def is_interrupt(self, exception: Exception) -> bool:
+        return isinstance(exception, UserInterrupt) or isinstance(exception, self.interruptType)
+
+    def is_error(self, exception: Exception) -> bool:
+        return isinstance(exception, ForbiddenError) or isinstance(exception, self.errorType)
+
     def pass_exception(self, exception: Exception, func: Callable, msg: Dict) -> Any:
         self.log_errors(func=func, msg=msg)
         if ("exception" in self.debug) or ("all" in self.debug):
             self.checkpoint("exception", where=func.__name__, msg=msg)
             raise exception
         return init_origin(func)
 
@@ -779,21 +797,21 @@
     pagination = False
     pageFrom = 1
     offsetFrom = 1
     pageUnit = 0
     pageLimit = 0
     interval = str()
 
-    def __init__(self, iterateUnit: Optional[int]=None, interval: Optional[Timedelta]=str()):
+    def __init__(self, iterateUnit: Optional[int]=None, interval: Optional[Timedelta]=None):
         self.set_iterator_unit(iterateUnit, interval)
         super().__init__()
 
-    def set_iterator_unit(self, iterateUnit: Optional[int]=None, interval: Timedelta=str()):
+    def set_iterator_unit(self, iterateUnit: Optional[int]=None, interval: Optional[Timedelta]=None):
         self.iterateUnit = iterateUnit if isinstance(iterateUnit, int) else self.iterateUnit
-        self.interval = interval if interval else self.interval
+        self.interval = interval if interval is not None else self.interval
 
     ###################################################################
     ########################### Set Iterator ##########################
     ###################################################################
 
     def get_iterator(self, _args=True, _page=True, _date=True, _product=True, _params=False, _index=False,
                     keys_only=False, values_only=False, if_null: Literal["drop","pass"]="drop",
@@ -1209,15 +1227,15 @@
         sub_path = path[-1] if (len(path) > 0) and is_array(path[-1]) else __value
         log_context = dict(context=context, name=name, log=False)
         return [self._get_value(__e, sub_path, apply=apply, **field, **log_context)
                 for __e in __value if self._match_data(__e, match, field=field, **log_context)]
 
     def _set_value(self, __base: Data, __value: _VT, field: Field, **context) -> Data:
         if (__value is __MISMATCH__) or ((field[MODE] in (OPTIONAL,REQUIRED)) and isna_plus(__value)):
-            if field[MODE] == REQUIRED: raise ValueError(REQUIRED_MSG(context, field))
+            if field[MODE] == REQUIRED: raise ParseError(REQUIRED_MSG(context, field))
             else: return __base
         __base[field[NAME]] = __value
         return __base
 
     ###################################################################
     ############################ Apply Data ###########################
     ###################################################################
@@ -1256,15 +1274,15 @@
         elif func == __RENAME__: return self.__rename__(__object, **kwargs)
         elif func == __SPLIT__: return self.__split__(__object, **kwargs)
         elif func == __STAT__: return self.__stat__(__object, **kwargs)
         elif func == __SUM__: return self.__stat__(__object, **kwargs)
         elif func == __MAP__:
             field = dict(type=field[TYPE], name=name)
             return self.__map__(__object, **dict(field, **kwargs), context=context)
-        else: raise ValueError(INVALID_APPLY_SPECIAL_MSG(func, context, field, name))
+        else: raise ForbiddenError(INVALID_APPLY_SPECIAL_MSG(func, context, field, name))
 
     def __cast__(self, __object, type: TypeHint, default=None, strict=True,
                 context: Context=dict(), **kwargs) -> _VT:
         context = dict(context, default=default, strict=strict)
         if isinstance(__object, List):
             return [cast_object(__e, type, **context) for __e in __object]
         else: return cast_object(__object, type, **context)
```

### Comparing `gcp-scraper-3.6.6/gscraper/base/spider.py` & `gcp-scraper-3.6.7/gscraper/base/spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 from gscraper.base.abstract import CustomDict, OptionalDict, TypedRecords, Query, INVALID_OBJECT_TYPE_MSG
 from gscraper.base.abstract import UNIQUE_CONTEXT, TASK_CONTEXT, REQUEST_CONTEXT, RESPONSE_CONTEXT
 from gscraper.base.abstract import SESSION_CONTEXT, PROXY_CONTEXT, REDIRECT_CONTEXT
 
-from gscraper.base.session import BaseSession, Iterator, Parser, Info, Schema, Field, Flow, Process
+from gscraper.base.session import BaseSession, Iterator, Parser
+from gscraper.base.session import UserInterrupt, ForbiddenError, ParseError
+from gscraper.base.session import Info, Schema, Field, Flow, Process
 from gscraper.base.session import ITER_INDEX, ITER_SUFFIX, ITER_MSG, PAGE_ITERATOR
 from gscraper.base.gcloud import GoogleQueryReader, GoogleUploader, GoogleQueryList, GoogleUploadList
-from gscraper.base.gcloud import fetch_gcloud_authorization, read_gcloud
+from gscraper.base.gcloud import Account, fetch_gcloud_authorization, read_gcloud
 
 from gscraper.base.types import _KT, _PASS, Arguments, Context, LogLevel, TypeHint, EncryptedKey, DecryptedKey
 from gscraper.base.types import IndexLabel, Keyword, Pagination, Status, Unit, Range, DateFormat, Timedelta, Timezone
-from gscraper.base.types import Records, Data, MappedData, JsonData, RedirectData, Account
+from gscraper.base.types import Records, Data, MappedData, JsonData, RedirectData
 from gscraper.base.types import is_datetime_type, is_date_type, is_array, is_int_array, init_origin
 
 from gscraper.utils import notna
 from gscraper.utils.cast import cast_list, cast_tuple, cast_int, cast_datetime_format
 from gscraper.utils.date import get_date_pair, get_datetime_pair
 from gscraper.utils.logs import log_encrypt, log_messages, log_response, log_client, log_data
 from gscraper.utils.map import to_array, align_array, transpose_array, unit_array, get_scala, union, inter, diff
@@ -83,34 +85,49 @@
 WORKER_EXTRA = ["message", "where", "which", "by"]
 
 NAME, OPERATOR, TASK, DATANAME, DATATYPE = "name", "operator", "task", "dataName", "dataType"
 FIELDS, ALLOWED, PARAMS, DERIV, CONTEXT = "fields", "allowedFields", "params", "derivData", "context"
 
 SUCCESS_RESULT = [{"response": "completed"}]
 
+class RequestInterrupt(requests.ConnectionError):
+    ...
+
+class AuthenticationError(ValueError):
+    ...
+
+class ParameterError(ValueError):
+    ...
+
+SPIDER_INTERRUPT = (UserInterrupt, RequestInterrupt, ParameterError)
+SPIDER_ERROR = (ForbiddenError, ParseError)
+
+ENCRYPTED_SESSION_INTERRUPT = (UserInterrupt, AuthenticationError, ParameterError)
+ENCRYPTED_SPIDER_INTERRUPT = (UserInterrupt, RequestInterrupt, AuthenticationError, ParameterError)
+
 
 ###################################################################
 ############################# Messages ############################
 ###################################################################
 
 INVALID_VALUE_MSG = lambda name, value: f"'{value}' value is not valid {name}."
 
-GATHER_MSG = lambda which, where=str(), by=str(): \
-    f"Collecting {which}{(' '+by) if by else str()}{(' from '+where) if where else str()}"
+GATHER_MSG = lambda action, which, by=str(), where=str(): \
+    f"{action} {which}{(' '+by) if by else str()}{(' from '+where) if where else str()}"
 INVALID_STATUS_MSG = lambda where: f"Response from {where} is not valid."
 
 REDIRECT_MSG = lambda operation: f"{operation} operation is redirecting"
 INVALID_REDIRECT_RESPONSE_MSG = "Please verify the redirect response."
 
 INVALID_USER_INFO_MSG = lambda where=str(): f"{where} user information is not valid.".strip()
 INVALID_API_INFO_MSG = lambda where=str(): f"{re.sub(' API$','',where)} API information is not valid.".strip()
 
 DEPENDENCY_HAS_NO_NAME_MSG = "Dependency has no operation name. Please define operation name."
 
-WHERE, WHICH = "urls", "data"
+ACTION, WHERE, WHICH = "Collecting", "urls", "data"
 FIRST_PAGE, NEXT_PAGE = "of first page", "of next pages"
 
 AUTH_KEY = "Auth Key"
 SAVE_SHEET = "Data"
 
 
 ###################################################################
@@ -503,14 +520,15 @@
 class Spider(RequestSession, Iterator, Parser):
     __metaclass__ = ABCMeta
     asyncio = False
     operation = "spider"
     host = str()
     where = WHERE
     which = WHICH
+    verb = ACTION
     by = str()
     fields = list()
     ranges = list()
     iterateArgs = list()
     iterateCount = dict()
     iterateProduct = list()
     iterateUnit = 1
@@ -535,15 +553,15 @@
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None,
                 fromNow: Optional[Unit]=None, discard=True, progress=True, where=str(), which=str(), by=str(), message=str(),
-                iterateUnit: Optional[int]=None, interval: Timedelta=str(), apiRedirect=False, redirectUnit: Optional[int]=None,
+                iterateUnit: Optional[int]=None, interval: Timedelta=None, apiRedirect=False, redirectUnit: Optional[int]=None,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None, **context):
         self.set_filter_variables(fields, ranges, returnType)
         self.set_init_time(tzinfo, datetimeUnit)
         self.set_logger(logName, logLevel, logFile, localSave, debug, extraSave, interrupt)
         self.set_request_variables(numRetries, delay, cookies)
         self.set_spider_variables(fromNow, discard, progress)
         self.set_gather_message(where, which, by, message)
@@ -574,14 +592,20 @@
             import urllib3
             urllib3.disable_warnings(InsecureRequestWarning)
 
     ###################################################################
     ############################# Override ############################
     ###################################################################
 
+    def is_interrupt(self, exception: Exception) -> bool:
+        return isinstance(exception, SPIDER_INTERRUPT) or isinstance(exception, self.interruptType)
+
+    def is_error(self, exception: Exception) -> bool:
+        return isinstance(exception, SPIDER_ERROR) or isinstance(exception, self.errorType)
+
     def log_errors(self, func: Callable, msg: Dict):
         iterator = self.get_iterator(**msg.get("context", dict()))
         super().log_errors(func=func, msg=(iterator if iterator else msg))
 
     def get_date(self, date: Optional[DateFormat]=None, if_null: Optional[Unit]=None, index=0, busdate=False) -> dt.date:
         if_null = if_null if if_null is not None else self.fromNow
         return super().get_date(date, if_null=get_scala(if_null, index), busdate=busdate)
@@ -675,19 +699,20 @@
         message = message if message else self.get_gather_message(**context)
         if not iterator:
             iterator, context = self._init_iterator(args, context, self.iterateArgs, self.iterateProduct, self.pagination)
         data = self._gather_data(iterator, message=message, progress=progress, fields=fields, **context)
         self.checkpoint("gather", where="gather", msg={"data":data}, save=data)
         return self.reduce(data, fields=fields, ranges=ranges, returnType=returnType, **context)
 
-    def get_gather_message(self, which=str(), where=str(), by=str(), **context) -> str:
+    def get_gather_message(self, where=str(), which=str(), verb=str(), by=str(), **context) -> str:
+        action = verb if verb else self.verb
         which = which if which else self.which
-        where = where if where else self.where
         by = by if by else self.by
-        return GATHER_MSG(which, where, by)
+        where = where if where else self.where
+        return GATHER_MSG(action, which, by, where)
 
     @RequestSession.arrange_data
     @RequestSession.validate_range
     def reduce(self, data: List[Data], fields: IndexLabel=list(), ranges: RangeFilter=list(),
                 returnType: Optional[TypeHint]=None, **context) -> Data:
         return chain_exists(data) if is_array(data) else data
 
@@ -845,27 +870,27 @@
                     params=None, encode: Optional[bool]=None, data=None, json=None, headers=None, cookies=str(),
                     allow_redirects=True, validate=False, exception: Literal["error","interrupt"]="interrupt",
                     valid: Optional[Status]=None, invalid: Optional[Status]=None, html=True, table_header=0, table_idx=0,
                     engine: Optional[Literal["xlrd","openpyxl","odf","pyxlsb"]]=None, **context) -> pd.DataFrame:
         with session.request(method, url, **messages, allow_redirects=allow_redirects, verify=self.ssl) as response:
             self.logger.info(log_response(response, url=url, **self.get_iterator(**context, _index=True)))
             if validate: self.validate_status(response, how=exception, valid=valid, invalid=invalid)
-            if html: return pd.read_html(response.text, header=table_header)[table_idx]
+            if html: return pd.read_html(response.content, header=table_header)[table_idx]
             else: return pd.read_excel(response.content, engine=engine)
 
     def encode_params(self, url: str, params: Optional[Dict]=None, encode: Optional[bool]=None) -> Tuple[str,Dict]:
         if not params: return url, None
         elif not isinstance(encode, bool): return url, params
         else: return encode_params(url, params, encode=encode), None
 
     def validate_status(self, response: requests.Response, how: Literal["error","interrupt"]="interrupt",
                         valid: Optional[Status]=None, invalid: Optional[Status]=None):
         status = response.status_code
         if (valid and (status not in cast_tuple(valid))) or (invalid and (status in cast_tuple(invalid))):
-            if how == "interrupt": raise KeyboardInterrupt(INVALID_STATUS_MSG(self.where))
+            if how == "interrupt": raise RequestInterrupt(INVALID_STATUS_MSG(self.where))
             else: raise requests.ConnectionError(INVALID_STATUS_MSG(self.where))
 
     def log_results(self, data: Data, **context):
         self.logger.info(log_data(data, **self.get_iterator(**context)))
 
     ###################################################################
     ######################### Redirect Request ########################
@@ -1022,21 +1047,21 @@
     ###################################################################
     ########################## Async Override #########################
     ###################################################################
 
     def catch_exception(func):
         @functools.wraps(func)
         async def wrapper(self: AsyncSession, *args, **context):
-            for retry in range(self.numRetries+1):
+            for count in reversed(range(self.numRetries+1)):
                 try: return await func(self, *args, **context)
-                except KeyboardInterrupt as interrupt:
-                    raise interrupt
                 except Exception as exception:
-                    if retry+1 < self.numRetries: await self.async_sleep()
-                    return self.pass_exception(exception, func=func, msg={"args":args, "context":context})
+                    if isinstance(exception, self.interruptType): raise exception
+                    elif isinstance(exception, self.errorType) or (count == 0):
+                        return self.pass_exception(exception, func=func, msg={"args":args, "context":context})
+                    else: await self.async_sleep()
         return wrapper
 
     def ignore_exception(func):
         @functools.wraps(func)
         async def wrapper(self: AsyncSession, *args, **context):
             try: return await func(self, *args, **context)
             except: return init_origin(func)
@@ -1069,14 +1094,15 @@
 class AsyncSpider(Spider, AsyncSession):
     __metaclass__ = ABCMeta
     asyncio = True
     operation = "spider"
     host = str()
     where = WHERE
     which = WHICH
+    verb = ACTION
     by = str()
     fields = list()
     ranges = list()
     iterateArgs = list()
     iterateCount = dict()
     iterateProduct = list()
     iterateUnit = 1
@@ -1103,15 +1129,15 @@
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None, numTasks=100,
                 fromNow: Optional[Unit]=None, discard=True, progress=True, where=str(), which=str(), by=str(), message=str(),
-                iterateUnit: Optional[int]=None, interval: Timedelta=str(), apiRedirect=False, redirectUnit: Optional[int]=None,
+                iterateUnit: Optional[int]=None, interval: Timedelta=None, apiRedirect=False, redirectUnit: Optional[int]=None,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None, **context):
         self.set_filter_variables(fields, ranges, returnType)
         self.set_init_time(tzinfo, datetimeUnit)
         self.set_logger(logName, logLevel, logFile, localSave, debug, extraSave, interrupt)
         self.set_async_variables(numRetries, delay, cookies, numTasks)
         self.set_max_limit(apiRedirect)
         self.set_spider_variables(fromNow, discard, progress)
@@ -1290,22 +1316,22 @@
                             params=None, encode: Optional[bool]=None, data=None, json=None, headers=None, cookies=str(),
                             allow_redirects=True, validate=False, exception: Literal["error","interrupt"]="interrupt",
                             valid: Optional[Status]=None, invalid: Optional[Status]=None, html=False, table_header=0, table_idx=0,
                             engine: Optional[Literal["xlrd","openpyxl","odf","pyxlsb"]]=None, **context) -> pd.DataFrame:
         async with session.request(method, url, **messages, allow_redirects=allow_redirects, ssl=self.ssl) as response:
             self.logger.info(await log_client(response, url=url, **self.get_iterator(**context, _index=True)))
             if validate: self.validate_status(response, how=exception, valid=valid, invalid=invalid)
-            if html: return pd.read_html(await response.text(), header=table_header)[table_idx]
+            if html: return pd.read_html(await response.read(), header=table_header)[table_idx]
             else: return pd.read_excel(await response.read(), engine=engine)
 
     def validate_status(self, response: aiohttp.ClientResponse, how: Literal["error","interrupt"]="interrupt",
                         valid: Optional[Status]=None, invalid: Optional[Status]=None):
         status = response.status
         if (valid and (status not in cast_tuple(valid))) or (invalid and (status in cast_tuple(invalid))):
-            if how == "interrupt": raise KeyboardInterrupt(INVALID_STATUS_MSG(self.where))
+            if how == "interrupt": raise RequestInterrupt(INVALID_STATUS_MSG(self.where))
             else: raise aiohttp.ServerConnectionError(INVALID_STATUS_MSG(self.where))
 
     ###################################################################
     ########################## Async Redirect #########################
     ###################################################################
 
     async def run_iterator(self, iterator: List[Context], self_var=True, **context) -> Data:
@@ -1520,19 +1546,22 @@
         self.set_secret(encryptedKey, decryptedKey)
 
     def set_secret(self, encryptedKey: Optional[EncryptedKey]=None, decryptedKey: Optional[DecryptedKey]=None):
         if (encryptedKey is None) and (decryptedKey is None): return
         elif isinstance(decryptedKey, Dict): pass
         elif isinstance(encryptedKey, str) or isinstance(decryptedKey, str):
             try: decryptedKey = json.loads((decryptedKey if decryptedKey else decrypt(encryptedKey)).replace('\'','\"'))
-            except JSONDecodeError: raise ValueError(INVALID_USER_INFO_MSG(self.where))
+            except JSONDecodeError: raise AuthenticationError(INVALID_USER_INFO_MSG(self.where))
         decryptedKey = decryptedKey if isinstance(decryptedKey, Dict) else self.decryptedKey
         if decryptedKey:
             self.update(encryptedKey=encrypt(decryptedKey,1), decryptedKey=decryptedKey)
 
+    def is_interrupt(self, exception: Exception) -> bool:
+        return isinstance(exception, ENCRYPTED_SESSION_INTERRUPT) or isinstance(exception, self.interruptType)
+
     ###################################################################
     ########################## Login Managers #########################
     ###################################################################
 
     def login_task(func):
         @functools.wraps(func)
         def wrapper(self: EncryptedSession, *args, self_var=True, **context):
@@ -1562,27 +1591,27 @@
         if cookies: return LoginCookie(cookies=cookies)
         else: return self.auth(**self.get_auth_info(update=True, **context))
 
     def get_auth_info(self, update=False, **context) -> Context:
         if not self.authKey: return dict()
         auth_info = self._from_auth_key(**context)
         if not (auth_info and isinstance(auth_info, Dict) and all(auth_info.values())):
-            raise ValueError(INVALID_USER_INFO_MSG(self.where))
+            raise AuthenticationError(INVALID_USER_INFO_MSG(self.where))
         self.logger.info(log_encrypt(**auth_info, show=3))
         return dict(context, **auth_info) if update else auth_info
 
     def _from_auth_key(self, **context) -> Context:
         auth_info = self.decryptedKey if self.decryptedKey else context
         if isinstance(self.authKey, Sequence): return kloc(auth_info, self.authKey, if_null="pass")
         elif isinstance(self.authKey, Callable): return self.authKey(**auth_info)
-        else: raise ValueError(INVALID_OBJECT_TYPE_MSG(self.authKey, AUTH_KEY))
+        else: raise AuthenticationError(INVALID_OBJECT_TYPE_MSG(self.authKey, AUTH_KEY))
 
     def validate_account(self, auth: LoginSpider, sessionCookies=False, **context) -> Context:
         try: self.login(auth, **context)
-        except: raise ValueError(INVALID_USER_INFO_MSG(self.where))
+        except: raise AuthenticationError(INVALID_USER_INFO_MSG(self.where))
         if isinstance(auth, LoginCookie) or not (sessionCookies and self.sessionCookies):
             context["cookies"] = self.cookies
         return context
 
     def login(self, auth: LoginSpider, **context):
         auth.login()
         auth.update_cookies(self.set_cookies(**context), if_exists="replace")
@@ -1626,14 +1655,15 @@
 class EncryptedSpider(Spider, EncryptedSession):
     __metaclass__ = ABCMeta
     asyncio = False
     operation = "spider"
     host = str()
     where = WHERE
     which = WHICH
+    verb = ACTION
     by = str()
     fields = list()
     ranges = list()
     iterateArgs = list()
     iterateCount = dict()
     iterateProduct = list()
     iterateUnit = 1
@@ -1661,20 +1691,23 @@
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None,
                 fromNow: Optional[Unit]=None, discard=True, progress=True, where=str(), which=str(), by=str(), message=str(),
-                iterateUnit: Optional[int]=None, interval: Timedelta=str(), apiRedirect=False, redirectUnit: Optional[int]=None,
+                iterateUnit: Optional[int]=None, interval: Timedelta=None, apiRedirect=False, redirectUnit: Optional[int]=None,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None,
                 encryptedKey: Optional[EncryptedKey]=None, decryptedKey: Optional[DecryptedKey]=None, **context):
         Spider.__init__(self, **self.from_locals(locals(), drop=ENCRYPTED_UNIQUE))
         self.set_secret(encryptedKey, decryptedKey)
 
+    def is_interrupt(self, exception: Exception) -> bool:
+        return isinstance(exception, ENCRYPTED_SPIDER_INTERRUPT) or isinstance(exception, self.interruptType)
+
 
 ###################################################################
 ##################### Encrypted Async Session #####################
 ###################################################################
 
 class EncryptedAsyncSession(AsyncSession, EncryptedSession):
     __metaclass__ = ABCMeta
@@ -1696,14 +1729,17 @@
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None, numTasks=100,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None,
                 encryptedKey: Optional[EncryptedKey]=None, decryptedKey: Optional[DecryptedKey]=None, **context):
         AsyncSession.__init__(self, **self.from_locals(locals(), drop=ENCRYPTED_UNIQUE))
         self.set_secret(encryptedKey, decryptedKey)
 
+    def is_interrupt(self, exception: Exception) -> bool:
+        return isinstance(exception, ENCRYPTED_SESSION_INTERRUPT) or isinstance(exception, self.interruptType)
+
     ###################################################################
     ########################## Login Managers #########################
     ###################################################################
 
     def login_task(func):
         @functools.wraps(func)
         async def wrapper(self: EncryptedAsyncSession, *args, self_var=True, **context):
@@ -1768,14 +1804,15 @@
 class EncryptedAsyncSpider(AsyncSpider, EncryptedAsyncSession):
     __metaclass__ = ABCMeta
     asyncio = True
     operation = "spider"
     host = str()
     where = WHERE
     which = WHICH
+    verb = ACTION
     by = str()
     fields = list()
     ranges = list()
     iterateArgs = list()
     iterateCount = dict()
     iterateProduct = list()
     iterateUnit = 1
@@ -1805,20 +1842,23 @@
 
     def __init__(self, fields: Optional[IndexLabel]=None, ranges: Optional[RangeFilter]=None, returnType: Optional[TypeHint]=None,
                 tzinfo: Optional[Timezone]=None, datetimeUnit: Optional[Literal["second","minute","hour","day"]]=None,
                 logName: Optional[str]=None, logLevel: LogLevel="WARN", logFile: Optional[str]=None, localSave=False,
                 debug: Optional[Keyword]=None, extraSave: Optional[Keyword]=None, interrupt: Optional[Keyword]=None,
                 numRetries: Optional[int]=None, delay: Range=1., cookies: Optional[str]=None, numTasks=100,
                 fromNow: Optional[Unit]=None, discard=True, progress=True, where=str(), which=str(), by=str(), message=str(),
-                iterateUnit: Optional[int]=None, interval: Timedelta=str(), apiRedirect=False, redirectUnit: Optional[int]=None,
+                iterateUnit: Optional[int]=None, interval: Timedelta=None, apiRedirect=False, redirectUnit: Optional[int]=None,
                 queryList: GoogleQueryList=list(), uploadList: GoogleUploadList=list(), account: Optional[Account]=None,
                 encryptedKey: Optional[EncryptedKey]=None, decryptedKey: Optional[DecryptedKey]=None, **context):
         AsyncSpider.__init__(self, **self.from_locals(locals(), drop=ENCRYPTED_UNIQUE))
         self.set_secret(encryptedKey, decryptedKey)
 
+    def is_interrupt(self, exception: Exception) -> bool:
+        return isinstance(exception, ENCRYPTED_SPIDER_INTERRUPT) or isinstance(exception, self.interruptType)
+
 
 ###################################################################
 ########################## Pipeline Task ##########################
 ###################################################################
 
 class Task(OptionalDict):
     def __init__(self, operator: Spider, task: str, dataName: str, dataType: Optional[TypeHint]=None,
```

### Comparing `gcp-scraper-3.6.6/gscraper/base/types.py` & `gcp-scraper-3.6.7/gscraper/base/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,16 +139,16 @@
 
 PandasData = Union[DataFrame, Series]
 PANDAS_DATA = (DataFrame, Series)
 
 HtmlData = Union[str, Tag, List[str], List[Tag]]
 HTML_DATA = (str, Tag, List)
 
-Account = Union[Dict[str,str], str]
-PostData = Union[Dict[str,Any],str]
+Account = Dict[str,str]
+PostData = Union[Dict[str,Any], str]
 
 ResponseData = Union[Records, DataFrame, Dict, List, NestedSequence, NestedDict, str, Tag, List[str], List[Tag]]
 
 DATA_TYPES = {
     "NestedDict":NestedDict, "RenameMap":RenameMap, "TypeMap":TypeMap, "NestedData":NestedData,
     "TabularData":TabularData, "MappingData":MappingData, "Data":Data, "JsonData":JsonData,
     "RedirectData":RedirectData, "HtmlData":HtmlData, "Account":Account, "PostData":PostData,
```

### Comparing `gcp-scraper-3.6.6/gscraper/utils/__init__.py` & `gcp-scraper-3.6.7/gscraper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.6/gscraper/utils/cast.py` & `gcp-scraper-3.6.7/gscraper/utils/cast.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,16 +181,16 @@
         elif isinstance(match, str) and re.search(match, str(__object)): pass
         else: return default
     if notna(__object, strict=strict):
         return str(__object).strip() if strip else str(__object)
     else: return default
 
 
-def cast_id(__object, default=str()) -> str:
-    return cast_str(cast_int(__object, default=__object), default, match=r"^((?!nan).)*$")
+def cast_id(__object, default=None) -> str:
+    return cast_str(cast_int(__object, default=None), default)
 
 
 def cast_list(__object, strict=True, iter_type: _TYPE=(List,Set,Tuple)) -> List:
     if isinstance(__object, List): return __object
     elif isinstance(__object, iter_type): return list(__object)
     elif notna(__object, strict=strict): return [__object]
     else: return list()
```

### Comparing `gcp-scraper-3.6.6/gscraper/utils/date.py` & `gcp-scraper-3.6.7/gscraper/utils/date.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.6/gscraper/utils/logs.py` & `gcp-scraper-3.6.7/gscraper/utils/logs.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.6/gscraper/utils/map.py` & `gcp-scraper-3.6.7/gscraper/utils/map.py`

 * *Files identical despite different names*

### Comparing `gcp-scraper-3.6.6/setup.py` & `gcp-scraper-3.6.7/setup.py`

 * *Files identical despite different names*

