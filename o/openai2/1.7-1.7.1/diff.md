# Comparing `tmp/openai2-1.7.tar.gz` & `tmp/openai2-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openai2-1.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openai2-1.7.tar` & `openai2-1.7.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 openai2-1.7/LICENSE
--rw-r--r--   0        0        0    13972 2024-03-01 12:35:49.672946 openai2-1.7/README.md
--rw-r--r--   0        0        0      167 2023-12-19 12:18:48.792856 openai2-1.7/__init__.py
--rw-r--r--   0        0        0     6923 2023-11-15 22:45:46.000000 openai2-1.7/_core/GroupChat.py
--rw-r--r--   0        0        0     9258 2023-12-17 18:34:22.000000 openai2-1.7/_core/chat.py
--rw-r--r--   0        0        0     2279 2024-02-23 04:06:51.826269 openai2-1.7/_core/chat_in_cmd.py
--rw-r--r--   0        0        0       44 2023-12-19 12:19:46.680720 openai2-1.7/art.json
--rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 openai2-1.7/licenses/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 openai2-1.7/licenses/openai/LICENSE
--rw-r--r--   0        0        0      203 2024-03-03 10:11:45.701543 openai2-1.7/openai2.py
--rw-r--r--   0        0        0      802 2024-03-03 10:11:57.006312 openai2-1.7/pyproject.toml
--rw-r--r--   0        0        0    14136 1970-01-01 00:00:00.000000 openai2-1.7/PKG-INFO
+-rw-r--r--   0        0        0    11281 2024-02-22 12:02:36.209038 openai2-1.7.1/LICENSE
+-rw-r--r--   0        0        0    13971 2024-03-31 09:40:29.216952 openai2-1.7.1/README.md
+-rw-r--r--   0        0        0      167 2023-12-19 12:18:48.792856 openai2-1.7.1/__init__.py
+-rw-r--r--   0        0        0     6923 2023-11-15 22:45:46.000000 openai2-1.7.1/_core/GroupChat.py
+-rw-r--r--   0        0        0     9298 2024-04-06 05:34:07.115496 openai2-1.7.1/_core/chat.py
+-rw-r--r--   0        0        0     2279 2024-02-23 04:06:51.826269 openai2-1.7.1/_core/chat_in_cmd.py
+-rw-r--r--   0        0        0       99 2024-03-05 23:28:04.263728 openai2-1.7.1/art.json
+-rw-r--r--   0        0        0      245 2023-09-04 06:15:02.000000 openai2-1.7.1/licenses/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:04.000000 openai2-1.7.1/licenses/openai/LICENSE
+-rw-r--r--   0        0        0      203 2024-03-03 10:11:45.701543 openai2-1.7.1/openai2.py
+-rw-r--r--   0        0        0      805 2024-04-06 05:38:16.070983 openai2-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    14138 1970-01-01 00:00:00.000000 openai2-1.7.1/PKG-INFO
```

### Comparing `openai2-1.7/LICENSE` & `openai2-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.7/README.md` & `openai2-1.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install openai2
 ```
```

### Comparing `openai2-1.7/_core/GroupChat.py` & `openai2-1.7.1/_core/GroupChat.py`

 * *Files identical despite different names*

### Comparing `openai2-1.7/_core/chat.py` & `openai2-1.7.1/_core/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
             **self._request_kwargs,  # 全局参数
             **kwargs,  # 单次请求的参数覆盖全局参数
             "messages": list(self._messages + messages),
             "stream": True,
         })
         answer: str = ""
         for chunk in completion:
-            if content := chunk.choices[0].delta.content:
+            if chunk.choices and (content := chunk.choices[0].delta.content):
                 answer += content
                 yield content
         self._messages.add_many(*messages, {"role": "assistant", "content": answer})
 
     async def async_request(self, text: str=None, **kwargs):
         messages = [{"role": "user", "content": text}]
         messages += (kwargs.pop('messages', None) or [])  # 兼容官方包[openai]用户, 使其代码可以无缝切换到[openai2]
@@ -205,15 +205,15 @@
             **self._request_kwargs,  # 全局参数
             **kwargs,  # 单次请求的参数覆盖全局参数
             "messages": list(self._messages + messages),
             "stream": True,
         })
         answer: str = ""
         async for chunk in completion:
-            if content := chunk.choices[0].delta.content:
+            if chunk.choices and (content := chunk.choices[0].delta.content):
                 answer += content
                 yield content
         self._messages.add_many(*messages, {"role": "assistant", "content": answer})
 
     def rollback(self, n=1):
         self._messages.core[-2 * n :] = []
         for x in self._messages.core[-2:]:
```

### Comparing `openai2-1.7/_core/chat_in_cmd.py` & `openai2-1.7.1/_core/chat_in_cmd.py`

 * *Files identical despite different names*

### Comparing `openai2-1.7/licenses/openai/LICENSE` & `openai2-1.7.1/licenses/openai/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.7/pyproject.toml` & `openai2-1.7.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "openai2"
-version = "1.7"
+version = "1.7.1"
 description = "ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。"
-dependencies = ["arts>=2024.2.25"]
+dependencies = ["arts>=2024.4.3.1"]
 keywords = ["openai", "chatgpt", "openai2"]
 
 
 readme = "README.md"
 authors = [{name = "江南雨上", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
```

### Comparing `openai2-1.7/PKG-INFO` & `openai2-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: openai2
-Version: 1.7
+Version: 1.7.1
 Summary: ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。
 Keywords: openai,chatgpt,openai2
 Author-email: 江南雨上 <lcctoor@outlook.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: arts>=2024.2.25
+Requires-Dist: arts>=2024.4.3.1
 Project-URL: HomePage, https://github.com/lcctoor/arts/tree/main/arts/openai2
 
 # 项目描述
 
 ChatGPT 工具包，支持连续对话、流式对话（逐字显示）、对话存档与载入、对话回滚、对话伪造、轮询 api_key 池、群聊多角色模拟、在命令行对话、限制历史消息数量、异步请求。
 
 # 作者
 
 [江南雨上](mailto:lcctoor@outlook.com)
 
-[主页](https://lcctoor.github.io/arts/) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
+[主页](https://lcctoor.github.io/arts) \| [Github](https://github.com/lcctoor) \| [PyPi](https://pypi.org/user/lcctoor) \| [微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) \| [邮箱](mailto:lcctoor@outlook.com) \| [捐赠](https://lcctoor.github.io/arts/arts/ip_static/DonationQRC-0rmb.jpg)
 
 # Bug提交、功能提议
 
-您可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
+你可以通过 [Github-Issues](https://github.com/lcctoor/arts/issues)、[微信](https://lcctoor.github.io/arts/arts/ip_static/WeChatQRC.jpg) 与我联系。
 
 # 安装
 
 ```
 pip install openai2
 ```
```

