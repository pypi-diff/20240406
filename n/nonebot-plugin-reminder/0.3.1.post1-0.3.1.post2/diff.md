# Comparing `tmp/nonebot_plugin_reminder-0.3.1.post1.tar.gz` & `tmp/nonebot_plugin_reminder-0.3.1.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_reminder-0.3.1.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_reminder-0.3.1.post2.tar", max compression
```

## Comparing `nonebot_plugin_reminder-0.3.1.post1.tar` & `nonebot_plugin_reminder-0.3.1.post2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2024-02-20 13:09:00.063763 nonebot_plugin_reminder-0.3.1.post1/LICENSE
--rw-r--r--   0        0        0     5030 2024-02-20 13:09:00.063763 nonebot_plugin_reminder-0.3.1.post1/README.md
--rw-r--r--   0        0        0    23027 2024-02-20 13:09:00.067763 nonebot_plugin_reminder-0.3.1.post1/nonebot_plugin_reminder/__init__.py
--rw-r--r--   0        0        0      544 2024-02-20 13:09:00.067763 nonebot_plugin_reminder-0.3.1.post1/nonebot_plugin_reminder/config.py
--rw-r--r--   0        0        0     4521 2024-02-20 13:09:00.067763 nonebot_plugin_reminder-0.3.1.post1/nonebot_plugin_reminder/data_utils.py
--rw-r--r--   0        0        0      581 2024-02-20 13:09:00.067763 nonebot_plugin_reminder-0.3.1.post1/pyproject.toml
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 nonebot_plugin_reminder-0.3.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/LICENSE
+-rw-r--r--   0        0        0     5030 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/README.md
+-rw-r--r--   0        0        0    23268 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/__init__.py
+-rw-r--r--   0        0        0      544 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/config.py
+-rw-r--r--   0        0        0     4491 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/data_utils.py
+-rw-r--r--   0        0        0      581 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/pyproject.toml
+-rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 nonebot_plugin_reminder-0.3.1.post2/PKG-INFO
```

### Comparing `nonebot_plugin_reminder-0.3.1.post1/LICENSE` & `nonebot_plugin_reminder-0.3.1.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_reminder-0.3.1.post1/README.md` & `nonebot_plugin_reminder-0.3.1.post2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_reminder-0.3.1.post1/nonebot_plugin_reminder/__init__.py` & `nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     if scheduler
     else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>，<r>禁用定时任务功能</r>"
 )
 # ^(?:(?:\@.*))* 用于兼容一些插件，群聊时被@,没有去掉@的那一部分
 remainer_matcher = on_regex(r"^(?:(?:\@.*))*定时[\s]*(\d{1,2}:\d{1,2})?$", priority=999, rule=to_me())
 fetch_matcher = on_regex(r"^(?:(?:\@.*))*定时请求[\s]*(\d{1,2}:\d{1,2})?$", priority=999,rule=to_me())
 list_matcher = on_regex(r"^(?:(?:\@.*))*定时列表[\s]*(\d+)?", priority=999, rule=to_me())
-list_apsjob_matcher = on_regex(r"^(?:(?:\@.*))*定时jobs$", priority=999,rule=to_me())
+list_apsjob_matcher = on_regex(r"^(?:(?:\@.*))*定时jobs[\s]*(\d+)?", priority=999,rule=to_me())
 clear_matcher = on_regex(r"^(?:(?:\@.*))*清(空|除)定时$", priority=999,rule=to_me())
 turn_matcher = on_regex(rf"^(?:(?:\@.*))*(查看|开启|关闭|删除|执行)定时[\s]*({plugin_config.reminder_id_prefix + '_'}[a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
 update_matcher = on_regex(rf"^(?:(?:\@.*))*(修改|更新)定时[\s]*({plugin_config.reminder_id_prefix + '_'}[a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
 backup_matcher = on_regex(rf"^(?:(?:\@.*))*(备份定时|定时备份)$", priority=999, permission=SUPERUSER,rule=to_me())
 backup_list_matcher = on_regex(rf"^(?:(?:\@.*))*备份列表[\s]*(\d+)?", priority=999, permission=SUPERUSER,rule=to_me())
 backup_recover_matcher = on_regex(rf"^(?:(?:\@.*))*(?:备份恢复|恢复备份|还原备份|备份还原|使用备份|备份使用)[\s]*([_a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
 backup_detail_mathcer = on_regex(rf"^(?:(?:\@.*))*查看备份[\s]*([_a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
@@ -247,20 +247,23 @@
         msg += "没有定时提醒"
     
     await sendReply(msg, target)
 
 @list_apsjob_matcher.handle()
 async def list_apsjob_matcher_handle(
     target: SaaTarget,
+    args: Tuple[Optional[int], ...] = RegexGroup(),
 ):
+    page = args[0] if len(args) > 0 and args[0] else 1
+    page = int(page)
     msg = None
     if not scheduler:
         msg = Text("未安装软依赖nonebot_plugin_apscheduler，不能使用此功能")
     else:
-        msg = Text(get_jobs_info())
+        msg = Text(get_jobs_info(page))
     
     await sendReply(msg, target)
     
 @backup_matcher.handle()
 async def backup_matcher_handle(
     target: SaaTarget
 ):
@@ -402,16 +405,14 @@
             new_time = current_time + timedelta(seconds=10)
             job.modify(next_run_time=new_time)
             await sendReply(f"正在执行{schId}的定时提醒",target)
             # new_job = scheduler.run_job(job, 'date', next_run_time=datetime.now())
                    
     await save_datas(CONFIG=CONFIG)
 
-    await sendReply(f"已成功{mode}{schId}的定时提醒",target)
-
 async def post_scheduler(botId: str, target_dict: Dict, msg: str, judgeWorkDay: bool = False, url: str = None, useId: str = None):
     logger.opt(colors=True).debug(
         f"执行任务<g>url: {url} msg:{msg}</g>"
     )
     if judgeWorkDay:
         if not is_workday(date.today()):
             logger.opt(colors=True).info(
@@ -439,14 +440,17 @@
     target = buildTarget(target_dict)
     # 非循环的任务，执行后删除
     if useId is not None and useId != "":
         removeScheduler(id=useId)
         logger.opt(colors=True).debug(
             f"<y>执行完成任务{useId}，清除记录</y>"
         )
+        CONFIG.pop(useId, {})
+        await save_datas(CONFIG=CONFIG)
+        
     await sendToReply(msg= msg, bot = bot, target=target)
 
 
 async def addScheduler(botId: str, target: SaaTarget, time: str, data: str, repeat: str = 1, url: str = None, id=None):
     if scheduler:
         logger.opt(colors=True).debug(
             f"<y>target: {target} time:{time}</y>"
@@ -628,8 +632,11 @@
     if(isinstance(msg, str)):
         msg = Text(msg)
     if(useId is not None):
         mention = Mention(user_id=useId)
         msg = MessageFactory([msg, mention])
     if messageId is not None:
         msg = MessageFactory([msg, Reply(message_id=messageId)])
-    await msg.send_to(bot=bot, target=target)
+    if bot is None:
+        await msg.send_to(bot=get_bot(), target=target)
+    else:
+        await msg.send_to(bot=bot, target=target)
```

### Comparing `nonebot_plugin_reminder-0.3.1.post1/nonebot_plugin_reminder/config.py` & `nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_reminder-0.3.1.post1/nonebot_plugin_reminder/data_utils.py` & `nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/data_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import json
 from nonebot import require
 require("nonebot_plugin_localstore")
 import nonebot_plugin_localstore as store
 from time import time
 from pathlib import Path
 lock = asyncio.Lock()
-data_file = store.get_data_file("nonebot_plugin_reminder","remain_plugin.json")
+plugin_name = 'nonebot_plugin_reminder'
+data_file = store.get_data_file(plugin_name,"remain_plugin.json")
 def get_datas(filepath: Path = None):
     if filepath is None:
         filepath = data_file
     if filepath.exists():
         with open(filepath, "r", encoding="utf8") as f:
             CONFIG: Dict[str, dict] = json.load(f)
     else:
@@ -46,15 +47,15 @@
 async def backup(config: Dict[str, Any] = None, maxBkNum:int = 2):
     try:
         data = None
         if config is None:
             data = get_datas()
         else:
             data = config
-        bkdir = store.get_data_dir("nonebot_plugin_reminder")
+        bkdir = store.get_data_dir(plugin_name)
         # 判断bkdir下面有多少backup文件，计算下一个文件名
         backup_files = [i for i in bkdir.iterdir() if i.is_file() and i.name.find("backup_") != -1]
         backup_files.sort() 
         # 如果达到上限，清除最早的一个
         while len(backup_files) >= maxBkNum:
             backup_files[0].unlink()
             backup_files.pop(0)
@@ -70,30 +71,30 @@
         raise e
     
 # 从备份中回复定时任务，但只是恢复配置，不会恢复底层的定时任务
 # filename不需要带后缀
 async def recover(filename: str):
     try:
         data = None
-        bkdir = store.get_data_dir("nonebot_plugin_reminder")
+        bkdir = store.get_data_dir(plugin_name)
         # 执行mv命令
         filename = Path.joinpath(bkdir, filename + ".json")
         if filename.exists():
             with open(filename, "r", encoding="utf8") as f:
                 data = json.load(f)
             await save_datas(data)
             return "恢复成功"
         else:
             return "文件不存在"
     except Exception as e:
         raise e
     
 async def list_backup(page_size:int = 5, page:int = 1):
     try:
-        bkdir = store.get_data_dir("nonebot_plugin_reminder")
+        bkdir = store.get_data_dir(plugin_name)
         backup_files = [i.name for i in bkdir.iterdir() if i.is_file() and i.name.find("backup_") != -1]
         # 去掉后缀
         backup_files = [i.replace(".json", "") for i in backup_files]
         # 返回特定页数的数据
         backup_files.sort(reverse=True)
         arrs = backup_files[page_size * (page - 1):page_size * page]
         res = "\n".join(arrs)
@@ -102,15 +103,15 @@
         raise e
 
 async def detail_backup(filename: str, page_size:int = 5, page:int = 1):
     try:
         logger.opt(colors=True).debug(
             f"<y>detail_backup 进入获取备份函数</y>"
         )
-        bkdir = store.get_data_dir("nonebot_plugin_reminder")
+        bkdir = store.get_data_dir(plugin_name)
         filename = Path.joinpath(bkdir, filename + ".json")
         logger.opt(colors=True).debug(
             f"<y>detail_backup filename:{filename}</y>"
         )
         data = get_datas(filename)
         logger.opt(colors=True).debug(
             f"<y>detail_backup data:{data}</y>"
```

### Comparing `nonebot_plugin_reminder-0.3.1.post1/pyproject.toml` & `nonebot_plugin_reminder-0.3.1.post2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-reminder"
-version = "0.3.1-1"
+version = "0.3.1-2"
 description = "This plugin can remind you not to forget something"
 authors = ["velor2012 <38395332+velor2012@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `nonebot_plugin_reminder-0.3.1.post1/PKG-INFO` & `nonebot_plugin_reminder-0.3.1.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-reminder
-Version: 0.3.1.post1
+Version: 0.3.1.post2
 Summary: This plugin can remind you not to forget something
 License: MIT
 Author: velor2012
 Author-email: 38395332+velor2012@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-reminder Version: 0.3.1.post1
+Metadata-Version: 2.1 Name: nonebot-plugin-reminder Version: 0.3.1.post2
 Summary: This plugin can remind you not to forget something License: MIT
 Author: velor2012 Author-email: 38395332+velor2012@users.noreply.github.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

