# Comparing `tmp/nonebot-plugin-acm-reminder-0.1.8.tar.gz` & `tmp/nonebot-plugin-acm-reminder-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-acm-reminder-0.1.8.tar", last modified: Mon May 15 11:31:06 2023, max compression
+gzip compressed data, was "nonebot-plugin-acm-reminder-0.1.9.tar", last modified: Sat Apr  6 09:31:06 2024, max compression
```

## Comparing `nonebot-plugin-acm-reminder-0.1.8.tar` & `nonebot-plugin-acm-reminder-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2023-01-15 11:05:12.918513 nonebot-plugin-acm-reminder-0.1.8/LICENSE
--rw-r--r--   0        0        0     3353 2023-05-15 11:29:35.875350 nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/__init__.py
--rw-r--r--   0        0        0      228 2023-04-30 14:06:17.044896 nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/config.py
--rw-r--r--   0        0        0     4017 2023-05-15 11:25:53.437244 nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/data_source.py
--rw-r--r--   0        0        0      636 2023-05-15 11:30:58.511125 nonebot-plugin-acm-reminder-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      852 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.8/README.md
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 nonebot-plugin-acm-reminder-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-01-15 11:05:12.918513 nonebot-plugin-acm-reminder-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3706 2024-04-06 08:58:11.101554 nonebot-plugin-acm-reminder-0.1.9/nonebot_plugin_acm_reminder/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-06 07:58:30.969750 nonebot-plugin-acm-reminder-0.1.9/nonebot_plugin_acm_reminder/config.py
+-rw-r--r--   0        0        0     4831 2024-04-06 09:02:26.351948 nonebot-plugin-acm-reminder-0.1.9/nonebot_plugin_acm_reminder/data_source.py
+-rw-r--r--   0        0        0      693 2024-04-06 09:31:00.589761 nonebot-plugin-acm-reminder-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      852 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.9/README.md
+-rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 nonebot-plugin-acm-reminder-0.1.9/PKG-INFO
```

### Comparing `nonebot-plugin-acm-reminder-0.1.8/LICENSE` & `nonebot-plugin-acm-reminder-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/__init__.py` & `nonebot-plugin-acm-reminder-0.1.9/nonebot_plugin_acm_reminder/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,60 @@
 from datetime import datetime
+from email.mime import application
+from turtle import home
 from typing import List
-from nonebot.adapters.onebot.v11 import MessageEvent, MessageSegment
+from nonebot.adapters import Event
 from nonebot.plugin import on_command, PluginMetadata
-from nonebot import get_driver, logger, require
+from nonebot import get_driver, logger, require, get_plugin_config
 
 
 from .config import Config
-from .data_source import ContestType, req_get, html_parse_cf, html_parse_nc
+from .data_source import ContestType, html_parse_at, req_get, html_parse_cf, html_parse_nc
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
+require("nonebot_plugin_alconna")
 from nonebot_plugin_htmlrender import md_to_pic
 from nonebot_plugin_apscheduler import scheduler
+from nonebot_plugin_alconna import UniMessage, on_alconna
 
 
 __plugin_meta__ = PluginMetadata(
     name="ACMReminder",
-    description="订阅牛客/CF平台的比赛信息",
+    description="订阅牛客/CF/AT平台的比赛信息",
     usage=
-    "/contest.list 获取所有/CF/牛客平台的比赛信息"
-    "/contest.subscribe 订阅CF/牛客平台的比赛信息"
-    "/contest.update 手动更新比赛信息")
+    "/contest.list 获取所有/CF/牛客/AT平台的比赛信息\n"
+    "/contest.subscribe 订阅CF/牛客/AT平台的比赛信息\n"
+    "/contest.update 手动更新比赛信息\n",
+    supported_adapters=None,
+    config=Config,
+    type="application",
+    homepage="https://github.com/BigOrangeQWQ/nonebot_plugin_acm_reminder",
+    )
 
 contest_list = on_command(("contest", "list"), aliases={"比赛列表"}, priority=5)
 contest_update = on_command(("contest", "update"),
                             aliases={"更新比赛"}, priority=5)
 contest_subscribe = on_command(
     ("contest", "subscribe"), aliases={"订阅比赛"}, priority=5)
 
 driver = get_driver()
 contest_data: List[ContestType] = []
-plugin_config: Config = Config.parse_obj(driver.config)
+plugin_config: Config = get_plugin_config(Config)
 
 
 async def update():
     """
     更新比赛信息
     """
     contest_data.clear()
     contest_data.extend(html_parse_cf(await req_get("https://codeforces.com/contests")))
     contest_data.extend(html_parse_nc(await req_get("https://ac.nowcoder.com/acm/contest/vip-index?topCategoryFilter=13")))
     contest_data.extend(html_parse_nc(await req_get("https://ac.nowcoder.com/acm/contest/vip-index?topCategoryFilter=14")))
+    contest_data.extend(html_parse_at(await req_get("https://atcoder.jp")))
 
 @scheduler.scheduled_job('interval', minutes=plugin_config.update_time, id="update_contest")
 async def update_contest():
     try:
         await update()
     except Exception as e:
         logger.warning("拉取竞赛信息更新失败!")
@@ -58,32 +68,32 @@
     except Exception as e:
         logger.warning("拉取竞赛信息更新失败!")
         logger.warning(e)
     # 防止因为网络问题导致机器人启动失败
 
 
 @contest_update.handle()
-async def update_handle(event: MessageEvent):
+async def update_handle(event: Event):
     try:
         await update()
     except Exception as e:
         logger.warning("拉取竞赛信息更新失败!")
         logger.warning(e)
-        await contest_update.finish(MessageSegment.image(await md_to_pic(f"更新失败 {e}")))
-
+        await contest_update.finish("更新失败")
     await contest_update.finish("更新成功")
 
 
 @contest_list.handle()
-async def get_list(event: MessageEvent):
+async def get_list(event: Event):
     msg = '<div align="center">\n <h1> 近期竞赛 </h1> \n</div>'
+    # contest_data.sort()
     for contest in contest_data:
         time = datetime.fromtimestamp(
             contest["time"]).strftime("%Y-%m-%d %H:%M")
         writes = ",".join(filter(None, contest["writes"])) if len(
             contest["writes"]) < 5 else ",".join(filter(None, contest["writes"][:5])) + "..."
         msg += f"## {contest['name']}\n" \
             f"* 竞赛平台  **{contest['platform']}**\n" \
             f"* 举办人员 {writes}\n" \
             f"* 开始时间 **{time}**\n" \
             f"* 竞赛时长 **{contest['length']/60}h**\n"
-    await contest_list.finish(MessageSegment.image(await md_to_pic(msg)))
+    await UniMessage.image(raw=await md_to_pic(msg)).send()
```

### Comparing `nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/data_source.py` & `nonebot-plugin-acm-reminder-0.1.9/nonebot_plugin_acm_reminder/data_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from json import loads
 from time import strptime, mktime, struct_time
 from html import unescape
-from typing import Any, Dict, Literal, Optional, TypedDict, List, Union
+from typing import Any, Dict, Optional, TypedDict, List, Union
 from httpx import AsyncClient, Response
 from httpx._types import URLTypes, ProxiesTypes
 from bs4 import BeautifulSoup, NavigableString, ResultSet, Tag
 
+
 class ContestType(TypedDict):
-    id: int  # 竞赛ID
+    # id: int  # 竞赛ID
     name: str  # 竞赛名称
     writes: List[str]  # 竞赛主办方
     length: int  # 竞赛时长 [分钟]
-    time: float  # 竞赛开始时间戳
-    platform: Literal["Codeforces", "Nowcoder"]  # 竞赛平台
+    time: float  # 竞赛开始时间
+    platform: str  # 竞赛平台
 
 
 async def req_get(url: URLTypes, proxies: Optional[ProxiesTypes] = None) -> str:
     """
     生成一个异步的GET请求
 
     Args:
@@ -25,83 +26,110 @@
     Returns:
         str: URL对应的HTML
     """
     async with AsyncClient(proxies=proxies) as client:
         r: Response = await client.get(url)
     return r.content.decode("utf-8")
 
+
 def html_parse_cf(content: str) -> List[ContestType]:
     """
     处理Codeforces的竞赛列表
 
     Args:
         content (str): HTML
 
     Returns:
         list: 竞赛列表
     """
     contest_data: List[ContestType] = []
-    
+
     soup = BeautifulSoup(content, 'html.parser')
-    datatable: Union[Tag,NavigableString,None] = soup.find('div', class_='datatable')  # 获取到数据表
-    if not isinstance(datatable,Tag):
+    datatable: Union[Tag, NavigableString, None] = soup.find(
+        'div', class_='datatable')  # 获取到数据表
+    if not isinstance(datatable, Tag):
         return contest_data
 
     # 解析竞赛信息
-    contest_list: ResultSet[Any] = datatable.find_all("tr") 
+    contest_list: ResultSet[Any] = datatable.find_all("tr")
     for contest in contest_list:
         cdata: ResultSet[Any] = contest.find_all("td")
         if cdata:
-            cwriters: List[str] = [i.string for i in cdata[1].find_all("a")] #获得主办方
-            ctime: float = mktime(strptime(cdata[2].find("span").string, "%b/%d/%Y %H:%M")) #获得开始时间戳
-            ctime+=5*60*60
+            cwriters: List[str] = [
+                i.string for i in cdata[1].find_all("a")]  # 获得主办方
+            ctime: float = mktime(strptime(cdata[2].find(
+                "span").string, "%b/%d/%Y %H:%M"))  # 获得开始时间戳
+            ctime += 5*60*60
             try:
-                clength: struct_time = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M")
+                clength: struct_time = strptime(
+                    str(cdata[3].string).strip("\n").strip(), "%H:%M")
             except:
-                clength: struct_time = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M:%S")
-            contest_data.append({"name": str(cdata[0].string).strip("\n").strip(), 
-                                "writes": cwriters, 
-                                "time": ctime, 
-                                "length": clength.tm_hour * 60 + clength.tm_min, 
-                                "platform": "Codeforces", 
-                                "id": contest.get("data-contestid")})
+                clength: struct_time = strptime(
+                    str(cdata[3].string).strip("\n").strip(), "%H:%M:%S")
+            contest_data.append({"name": str(cdata[0].string).strip("\n").strip(),
+                                "writes": cwriters,
+                                "time": ctime,
+                                "length": clength.tm_hour * 60 + clength.tm_min,
+                                "platform": "Codeforces"})
     return contest_data
 
+
 def html_parse_nc(content: str) -> List[ContestType]:
     """
     处理牛客的竞赛列表 
 
     Args:
         content (str): HTML
 
     Returns:
         list: 竞赛列表
-    """ 
+    """
     contest_data: List[ContestType] = []
     soup = BeautifulSoup(content, 'html.parser')
-    find_item: Union[Tag,NavigableString,None] = soup.find('div', class_='platform-mod js-current')
+    find_item: Union[Tag, NavigableString, None] = soup.find(
+        'div', class_='platform-mod js-current')
     if not isinstance(find_item, Tag):
         return contest_data
-    datatable: ResultSet = find_item.find_all('div', class_='platform-item js-item')
+    datatable: ResultSet[Tag] = find_item.find_all(
+        'div', class_='platform-item js-item')
     for contest in datatable:
-        cdata: Dict[str, Any] = loads(unescape(contest.get("data-json")))
+        cdata: Dict[str, Any] = loads(unescape(contest.get_text("data-json")))
         if cdata:
-            contest_data.append({"name": cdata["contestName"], 
-                                "writes": [cdata["settingInfo"]["organizerName"]], 
-                                "time":  cdata["contestStartTime"] / 1000, 
-                                "length": cdata["contestDuration"] / 1000 / 60, 
-                                "platform": "Nowcoder", 
-                                "id": cdata["contestId"]})
+            contest_data.append({"name": cdata["contestName"],
+                                "writes": [cdata["settingInfo"]["organizerName"]],
+                                "time":  cdata["contestStartTime"] / 1000,
+                                "length": cdata["contestDuration"] / 1000 / 60,
+                                "platform": "Nowcoder",})
     return contest_data
 
+
+def html_parse_at(content: str) -> List[ContestType]:
+    contest_data: List[ContestType] = []
+    soup = BeautifulSoup(content, 'html.parser')
+    table: Tag = soup.select("#contest-table-upcoming > div > table")[0]
+    table_body: ResultSet[Tag] = table.find_all("tr")
+    for contest in table_body:
+        
+        cdata = contest.find_all("td")
+        if cdata:
+            time = cdata[0].find("a").string
+            name = cdata[1].find("a").string
+            contest_data.append({"name": name,
+                                "writes": ["Atcoder"],
+                                "time": mktime(strptime(time, "%Y-%m-%d %H:%M:%S%z")),
+                                "length": 0,
+                                "platform": "Atcoder",})
+    return contest_data
+    
 # import asyncio
 
 # async def update():
 #     """
 #     更新比赛信息
 #     """
-    
-#     a = html_parse_cf(await req_get("https://codeforces.com/contests"))
-#     b = html_parse_nc(await req_get("https://ac.nowcoder.com/acm/contest/vip-index?topCategoryFilter=14"))
-#     print(a,b)
-    
+
+#     # a = html_parse_cf(await req_get("https://codeforces.com/contests"))
+#     # b = html_parse_nc(await req_get("https://ac.nowcoder.com/acm/contest/vip-index?topCategoryFilter=14"))
+#     # print(a,b)
+#     print(html_parse_at(await req_get("https://atcoder.jp")))
+
 # asyncio.run(update())
```

### Comparing `nonebot-plugin-acm-reminder-0.1.8/pyproject.toml` & `nonebot-plugin-acm-reminder-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-[tool.pdm]
+[tool.pdm.dev-dependencies]
+dev = [
+    "keyring>=25.1.0",
+]
 
 [project]
 name = "nonebot_plugin_acm_reminder"
-version = "0.1.8"
-description = "A subscribe CodeForces/NowCoder contest info plugin for nonebot2"
+version = "0.1.9"
+description = "A subscribe CodeForces/NowCoder/Atcoder contest info plugin for nonebot2"
 authors = [
     { name = "BigOrangeQWQ", email = "2284086963@qq.com" },
 ]
 dependencies = [
-    "BeautifulSoup4>=4.11.2",
-    "nonebot2>=2.0.0b5",
-    "nonebot-adapter-onebot>=2.1.3",
-    "pydantic>=1.9.2",
+    "BeautifulSoup4>=4.12.3",
+    "nonebot2>=2.2.1",
+    "pydantic>=2.6.4",
     "httpx>=0.23.3",
     "nonebot-plugin-apscheduler>=0.2.0",
     "nonebot-plugin-htmlrender>=0.2.0.3",
+    "nonebot-plugin-alconna>=0.42.0",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
```

### Comparing `nonebot-plugin-acm-reminder-0.1.8/README.md` & `nonebot-plugin-acm-reminder-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-acm-reminder-0.1.8/PKG-INFO` & `nonebot-plugin-acm-reminder-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_acm_reminder
-Version: 0.1.8
-Summary: A subscribe CodeForces/NowCoder contest info plugin for nonebot2
+Version: 0.1.9
+Summary: A subscribe CodeForces/NowCoder/Atcoder contest info plugin for nonebot2
 License: MIT
 Author-email: BigOrangeQWQ <2284086963@qq.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # ACMReminder
 
 一款可查询与订阅牛客/CF竞赛的插件
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_acm_reminder Version: 0.1.8 Summary:
-A subscribe CodeForces/NowCoder contest info plugin for nonebot2 License: MIT
-Author-email: BigOrangeQWQ <2284086963@qq.com> Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: nonebot_plugin_acm_reminder Version: 0.1.9 Summary:
+A subscribe CodeForces/NowCoder/Atcoder contest info plugin for nonebot2
+License: MIT Author-email: BigOrangeQWQ <2284086963@qq.com> Requires-Python:
+>=3.9 Description-Content-Type: text/markdown
    # ACMReminder ä¸æ¬¾å¯æ¥è¯¢ä¸è®¢éçå®¢/CFç«èµçæä»¶_[_D_o_w_n_l_o_a_d_]
 ## å®è£ ``` pip install nonebot-plugin-acm-reminder nb plugin install
 nonebot-plugin-acm-reminder ``` ## éç½®é¡¹ *
 æåç«èµåè¡¨çæ´æ°æ¶é´(åé) ``` update_time = 720 ``` ## ç¨æ³
 ``` / := [å½ä»¤èµ·å§ç¬¦] . := [å½ä»¤åéç¬¦] /contest.list
 æåç«èµåè¡¨ /contest.update æ´æ°ç«èµåè¡¨ ``` ## TODO - [x]
 è·åç«èµä¿¡æ¯å¹¶å½¢æåè¡¨ - [x] æ¯æCodeForceså¹³å° - [x]
```

