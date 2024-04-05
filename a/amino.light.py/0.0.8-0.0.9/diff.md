# Comparing `tmp/amino.light.py-0.0.8.tar.gz` & `tmp/amino.light.py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.light.py-0.0.8.tar", last modified: Tue Apr  2 15:12:27 2024, max compression
+gzip compressed data, was "amino.light.py-0.0.9.tar", last modified: Fri Apr  5 22:39:34 2024, max compression
```

## Comparing `amino.light.py-0.0.8.tar` & `amino.light.py-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.161224 amino.light.py-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.129531 amino.light.py-0.0.8/AminoLightPy/
--rw-rw-rw-   0        0        0      287 2024-03-31 23:25:44.000000 amino.light.py-0.0.8/AminoLightPy/__init__.py
--rw-rw-rw-   0        0        0     9363 2024-03-29 00:27:12.000000 amino.light.py-0.0.8/AminoLightPy/acm.py
--rw-rw-rw-   0        0        0    70320 2024-03-30 19:18:45.000000 amino.light.py-0.0.8/AminoLightPy/client.py
--rw-rw-rw-   0        0        0     1513 2024-03-30 16:04:39.000000 amino.light.py-0.0.8/AminoLightPy/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.130530 amino.light.py-0.0.8/AminoLightPy/lib/
--rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.0.8/AminoLightPy/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.136534 amino.light.py-0.0.8/AminoLightPy/lib/util/
--rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.0.8/AminoLightPy/lib/util/__init__.py
--rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.0.8/AminoLightPy/lib/util/exceptions.py
--rw-rw-rw-   0        0        0     1238 2024-03-30 22:17:35.000000 amino.light.py-0.0.8/AminoLightPy/lib/util/helpers.py
--rw-rw-rw-   0        0        0   100212 2024-04-02 15:03:13.000000 amino.light.py-0.0.8/AminoLightPy/lib/util/objects.py
--rw-rw-rw-   0        0        0    11163 2024-03-29 01:00:51.000000 amino.light.py-0.0.8/AminoLightPy/socket.py
--rw-rw-rw-   0        0        0    73627 2024-03-30 19:42:47.000000 amino.light.py-0.0.8/AminoLightPy/sub_client.py
--rw-rw-rw-   0        0        0     1417 2024-04-02 15:12:27.161224 amino.light.py-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      878 2024-03-29 01:32:56.000000 amino.light.py-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 15:12:27.160222 amino.light.py-0.0.8/amino.light.py.egg-info/
--rw-rw-rw-   0        0        0     1417 2024-04-02 15:12:26.000000 amino.light.py-0.0.8/amino.light.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2024-04-02 15:12:27.000000 amino.light.py-0.0.8/amino.light.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 15:12:26.000000 amino.light.py-0.0.8/amino.light.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-02 15:12:26.000000 amino.light.py-0.0.8/amino.light.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-02 15:12:26.000000 amino.light.py-0.0.8/amino.light.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 15:12:27.163224 amino.light.py-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      889 2024-04-02 15:12:23.000000 amino.light.py-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.294325 amino.light.py-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.244815 amino.light.py-0.0.9/AminoLightPy/
+-rw-rw-rw-   0        0        0      286 2024-04-05 22:39:01.000000 amino.light.py-0.0.9/AminoLightPy/__init__.py
+-rw-rw-rw-   0        0        0     8472 2024-04-03 00:57:53.000000 amino.light.py-0.0.9/AminoLightPy/acm.py
+-rw-rw-rw-   0        0        0    65864 2024-04-05 22:01:03.000000 amino.light.py-0.0.9/AminoLightPy/client.py
+-rw-rw-rw-   0        0        0     2613 2024-04-05 22:38:53.000000 amino.light.py-0.0.9/AminoLightPy/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.247457 amino.light.py-0.0.9/AminoLightPy/lib/
+-rw-rw-rw-   0        0        0        0 2023-02-13 07:38:45.000000 amino.light.py-0.0.9/AminoLightPy/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.252808 amino.light.py-0.0.9/AminoLightPy/lib/util/
+-rw-rw-rw-   0        0        0       73 2024-03-27 16:01:15.000000 amino.light.py-0.0.9/AminoLightPy/lib/util/__init__.py
+-rw-rw-rw-   0        0        0    31621 2024-03-29 00:26:02.000000 amino.light.py-0.0.9/AminoLightPy/lib/util/exceptions.py
+-rw-rw-rw-   0        0        0     1238 2024-03-30 22:17:35.000000 amino.light.py-0.0.9/AminoLightPy/lib/util/helpers.py
+-rw-rw-rw-   0        0        0    96118 2024-04-05 22:01:47.000000 amino.light.py-0.0.9/AminoLightPy/lib/util/objects.py
+-rw-rw-rw-   0        0        0    14834 2024-04-05 02:48:00.000000 amino.light.py-0.0.9/AminoLightPy/socket.py
+-rw-rw-rw-   0        0        0    72389 2024-04-05 22:14:27.000000 amino.light.py-0.0.9/AminoLightPy/sub_client.py
+-rw-rw-rw-   0        0        0     1721 2024-04-05 22:39:34.294325 amino.light.py-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1019 2024-04-04 18:43:15.000000 amino.light.py-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-05 22:39:34.290329 amino.light.py-0.0.9/amino.light.py.egg-info/
+-rw-rw-rw-   0        0        0     1721 2024-04-05 22:39:32.000000 amino.light.py-0.0.9/amino.light.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2024-04-05 22:39:33.000000 amino.light.py-0.0.9/amino.light.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 22:39:32.000000 amino.light.py-0.0.9/amino.light.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-05 22:39:32.000000 amino.light.py-0.0.9/amino.light.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-05 22:39:32.000000 amino.light.py-0.0.9/amino.light.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-05 22:39:34.300326 amino.light.py-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2024-04-04 19:24:01.000000 amino.light.py-0.0.9/setup.py
```

### Comparing `amino.light.py-0.0.8/AminoLightPy/acm.py` & `amino.light.py-0.0.9/AminoLightPy/acm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import BinaryIO
+from requests import Session
 from time import time as timestamp
 
-from .constants import api, device_id
 from .lib.util import exceptions, objects
+from .constants import api, device_id, upload_media
 
 class ACM():
-    def __init__(self, profile: objects.UserProfile, comId: int = None):
-        self.session  = profile.session
+    def __init__(self, comId: int = None, *, profile: objects.UserProfile):
+        self.session: Session = profile.session
         self.profile = profile
         self.comId = comId
 
     # TODO : Finish the imaging sizing, might not work for every picture...
     def create_community(self, name: str, tagline: str, icon: BinaryIO, themeColor: str, joinType: int = 0, primaryLanguage: str = "en"):
         data = {
             "icon": {
                 "height": 512.0,
                 "imageMatrix": [1.6875, 0.0, 108.0, 0.0, 1.6875, 497.0, 0.0, 0.0, 1.0],
-                "path": self.upload_media(icon),
+                "path": upload_media(self, icon),
                 "width": 512.0,
                 "x": 0.0,
                 "y": 0.0
             },
             "joinType": joinType,
             "name": name,
             "primaryLanguage": primaryLanguage,
@@ -41,115 +42,109 @@
                 },
                 "type": 1,
                 "identity": email
             },
             "deviceID": device_id
         }
 
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"{api}/g/s-x{self.comId}/community/delete-request", json=data)
         return response.status_code
 
     def list_communities(self, start: int = 0, size: int = 25):
         response = self.session.get(f"{api}/g/s/community/managed?start={start}&size={size}")
         return objects.CommunityList(response.json()["communityList"]).CommunityList
 
     def get_categories(self, start: int = 0, size: int = 25):
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.get(f"{api}/x{self.comId}/s/blog-category?start={start}&size={size}")
         return response.json()
 
     def change_sidepanel_color(self, color: str):
         data = {
             "path": "appearance.leftSidePanel.style.iconColor",
             "value": color
         }
 
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"{api}/x{self.comId}/s/community/configuration", json=data)
         return response.json()
 
     def promote(self, userId: str, rank: str):
         rank = rank.lower().replace("agent", "transfer-agent")
 
         if rank.lower() not in ["transfer-agent", "leader", "curator"]:
             raise exceptions.WrongType(rank)
 
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"{api}/x{self.comId}/s/user-profile/{userId}/{rank}")
         return response.status_code
 
     def get_join_requests(self, start: int = 0, size: int = 25):
-        if self.comId is None: raise exceptions.CommunityNeeded()
-
-        response = self.session.get(f"{api}/x{self.comId}/s/community/membership-request?status=pending&start={start}&size={size}")
+        data = {
+            "status": "pending",
+            "start": start,
+            "size": size
+        }
+        
+        response = self.session.get(f"{api}/x{self.comId}/s/community/membership-request", params=data)
         return objects.JoinRequest(response.json()).JoinRequest
 
     def accept_join_request(self, userId: str):
         data = dict()
-
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"{api}/x{self.comId}/s/community/membership-request/{userId}/accept", json=data)
         return response.status_code
 
     def reject_join_request(self, userId: str):
         data = dict()
-
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"{api}/x{self.comId}/s/community/membership-request/{userId}/reject", json=data)
         return response.status_code
 
     def get_community_stats(self):
-        if self.comId is None: raise exceptions.CommunityNeeded()
-
         response = self.session.get(f"{api}/x{self.comId}/s/community/stats")
         if response.status_code != 200: return exceptions.CheckException(response.text)
         else: return objects.CommunityStats(response.json()["communityStats"]).CommunityStats
 
     def get_community_user_stats(self, type: str, start: int = 0, size: int = 25):
-        if self.comId is None: raise exceptions.CommunityNeeded()
-
         if type.lower() == "leader": target = "leader"
         elif type.lower() == "curator": target = "curator"
         else: raise exceptions.WrongType(type)
 
-        response = self.session.get(f"{api}/x{self.comId}/s/community/stats/moderation?type={target}&start={start}&size={size}")
+        data = {
+            "type": target,
+            "start": start,
+            "size": size
+        }
+
+        response = self.session.get(f"{api}/x{self.comId}/s/community/stats/moderation", params=data)
         return objects.UserProfileList(response.json()["userProfileList"]).UserProfileList
 
     def change_welcome_message(self, message: str, isEnabled: bool = True):
         data = {
             "path": "general.welcomeMessage",
             "value": {
                 "enabled": isEnabled,
                 "text": message
             }
         }
 
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"{api}/x{self.comId}/s/community/configuration", json=data)
         return response.status_code
 
     def change_guidelines(self, message: str):
         data = { "content": message }
-
-        if self.comId is None: raise exceptions.CommunityNeeded()
+        
         response = self.session.post(f"{api}/x{self.comId}/s/community/guideline", json=data)
         return response.status_code
 
     def edit_community(self, name: str = None, description: str = None, aminoId: str = None, primaryLanguage: str = None, themePackUrl: str = None):
         data = {"timestamp": int(timestamp() * 1000)}
 
         if name is not None: data["name"] = name
         if description is not None: data["content"] = description
         if aminoId is not None: data["endpoint"] = aminoId
         if primaryLanguage is not None: data["primaryLanguage"] = primaryLanguage
         if themePackUrl is not None: data["themePackUrl"] = themePackUrl
-
-
-        if self.comId is None: raise exceptions.CommunityNeeded()
+        
         response = self.session.post(f"{api}/x{self.comId}/s/community/settings", json=data)
         return response.status_code
 
     def change_module(self, module: str, isEnabled: bool):
         if module.lower() == "chat": mod = "module.chat.enabled"
         elif module.lower() == "livechat": mod = "module.chat.avChat.videoEnabled"
         elif module.lower() == "screeningroom": mod = "module.chat.avChat.screeningRoomEnabled"
@@ -169,34 +164,29 @@
         else: raise exceptions.SpecifyType()
 
         data = {
             "path": mod,
             "value": isEnabled
         }
 
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"{api}/x{self.comId}/s/community/configuration", json=data)
         return response.status_code
 
     def add_influencer(self, userId: str, monthlyFee: int):
         data = {
             "monthlyFee": monthlyFee
         }
 
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.post(f"{api}/x{self.comId}/s/influencer/{userId}", json=data)
         return response.status_code
 
     def remove_influencer(self, userId: str):
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.delete(f"{api}/x{self.comId}/s/influencer/{userId}")
         return response.status_code
 
     def get_notice_list(self, start: int = 0, size: int = 25):
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.get(f"{api}/x{self.comId}/s/notice?type=management&status=1&start={start}&size={size}")
         return objects.NoticeList(response.json()["noticeList"]).NoticeList
 
     def delete_pending_role(self, noticeId: str):
-        if self.comId is None: raise exceptions.CommunityNeeded()
         response = self.session.delete(f"{api}/x{self.comId}/s/notice/{noticeId}")
         return response.status_code
```

### Comparing `amino.light.py-0.0.8/AminoLightPy/client.py` & `amino.light.py-0.0.9/AminoLightPy/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,162 +1,42 @@
 from uuid import uuid4
-from json import dumps
-from .constants import *
 from base64 import b64encode
-from threading import Thread
-from time import timezone, sleep
 from typing import BinaryIO, Union
-from locale import getdefaultlocale as locale
 
-from .socket import Callbacks, SocketHandler
+from .constants import *
 from .lib.util import exceptions, objects, helpers
+from .socket import Callbacks, SocketHandler, SocketRequests
 
 
 #@dorthegra/IDörthe#8835 thanks for support!
 
-class Client(Callbacks, SocketHandler):
+class Client(Callbacks, SocketHandler, SocketRequests):
     def __init__(self, proxies: dict = None, socketDebugging = False, socket_enabled = True):
         self.authenticated = False
-        self.session = CustomSession()
+        self.session = AminoSession()
 
         self.socket_enabled = socket_enabled
         if socket_enabled:
-            SocketHandler.__init__(self, self, socketDebugging)
+            handler = SocketHandler.__init__(self, self, socketDebugging)
+            SocketRequests.__init__(self, handler)
             Callbacks.__init__(self)
 
         self.session.proxies = proxies
 
         self.sid = None
         self.profile: objects.UserProfile = objects.UserProfile(None).UserProfile
+        self.profile.session = self.session
 
-        self.active_live_chats = set()
-
-    @socket_required
-    def join_voice_chat(self, comId: int, chatId: str, joinType: int = 1):
-        """
-        Joins a Voice Chat
-        **Parameters**
-            - **comId** : ID of the Community
-            - **chatId** : ID of the Chat
-        """
-
-        # Made by Light, Ley and Phoenix
-
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-            },
-            "t": 112
-        }
-        data = dumps(data)
-        self.send(data)
-
-    @socket_required
-    def join_video_chat(self, comId: int, chatId: str, joinType: int = 1):
-        """
-        Joins a Video Chat
-        **Parameters**
-            - **comId** : ID of the Community
-            - **chatId** : ID of the Chat
-        """
-
-        # Made by Light, Ley and Phoenix
 
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-                "channelType": 5,
-            },
-            "t": 108
-        }
-        data = dumps(data)
-        self.send(data)
+    def parse_headers(self, data: str = None) -> dict:
+        base_headers: dict = self.session.headers
+        if data:
+            base_headers["NDC-MSG-SIG"] = helpers.signature(data)
 
-    @socket_required
-    def join_video_chat_as_viewer(self, comId: int, chatId: str):
-        data = {
-            "o":
-                {
-                    "ndcId": int(comId),
-                    "threadId": chatId,
-                    "joinRole": 2,
-                },
-            "t": 112
-        }
-        data = dumps(data)
-        self.send(data)
-    
-    @socket_required
-    # Fixed by vedansh#4039
-    def leave_from_live_chat(self, chatId: str):
-        if chatId in self.active_live_chats:
-            self.active_live_chats.remove(chatId)
-
-    @socket_required
-    def run_vc(self, comId: int, chatId: str, joinType: str):
-        while chatId in self.active_live_chats:
-            try:
-                data = {
-                    "o": {
-                        "ndcId": int(comId),
-                        "threadId": chatId,
-                        "joinRole": joinType,
-                    },
-                    "t": 112
-                }
-                data = dumps(data)
-                self.send(data)
-                sleep(60)
-
-            except Exception as e:
-                print(e)
-
-    @socket_required
-    def start_vc(self, comId: int, chatId: str, joinType: int = 1):
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-            },
-            "t": 112
-        }
-        data = dumps(data)
-        self.send(data)
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "channelType": 1,
-            },
-            "t": 108
-        }
-        data = dumps(data)
-        self.send(data)
-        self.active_live_chats.add(chatId)
-        Thread(target=self.run_vc, args=(comId, chatId, joinType)).start()
-
-    @socket_required
-    def end_vc(self, comId: int, chatId: str, joinType: int = 2):
-        self.leave_from_live_chat(chatId)
-        data = {
-            "o": {
-                "ndcId": int(comId),
-                "threadId": chatId,
-                "joinRole": joinType,
-            },
-            "t": 112
-        }
-        data = dumps(data)
-        self.send(data)
-        self.active_live_chats.remove(chatId)
+        return base_headers
 
 
     def login_sid(self, SID: str):
         """
         Login into an account with an SID
 
         **Parameters**
@@ -409,17 +289,17 @@
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if gender.lower() == "male": gender = 1
         elif gender.lower() == "female": gender = 2
         elif gender.lower() == "non-binary": gender = 255
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
-        if age <= 12: raise exceptions.AgeTooLow()
+        if age <= 12: raise exceptions.AgeTooLow
 
         data = {
             "age": age,
             "gender": gender,
         }
 
         response = self.session.post(f"{api}/g/s/persona/profile/basic", json=data)
@@ -550,65 +430,19 @@
             "phoneNumberValidationContext": None,
             "deviceID": device_id
         }
 
         response = self.session.post(f"{api}/g/s/auth/reset-password", json=data)
         return response.status_code
 
-    def check_device(self, deviceId: str):
-        """
-        Check if the Device ID is valid.
-
-        **Parameters**
-            - **deviceId** : ID of the Device.
-
-        **Returns**
-            - **Success** : 200 (int)
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        data = {
-            "deviceID": deviceId,
-            "bundleID": "com.narvii.amino.master",
-            "clientType": 100,
-            "timezone": timezone // 1000,
-            "systemPushEnabled": True,
-            "locale": locale()[0]
-        }
-
-        response = self.session.post(f"{api}/g/s/device", json=data)
-        return response.status_code
 
     def get_account_info(self):
         response = self.session.get(f"{api}/g/s/account")
         return objects.UserProfile(response.json()["account"]).UserProfile
 
-    def upload_media(self, file: BinaryIO, fileType: str):
-        """
-        Upload file to the amino servers.
-
-        **Parameters**
-            - **file** : File to be uploaded.
-
-        **Returns**
-            - **Success** : Url of the file uploaded to the server.
-
-            - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
-        """
-        if fileType == "audio":
-            t = "audio/aac"
-        elif fileType == "image":
-            t = "image/jpg"
-        else: raise exceptions.SpecifyType(fileType)
-
-        data = file.read()
-        #TODO
-        response = self.session.post(f"{api}/g/s/media/upload", data=data, headers={"Content-Type": t})
-        return response.json()["mediaValue"]
-
     def handle_socket_message(self, data):
         return self.resolve(data)
 
     def get_eventlog(self):
         response = self.session.get(f"{api}/g/s/eventlog/profile?language=en")
         return response.json()
 
@@ -621,20 +455,20 @@
             - *size* : Size of the list.
 
         **Returns**
             - **Success** : :meth:`Community List <amino.lib.util.objects.CommunityList>`
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if not self.authenticated: raise exceptions.NotLoggedIn()
+        if not self.authenticated: raise exceptions.NotLoggedIn
         response = self.session.get(f"{api}/g/s/community/joined?v=1&start={start}&size={size}")
         return objects.CommunityList(response.json()["communityList"]).CommunityList
 
     def sub_clients_profile(self, start: int = 0, size: int = 25):
-        if not self.authenticated: raise exceptions.NotLoggedIn()
+        if not self.authenticated: raise exceptions.NotLoggedIn
         response = self.session.get(f"{api}/g/s/community/joined?v=1&start={start}&size={size}")
         return response.json()["userInfoInCommunities"]
 
     def get_user_info(self, userId: str):
         """
         Information of an User.
 
@@ -730,15 +564,15 @@
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
         if isinstance(userId, str): userIds = [userId]
         elif isinstance(userId, list): userIds = userId
-        else: raise exceptions.WrongType()
+        else: raise exceptions.WrongType
 
         data = {
             "title": title,
             "inviteeUids": userIds,
             "initialMessageContent": message,
             "content": content,
         }
@@ -929,15 +763,15 @@
 
         if blogId or quizId:
             if not quizId: 
                 blogId = quizId
             url = f"{api}/g/s/blog/{blogId}/comment?sort={sorting}&start={start}&size={size}"
         elif wikiId: url = f"{api}/g/s/item/{wikiId}/comment?sort={sorting}&start={start}&size={size}"
         elif fileId: url = f"{api}/g/s/shared-folder/files/{fileId}/comment?sort={sorting}&start={start}&size={size}",
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         response = self.session.get(url)
         return objects.CommentList(response.json()["commentList"]).CommentList
 
     def get_blocker_users(self, start: int = 0, size: int = 25):
         """
         List of Users that are Blocking the User.
@@ -1019,14 +853,17 @@
 
         if asGuest: flg = "g-flag"
         else: flg = "flag"
 
         response = self.session.post(f"{api}/g/s/{flg}", json=data)
         return response.status_code
 
+    def check_values(self, *args):
+        return any(arg is None for arg in args)
+
     def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
         """
         Send a Message to a Chat.
 
         **Parameters**
             - **message** : Message to be sent
             - **chatId** : ID of the Chat.
@@ -1045,38 +882,45 @@
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
 
-        if message is not None and file is None:
-            message = message.replace("<$", "‎‏").replace("$>", "‬‭")
-
-        mentions = []
-        if mentionUserIds:
-            for mention_uid in mentionUserIds:
-                mentions.append({"uid": mention_uid})
-
-        if embedImage:
-            embedImage = [[100, self.upload_media(embedImage, "image"), None]]
-
         data = {
             "type": messageType,
-            "content": message,
-            "attachedObject": {
-                "objectId": embedId,
-                "objectType": embedType,
-                "link": embedLink,
-                "title": embedTitle,
-                "content": embedContent,
-                "mediaList": embedImage
-            },
-            "extensions": {"mentionedArray": mentions},
+            "content": message
         }
+        
+        if self.check_values(embedId, embedType, embedLink, embedTitle, embedContent, embedImage):
+            attachedObject = dict()
+
+            if embedId:
+                attachedObject["objectId"] = embedId
+
+            if embedType:
+                attachedObject["objectType"] = embedType
+
+            if embedLink:
+                attachedObject["link"] = embedLink
+
+            if embedTitle:
+                attachedObject["title"] = embedTitle
+
+            if embedContent:
+                attachedObject["content"] = embedContent
+
+            if embedImage:
+                attachedObject["mediaList"] = [[100, upload_media(self, embedImage, "image"), None]]
+
+            data["attachedObject"] = attachedObject
+        
+        if mentionUserIds:
+            mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
+            data["extensions"] = {"mentionedArray": mentions}
 
         if replyTo: data["replyMessageId"] = replyTo
 
         if stickerId:
             data["content"] = None
             data["stickerId"] = stickerId
             data["type"] = 3
@@ -1093,15 +937,15 @@
                 data["mediaUhqEnabled"] = True
 
             elif fileType == "gif":
                 data["mediaType"] = 100
                 data["mediaUploadValueContentType"] = "image/gif"
                 data["mediaUhqEnabled"] = True
 
-            else: raise exceptions.SpecifyType
+            else: raise exceptions.SpecifyType(fileType)
 
             data["mediaUploadValue"] = b64encode(file.read()).decode()
 
         response = self.session.post(f"{api}/g/s/chat/thread/{chatId}/message", json=data)
         return response.status_code
 
     def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
@@ -1276,15 +1120,15 @@
         if blogId != None: url = f"{api}/g/s/blog/{blogId}/tipping"
         if chatId != None: url = f"{api}/g/s/chat/thread/{chatId}/tipping"
         if objectId != None:
             data["objectId"] = objectId
             data["objectType"] = 2
             url = f"{api}/g/s/tipping"
 
-        if url is None: raise exceptions.SpecifyType()
+        if url is None: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
         return response.status_code
 
     def follow(self, userId: Union[str, list]):
         """
         Follow an User or Multiple Users.
@@ -1458,15 +1302,15 @@
             "latitude": 0,
             "longitude": 0,
             "mediaList": None,
             "eventSource": "UserProfileView",
         }
 
         if nickname: data["nickname"] = nickname
-        if icon: data["icon"] = self.upload_media(icon, "image")
+        if icon: data["icon"] = upload_media(self, icon, "image")
         if content: data["content"] = content
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
         if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
 
         response = self.session.post(f"{api}/g/s/user-profile/{self.profile.userId}", json=data)
         return response.status_code
@@ -1666,15 +1510,15 @@
 
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
             
             url = f"{api}/g/s/item/{wikiId}/g-vote?cv=1.2"
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
         return response.status_code
 
     def unlike_blog(self, blogId: str = None, wikiId: str = None):
         """
         Remove a like from a Blog or Wiki.
```

### Comparing `amino.light.py-0.0.8/AminoLightPy/lib/util/exceptions.py` & `amino.light.py-0.0.9/AminoLightPy/lib/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.8/AminoLightPy/lib/util/helpers.py` & `amino.light.py-0.0.9/AminoLightPy/lib/util/helpers.py`

 * *Files identical despite different names*

### Comparing `amino.light.py-0.0.8/AminoLightPy/lib/util/objects.py` & `amino.light.py-0.0.9/AminoLightPy/lib/util/objects.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # You don't even know how long this shit took...
 # F*ck you Sand for making me do this.
 
-class Objects:
-    class Users:
-        team_amino = "000000000-0000-0000-0000-000000000000"
-        news_feed = "000000000-0000-0000-0000-000000000001"
+from typing import List, Optional, Dict, TypeVar
 
 class UserProfile:
     __slots__ = (
         "json", "fanClub", "accountMembershipStatus", "activation", "activePublicLiveThreadId",
         "age", "aminoId", "aminoIdEditable", "avatarFrame", "avatarFrameId",
         "blogsCount", "commentsCount", "content", "createdTime",
         "followersCount", "followingCount", "followingStatus", "gender",
@@ -23,105 +20,106 @@
         "disabledLevel", "disabledStatus", "disabledTime", "isMemberOfTeamAmino",
         "privilegeOfChatInviteRequest", "privilegeOfCommentOnUserProfile", "influencerInfo",
         "fansCount", "influencerCreatedTime", "influencerMonthlyFee", "influencerPinned",
         "staffInfo", "globalStrikeCount", "lastStrikeTime", "lastWarningTime", "strikeCount",
         "warningCount", "session"
     )
 
-    def __init__(self, data: dict):
-        if not data:
+    def __init__(self, data: Dict):
+        if data is None:
             for attr in self.__slots__:
                 setattr(self, attr, None)
         
             return
 
-        self.json = data
+        self.json: Optional[Dict] = data
 
-        self.fanClub = FanClubList(data.get("fanClubList", [])).FanClubList if data else None
+        self.fanClub = FanClubList(data.get("fanClubList", [])).FanClubList
 
-        self.accountMembershipStatus = data.get("accountMembershipStatus")
-        self.activation = data.get("activation")
-        self.activePublicLiveThreadId = data.get("activePublicLiveThreadId")
-        self.age = data.get("age")
-        self.aminoId = data.get("aminoId")
-        self.aminoIdEditable = data.get("aminoIdEditable")
-        self.avatarFrame = data.get("avatarFrame")
-        self.avatarFrameId = data.get("avatarFrameId")
-        self.blogsCount = data.get("blogsCount")
-        self.commentsCount = data.get("commentsCount")
-        self.content = data.get("content")
-        self.createdTime = data.get("createdTime")
-        self.followersCount = data.get("membersCount")
-        self.followingCount = data.get("joinedCount")
-        self.followingStatus = data.get("followingStatus")
-        self.gender = data.get("gender")
-        self.icon = data.get("icon")
-        self.isGlobal = data.get("isGlobal")
-        self.isNicknameVerified = data.get("isNicknameVerified")
-        self.itemsCount = data.get("itemsCount")
-        self.level = data.get("level")
-        self.mediaList = data.get("mediaList")
-        self.membershipStatus = data.get("membershipStatus")
-        self.modifiedTime = data.get("modifiedTime")
-        self.mood = data.get("mood")
-        self.moodSticker = data.get("moodSticker")
-        self.nickname = data.get("nickname")
-        self.notificationSubscriptionStatus = data.get("notificationSubscriptionStatus")
-        self.onlineStatus = data.get("onlineStatus")
-        self.onlineStatus2 = data.get("settings", {}).get("onlineStatus")
-        self.postsCount = data.get("postsCount")
-        self.pushEnabled = data.get("pushEnabled")
-        self.race = data.get("race")
-        self.reputation = data.get("reputation")
-        self.role = data.get("role")
-        self.securityLevel = data.get("securityLevel")
-        self.status = data.get("status")
-        self.storiesCount = data.get("storiesCount")
-        self.tagList = data.get("tagList")
-        self.userId = data.get("uid")
-        self.verified = data.get("verified")
-        self.totalQuizHighestScore = data.get("totalQuizHighestScore")
-        self.totalQuizPlayedTimes = data.get("totalQuizPlayedTimes")
-        self.requestId = data.get("requestId")
-        self.message = data.get("message")
-        self.applicant = data.get("applicant")
-        self.avgDailySpendTimeIn7Days = data.get("avgDailySpendTimeIn7Days")
-        self.adminLogCountIn7Days = data.get("adminLogCountIn7Days")
+        self.accountMembershipStatus: Optional[int] = data.get("accountMembershipStatus")
+        self.activation: Optional[int] = data.get("activation")
+        self.activePublicLiveThreadId: Optional[str] = data.get("activePublicLiveThreadId")
+        self.age: Optional[int] = data.get("age")
+        self.aminoId: Optional[str] = data.get("aminoId")
+        self.aminoIdEditable: Optional[bool] = data.get("aminoIdEditable")
+        self.avatarFrame: Optional[str] = data.get("avatarFrame")
+        self.avatarFrameId: Optional[str] = data.get("avatarFrameId")
+        self.blogsCount: Optional[int] = data.get("blogsCount")
+        self.commentsCount: Optional[int] = data.get("commentsCount")
+        self.content: Optional[str] = data.get("content")
+        self.createdTime: Optional[int] = data.get("createdTime")
+        self.followersCount: Optional[int] = data.get("followersCount")
+        self.followingCount: Optional[int] = data.get("followingCount")
+        self.followingStatus: Optional[int] = data.get("followingStatus")
+        self.gender: Optional[str] = data.get("gender")
+        self.icon: Optional[str] = data.get("icon")
+        self.isGlobal: Optional[bool] = data.get("isGlobal")
+        self.isNicknameVerified: Optional[bool] = data.get("isNicknameVerified")
+        self.itemsCount: Optional[int] = data.get("itemsCount")
+        self.level: Optional[int] = data.get("level")
+        self.mediaList: Optional[MediaObject] = data.get("mediaList")
+        self.membershipStatus: Optional[int] = data.get("membershipStatus")
+        self.modifiedTime: Optional[int] = data.get("modifiedTime")
+        self.mood: Optional[str] = data.get("mood")
+        self.moodSticker: Optional[str] = data.get("moodSticker")
+        self.nickname: Optional[str] = data.get("nickname")
+        self.notificationSubscriptionStatus: Optional[int] = data.get("notificationSubscriptionStatus")
+        self.onlineStatus: Optional[int] = data.get("onlineStatus")
+        self.onlineStatus2: Optional[int] = data.get("onlineStatus2")
+        self.postsCount: Optional[int] = data.get("postsCount")
+        self.pushEnabled: Optional[bool] = data.get("pushEnabled")
+        self.race: Optional[str] = data.get("race")
+        self.reputation: Optional[int] = data.get("reputation")
+        self.role: Optional[str] = data.get("role")
+        self.securityLevel: Optional[int] = data.get("securityLevel")
+        self.status: Optional[str] = data.get("status")
+        self.storiesCount: Optional[int] = data.get("storiesCount")
+        self.tagList: Optional[List[str]] = data.get("tagList")
+        self.userId: Optional[str] = data.get("uid")
+        self.verified: Optional[bool] = data.get("verified")
+        self.totalQuizHighestScore: Optional[int] = data.get("totalQuizHighestScore")
+        self.totalQuizPlayedTimes: Optional[int] = data.get("totalQuizPlayedTimes")
+        self.requestId: Optional[str] = data.get("requestId")
+        self.message: Optional[str] = data.get("message")
+        self.applicant: Optional[str] = data.get("applicant")
+        self.avgDailySpendTimeIn7Days: Optional[int] = data.get("avgDailySpendTimeIn7Days")
+        self.adminLogCountIn7Days: Optional[int] = data.get("adminLogCountIn7Days")
+
+        # extensions
+        self.extensions: Optional[Dict] = data.get("extensions") or {}
+        # style
+        self.style: Optional[Dict] = self.extensions.get("style", {})
+        self.backgroundImage: Optional[str] = self.style.get("backgroundImage")
+        self.backgroundColor: Optional[str] = self.style.get("backgroundColor")
+
+        self.coverAnimation: Optional[str] = self.extensions.get("coverAnimation")
+        self.customTitles: Optional[List[str]] = self.extensions.get("customTitles")
+        self.defaultBubbleId: Optional[str] = self.extensions.get("defaultBubbleId")
+        self.disabledLevel: Optional[int] = self.extensions.get("__disabledLevel__")
+        self.disabledStatus: Optional[str] = self.extensions.get("__disabledStatus__")
+        self.disabledTime: Optional[int] = self.extensions.get("__disabledTime__")
+        self.isMemberOfTeamAmino: Optional[bool] = self.extensions.get("isMemberOfTeamAmino")
+        self.privilegeOfChatInviteRequest: Optional[bool] = self.extensions.get("privilegeOfChatInviteRequest")
+        self.privilegeOfCommentOnUserProfile: Optional[bool] = self.extensions.get("privilegeOfCommentOnUserProfile")
+
+        # influencerInfo
+        self.influencerInfo: Optional[Dict] = data.get("influencerInfo", {})
+        self.fansCount: Optional[int] = self.influencerInfo.get("fansCount")
+        self.influencerCreatedTime: Optional[int] = self.influencerInfo.get("createdTime")
+        self.influencerMonthlyFee: Optional[int] = data.get("monthlyFee")
+        self.influencerPinned: Optional[bool] = data.get("pinned")
+
+        # adminInfo
+        self.staffInfo: Optional[Dict] = data.get("adminInfo", {})
+        self.globalStrikeCount: Optional[int] = self.staffInfo.get("globalStrikeCount")
+        self.lastStrikeTime: Optional[int] = self.staffInfo.get("lastStrikeTime")
+        self.lastWarningTime: Optional[int] = self.staffInfo.get("lastWarningTime")
+        self.strikeCount: Optional[int] = self.staffInfo.get("strikeCount")
+        self.warningCount: Optional[int] = self.staffInfo.get("warningCount")
 
-        #extensions
-        self.extensions = data.get("extensions", {"style": {}})
-        #style
-        self.style = self.extensions.get("style", {}) if self.extensions else {}
-        self.backgroundImage = self.style.get("backgroundImage") 
-        self.backgroundColor = self.style.get("backgroundColor")
-
-        self.coverAnimation = self.extensions.get("coverAnimation") if self.extensions else None
-        self.customTitles = self.extensions.get("customTitles") if self.extensions else None
-        self.defaultBubbleId = self.extensions.get("defaultBubbleId") if self.extensions else None
-        self.disabledLevel = self.extensions.get("__disabledLevel__") if self.extensions else None
-        self.disabledStatus = self.extensions.get("__disabledStatus__") if self.extensions else None
-        self.disabledTime = self.extensions.get("__disabledTime__") if self.extensions else None
-        self.isMemberOfTeamAmino = self.extensions.get("isMemberOfTeamAmino") if self.extensions else None
-        self.privilegeOfChatInviteRequest = self.extensions.get("privilegeOfChatInviteRequest") if self.extensions else None
-        self.privilegeOfCommentOnUserProfile = self.extensions.get("privilegeOfCommentOnUserProfile") if self.extensions else None
-        
-        #influencerInfo
-        self.influencerInfo = data.get("influencerInfo", {})
-        self.fansCount = self.influencerInfo.get("fansCount") if self.influencerInfo else None
-        self.influencerCreatedTime = self.influencerInfo.get("createdTime") if self.influencerInfo else None
-        self.influencerMonthlyFee = data.get("monthlyFee") if self.influencerInfo else None
-        self.influencerPinned = data.get("pinned") if self.influencerInfo else None
-
-        #adminInfo
-        self.staffInfo = data.get("adminInfo", {})
-        self.globalStrikeCount = self.staffInfo.get("globalStrikeCount") if self.staffInfo else None
-        self.lastStrikeTime = self.staffInfo.get("lastStrikeTime") if self.staffInfo else None
-        self.lastWarningTime = self.staffInfo.get("lastWarningTime") if self.staffInfo else None
-        self.strikeCount = self.staffInfo.get("strikeCount") if self.staffInfo else None
-        self.warningCount = self.staffInfo.get("warningCount") if self.staffInfo else None
 
         
         self.session = None
 
     @property
     def UserProfile(self):
 
@@ -130,18 +128,15 @@
 class UserProfileList:
     __slots__ = UserProfile.__slots__
 
     def __init__(self, data):
         self.json = data
         _userObjects = tuple(UserProfile(x).UserProfile for x in data)
 
-        if _userObjects:
-            attributes = tuple(attr for attr in dir(_userObjects[0]) if not attr.startswith('__') and not callable(getattr(_userObjects[0], attr)) and attr != _userObjects[0].__class__.__name__)
-            for attr in attributes:
-                setattr(self, attr, tuple(getattr(user, attr, None) for user in _userObjects))
+        set_attributes(self, _userObjects)
 
     @property
     def UserProfileList(self):
         return self
 
 class BlogList:
     def __init__(self, data, nextPageToken = None, prevPageToken = None):
@@ -160,15 +155,15 @@
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.quizQuestionList = _quizQuestionList
 
         self.createdTime = []
         self.globalVotesCount = []
         self.globalVotedValue = []
         self.keywords = []
-        self.mediaList = []
+        self.mediaList: Optional[List[MediaObject]] = []
         self.style = []
         self.totalQuizPlayCount = []
         self.title = []
         self.tipInfo = []
         self.tippersCount = []
         self.tippable = []
         self.tippedCoins = []
@@ -310,15 +305,15 @@
         extensions = self.json.get("extensions", {})
         tipInfo = self.json.get("tipInfo", {})
         style = extensions.get("style", {})
 
         self.globalVotesCount = self.json.get("globalVotesCount")
         self.globalVotedValue = self.json.get("globalVotedValue")
         self.keywords = self.json.get("keywords")
-        self.mediaList = self.json.get("mediaList")
+        self.mediaList: Optional[MediaObject] = self.json.get("mediaList")
         self.style = self.json.get("style")
         self.totalQuizPlayCount = self.json.get("totalQuizPlayCount")
         self.title = self.json.get("title")
         self.tipInfo = tipInfo
         self.tippersCount = tipInfo.get("tippersCount")
         self.tippable = tipInfo.get("tippable")
         self.tippedCoins = tipInfo.get("tippedCoins")
@@ -384,40 +379,37 @@
         self.keywords = self.json.get("keywords")
         self.needHidden = self.json.get("needHidden")
         self.guestVotesCount = self.json.get("guestVotesCount")
         self.extensions = extensions
         self.votesCount = self.json.get("votesCount")
         self.comId = self.json.get("ndcId")
         self.createdTime = self.json.get("createdTime")
-        self.mediaList = self.json.get("mediaList")
+        self.mediaList: Optional[MediaObject] = self.json.get("mediaList")
         self.commentsCount = self.json.get("commentsCount")
         self.backgroundColor = style.get("backgroundColor")
         self.fansOnly = extensions.get("fansOnly")
         self.knowledgeBase = knowledgeBase
         self.version = knowledgeBase.get("version")
         self.originalWikiId = knowledgeBase.get("originalItemId")
         self.contributors = knowledgeBase.get("contributors")
 
     @property
     def Wiki(self):
         return self
 
 class WikiList:
-    def __init__(self, data: dict):
+    def __init__(self, data: Dict):
         self.json = data
 
-        self.author = UserProfileList([y.get("author") for y in data]).UserProfileList
+        self.author = UserProfileList(tuple(y.get("author") for y in data)).UserProfileList
         self.labels = tuple(WikiLabelList(y["extensions"]["props"]).WikiLabelList if "extensions" in y and "props" in y["extensions"] else None for y in data)
 
         _wikiObjects = tuple(Wiki(x).Wiki for x in data)
 
-        if _wikiObjects:
-            attributes = tuple(attr for attr in dir(_wikiObjects[0]) if not attr.startswith('__') and not callable(getattr(_wikiObjects[0], attr)) and attr != _wikiObjects[0].__class__.__name__)
-            for attr in attributes:
-                setattr(self, attr, tuple(getattr(user, attr, None) for user in _wikiObjects))
+        set_attributes(self, _wikiObjects)
 
     @property
     def WikiList(self):
 
         return self
 
 
@@ -460,42 +452,48 @@
         "pollMinFullBarVoteCount", "leaderboardStyle", "facebookAppIdList",
         "welcomeMessage", "welcomeMessageEnabled", "hasPendingReviewRequest",
         "frontPageLayout", "themeColor", "themeHash", "themeVersion", "themeUrl",
         "themeHomePageAppearance", "themeLeftSidePanelTop", "themeLeftSidePanelBottom",
         "themeLeftSidePanelColor", "customList"
     )
 
-    def __init__(self, data):
+    def __init__(self, data: Dict):
+        if data is None:
+            for attr in self.__slots__:
+                setattr(self, attr, None)
+        
+            return
+
         self.json = data
 
-        try: self.agent: UserProfile = UserProfile(data["agent"]).UserProfile
-        except (KeyError, TypeError): self.agent: UserProfile = UserProfile([])
+        self.agent: UserProfile = UserProfile(data.get("agent", [])).UserProfile
+
         try: self.rankingTable: RankingTableList = RankingTableList(data["advancedSettings"]["rankingTable"]).RankingTableList
         except (KeyError, TypeError): self.rankingTable: RankingTableList = RankingTableList([])
 
-        themePack = self.json.get("themePack", {})
-        configuration = self.json.get("configuration", {})
-        appearance = configuration.get("appearance", {})
-        leftSidePanel = appearance.get("leftSidePanel", {})
-        style = leftSidePanel.get("style", {})
-        page = configuration.get("page", {})
-        advancedSettings = self.json.get("advancedSettings", {})
-        extensions = self.json.get("extensions", {})
-
-        self.name = self.json.get("name")
-        self.usersCount = self.json.get("membersCount")
-        self.createdTime = self.json.get("createdTime")
-        self.aminoId = self.json.get("endpoint")
-        self.icon = self.json.get("icon")
-        self.link = self.json.get("link")
-        self.comId = self.json.get("ndcId")
-        self.modifiedTime = self.json.get("modifiedTime")
-        self.status = self.json.get("status")
-        self.joinType = self.json.get("joinType")
-        self.primaryLanguage = self.json.get("primaryLanguage")
+        themePack: Dict = data.get("themePack", {})
+        configuration: Dict = data.get("configuration", {})
+        appearance: Dict = configuration.get("appearance", {})
+        leftSidePanel: Dict = appearance.get("leftSidePanel", {})
+        style: Dict = leftSidePanel.get("style", {})
+        page: Dict = configuration.get("page", {})
+        advancedSettings: Dict = data.get("advancedSettings", {})
+        extensions: Dict = data.get("extensions", {})
+
+        self.name: Optional[str] = data.get("name")
+        self.usersCount: Optional[int] = data.get("membersCount")
+        self.createdTime: Optional[str] = data.get("createdTime")
+        self.aminoId = data.get("endpoint")
+        self.icon = data.get("icon")
+        self.link = data.get("link")
+        self.comId = data.get("ndcId")
+        self.modifiedTime = data.get("modifiedTime")
+        self.status = data.get("status")
+        self.joinType = data.get("joinType")
+        self.primaryLanguage = data.get("primaryLanguage")
         self.heat = self.json.get("communityHeat")
         self.userAddedTopicList = self.json.get("userAddedTopicList")
         self.probationStatus = self.json.get("probationStatus")
         self.listedStatus = self.json.get("listedStatus")
         self.themePack = themePack
         self.themeColor = themePack.get("themeColor")
         self.themeHash = themePack.get("themePackHash")
@@ -506,95 +504,91 @@
         self.themeLeftSidePanelBottom = leftSidePanel.get("navigation", {}).get("level2")
         self.themeLeftSidePanelColor = style.get("iconColor")
         self.customList = page.get("customList")
         self.tagline = self.json.get("tagline")
         self.searchable = self.json.get("searchable")
         self.isStandaloneAppDeprecated = self.json.get("isStandaloneAppDeprecated")
         self.influencerList = self.json.get("influencerList")
-        self.keywords = self.json.get("keywords")
-        self.mediaList = self.json.get("mediaList")
-        self.description = self.json.get("content")
-        self.isStandaloneAppMonetizationEnabled = self.json.get("isStandaloneAppMonetizationEnabled")
+        self.keywords = data.get("keywords")
+        self.mediaList: Optional[MediaObject] = data.get("mediaList")
+        self.description = data.get("content")
+        self.isStandaloneAppMonetizationEnabled = data.get("isStandaloneAppMonetizationEnabled")
         self.advancedSettings = advancedSettings
         self.defaultRankingTypeInLeaderboard = advancedSettings.get("defaultRankingTypeInLeaderboard")
         self.frontPageLayout = advancedSettings.get("frontPageLayout")
         self.hasPendingReviewRequest = advancedSettings.get("hasPendingReviewRequest")
         self.welcomeMessageEnabled = advancedSettings.get("welcomeMessageEnabled")
         self.welcomeMessage = advancedSettings.get("welcomeMessageText")
         self.pollMinFullBarVoteCount = advancedSettings.get("pollMinFullBarVoteCount")
         self.catalogEnabled = advancedSettings.get("catalogEnabled")
         self.leaderboardStyle = advancedSettings.get("leaderboardStyle")
         self.facebookAppIdList = advancedSettings.get("facebookAppIdList")
         self.newsfeedPages = advancedSettings.get("newsfeedPages")
         self.joinedBaselineCollectionIdList = advancedSettings.get("joinedBaselineCollectionIdList")
-        self.activeInfo = self.json.get("activeInfo")
+        self.activeInfo = data.get("activeInfo")
         self.configuration = configuration
         self.extensions = extensions
         self.nameAliases = extensions.get("communityNameAliases")
-        self.templateId = self.json.get("templateId")
-        self.promotionalMediaList = self.json.get("promotionalMediaList")
+        self.templateId = data.get("templateId")
+        self.promotionalMediaList: Optional[MediaObject] = data.get("promotionalMediaList")
 
 
     @property
     def Community(self):
         return self
 
 class CommunityList:
     __slots__ = Community.__slots__
 
     def __init__(self, data: dict):
         self.json = data
-
         _communtyObjects = tuple(Community(x).Community for x in data)
 
-        if _communtyObjects:
-            attributes = tuple(attr for attr in dir(_communtyObjects[0]) if not attr.startswith('__') and not callable(getattr(_communtyObjects[0], attr)) and attr != _communtyObjects[0].__class__.__name__)
-            for attr in attributes:
-                setattr(self, attr, tuple(getattr(user, attr, None) for user in _communtyObjects))
+        set_attributes(self, _communtyObjects)
 
     @property
     def CommunityList(self):
     
         return self
 
 class CommentList:
     def __init__(self, data):
         self.json = data
-        self.author = UserProfileList([y.get("author") for y in data]).UserProfileList
-        self.votesSum = tuple(x.get("votesSum") for x in self.json)
-        self.votedValue = tuple(x.get("votedValue") for x in self.json)
-        self.mediaList = tuple(x.get("mediaList") for x in self.json)
-        self.parentComId = tuple(x.get("parentNdcId") for x in self.json)
-        self.parentId = tuple(x.get("parentId") for x in self.json)
-        self.parentType = tuple(x.get("parentType") for x in self.json)
-        self.content = tuple(x.get("content") for x in self.json)
-        self.extensions = tuple(x.get("extensions") for x in self.json)
-        self.comId = tuple(x.get("ndcId") for x in self.json)
-        self.modifiedTime = tuple(x.get("modifiedTime") for x in self.json)
-        self.createdTime = tuple(x.get("createdTime") for x in self.json)
-        self.commentId = tuple(x.get("commentId") for x in self.json)
-        self.subcommentsCount = tuple(x.get("subcommentsCount") for x in self.json)
-        self.type = tuple(x.get("type") for x in self.json)
+        self.author = UserProfileList(tuple(y.get("author") for y in data)).UserProfileList
+        self.votesSum = tuple(x.get("votesSum") for x in data)
+        self.votedValue = tuple(x.get("votedValue") for x in data)
+        self.mediaList: Optional[List[MediaObject]] = tuple(x.get("mediaList") for x in data)
+        self.parentComId = tuple(x.get("parentNdcId") for x in data)
+        self.parentId = tuple(x.get("parentId") for x in data)
+        self.parentType = tuple(x.get("parentType") for x in data)
+        self.content = tuple(x.get("content") for x in data)
+        self.extensions = tuple(x.get("extensions") for x in data)
+        self.comId = tuple(x.get("ndcId") for x in data)
+        self.modifiedTime = tuple(x.get("modifiedTime") for x in data)
+        self.createdTime = tuple(x.get("createdTime") for x in data)
+        self.commentId = tuple(x.get("commentId") for x in data)
+        self.subcommentsCount = tuple(x.get("subcommentsCount") for x in data)
+        self.type = tuple(x.get("type") for x in data)
 
     @property
     def CommentList(self):
         return self
 
 
 class Membership:
     def __init__(self, data):
         self.json = data
 
-        membership = self.json.get("membership", {})
+        membership = data.get("membership", {})
 
-        self.premiumFeature = self.json.get("premiumFeatureEnabled")
-        self.hasAnyAndroidSubscription = self.json.get("hasAnyAndroidSubscription")
-        self.hasAnyAppleSubscription = self.json.get("hasAnyAppleSubscription")
-        self.accountMembership = self.json.get("accountMembershipEnabled")
-        self.paymentType = self.json.get("paymentType")
+        self.premiumFeature = data.get("premiumFeatureEnabled")
+        self.hasAnyAndroidSubscription = data.get("hasAnyAndroidSubscription")
+        self.hasAnyAppleSubscription = data.get("hasAnyAppleSubscription")
+        self.accountMembership = data.get("accountMembershipEnabled")
+        self.paymentType = data.get("paymentType")
         self.membershipStatus = membership.get("membershipStatus")
         self.isAutoRenew = membership.get("isAutoRenew")
         self.createdTime = membership.get("createdTime")
         self.modifiedTime = membership.get("modifiedTime")
         self.renewedTime = membership.get("renewedTime")
         self.expiredTime = membership.get("expiredTime")
 
@@ -602,21 +596,19 @@
     def Membership(self):
         return self
 
 class FromCode:
     def __init__(self, data):
         self.json = data
 
-        try: self.community: Community = Community(data["extensions"]["community"]).Community
-        except (KeyError, TypeError): self.community: Community = Community({})
-
-        extensions = self.json.get("extensions", {})
+        extensions = data.get("extensions", {})
         linkInfo = extensions.get("linkInfo", {})
 
-        self.path = self.json.get("path")
+        self.community: Community = Community(extensions.get("community")).Community
+        self.path = data.get("path")
         self.objectType = linkInfo.get("objectType")
         self.shortCode = linkInfo.get("shortCode")
         self.fullPath = linkInfo.get("fullPath")
         self.targetCode = linkInfo.get("targetCode")
         self.objectId = linkInfo.get("objectId")
         self.shortUrl = linkInfo.get("shareURLShortCode")
         self.fullUrl = linkInfo.get("shareURLFullPath")
@@ -643,22 +635,22 @@
     def UserProfileCountList(self):
         return self
 
 
 class WalletInfo:
     def __init__(self, data):
         self.json = data
-        self.totalCoinsFloat = self.json.get("totalCoinsFloat")
-        self.adsEnabled = self.json.get("adsEnabled")
-        self.adsVideoStats = self.json.get("adsVideoStats")
-        self.adsFlags = self.json.get("adsFlags")
-        self.totalCoins = self.json.get("totalCoins")
-        self.businessCoinsEnabled = self.json.get("businessCoinsEnabled")
-        self.totalBusinessCoins = self.json.get("totalBusinessCoins")
-        self.totalBusinessCoinsFloat = self.json.get("totalBusinessCoinsFloat")
+        self.totalCoinsFloat = data.get("totalCoinsFloat")
+        self.adsEnabled = data.get("adsEnabled")
+        self.adsVideoStats = data.get("adsVideoStats")
+        self.adsFlags = data.get("adsFlags")
+        self.totalCoins = data.get("totalCoins")
+        self.businessCoinsEnabled = data.get("businessCoinsEnabled")
+        self.totalBusinessCoins = data.get("totalBusinessCoins")
+        self.totalBusinessCoinsFloat = data.get("totalBusinessCoinsFloat")
 
     @property
     def WalletInfo(self):
         return self
 
 class WalletHistory:
     def __init__(self, data):
@@ -681,46 +673,47 @@
         self.title = []
         self.description = []
         self.icon = []
         self.objectDeeplinkUrl = []
 
     @property
     def WalletHistory(self):
-        for n, x in enumerate(self.json):
+        for x in self.json:
+            _extData = x.get("extData")
             self.taxCoins.append(x.get("taxCoins"))
             self.bonusCoinsFloat.append(x.get("bonusCoinsFloat"))
             self.isPositive.append(x.get("isPositive"))
             self.bonusCoins.append(x.get("bonusCoins"))
             self.taxCoinsFloat.append(x["taxCoinsFloat"])
             self.transanctionId.append(x.get("uid"))
             self.changedCoins.append(x.get("changedCoins"))
             self.totalCoinsFloat.append(x.get("totalCoinsFloat"))
             self.changedCoinsFloat.append(x.get("changedCoinsFloat"))
             self.sourceType.append(x.get("sourceType"))
             self.createdTime.append(x.get("createdTime"))
             self.totalCoins.append(x.get("totalCoins"))
             self.originCoinsFloat.append(x.get("originCoinsFloat"))
             self.originCoins.append(x.get("originCoins"))
-            self.extData.append(x.get("extData"))
-            self.title.append(self.extData[n].get("description"))
-            self.icon.append(self.extData[n].get("icon"))
-            self.description.append(self.extData[n].get("subtitle"))
-            self.objectDeeplinkUrl.append(self.extData[n].get("objectDeeplinkUrl"))
+            self.extData.append(_extData)
+            self.title.append(_extData.get("description"))
+            self.icon.append(_extData.get("icon"))
+            self.description.append(_extData.get("subtitle"))
+            self.objectDeeplinkUrl.append(_extData.get("objectDeeplinkUrl"))
 
 
         return self
 
 
 class UserAchievements:
     def __init__(self, data):
         self.json = data
-        self.secondsSpentOfLast24Hours = self.json.get("secondsSpentOfLast24Hours")
-        self.secondsSpentOfLast7Days = self.json.get("secondsSpentOfLast7Days")
-        self.numberOfFollowersCount = self.json.get("numberOfMembersCount")
-        self.numberOfPostsCreated = self.json.get("numberOfPostsCreated")
+        self.secondsSpentOfLast24Hours = data.get("secondsSpentOfLast24Hours")
+        self.secondsSpentOfLast7Days = data.get("secondsSpentOfLast7Days")
+        self.numberOfFollowersCount = data.get("numberOfMembersCount")
+        self.numberOfPostsCreated = data.get("numberOfPostsCreated")
 
     @property
     def UserAchievements(self):
         return self
 
 class UserSavedBlogs:
     def __init__(self, data):
@@ -809,20 +802,18 @@
         try: self.fileCount = self.json["fileCount"]
         except (KeyError, TypeError): pass
 
         return self
 
 class WikiCategoryList:
     def __init__(self, data):
+        self.json = data
         _categoryObjects = tuple(WikiCategory(x).WikiCategory for x in data)
 
-        if _categoryObjects:
-            attributes = tuple(attr for attr in dir(_categoryObjects[0]) if not attr.startswith('__') and not callable(getattr(_categoryObjects[0], attr)) and attr != _categoryObjects[0].__class__.__name__)
-            for attr in attributes:
-                setattr(self, attr, tuple(getattr(user, attr, None) for user in _categoryObjects))
+        set_attributes(self, _categoryObjects)
 
     @property
     def WikiCategoryList(self):
 
         return self
 
 class WikiCategory:
@@ -830,110 +821,92 @@
         self.json = data
 
         try: self.author = UserProfile(data["itemCategory"]["author"]).UserProfile
         except (KeyError, TypeError): self.author: UserProfile = UserProfile([])
         try: self.subCategory = WikiCategoryList(data["childrenWrapper"]["itemCategoryList"]).WikiCategoryList
         except (KeyError, TypeError): self.subCategory: WikiCategoryList = WikiCategoryList([])
 
-        itemCategory = self.json.get("itemCategory", {})
-        childrenWrapper = self.json.get("childrenWrapper", {})
+        itemCategory = data.get("itemCategory", {})
+        childrenWrapper = data.get("childrenWrapper", {})
 
         self.itemsCount = itemCategory.get("itemsCount")
         self.parentCategoryId = itemCategory.get("parentCategoryId")
         self.categoryId = itemCategory.get("categoryId")
         self.extensions = itemCategory.get("extensions")
         self.createdTime = itemCategory.get("createdTime")
         self.title = itemCategory.get("label")
-        self.mediaList = itemCategory.get("mediaList")
+        self.mediaList: Optional[MediaObject] = itemCategory.get("mediaList")
         self.icon = itemCategory.get("icon")
         self.parentType = childrenWrapper.get("type")
 
     @property
     def WikiCategory(self):
         return self
 
 class TippedUsersSummary:
     def __init__(self, data):
         _author = []
 
         self.json = data
 
         for y in data["tippedUserList"]:
-            try: _author.append(y["tipper"])
-            except (KeyError, TypeError): _author.append(None)
+            _author.append(y.get("tipper"))
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
-        self.tipSummary = None
-        self.totalCoins = None
-        self.tippersCount = None
-        self.globalTipSummary = None
-        self.globalTippersCount = None
-        self.globalTotalCoins = None
+        self.tipSummary = data.get("tipSummary") or {}
+        self.totalCoins = self.tipSummary.get("totalCoins")
+        self.tippersCount = self.tipSummary.get("tippersCount")
+        self.globalTipSummary = data.get("globalTipSummary") or {}
+        self.globalTippersCount = self.globalTipSummary.get("tippersCount")
+        self.globalTotalCoins = self.globalTipSummary.get("totalCoins")
+
         self.lastTippedTime = []
         self.totalTippedCoins = []
         self.lastThankedTime = []
 
     @property
     def TippedUsersSummary(self):
-        try: self.tipSummary = self.json["tipSummary"]
-        except (KeyError, TypeError): pass
-        try: self.totalCoins = self.json["tipSummary"]["totalCoins"]
-        except (KeyError, TypeError): pass
-        try: self.tippersCount = self.json["tipSummary"]["tippersCount"]
-        except (KeyError, TypeError): pass
-        try: self.globalTipSummary = self.json["globalTipSummary"]
-        except (KeyError, TypeError): pass
-        try: self.globalTippersCount = self.json["globalTipSummary"]["tippersCount"]
-        except (KeyError, TypeError): pass
-        try: self.globalTotalCoins = self.json["globalTipSummary"]["totalCoins"]
-        except (KeyError, TypeError): pass
-
         for tippedUserList in self.json["tippedUserList"]:
-            try: self.lastTippedTime.append(tippedUserList["lastTippedTime"])
-            except (KeyError, TypeError): self.lastTippedTime.append(None)
-            try: self.totalTippedCoins.append(tippedUserList["totalTippedCoins"])
-            except (KeyError, TypeError): self.totalTippedCoins.append(None)
-            try: self.lastThankedTime.append(tippedUserList["lastThankedTime"])
-            except (KeyError, TypeError): self.lastThankedTime.append(None)
+            self.lastTippedTime.append(tippedUserList.get("lastTippedTime"))
+            self.totalTippedCoins.append(tippedUserList.get("totalTippedCoins"))
+            self.lastThankedTime.append(tippedUserList.get("lastThankedTime"))
 
         return self
 
 class Thread:
     def __init__(self, data):
         self.json = data
 
-        try: self.author: UserProfile = UserProfile(data["author"]).UserProfile
-        except (KeyError, TypeError): self.author: UserProfile = UserProfile([])
-        try: self.membersSummary: UserProfileList = UserProfileList(data["membersSummary"]).UserProfileList
-        except (KeyError, TypeError): self.membersSummary: UserProfileList = UserProfileList([])
+        self.author: UserProfile = UserProfile(data.get("author")).UserProfile
+        self.membersSummary: UserProfileList = UserProfileList(data.get("membersSummary")).UserProfileList
 
-        self.userAddedTopicList = self.json.get("userAddedTopicList")
-        self.membersQuota = self.json.get("membersQuota")
-        self.chatId = self.json.get("threadId")
-        self.keywords = self.json.get("keywords")
-        self.membersCount = self.json.get("membersCount")
-        self.isPinned = self.json.get("isPinned")
-        self.title = self.json.get("title")
-        self.membershipStatus = self.json.get("membershipStatus")
-        self.content = self.json.get("content")
-        self.needHidden = self.json.get("needHidden")
-        self.alertOption = self.json.get("alertOption")
-        self.lastReadTime = self.json.get("lastReadTime")
-        self.type = self.json.get("type")
-        self.status = self.json.get("status")
-        self.publishToGlobal = self.json.get("publishToGlobal")
-        self.modifiedTime = self.json.get("modifiedTime")
-        self.condition = self.json.get("condition")
-        self.icon = self.json.get("icon")
-        self.latestActivityTime = self.json.get("latestActivityTime")
-        self.comId = self.json.get("ndcId")
-        self.createdTime = self.json.get("createdTime")
+        self.userAddedTopicList = data.get("userAddedTopicList")
+        self.membersQuota = data.get("membersQuota")
+        self.chatId = data.get("threadId")
+        self.keywords = data.get("keywords")
+        self.membersCount = data.get("membersCount")
+        self.isPinned = data.get("isPinned")
+        self.title = data.get("title")
+        self.membershipStatus = data.get("membershipStatus")
+        self.content = data.get("content")
+        self.needHidden = data.get("needHidden")
+        self.alertOption = data.get("alertOption")
+        self.lastReadTime = data.get("lastReadTime")
+        self.type = data.get("type")
+        self.status = data.get("status")
+        self.publishToGlobal = data.get("publishToGlobal")
+        self.modifiedTime = data.get("modifiedTime")
+        self.condition = data.get("condition")
+        self.icon = data.get("icon")
+        self.latestActivityTime = data.get("latestActivityTime")
+        self.comId = data.get("ndcId")
+        self.createdTime = data.get("createdTime")
 
         # extensions
-        self.extensions = self.json.get("extensions", {})
+        self.extensions = data.get("extensions", {})
         self.viewOnly = self.extensions.get("viewOnly")
         self.coHosts = self.extensions.get("coHost")
         self.membersCanInvite = self.extensions.get("membersCanInvite")
         self.language = self.extensions.get("language")
         self.announcement = self.extensions.get("announcement")
         self.backgroundImage = self.extensions.get("bm", [None, None])[1]
         self.lastMembersSummaryUpdateTime = self.extensions.get("lastMembersSummaryUpdateTime")
@@ -965,19 +938,16 @@
 class ThreadList:
     def __init__(self, data):
         _author, _membersSummary = [], []
 
         self.json = data
 
         for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
-
-            try: _membersSummary.append(UserProfileList(y["membersSummary"]).UserProfileList)
-            except (KeyError, TypeError): _membersSummary.append(None)
+            _author.append(y.get("author"))
+            _membersSummary.append(UserProfileList(y.get("membersSummary")).UserProfileList)
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.membersSummary = _membersSummary
         self.userAddedTopicList = []
         self.membersQuota = []
         self.chatId = []
         self.keywords = []
@@ -1069,111 +1039,85 @@
             self.screeningRoomPermission.append(screeningRoomPermission.get("action"))
             self.organizerTransferCreatedTime.append(organizerTransferRequest.get("createdTime"))
             self.organizerTransferId.append(organizerTransferRequest.get("requestId"))
 
         return self
 
 class Sticker:
+    __slots__ = (
+        "json", "collection", "status", "icon", "iconV2", "name", "stickerId",
+        "smallIcon", "smallIconV2", "stickerCollectionId", "mediumIcon",
+        "mediumIconV2", "extensions", "usedCount", "createdTime"
+    )
+
     def __init__(self, data):
         self.json = data
 
-        try: self.collection: StickerCollection = StickerCollection(data["stickerCollectionSummary"]).StickerCollection
-        except (KeyError, TypeError): self.collection: StickerCollection = StickerCollection([])
+        self.collection: StickerCollection = StickerCollection(data.get("stickerCollectionSummary")).StickerCollection
 
-        self.status = data.get("status")
-        self.icon = data.get("icon")
-        self.iconV2 = data.get("iconV2")
-        self.name = data.get("name")
-        self.stickerId = data.get("stickerId")
-        self.smallIcon = data.get("smallIcon")
-        self.smallIconV2 = data.get("smallIconV2")
-        self.stickerCollectionId = data.get("stickerCollectionId")
-        self.mediumIcon = data.get("mediumIcon")
-        self.mediumIconV2 = data.get("mediumIconV2")
-        self.extensions = data.get("extensions")
-        self.usedCount = data.get("usedCount")
-        self.createdTime = data.get("createdTime")
+        self.status: Optional[str] = data.get("status")
+        self.icon: Optional[str] = data.get("icon")
+        self.iconV2: Optional[str] = data.get("iconV2")
+        self.name: Optional[str] = data.get("name")
+        self.stickerId: Optional[str] = data.get("stickerId")
+        self.smallIcon: Optional[str] = data.get("smallIcon")
+        self.smallIconV2: Optional[str] = data.get("smallIconV2")
+        self.stickerCollectionId: Optional[str] = data.get("stickerCollectionId")
+        self.mediumIcon: Optional[str] = data.get("mediumIcon")
+        self.mediumIconV2: Optional[str] = data.get("mediumIconV2")
+        self.extensions: Optional[str] = data.get("extensions")
+        self.usedCount: Optional[str] = data.get("usedCount")
+        self.createdTime: Optional[str] = data.get("createdTime")
 
     @property
     def Sticker(self):
         return self
 
 class StickerList:
-    def __init__(self, data):
-        _collection = []
+    __slots__ = Sticker.__slots__
 
+    def __init__(self, data: dict):
         self.json = data
 
-        for y in data:
-            try: _collection.append(y["stickerCollectionSummary"])
-            except (KeyError, TypeError): _collection.append(None)
-
-        self.collection: StickerCollectionList = StickerCollectionList(_collection).StickerCollectionList
-        self.status = []
-        self.icon = []
-        self.iconV2 = []
-        self.name = []
-        self.stickerId = []
-        self.smallIcon = []
-        self.smallIconV2 = []
-        self.stickerCollectionId = []
-        self.mediumIcon = []
-        self.mediumIconV2 = []
-        self.extensions = []
-        self.usedCount = []
-        self.createdTime = []
+        _StickerObjects = tuple(Sticker(x).Sticker for x in data)
+        set_attributes(self, _StickerObjects)
 
     @property
     def StickerList(self):
-        for x in self.json:
-            self.status.append(x.get("status"))
-            self.icon.append(x.get("icon"))
-            self.iconV2.append(x.get("iconV2"))
-            self.name.append(x.get("name"))
-            self.stickerId.append(x.get("stickerId"))
-            self.smallIcon.append(x.get("smallIcon"))
-            self.smallIconV2.append(x.get("smallIconV2"))
-            self.stickerCollectionId.append(x.get("stickerCollectionId"))
-            self.mediumIcon.append(x.get("mediumIcon"))
-            self.mediumIconV2.append(x.get("mediumIconV2"))
-            self.extensions.append(x.get("extensions"))
-            self.usedCount.append(x.get("usedCount"))
-            self.createdTime.append(x.get("createdTime"))
-
         return self
 
 class StickerCollection:
     def __init__(self, data):
         self.json = data
 
-        try: self.author: UserProfile = UserProfile(data["author"]).UserProfile
-        except (KeyError, TypeError): self.author: UserProfile = UserProfile([])
-        try: self.originalAuthor: UserProfile = UserProfile(data["extensions"]["originalAuthor"]).UserProfile
-        except (KeyError, TypeError): self.originalAuthor: UserProfile = UserProfile([])
-        try: self.originalCommunity: Community = Community(data["extensions"]["originalCommunity"]).Community
-        except (KeyError, TypeError): self.originalCommunity: Community = Community([])
+        self.author: UserProfile = UserProfile(data.get("author")).UserProfile
 
         self.status = data.get("status")
         self.collectionType = data.get("collectionType")
         self.modifiedTime = data.get("modifiedTime")
         self.bannerUrl = data.get("bannerUrl")
         self.smallIcon = data.get("smallIcon")
         self.stickersCount = data.get("stickersCount")
         self.usedCount = data.get("usedCount")
         self.icon = data.get("icon")
         self.title = data.get("name")
         self.collectionId = data.get("collectionId")
-        self.extensions = data.get("extensions")
-        self.iconSourceStickerId = self.extensions.get("iconSourceStickerId")
+        
         self.isActivated = data.get("isActivated")
         self.ownershipStatus = data.get("ownershipStatus")
         self.isNew = data.get("isNew")
         self.availableComIds = data.get("availableNdcIds")
         self.description = data.get("description")
 
+        #extensions
+        self.extensions = data.get("extensions") or {}
+        self.iconSourceStickerId = self.extensions.get("iconSourceStickerId")
+        self.originalAuthor: UserProfile = UserProfile(self.extensions.get("originalAuthor")).UserProfile
+        self.originalCommunity: Community = Community(self.extensions.get("originalCommunity")).Community
+
         #restrictionInfo
         self.restrictionInfo = data.get("restrictionInfo", {})
         self.discountStatus = self.restrictionInfo.get("discountStatus")
         self.discountValue = self.restrictionInfo.get("discountValue")
         self.ownerId = self.restrictionInfo.get("ownerUid")
         self.ownerType = self.restrictionInfo.get("ownerType")
         self.restrictType = self.restrictionInfo.get("restrictType")
@@ -1188,16 +1132,16 @@
 class StickerCollectionList:
     def __init__(self, data):
         _author, _originalAuthor, _originalCommunity = [], [], []
 
         self.json = data
 
         for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
+            _author.append(y.get("author"))
+
             try: _originalAuthor.append(y["extensions"]["originalAuthor"])
             except (KeyError, TypeError): _originalAuthor.append(None)
             try: _originalCommunity.append(y["extensions"]["originalCommunity"])
             except (KeyError, TypeError): _originalCommunity.append(None)
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.originalAuthor: UserProfileList = UserProfileList(_originalAuthor).UserProfileList
@@ -1262,44 +1206,44 @@
 
         return self
 
 class Message:
     def __init__(self, data):
         self.json = data
 
-        try: self.author: UserProfile = UserProfile(data["author"]).UserProfile
-        except (KeyError, TypeError): self.author: UserProfile = UserProfile([])
+        self.author: UserProfile = UserProfile(data.get("author", [])).UserProfile
+
         try: self.sticker: Sticker = Sticker(data["extensions"]["sticker"]).Sticker
         except (KeyError, TypeError): self.sticker: Sticker = Sticker([])
 
-        extensions = self.json.get("extensions", {})
+        extensions = data.get("extensions", {})
         videoExtensions = extensions.get("videoExtensions", {})
 
-        self.content = self.json.get("content")
-        self.includedInSummary = self.json.get("includedInSummary")
-        self.isHidden = self.json.get("isHidden")
-        self.messageId = self.json.get("messageId")
-        self.messageType = self.json.get("messageType")
-        self.mediaType = self.json.get("mediaType")
-        self.chatBubbleId = self.json.get("chatBubbleId")
-        self.clientRefId = self.json.get("clientRefId")
-        self.chatId = self.json.get("threadId")
-        self.createdTime = self.json.get("createdTime")
-        self.chatBubbleVersion = self.json.get("chatBubbleVersion")
-        self.type = self.json.get("type")
+        self.content = data.get("content")
+        self.includedInSummary = data.get("includedInSummary")
+        self.isHidden = data.get("isHidden")
+        self.messageId = data.get("messageId")
+        self.messageType = data.get("messageType")
+        self.mediaType = data.get("mediaType")
+        self.chatBubbleId = data.get("chatBubbleId")
+        self.clientRefId = data.get("clientRefId")
+        self.chatId = data.get("threadId")
+        self.createdTime = data.get("createdTime")
+        self.chatBubbleVersion = data.get("chatBubbleVersion")
+        self.type = data.get("type")
         self.replyMessage = extensions.get("replyMessage")
-        self.mediaValue = self.json.get("mediaValue")
+        self.mediaValue = data.get("mediaValue")
         self.extensions = extensions
         self.duration = extensions.get("duration")
         self.videoDuration = videoExtensions.get("duration")
         self.videoHeight = videoExtensions.get("height")
         self.videoWidth = videoExtensions.get("width")
         self.videoCoverImage = videoExtensions.get("coverImage")
         self.originalStickerId = extensions.get("originalStickerId")
-        self.mentionUserIds = [m.get("uid") for m in extensions.get("mentionedArray", [])]
+        self.mentionUserIds = tuple(m.get("uid") for m in extensions.get("mentionedArray", ()))
         self.tippingCoins = extensions.get("tippingCoins")
 
 
     @property
     def Message(self):
         return self
 
@@ -1503,37 +1447,37 @@
 
         return self
 
 class LotteryLog:
     def __init__(self, data):
         self.json = data
         
-        self.awardValue = self.json.get("awardValue")
-        self.parentId = self.json.get("parentId")
-        self.parentType = self.json.get("parentType")
-        self.objectId = self.json.get("objectId")
-        self.objectType = self.json.get("objectType")
-        self.createdTime = self.json.get("createdTime")
-        self.awardType = self.json.get("awardType")
-        self.refObject = self.json.get("refObject")
+        self.awardValue = data.get("awardValue")
+        self.parentId = data.get("parentId")
+        self.parentType = data.get("parentType")
+        self.objectId = data.get("objectId")
+        self.objectType = data.get("objectType")
+        self.createdTime = data.get("createdTime")
+        self.awardType = data.get("awardType")
+        self.refObject = data.get("refObject")
 
     @property
     def LotteryLog(self):
         return self
 
 class VcReputation:
     def __init__(self, data):
         self.json = data
 
-        self.availableReputation = self.json.get("availableReputation")
-        self.maxReputation = self.json.get("maxReputation")
-        self.reputation = self.json.get("reputation")
-        self.participantCount = self.json.get("participantCount")
-        self.totalReputation = self.json.get("totalReputation")
-        self.duration = self.json.get("duration")
+        self.availableReputation = data.get("availableReputation")
+        self.maxReputation = data.get("maxReputation")
+        self.reputation = data.get("reputation")
+        self.participantCount = data.get("participantCount")
+        self.totalReputation = data.get("totalReputation")
+        self.duration = data.get("duration")
 
     @property
     def VcReputation(self):
         return self
 
 class FanClubList:
     __slots__ = (
@@ -1579,26 +1523,22 @@
     def FanClubList(self):
         return self
 
 class InfluencerFans:
     def __init__(self, data):
         self.json = data
 
-        try: self.influencerProfile: UserProfile = UserProfile(data["influencerUserProfile"]).UserProfile
-        except (KeyError, TypeError): self.influencerProfile: UserProfile = UserProfile([])
-        try: self.fanClubList: FanClubList = FanClubList(data["fanClubList"]).FanClubList
-        except (KeyError, TypeError): self.fanClubList: FanClubList = FanClubList([])
+        self.influencerProfile: UserProfile = UserProfile(data.get("influencerUserProfile", [])).UserProfile
+        self.fanClubList: FanClubList = FanClubList(data.get("fanClubList", [])).FanClubList
 
-        self.myFanClub = None
+
+        self.myFanClub = data.get("myFanClub")
 
     @property
     def InfluencerFans(self):
-        try: self.myFanClub = self.json["myFanClub"]
-        except (KeyError, TypeError): pass
-
         return self
 
 class QuizQuestionList:
     def __init__(self, data):
         _answersList = []
 
         self.json = data
@@ -1609,28 +1549,28 @@
 
         self.status = []
         self.parentType = []
         self.title = []
         self.createdTime = []
         self.questionId = []
         self.parentId = []
-        self.mediaList = []
+        self.mediaList: Optional[List[MediaObject]] = []
         self.extensions = []
         self.style = []
         self.backgroundImage = []
         self.backgroundColor = []
         self.answerExplanation = []
         self.answersList = _answersList
 
     @property
     def QuizQuestionList(self):
         for x in self.json:
             extensions = x.get("extensions", {})
             style = extensions.get("style", {})
-            backgroundMediaList = style.get("backgroundMediaList", [None, None])
+            backgroundMediaList: Optional[MediaObject] = style.get("backgroundMediaList", [None, None])
 
             self.status.append(x.get("status"))
             self.parentType.append(x.get("parentType"))
             self.title.append(x.get("title"))
             self.createdTime.append(x.get("createdTime"))
             self.questionId.append(x.get("quizQuestionId"))
             self.parentId.append(x.get("parentId"))
@@ -1644,15 +1584,15 @@
         return self
 
 class QuizAnswers:
     def __init__(self, data):
         self.json = data
         self.answerId = []
         self.isCorrect = []
-        self.mediaList = []
+        self.mediaList: List[Optional[MediaObject]] = []
         self.title = []
         self.qhash = []
 
     @property
     def QuizAnswers(self):
         for x in self.json:
             self.answerId.append(x.get("optId"))
@@ -1759,15 +1699,15 @@
         self.votesCount = self.json.get("votesCount")
         self.createdTime = self.json.get("createdTime")
         self.modifiedTime = self.json.get("modifiedTime")
         self.extensions = self.json.get("extensions")
         self.width = self.json.get("width_hq")
         self.height = self.json.get("height_hq")
         self.title = self.json.get("title")
-        self.media = self.json.get("media", [None, None])
+        self.media: Optional[MediaObject] = self.json.get("media", [None, None])
         self.mediaType = self.media[0]
         self.fileUrl = self.media[1]
         self.commentsCount = self.json.get("commentsCount")
         self.fileType = self.json.get("fileType")
         self.votedValue = self.json.get("votedValue")
         self.fileId = self.json.get("fileId")
         self.comId = self.json.get("ndcId")
@@ -1789,15 +1729,15 @@
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.votesCount = []
         self.createdTime = []
         self.modifiedTime = []
         self.extensions = []
         self.title = []
-        self.media = []
+        self.media: Optional[MediaObject] = []
         self.width = []
         self.height = []
         self.commentsCount = []
         self.fileType = []
         self.votedValue = []
         self.fileId = []
         self.comId = []
@@ -1827,17 +1767,18 @@
             self.comId.append(x.get("ndcId"))
             self.status.append(x.get("status"))
 
 
         return self
 
 class Event:
-    __sloots__ = ("json", "comId", "alertOption", "membershipStatus",
-            "actions", "target", "params", "threadType", "duration",
-            "id", "message"
+    __sloots__ = (
+        "json", "comId", "alertOption", "membershipStatus",
+        "actions", "target", "params", "threadType", "duration",
+        "id", "message"
     )
 
     def __init__(self, data):
         self.json = data
         params = self.json.get("params", {})
 
         self.comId = self.json.get("ndcId")
@@ -1855,30 +1796,23 @@
     @property
     def Event(self):
 
         return self
 
 class JoinRequest:
     def __init__(self, data):
-        _author = []
+        _author = tuple(x for x in data["communityMembershipRequestList"])
 
         self.json = data
 
-        for y in data["communityMembershipRequestList"]:
-            try: _author.append(y)
-            except (KeyError, TypeError): _author.append(None)
-
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
-        self.communityMembershipRequestCount = None
+        self.communityMembershipRequestCount = self.json.get("communityMembershipRequestCount")
 
     @property
     def JoinRequest(self):
-        try: self.communityMembershipRequestCount = self.json["communityMembershipRequestCount"]
-        except (KeyError, TypeError): pass
-
         return self
 
 class CommunityStats:
     def __init__(self, data):
         self.json = data
 
         self.dailyActiveMembers = self.json.get("dailyActiveMembers")
@@ -1893,16 +1827,15 @@
         return self
 
 
 class InviteCode:
     def __init__(self, data):
         self.json = data
 
-        try: self.author: UserProfile = UserProfile(data["author"]).UserProfile
-        except (KeyError, TypeError): self.author: UserProfile = UserProfile([])
+        self.author: UserProfile = UserProfile(data.get("author", [])).UserProfile
 
         self.status = self.json.get("status")
         self.duration = self.json.get("duration")
         self.invitationId = self.json.get("invitationId")
         self.link = self.json.get("link")
         self.modifiedTime = self.json.get("modifiedTime")
         self.comId = self.json.get("ndcId")
@@ -1917,16 +1850,15 @@
 class InviteCodeList:
     def __init__(self, data):
         _author = []
 
         self.json = data
 
         for y in data:
-            try: _author.append(y["author"])
-            except (KeyError, TypeError): _author.append(None)
+            _author.append(y.get("author"))
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.status = []
         self.duration = []
         self.invitationId = []
         self.link = []
         self.modifiedTime = []
@@ -1951,20 +1883,17 @@
 class WikiRequestList:
     def __init__(self, data):
         _author, _wiki, _originalWiki = [], [], []
 
         self.json = data
 
         for y in data:
-            try: _author.append(y["operator"])
-            except (KeyError, TypeError): _author.append(None)
-            try: _wiki.append(y["item"])
-            except (KeyError, TypeError): _wiki.append(None)
-            try: _originalWiki.append(y["originalItem"])
-            except (KeyError, TypeError): _originalWiki.append(None)
+            _author.append(y.get("operator"))
+            _wiki.append(y.get("item"))
+            _originalWiki.append(y.get("originalItem"))
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.wiki: WikiList = WikiList(_wiki).WikiList
         self.originalWiki: WikiList = WikiList(_originalWiki).WikiList
 
         self.authorId = []
         self.status = []
@@ -1995,18 +1924,16 @@
 class NoticeList:
     def __init__(self, data):
         _author, _targetUser = [], []
 
         self.json = data
 
         for y in data:
-            try: _author.append(y["operator"])
-            except (KeyError, TypeError): _author.append(None)
-            try: _targetUser.append(y["targetUser"])
-            except (KeyError, TypeError): _targetUser.append(None)
+            _author.append(y.get("operator"))
+            _targetUser.append(y.get("targetUser"))
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.targetUser: UserProfileList = UserProfileList(_targetUser).UserProfileList
 
         self.title = []
         self.icon = []
         self.noticeId = []
@@ -2078,16 +2005,16 @@
 
 
         return self
 
 
 class AvatarFrameList:
     def __init__(self, data):
-        _author = [x.get("operator") for x in data]
-        _targetUser = [x.get("targetUser") for x in data]
+        _author = tuple(x.get("operator") for x in data)
+        _targetUser = tuple(x.get("targetUser") for x in data)
 
         self.json = data
 
         self.author: UserProfileList = UserProfileList(_author).UserProfileList
         self.targetUser: UserProfileList = UserProfileList(_targetUser).UserProfileList
 
         self.isGloballyAvailable = []
@@ -2197,44 +2124,44 @@
 
 
 class Bubble:
     def __init__(self, data):
         self.config: BubbleConfig = BubbleConfig(data.get("config", [])).BubbleConfig
 
         self.json = data
-        self.uid = self.json.get("uid")
-        self.isActivated = self.json.get("isActivated")
-        self.isNew = self.json.get("isNew")
-        self.bubbleId = self.json.get("bubbleId")
-        self.resourceUrl = self.json.get("resourceUrl")
-        self.backgroundImage = self.json.get("backgroundImage")
-        self.status = self.json.get("status")
-        self.modifiedTime = self.json.get("modifiedTime")
+        self.uid = data.get("uid")
+        self.isActivated = data.get("isActivated")
+        self.isNew = data.get("isNew")
+        self.bubbleId = data.get("bubbleId")
+        self.resourceUrl = data.get("resourceUrl")
+        self.backgroundImage = data.get("backgroundImage")
+        self.status = data.get("status")
+        self.modifiedTime = data.get("modifiedTime")
 
-        ownershipInfo = self.json.get("ownershipInfo", {})
+        ownershipInfo = data.get("ownershipInfo", {})
         self.ownershipInfo = ownershipInfo
         self.expiredTime = ownershipInfo.get("expiredTime")
         self.isAutoRenew = ownershipInfo.get("isAutoRenew")
 
-        self.ownershipStatus = self.json.get("ownershipStatus")
-        self.bannerImage = self.json.get("bannerImage")
-        self.md5 = self.json.get("md5")
-        self.name = self.json.get("name")
-        self.coverImage = self.json.get("coverImage")
-        self.bubbleType = self.json.get("bubbleType")
-        self.extensions = self.json.get("extensions")
-        self.templateId = self.json.get("templateId")
-        self.createdTime = self.json.get("createdTime")
-        self.deletable = self.json.get("deletable")
-        self.backgroundMedia = self.json.get("backgroundMedia")
-        self.description = self.json.get("description")
-        self.materialUrl = self.json.get("materialUrl")
-        self.comId = self.json.get("ndcId")
+        self.ownershipStatus = data.get("ownershipStatus")
+        self.bannerImage = data.get("bannerImage")
+        self.md5 = data.get("md5")
+        self.name = data.get("name")
+        self.coverImage = data.get("coverImage")
+        self.bubbleType = data.get("bubbleType")
+        self.extensions = data.get("extensions")
+        self.templateId = data.get("templateId")
+        self.createdTime = data.get("createdTime")
+        self.deletable = data.get("deletable")
+        self.backgroundMedia = data.get("backgroundMedia")
+        self.description = data.get("description")
+        self.materialUrl = data.get("materialUrl")
+        self.comId = data.get("ndcId")
 
-        restrictionInfo = self.json.get("restrictionInfo", {})
+        restrictionInfo = data.get("restrictionInfo", {})
         self.restrictionInfo = restrictionInfo
         self.discountStatus = restrictionInfo.get("discountStatus")
         self.discountValue = restrictionInfo.get("discountValue")
         self.ownerId = restrictionInfo.get("ownerUid")
         self.ownerType = restrictionInfo.get("ownerType")
         self.restrictType = restrictionInfo.get("restrictType")
         self.restrictValue = restrictionInfo.get("restrictValue")
@@ -2244,14 +2171,15 @@
     def Bubble(self):
         return self
 
 
 class BubbleConfigList:
     def __init__(self, data):
         self.json = data
+
         self.status = []
         self.allowedSlots = []
         self.name = []
         self.vertexInset = []
         self.zoomPoint = []
         self.coverImage = []
         self.bubbleType = []
@@ -2279,22 +2207,18 @@
             self.id.append(x.get("id"))
             self.previewBackgroundUrl.append(x.get("previewBackgroundUrl"))
 
         return self
 
 class BubbleList:
     def __init__(self, data):
-        _config = []
+        _config = tuple(x.get("config") for x in data)
 
         self.json = data
 
-        for y in data:
-            try: _config.append(y["config"])
-            except (KeyError, TypeError): _config.append(None)
-
         self.config: BubbleConfigList = BubbleConfigList(_config).BubbleConfigList
         self.uid = []
         self.isActivated = []
         self.isNew = []
         self.bubbleId = []
         self.resourceUrl = []
         self.version = []
@@ -2310,15 +2234,15 @@
         self.name = []
         self.coverImage = []
         self.bubbleType = []
         self.extensions = []
         self.templateId = []
         self.createdTime = []
         self.deletable = []
-        self.backgroundMedia = []
+        self.backgroundMedia: List[Optional[MediaObject]] = []
         self.description = []
         self.materialUrl = []
         self.comId = []
         self.restrictionInfo = []
         self.discountValue = []
         self.discountStatus = []
         self.ownerId = []
@@ -2444,8 +2368,17 @@
 
             self.id.append(refObject.get("collectionId"))
             self.name.append(itemBasicInfo.get("name"))
             self.icon.append(itemBasicInfo.get("icon"))
             self.value.append(restrictionInfo.get("restrictValue"))
             self.smallIcon.append(refObject.get("smallIcon"))
 
-        return self
+        return self
+
+class MediaObject(List[List[TypeVar('T')]]):
+    pass
+
+def set_attributes(instance, _ListObjects):
+    if _ListObjects:
+        attributes = tuple(attr for attr in dir(_ListObjects[0]) if not attr.startswith('__') and not callable(getattr(_ListObjects[0], attr)) and attr != _ListObjects[0].__class__.__name__)
+        for attr in attributes:
+            setattr(instance, attr, tuple(getattr(user, attr, None) for user in _ListObjects))
```

### Comparing `amino.light.py-0.0.8/AminoLightPy/sub_client.py` & `amino.light.py-0.0.9/AminoLightPy/sub_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from uuid import uuid4
-from json import dumps
 from time import timezone
-from .constants import api
 from requests import Session
 from base64 import b64encode
 from typing import BinaryIO, Union
-from time import time as timestamp
 
+from .constants import api, upload_media
 from .lib.util import exceptions, objects
 
 
 class SubClient():
     def __init__(self, comId: int = None, *, profile: objects.UserProfile):
         self.vc_connect = False
         self.profile = profile
@@ -36,21 +34,20 @@
         return response.status_code
 
     def post_blog(self, title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False):
         mediaList = list()
 
         if captionList is not None:
             for image, caption in zip(imageList, captionList):
-                mediaList.append([100, self.upload_media(image, "image"), caption])
+                mediaList.append([100, upload_media(self, image, "image"), caption])
 
         else:
             if imageList is not None:
                 for image in imageList:
-                    print(self.upload_media(image, "image"))
-                    mediaList.append([100, self.upload_media(image, "image"), None])
+                    mediaList.append([100, upload_media(self, image, "image"), None])
 
         data = {
             "address": None,
             "content": content,
             "title": title,
             "mediaList": mediaList,
             "extensions": extensions,
@@ -87,15 +84,15 @@
         response = self.session.post(f"{api}/x{self.comId}/s/item", json=data)
         return response.status_code
 
     def edit_blog(self, blogId: str, title: str = None, content: str = None, imageList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False):
         mediaList = list()
 
         for image in imageList:
-            mediaList.append([100, self.upload_media(image, "image"), None])
+            mediaList.append([100, upload_media(self, image, "image"), None])
 
         data = {
             "address": None,
             "mediaList": mediaList,
             "latitude": 0,
             "longitude": 0,
             "eventSource": "PostDetailView",
@@ -117,15 +114,15 @@
     def delete_wiki(self, wikiId: str):
         response = self.session.delete(f"{api}/x{self.comId}/s/item/{wikiId}")
         return response.status_code
 
     def repost_blog(self, content: str = None, blogId: str = None, wikiId: str = None):
         if blogId is not None: refObjectId, refObjectType = blogId, 1
         elif wikiId is not None: refObjectId, refObjectType = wikiId, 2
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         data = {
             "content": content,
             "refObjectId": refObjectId,
             "refObjectType": refObjectType,
             "type": 2,
         }
@@ -136,15 +133,15 @@
     def check_in(self, tz: int = -timezone // 1000):
         data = { "timezone": tz }
         
         response = self.session.post(f"{api}/x{self.comId}/s/check-in", json=data)
         return response.status_code
 
     def repair_check_in(self, method: int = 0):
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = dict()
         if method == 0: data["repairMethod"] = "1"  # Coins
         if method == 1: data["repairMethod"] = "2"  # Amino+
         
         response = self.session.post(f"{api}/x{self.comId}/s/check-in/repair", json=data)
         return response.status_code
 
     def lottery(self, tz: int = -timezone // 1000):
@@ -156,40 +153,41 @@
     def edit_profile(self, nickname: str = None, content: str = None, icon: BinaryIO = None, chatRequestPrivilege: str = None, imageList: list = None, captionList: list = None, backgroundImage: str = None, backgroundColor: str = None, titles: list = None, colors: list = None, defaultBubbleId: str = None):
         mediaList = list()
 
         data = dict()
 
         if captionList is not None:
             for image, caption in zip(imageList, captionList):
-                mediaList.append([100, self.upload_media(image, "image"), caption])
+                mediaList.append([100, upload_media(self, image, "image"), caption])
 
         else:
             if imageList is not None:
                 for image in imageList:
-                    mediaList.append([100, self.upload_media(image, "image"), None])
+                    mediaList.append([100, upload_media(self, image, "image"), None])
 
         if imageList is not None or captionList is not None:
             data["mediaList"] = mediaList
 
         if nickname: data["nickname"] = nickname
-        if icon: data["icon"] = [100, self.upload_media(icon, "image"), None]
+        if icon: data["icon"] = upload_media(self, icon, "image")
         if content: data["content"] = content
 
         if chatRequestPrivilege: data["extensions"] = {"privilegeOfChatInviteRequest": chatRequestPrivilege}
         if backgroundImage: data["extensions"] = {"style": {"backgroundMediaList": [[100, backgroundImage, None, None, None]]}}
         if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
         if defaultBubbleId: data["extensions"] = {"defaultBubbleId": defaultBubbleId}
 
         if titles or colors:
             tlt = []
             for titles, colors in zip(titles, colors):
                 tlt.append({"title": titles, "color": colors})
 
             data["extensions"] = {"customTitles": tlt}
         
+
         response = self.session.post(f"{api}/x{self.comId}/s/user-profile/{self.profile.userId}", json=data)
         return response.status_code
 
     def vote_poll(self, blogId: str, optionId: str):
         data = {
             "value": 1,
             "eventSource": "PostDetailView"
@@ -218,25 +216,25 @@
             data["eventSource"] = "PostDetailView"
             url = f"{api}/x{self.comId}/s/blog/{blogId}/{comType}"
 
         elif wikiId:
             data["eventSource"] = "PostDetailView"
             url = f"{api}/x{self.comId}/s/item/{wikiId}/{comType}"
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
 
         return response.status_code
 
     def delete_comment(self, commentId: str, userId: str = None, blogId: str = None, wikiId: str = None):
         if userId: url = f"{api}/x{self.comId}/s/user-profile/{userId}/comment/{commentId}"
         elif blogId: url = f"{api}/x{self.comId}/s/blog/{blogId}/comment/{commentId}"
         elif wikiId: url = f"{api}/x{self.comId}/s/item/{wikiId}/comment/{commentId}"
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         response = self.session.delete(url)
         return response.status_code
 
     def like_blog(self, blogId: Union[str, list] = None, wikiId: str = None):
         """
         Like a Blog, Multiple Blogs or a Wiki.
@@ -346,16 +344,16 @@
             "type": 0,
             "eventSource": "UserProfileView"
         }
         
         response = self.session.post(f"{api}/x{self.comId}/s/user-profile/{userId}/comment", json=data)
         return response.status_code
 
-    def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None, timestamp: int = int(timestamp() * 1000)): 
-        data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "timestamp": timestamp, "optInAdsFlags": optInAdsFlags, "timezone": tz} 
+    def send_active_obj(self, startTime: int = None, endTime: int = None, optInAdsFlags: int = 2147483647, tz: int = -timezone // 1000, timers: list = None): 
+        data = {"userActiveTimeChunkList": [{"start": startTime, "end": endTime}], "optInAdsFlags": optInAdsFlags, "timezone": tz} 
         if timers: data["userActiveTimeChunkList"] = timers 
         
         response = self.session.post(f"{api}/x{self.comId}/s/community/stats/user-active-time", json=data) 
         return response.status_code
 
     def activity_status(self, status: str):
         if "on" in status.lower(): status = 1
@@ -430,26 +428,25 @@
 
     def send_coins(self, coins: int, blogId: str = None, chatId: str = None, objectId: str = None, transactionId: str = None):
         url = None
         if transactionId is None: transactionId = str(uuid4())
 
         data = {
             "coins": coins,
-            "tippingContext": {"transactionId": transactionId},
-            "timestamp": int(timestamp() * 1000)
+            "tippingContext": {"transactionId": transactionId}
         }
 
         if blogId is not None: url = f"{api}/x{self.comId}/s/blog/{blogId}/tipping"
         if chatId is not None: url = f"{api}/x{self.comId}/s/chat/thread/{chatId}/tipping"
         if objectId is not None:
             data["objectId"] = objectId
             data["objectType"] = 2
             url = f"{api}/x{self.comId}/s/tipping"
 
-        if url is None: raise exceptions.SpecifyType()
+        if url is None: raise exceptions.SpecifyType
         
         response = self.session.post(url, json=data)
         return response.status_code
 
     def thank_tip(self, chatId: str, userId: str):
         response = self.session.post(f"{api}/x{self.comId}/s/chat/thread/{chatId}/tipping/tipped-users/{userId}/thank")
         return response.status_code
@@ -536,16 +533,16 @@
             - *asGuest* : Execute as a Guest.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        if reason is None: raise exceptions.ReasonNeeded()
-        if flagType is None: raise exceptions.FlagTypeNeeded()
+        if reason is None: raise exceptions.ReasonNeeded
+        if flagType is None: raise exceptions.FlagTypeNeeded
 
         data = {
             "flagType": flagType,
             "message": reason
         }
 
         if userId:
@@ -556,15 +553,15 @@
             data["objectId"] = blogId
             data["objectType"] = 1
 
         elif wikiId:
             data["objectId"] = wikiId
             data["objectType"] = 2
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         if asGuest: flg = "g-flag"
         else: flg = "flag"
 
         
         response = self.session.post(f"{api}/x{self.comId}/s/{flg}", json=data)
         return response.status_code
@@ -600,67 +597,67 @@
         
 
         data = {
             "type": messageType,
             "content": message
         }
         
-        # if self.check_values(embedId, embedType, embedLink, embedTitle, embedContent, embedImage):
-        #     attachedObject = dict()
+        if self.check_values(embedId, embedType, embedLink, embedTitle, embedContent, embedImage):
+            attachedObject = dict()
 
-        #     if embedId:
-        #         attachedObject["objectId"] = embedId
+            if embedId:
+                attachedObject["objectId"] = embedId
 
-        #     if embedType:
-        #         attachedObject["objectType"] = embedType
+            if embedType:
+                attachedObject["objectType"] = embedType
 
-        #     if embedLink:
-        #         attachedObject["link"] = embedLink
+            if embedLink:
+                attachedObject["link"] = embedLink
 
-        #     if embedTitle:
-        #         attachedObject["title"] = embedTitle
+            if embedTitle:
+                attachedObject["title"] = embedTitle
 
-        #     if embedContent:
-        #         attachedObject["content"] = embedContent
+            if embedContent:
+                attachedObject["content"] = embedContent
 
-        #     if embedImage:
-        #         attachedObject["mediaList"] = [[100, self.upload_media(embedImage, "image"), None]]
+            if embedImage:
+                attachedObject["mediaList"] = [[100, upload_media(self, embedImage, "image"), None]]
 
-        #     data["attachedObject"] = attachedObject
+            data["attachedObject"] = attachedObject
         
-        # if mentionUserIds:
-        #     mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
-        #     data["extensions"] = {"mentionedArray": mentions}
+        if mentionUserIds:
+            mentions = [{"uid": mention_uid} for mention_uid in mentionUserIds]
+            data["extensions"] = {"mentionedArray": mentions}
 
-        # if replyTo: data["replyMessageId"] = replyTo
+        if replyTo: data["replyMessageId"] = replyTo
 
-        # if stickerId:
-        #     data["content"] = None
-        #     data["stickerId"] = stickerId
-        #     data["type"] = 3
+        if stickerId:
+            data["content"] = None
+            data["stickerId"] = stickerId
+            data["type"] = 3
 
-        # if file:
-        #     data["content"] = None
-        #     if fileType == "audio":
-        #         data["type"] = 2
-        #         data["mediaType"] = 110
+        if file:
+            data["content"] = None
+            if fileType == "audio":
+                data["type"] = 2
+                data["mediaType"] = 110
 
-        #     elif fileType == "image":
-        #         data["mediaType"] = 100
-        #         data["mediaUploadValueContentType"] = "image/jpg"
-        #         data["mediaUhqEnabled"] = True
+            elif fileType == "image":
+                data["mediaType"] = 100
+                data["mediaUploadValueContentType"] = "image/jpg"
+                data["mediaUhqEnabled"] = True
 
-        #     elif fileType == "gif":
-        #         data["mediaType"] = 100
-        #         data["mediaUploadValueContentType"] = "image/gif"
-        #         data["mediaUhqEnabled"] = True
+            elif fileType == "gif":
+                data["mediaType"] = 100
+                data["mediaUploadValueContentType"] = "image/gif"
+                data["mediaUhqEnabled"] = True
 
-        #     else: raise exceptions.SpecifyType(fileType)
+            else: raise exceptions.SpecifyType(fileType)
 
-        #     data["mediaUploadValue"] = b64encode(file.read()).decode()
+            data["mediaUploadValue"] = b64encode(file.read()).decode()
 
 
         response = self.session.post(
             url=f"{api}/x{self.comId}/s/chat/thread/{chatId}/message",
             json=data
         )
 
@@ -755,15 +752,15 @@
             - **pinChat** : If the Chat should Pinned or not.
 
         **Returns**
             - **Success** : 200 (int)
 
             - **Fail** : :meth:`Exceptions <aminofix.lib.util.exceptions>`
         """
-        data = {"timestamp": int(timestamp() * 1000)}
+        data = dict()
 
         if title: data["title"] = title
         if content: data["content"] = content
         if icon: data["icon"] = icon
         if keywords: data["keywords"] = keywords
         if announcement: data["extensions"] = {"announcement": announcement}
         if pinAnnouncement: data["extensions"] = {"pinAnnouncement": pinAnnouncement}
@@ -1150,15 +1147,15 @@
         }
 
         for key, value in object_types.items():
             if value['id']:
                 response = self.session.get(f"{value['url']}?start={start}&size={size}")
                 break
         else:
-            raise exceptions.SpecifyType()
+            raise exceptions.SpecifyType
 
         return objects.TippedUsersSummary(response.json()).TippedUsersSummary
 
 
     def get_chat_threads(self, start: int = 0, size: int = 25):
         """
         List of Chats the account is in.
@@ -1253,15 +1250,15 @@
             response = self.session.get(f"{api}/x{self.comId}/s/item/{wikiId}")
             return objects.GetWikiInfo(response.json()).GetWikiInfo
 
         elif fileId:
             response = self.session.get(f"{api}/x{self.comId}/s/shared-folder/files/{fileId}")
             return objects.SharedFolderFile(response.json()["file"]).SharedFolderFile
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
     def get_blog_comments(self, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, sorting: str = "newest", start: int = 0, size: int = 25):
         if sorting not in ["newest", "oldest", "top"]:
             raise ValueError("Invalid sorting type. Must be 'newest', 'oldest' or 'top'.")
 
         sorting = "vote" if sorting == "top" else sorting
 
@@ -1272,15 +1269,15 @@
         }
 
         for key, value in object_types.items():
             if value['id']:
                 response = self.session.get(f"{value['url']}?sort={sorting}&start={start}&size={size}")
                 break
         else:
-            raise exceptions.SpecifyType()
+            raise exceptions.SpecifyType
 
         return objects.CommentList(response.json()["commentList"]).CommentList
 
 
     def get_blog_categories(self, size: int = 25):
         response = self.session.get(f"{api}/x{self.comId}/s/blog-category?size={size}")
         return objects.BlogCategoryList(response.json()["blogCategoryList"]).BlogCategoryList
@@ -1428,15 +1425,15 @@
             data["adminOpValue"] = {"featuredType": 1}
             url = f"{api}/x{self.comId}/s/item/{wikiId}/admin"
 
         elif chatId:
             data["adminOpValue"] = {"featuredType": 5}
             url = f"{api}/x{self.comId}/s/chat/thread/{chatId}/admin"
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
 
         return response.json()
 
     def unfeature(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None):
         data = {
@@ -1460,15 +1457,15 @@
             url = f"{api}/x{self.comId}/s/item/{wikiId}/admin"
 
         elif chatId:
             data["adminOpValue"] = {"featuredType": 0}
             
             url = f"{api}/x{self.comId}/s/chat/thread/{chatId}/admin"
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
 
         return response.json()
 
     def hide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
         data = {
@@ -1508,15 +1505,15 @@
 
         elif fileId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 9
 
             url = f"{api}/x{self.comId}/s/shared-folder/files/{fileId}/admin"
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
         return response.json()
 
     def unhide(self, userId: str = None, chatId: str = None, blogId: str = None, wikiId: str = None, quizId: str = None, fileId: str = None, reason: str = None):
         data = {
             "adminOpNote": {
@@ -1555,15 +1552,15 @@
 
         elif fileId:
             data["adminOpName"] = 110
             data["adminOpValue"] = 0
 
             url = f"{api}/x{self.comId}/s/shared-folder/files/{fileId}/admin"
 
-        else: raise exceptions.SpecifyType()
+        else: raise exceptions.SpecifyType
 
         response = self.session.post(url, json=data)
         return response.json()
 
     def edit_titles(self, userId: str, tlt: list):
 
         data = {
@@ -1667,38 +1664,14 @@
         response = self.session.get(f"{api}/x{self.comId}/s/feed/quiz-trending?start={start}&size={size}")
         return objects.BlogList(response.json()["blogList"]).BlogList
 
     def get_best_quiz(self, start: int = 0, size: int = 25):
         response = self.session.get(f"{api}/x{self.comId}/s/feed/quiz-best-quizzes?start={start}&size={size}")
         return objects.BlogList(response.json()["blogList"]).BlogList
 
-    def send_action(self, actions: list, blogId: str = None, quizId: str = None, lastAction: bool = False):
-        # Action List
-        # Browsing
-
-        if lastAction is True: t = 306
-        else: t = 304
-
-        data = {
-            "o": {
-                "actions": actions,
-                "target": f"ndc://x{self.comId}/",
-                "ndcId": int(self.comId),
-                "params": {"topicIds": [45841, 17254, 26542, 42031, 22542, 16371, 6059, 41542, 15852]},
-            },
-            "t": t
-        }
-
-        if blogId is not None or quizId is not None:
-            data["target"] = f"ndc://x{self.comId}/blog/{blogId}"
-            if blogId is not None: data["params"]["blogType"] = 0
-            if quizId is not None: data["params"]["blogType"] = 6
-
-        return self.send(dumps(data))
-
     # Provided by "spectrum#4691"
     def purchase(self, objectId: str, objectType: int, aminoPlus: bool = True, autoRenew: bool = False):
         data = {
             "objectId": objectId,
             "objectType": objectType,
             "v": 1,
         }
```

### Comparing `amino.light.py-0.0.8/PKG-INFO` & `amino.light.py-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: amino.light.py
-Version: 0.0.8
-Summary: Best Amino.py alternative
-Author: AugustLight
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-Requires-Dist: requests
-Requires-Dist: websocket-client
-
 # AminoLightPy
 ## _The best Amino.py alternative!_
 
 Why should you choose this library?
 
 ## Features
 
@@ -47,12 +31,16 @@
 Want to contribute? Great!
 
 
 Contact me on telegram to suggest ideas!
 
 -> @AugustLight
 
+## API Reference
+Read The Docs: [Link Here](https://aminopy.readthedocs.io/en/latest/index.html)
+
+p.s: documentation is still up to date
 ## License
 
 MIT
 
-**Free Software, Hell Yeah!**
+**Free Software, Hell Yeah!**
```

### Comparing `amino.light.py-0.0.8/amino.light.py.egg-info/PKG-INFO` & `amino.light.py-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: amino.light.py
-Version: 0.0.8
+Version: 0.0.9
 Summary: Best Amino.py alternative
 Author: AugustLight
 License: MIT
+Keywords: amino,aminoapps,amino.fix,amino.light,amino.ligt.py,AminoLightPy,amino,amino-bot,narvii,medialab,api,python,python3,python3.x,minori,august,augustlight
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
@@ -47,12 +48,16 @@
 Want to contribute? Great!
 
 
 Contact me on telegram to suggest ideas!
 
 -> @AugustLight
 
+## API Reference
+Read The Docs: [Link Here](https://aminopy.readthedocs.io/en/latest/index.html)
+
+p.s: documentation is still up to date
 ## License
 
 MIT
 
 **Free Software, Hell Yeah!**
```

### Comparing `amino.light.py-0.0.8/amino.light.py.egg-info/SOURCES.txt` & `amino.light.py-0.0.9/amino.light.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

