# Comparing `tmp/amino.light.py-0.0.9.tar.gz` & `tmp/amino.light.py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.0.9.tar", last modified: Fri Apr  5 22:39:34 2024, max compression
+gzip compressed data, was "amino.light.py-0.1.0.tar", last modified: Sat Apr  6 02:59:51 2024, max compression
```

## Comparing `amino.light.py-0.0.9.tar` & `amino.light.py-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.294325 amino.light.py-0.0.9/
-drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.244815 amino.light.py-0.0.9/AminoLightPy/
--rw-rw-rw-   0        0        0      286 2024-04-05 22:39:01.000000 amino.light.py-0.0.9/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0     8472 2024-04-03 00:57:53.000000 amino.light.py-0.0.9/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    65864 2024-04-05 22:01:03.000000 amino.light.py-0.0.9/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     2613 2024-04-05 22:38:53.000000 amino.light.py-0.0.9/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.247457 amino.light.py-0.0.9/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.0.9/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.252808 amino.light.py-0.0.9/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.0.9/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.0.9/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1238 2024-03-30 22:17:35.000000 amino.light.py-0.0.9/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0    96118 2024-04-05 22:01:47.000000 amino.light.py-0.0.9/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0    14834 2024-04-05 02:48:00.000000 amino.light.py-0.0.9/AminoLightPy/socket.py
--rw-rw-rw-   0        0        0    72389 2024-04-05 22:14:27.000000 amino.light.py-0.0.9/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1721 2024-04-05 22:39:34.294325 amino.light.py-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1019 2024-04-04 18:43:15.000000 amino.light.py-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.290329 amino.light.py-0.0.9/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     1721 2024-04-05 22:39:32.000000 amino.light.py-0.0.9/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2024-04-05 22:39:33.000000 amino.light.py-0.0.9/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 22:39:32.000000 amino.light.py-0.0.9/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-05 22:39:32.000000 amino.light.py-0.0.9/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-05 22:39:32.000000 amino.light.py-0.0.9/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-05 22:39:34.300326 amino.light.py-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1219 2024-04-04 19:24:01.000000 amino.light.py-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.568533 amino.light.py-0.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.399806 amino.light.py-0.1.0/AminoLightPy/
+-rw-rw-rw-   0        0        0      296 2024-04-06 02:59:21.000000 amino.light.py-0.1.0/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0     8472 2024-04-03 00:57:53.000000 amino.light.py-0.1.0/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    66004 2024-04-06 02:17:50.000000 amino.light.py-0.1.0/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2613 2024-04-05 22:38:53.000000 amino.light.py-0.1.0/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.400772 amino.light.py-0.1.0/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.1.0/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.484558 amino.light.py-0.1.0/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.1.0/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.1.0/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1238 2024-03-30 22:17:35.000000 amino.light.py-0.1.0/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    95980 2024-04-06 02:40:15.000000 amino.light.py-0.1.0/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0    17215 2024-04-06 02:33:53.000000 amino.light.py-0.1.0/AminoLightPy/socket.py
+-rw-rw-rw-   0        0        0    72505 2024-04-06 02:19:35.000000 amino.light.py-0.1.0/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1089 2024-04-06 02:55:57.000000 amino.light.py-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1799 2024-04-06 02:59:51.568533 amino.light.py-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1019 2024-04-04 18:43:15.000000 amino.light.py-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-06 02:59:51.566523 amino.light.py-0.1.0/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     1799 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-06 02:59:49.000000 amino.light.py-0.1.0/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-06 02:59:51.574526 amino.light.py-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1274 2024-04-06 02:58:52.000000 amino.light.py-0.1.0/setup.py
```

### Comparing `amino.light.py-0.0.9/AminoLightPy/acm.py` & `amino.light.py-0.1.0/AminoLightPy/acm.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.9/AminoLightPy/client.py` & `amino.light.py-0.1.0/AminoLightPy/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .socket import Callbacks, SocketHandler, SocketRequests
 
 
 #@dorthegra/IDörthe#8835 thanks for support!
 
 class Client(Callbacks, SocketHandler, SocketRequests):
     def __init__(self, proxies: dict = None, socketDebugging = False, socket_enabled = True):
+        self.api = api
         self.authenticated = False
         self.session = AminoSession()
 
         self.socket_enabled = socket_enabled
         if socket_enabled:
             handler = SocketHandler.__init__(self, self, socketDebugging)
             SocketRequests.__init__(self, handler)
@@ -564,14 +565,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
+        elif isinstance(userId, tuple): userIds = userId
         else: raise exceptions.WrongType
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
@@ -600,14 +602,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
+        elif isinstance(userId, tuple): userIds = userId
         else: raise exceptions.WrongType
 
         data = {
             "uids": userIds
         }
 
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/member/invite", json=data)
```

### Comparing `amino.light.py-0.0.9/AminoLightPy/constants.py` & `amino.light.py-0.1.0/AminoLightPy/constants.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.9/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.1.0/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.9/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.1.0/AminoLightPy/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.9/AminoLightPy/lib/util/objects.py` & `amino.light.py-0.1.0/AminoLightPy/lib/util/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self.disabledStatus: Optional[str] = self.extensions.get("__disabledStatus__")
         self.disabledTime: Optional[int] = self.extensions.get("__disabledTime__")
         self.isMemberOfTeamAmino: Optional[bool] = self.extensions.get("isMemberOfTeamAmino")
         self.privilegeOfChatInviteRequest: Optional[bool] = self.extensions.get("privilegeOfChatInviteRequest")
         self.privilegeOfCommentOnUserProfile: Optional[bool] = self.extensions.get("privilegeOfCommentOnUserProfile")
 
         # influencerInfo
-        self.influencerInfo: Optional[Dict] = data.get("influencerInfo", {})
+        self.influencerInfo: Optional[Dict] = data.get("influencerInfo") or {}
         self.fansCount: Optional[int] = self.influencerInfo.get("fansCount")
         self.influencerCreatedTime: Optional[int] = self.influencerInfo.get("createdTime")
         self.influencerMonthlyFee: Optional[int] = data.get("monthlyFee")
         self.influencerPinned: Optional[bool] = data.get("pinned")
 
         # adminInfo
         self.staffInfo: Optional[Dict] = data.get("adminInfo", {})
@@ -143,18 +143,16 @@
         _author, _quizQuestionList = [], []
 
         self.json = data
         self.nextPageToken = nextPageToken
         self.prevPageToken = prevPageToken
 
         for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
-            try: _quizQuestionList.append(QuizQuestionList(y["quizQuestionList"]).QuizQuestionList)
-            except (KeyError, TypeError): _quizQuestionList.append(None)
+            _author.append(y.get("author"))
+            _quizQuestionList.append(QuizQuestionList(y.get("quizQuestionList")).QuizQuestionList)
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.quizQuestionList = _quizQuestionList
 
         self.createdTime = []
         self.globalVotesCount = []
         self.globalVotedValue = []
```

### Comparing `amino.light.py-0.0.9/AminoLightPy/socket.py` & `amino.light.py-0.1.0/AminoLightPy/socket.py`

 * *Files 5% similar despite different names*

```diff
@@ -239,14 +239,102 @@
                 "params": {"blogType": blogType},
             },
             "t": 306
         }
         data = dumps(data)
         self.socket.send(data)
 
+    def Chatting(self, comId: int, chatId: str, threadType: int = 2):
+        """
+        Send Chatting Action
+
+        **Paramaters**
+            - **threadType**: 2 For Public 1 & 0 For Private (int)
+
+        **Return**
+            - **SetAction**:  (Class)
+        """
+        data = {
+            "o": {
+                "actions": ["Chatting"],
+                "target": f"ndc://x{comId}/chat-thread/{chatId}",
+                "ndcId": int(comId),
+                "params": {
+                    "duration": 12800,
+                    "membershipStatus": 1,
+                    "threadType": threadType
+                },
+            },
+            "t": 306
+        }
+        data = dumps(data)
+        self.socket.send(data)
+
+    def PublicChats(self, comId: int,):
+        """
+        Send PublicChats Action
+
+        **Return**
+            - **SetAction**:  (Class)
+        """
+        data = {
+            "o": {
+                "actions": ["Browsing"],
+                "target": f"ndc://x{comId}/public-chats",
+                "ndcId": int(comId),
+                "params": {"duration": 859},
+            },
+            "t": 306
+        }
+        data = dumps(data)
+        self.socket.send(data)
+
+    def LeaderBoards(self, comId: int,):
+        """
+        Send LeaderBoard Action
+
+        **Return**
+            - **SetAction**:  (Class)
+        """
+        data = {
+            "o": {
+                "actions": ["Browsing"],
+                "target": f"ndc://x{comId}/leaderboards",
+                "ndcId": int(comId),
+                "params": {"duration": 859},
+            },
+            "t": 306
+        }
+        data = dumps(data)
+        self.socket.send(data)
+
+    def start_video_chat(self, comId: str, chatId: str, joinType: int = 1):
+        data = {
+            "o": {
+                "ndcId": comId,
+                "threadId": chatId,
+                "joinRole": joinType,
+            },
+            "t": 112
+        }
+        data = dumps(data)
+        self.socket.send(data)
+
+        data = {
+            "o": {
+                "ndcId": int(comId),
+                "threadId": chatId,
+                "joinRole": joinType,
+                "channelType": 4,
+            },
+            "t": 108
+        }
+        data = dumps(data)
+        self.socket.send(data)
+
 
 class Callbacks:
     def __init__(self):
         self.handlers = {}
 
         self.methods = {
             304: self._resolve_chat_action_start,
```

### Comparing `amino.light.py-0.0.9/AminoLightPy/sub_client.py` & `amino.light.py-0.1.0/AminoLightPy/sub_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,14 +384,15 @@
     def clear_notifications(self):
         response = self.session.delete(f"{api}/x{self.comId}/s/notification")
         return response.status_code
 
     def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
+        elif isinstance(userId, tuple): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content
@@ -411,14 +412,15 @@
         
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread", json=data)
         return objects.Thread(response.json()["thread"]).Thread
 
     def invite_to_chat(self, userId: Union[str, list], chatId: str):
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
+        elif isinstance(userId, tuple): userIds = userId
         else: raise exceptions.WrongType(type(userId))
 
         data = { "uids": userIds }
         
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/member/invite", json=data)
         return response.status_code
```

### Comparing `amino.light.py-0.0.9/PKG-INFO` & `amino.light.py-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.0.9
+Version: 0.1.0
 Summary: Best Amino.py alternative
+Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: websocket-client
 
 # AminoLightPy
 ## _The best Amino.py alternative!_
 
 Why should you choose this library?
```

### Comparing `amino.light.py-0.0.9/README.md` & `amino.light.py-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.9/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.1.0/amino.light.py.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.0.9
+Version: 0.1.0
 Summary: Best Amino.py alternative
+Home-page: https://github.com/AugustLigh/AminoLightPy
 Author: AugustLight
 License: MIT
 Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: websocket-client
 
 # AminoLightPy
 ## _The best Amino.py alternative!_
 
 Why should you choose this library?
```

### Comparing `amino.light.py-0.0.9/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.1.0/amino.light.py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 AminoLightPy/__init__.py
 AminoLightPy/acm.py
 AminoLightPy/client.py
 AminoLightPy/constants.py
```

### Comparing `amino.light.py-0.0.9/setup.py` & `amino.light.py-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     'minori',
     'august',
     'augustlight'
 ]
 
 setup(
     name="amino.light.py",
-    version="0.0.9",
+    version="0.1.0",
+    url="https://github.com/AugustLigh/AminoLightPy",
     license="MIT",
     description="Best Amino.py alternative",
     author="AugustLight",
     packages=find_packages(),
     install_requires=["requests", "websocket-client"],
     long_description=long_description,
     long_description_content_type='text/markdown',
```

