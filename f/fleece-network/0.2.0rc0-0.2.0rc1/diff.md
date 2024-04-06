# Comparing `tmp/fleece_network-0.2.0rc0.tar.gz` & `tmp/fleece_network-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleece_network-0.2.0rc0.tar", max compression
+gzip compressed data, was "fleece_network-0.2.0rc1.tar", max compression
```

## Comparing `fleece_network-0.2.0rc0.tar` & `fleece_network-0.2.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1045 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/README.md
--rw-r--r--   0        0        0        0 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/__init__.py
--rw-r--r--   0        0        0      349 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/candidate.py
--rw-r--r--   0        0        0    41179 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/ice.py
--rw-r--r--   0        0        0     6655 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/mdns.py
--rw-r--r--   0        0        0    12121 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/stun.py
--rw-r--r--   0        0        0    14905 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/turn.py
--rw-r--r--   0        0        0      264 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aioice/utils.py
--rw-r--r--   0        0        0     1226 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/__init__.py
--rw-r--r--   0        0        0      824 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/clock.py
--rw-r--r--   0        0        0      180 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/exceptions.py
--rw-r--r--   0        0        0    21027 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/rate.py
--rw-r--r--   0        0        0     1040 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcconfiguration.py
--rw-r--r--   0        0        0     6531 2024-04-04 11:59:31.091984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcdatachannel.py
--rw-r--r--   0        0        0    13595 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcdtlstransport.py
--rw-r--r--   0        0        0    11425 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcicetransport.py
--rw-r--r--   0        0        0    32180 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcpeerconnection.py
--rw-r--r--   0        0        0     4612 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcrtpparameters.py
--rw-r--r--   0        0        0    61599 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcsctptransport.py
--rw-r--r--   0        0        0      500 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtcsessiondescription.py
--rw-r--r--   0        0        0    24050 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/rtp.py
--rw-r--r--   0        0        0    21763 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/sdp.py
--rw-r--r--   0        0        0     2879 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/stats.py
--rw-r--r--   0        0        0      978 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/aiortc/utils.py
--rw-r--r--   0        0        0      716 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/messages.py
--rw-r--r--   0        0        0    21346 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/peer.py
--rw-r--r--   0        0        0        0 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/py.typed
--rw-r--r--   0        0        0     2144 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/fleece_network/signaling.py
--rw-r--r--   0        0        0      479 2024-04-04 11:59:31.095984 fleece_network-0.2.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1701 1970-01-01 00:00:00.000000 fleece_network-0.2.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      327 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/__init__.py
+-rw-r--r--   0        0        0     4060 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/candidate.py
+-rw-r--r--   0        0        0    41238 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/ice.py
+-rw-r--r--   0        0        0     6655 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/mdns.py
+-rw-r--r--   0        0        0    12298 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/stun.py
+-rw-r--r--   0        0        0    15077 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/turn.py
+-rw-r--r--   0        0        0      264 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aioice/utils.py
+-rw-r--r--   0        0        0     1226 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aiortc/__init__.py
+-rw-r--r--   0        0        0      824 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aiortc/clock.py
+-rw-r--r--   0        0        0      180 2024-04-06 11:22:41.411003 fleece_network-0.2.0rc1/fleece_network/aiortc/exceptions.py
+-rw-r--r--   0        0        0    21027 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rate.py
+-rw-r--r--   0        0        0     1040 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcconfiguration.py
+-rw-r--r--   0        0        0     6531 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcdatachannel.py
+-rw-r--r--   0        0        0    13595 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcdtlstransport.py
+-rw-r--r--   0        0        0    11425 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcicetransport.py
+-rw-r--r--   0        0        0    32180 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcpeerconnection.py
+-rw-r--r--   0        0        0     4612 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcrtpparameters.py
+-rw-r--r--   0        0        0    61599 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcsctptransport.py
+-rw-r--r--   0        0        0      500 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtcsessiondescription.py
+-rw-r--r--   0        0        0    24050 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/rtp.py
+-rw-r--r--   0        0        0    21763 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/sdp.py
+-rw-r--r--   0        0        0     2879 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/stats.py
+-rw-r--r--   0        0        0      978 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/aiortc/utils.py
+-rw-r--r--   0        0        0      716 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/messages.py
+-rw-r--r--   0        0        0    21451 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/peer.py
+-rw-r--r--   0        0        0        0 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/py.typed
+-rw-r--r--   0        0        0     2144 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/fleece_network/signaling.py
+-rw-r--r--   0        0        0      479 2024-04-06 11:22:41.415003 fleece_network-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 fleece_network-0.2.0rc1/PKG-INFO
```

### Comparing `fleece_network-0.2.0rc0/fleece_network/aioice/candidate.py` & `fleece_network-0.2.0rc1/fleece_network/aioice/candidate.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aioice/ice.py` & `fleece_network-0.2.0rc1/fleece_network/aioice/ice.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     return candidate
 
 
 class CandidatePair:
     def __init__(self, protocol, remote_candidate: Candidate) -> None:
         self.task: Optional[asyncio.Task] = None
         self.nominated = False
-        self.protocol = protocol
+        self.protocol: StunProtocol = protocol
         self.remote_candidate = remote_candidate
         self.remote_nominated = False
         self.state = CandidatePair.State.FROZEN
 
     def __repr__(self) -> str:
         return "CandidatePair(%s -> %s)" % (self.local_addr, self.remote_addr)
 
@@ -164,14 +164,15 @@
 
     @property
     def local_addr(self) -> Tuple[str, int]:
         return (self.local_candidate.host, self.local_candidate.port)
 
     @property
     def local_candidate(self) -> Candidate:
+        assert self.protocol.local_candidate
         return self.protocol.local_candidate
 
     @property
     def remote_addr(self) -> Tuple[str, int]:
         return (self.remote_candidate.host, self.remote_candidate.port)
 
     class State(enum.Enum):
```

### Comparing `fleece_network-0.2.0rc0/fleece_network/aioice/mdns.py` & `fleece_network-0.2.0rc1/fleece_network/aioice/mdns.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aioice/stun.py` & `fleece_network-0.2.0rc1/fleece_network/aioice/stun.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from abc import abstractmethod
 import asyncio
 import binascii
 import enum
 import hmac
 import ipaddress
 from collections import OrderedDict
 from struct import pack, unpack
-from typing import Callable, Dict, List, Optional, Tuple
+from typing import Callable, Dict, List, Optional, Protocol, Tuple
 
 from .utils import random_transaction_id
 
 COOKIE = 0x2112A442
 FINGERPRINT_LENGTH = 8
 FINGERPRINT_XOR = 0x5354554E
 HEADER_LENGTH = 20
@@ -262,20 +263,25 @@
 
 
 class TransactionTimeout(TransactionError):
     def __str__(self) -> str:
         return "STUN transaction timed out"
 
 
+class SendStun(Protocol):
+    @abstractmethod
+    def send_stun(self, message: Message, addr: Tuple[str, int]) -> None: ...
+
+
 class Transaction:
     def __init__(
         self,
         request: Message,
         addr: Tuple[str, int],
-        protocol,
+        protocol: SendStun,
         retransmissions: Optional[int] = None,
     ) -> None:
         self.__addr = addr
         self.__future: asyncio.Future[Tuple[Message, Tuple[str, int]]] = (
             asyncio.Future()
         )
         self.__request = request
```

### Comparing `fleece_network-0.2.0rc0/fleece_network/aioice/turn.py` & `fleece_network-0.2.0rc1/fleece_network/aioice/turn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 import asyncio
 import hashlib
 import logging
 import socket
 import struct
 import time
 from typing import (
@@ -177,26 +178,27 @@
         """
         Delete the TURN allocation.
         """
         if self.refresh_task:
             self.refresh_task.cancel()
             self.refresh_task = None
 
-        request = stun.Message(
-            message_method=stun.Method.REFRESH, message_class=stun.Class.REQUEST
-        )
-        request.attributes["LIFETIME"] = 0
-        try:
-            await self.request_with_retry(request)
-        except stun.TransactionError:
-            # we do not care, we need to shutdown
-            pass
-
-        logger.info("TURN allocation deleted %s", self.relayed_address)
-        self.transport.close()
+            request = stun.Message(
+                message_method=stun.Method.REFRESH, message_class=stun.Class.REQUEST
+            )
+            request.attributes["LIFETIME"] = 0
+            try:
+                await self.request_with_retry(request)
+            except stun.TransactionError:
+                # we do not care, we need to shutdown
+                pass
+
+            logger.info("TURN allocation deleted %s", self.relayed_address)
+            # inner protocol itself does not need to close the outer transport
+            # because each transport has its unique inner protocol
 
     async def refresh(self, time_to_expiry) -> None:
         """
         Periodically refresh the TURN allocation.
         """
         while True:
             await asyncio.sleep(5 / 6 * time_to_expiry)
```

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/__init__.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/__init__.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/clock.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/clock.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rate.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rate.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rtcconfiguration.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcconfiguration.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rtcdatachannel.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcdatachannel.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rtcdtlstransport.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcdtlstransport.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rtcicetransport.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcicetransport.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rtcpeerconnection.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcpeerconnection.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rtcrtpparameters.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcrtpparameters.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rtcsctptransport.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rtcsctptransport.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/rtp.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/rtp.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/sdp.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/sdp.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/stats.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/stats.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/aiortc/utils.py` & `fleece_network-0.2.0rc1/fleece_network/aiortc/utils.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/messages.py` & `fleece_network-0.2.0rc1/fleece_network/messages.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc0/fleece_network/peer.py` & `fleece_network-0.2.0rc1/fleece_network/peer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Coroutine,
     Optional,
     Protocol,
     TypeVar,
     Union,
     get_type_hints,
 )
-from aiortc import (  # type: ignore
+from .aiortc import (  # type: ignore
     RTCPeerConnection,
     RTCConfiguration,
     RTCIceServer,
     RTCDataChannel,
     RTCSessionDescription,
 )
 from fastapi import HTTPException, Response
@@ -302,22 +302,25 @@
         self.state = PeerConnection.State.DEAD
         self.in_channel: Optional[InwardDataChannel] = None
         self.out_channel: Optional[OutwardDataChannel] = None
         self.recv_stream = anyio.Lock()
         self.lock = anyio.Lock()
         self.condition = anyio.Condition(self.lock)
 
-    async def _kill_inner(self):
+    def _reset_inner(self):
         self.state = PeerConnection.State.DEAD
-        if self.inner is not None:
-            await self.inner.close()
-            self.inner = None
         self.in_channel = None
         self.out_channel = None
 
+    async def _kill_inner(self):
+        self._reset_inner()
+        if self.inner is not None:
+            self.tg.start_soon(self.inner.close)
+            self.inner = None
+
     async def _init_inner(self) -> RTCPeerConnection:
         pc = RTCPeerConnection(
             RTCConfiguration(
                 [
                     RTCIceServer(config[0], config[1], config[2])
                     for config in self.configs
                 ]
@@ -338,16 +341,16 @@
                     self.condition.notify_all()
 
                     self._logger.info(
                         "Connection (%s, %s) changes state to CONNECTED",
                         self.from_id,
                         self.to_id,
                     )
-                elif pc.connectionState == "failed":
-                    await self._kill_inner()
+                elif pc.connectionState == "failed" or pc.connectionState == "closed":
+                    await self._reset_inner()
 
                     self._logger.info(
                         "Connection (%s, %s) changes state to FAILED",
                         self.from_id,
                         self.to_id,
                     )
```

### Comparing `fleece_network-0.2.0rc0/fleece_network/signaling.py` & `fleece_network-0.2.0rc1/fleece_network/signaling.py`

 * *Files identical despite different names*

