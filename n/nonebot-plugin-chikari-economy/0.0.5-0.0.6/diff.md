# Comparing `tmp/nonebot_plugin_chikari_economy-0.0.5.tar.gz` & `tmp/nonebot_plugin_chikari_economy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chikari_economy-0.0.5.tar", last modified: Sat Apr  6 03:29:29 2024, max compression
+gzip compressed data, was "nonebot_plugin_chikari_economy-0.0.6.tar", last modified: Sat Apr  6 03:32:01 2024, max compression
```

## Comparing `nonebot_plugin_chikari_economy-0.0.5.tar` & `nonebot_plugin_chikari_economy-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 03:29:29.774238 nonebot_plugin_chikari_economy-0.0.5/
--rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_economy-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     4492 2024-04-06 03:29:29.773240 nonebot_plugin_chikari_economy-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3924 2024-04-04 13:03:33.000000 nonebot_plugin_chikari_economy-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 03:29:29.765262 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy/
--rw-rw-rw-   0        0        0     1151 2024-04-04 14:14:46.000000 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy/__init__.py
--rw-rw-rw-   0        0        0     4352 2024-04-04 12:04:52.000000 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy/data_handles.py
--rw-rw-rw-   0        0        0     1206 2024-04-04 11:35:25.000000 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy/handles.py
-drwxrwxrwx   0        0        0        0 2024-04-06 03:29:29.773240 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy.egg-info/
--rw-rw-rw-   0        0        0     4492 2024-04-06 03:29:29.000000 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2024-04-06 03:29:29.000000 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 03:29:29.000000 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-04-06 03:29:29.000000 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-04-06 03:29:29.000000 nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-06 03:29:29.775236 nonebot_plugin_chikari_economy-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      785 2024-04-04 14:14:49.000000 nonebot_plugin_chikari_economy-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:32:01.657017 nonebot_plugin_chikari_economy-0.0.6/
+-rw-rw-rw-   0        0        0     1065 2024-02-11 07:24:25.000000 nonebot_plugin_chikari_economy-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4492 2024-04-06 03:32:01.657017 nonebot_plugin_chikari_economy-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3924 2024-04-04 13:03:33.000000 nonebot_plugin_chikari_economy-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 03:32:01.648042 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/
+-rw-rw-rw-   0        0        0     1151 2024-04-06 03:31:21.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/__init__.py
+-rw-rw-rw-   0        0        0     4352 2024-04-04 12:04:52.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/data_handles.py
+-rw-rw-rw-   0        0        0     1159 2024-04-06 03:31:18.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/handles.py
+drwxrwxrwx   0        0        0        0 2024-04-06 03:32:01.656020 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/
+-rw-rw-rw-   0        0        0     4492 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-04-06 03:32:01.000000 nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-06 03:32:01.658014 nonebot_plugin_chikari_economy-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      785 2024-04-06 03:31:25.000000 nonebot_plugin_chikari_economy-0.0.6/setup.py
```

### Comparing `nonebot_plugin_chikari_economy-0.0.5/LICENSE` & `nonebot_plugin_chikari_economy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.5/PKG-INFO` & `nonebot_plugin_chikari_economy-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_economy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A economy plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_economy
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_chikari_economy-0.0.5/README.md` & `nonebot_plugin_chikari_economy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy/__init__.py` & `nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     description="一个经济插件（库），可由其他插件调用，以便插件间的经济联动",
     usage="",
     type="library",
     homepage="https://github.com/mrqx0195/nonebot_plugin_chikari_economy",
     supported_adapters={}
 )
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 from .data_handles import def_money_type as def_money_type
 from .data_handles import set_money as set_money
 from .data_handles import add_money as add_money
 from .data_handles import inquire_money as inquire_money
 
 __all__ = (
```

### Comparing `nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy/data_handles.py` & `nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/data_handles.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy/handles.py` & `nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy/handles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from nonebot.adapters.onebot.v11 import GroupMessageEvent,Message
+from nonebot.adapters import Event,Message
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg
 
 from . import data_handles
 
 class message_Handles():
     """消息处理
     """
     async def inquire_one_money(
-            matcher: Matcher,event: GroupMessageEvent,args: Message = CommandArg()
+            matcher: Matcher,event: Event,args: Message = CommandArg()
     ):
         """内置的单种货币查询指令，一般不建议使用
         """
         command: str = args.extract_plain_text()
         uid: str = event.get_user_id()
         s = f"{uid}的{command}量："
         try:
             s += data_handles.inquire_money(command)
         except NameError:
             s = "未注册的货币类型！"
         await matcher.finish(s)
         
     async def inquire_all_money(
-            matcher: Matcher,event: GroupMessageEvent,args: Message = CommandArg()
+            matcher: Matcher,event: Event,args: Message = CommandArg()
     ):
         """内置的所有货币查询指令，一般不建议使用
         """
         uid: str = event.get_user_id()
         s = f"{uid}的所有货币量："
         for i in data_handles.configdata["money_types"].keys:
             s += "\n" + data_handles.inquire_money(i)
```

### Comparing `nonebot_plugin_chikari_economy-0.0.5/nonebot_plugin_chikari_economy.egg-info/PKG-INFO` & `nonebot_plugin_chikari_economy-0.0.6/nonebot_plugin_chikari_economy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_chikari_economy
-Version: 0.0.5
+Version: 0.0.6
 Summary: A economy plugin for nonebot 2
 Home-page: https://github.com/mrqx0195/nonebot_plugin_chikari_economy
 Author: mrqx0195
 Author-email: 2317249571@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nonebot_plugin_chikari_economy-0.0.5/setup.py` & `nonebot_plugin_chikari_economy-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_chikari_economy",
-    version="0.0.5",
+    version="0.0.6",
     author="mrqx0195",
     author_email="2317249571@qq.com",
     description="A economy plugin for nonebot 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrqx0195/nonebot_plugin_chikari_economy",
     packages=setuptools.find_packages(),
```

