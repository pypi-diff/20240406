# Comparing `tmp/glhf-0.0.1.dev5.tar.gz` & `tmp/glhf-0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glhf-0.0.1.dev5.tar", last modified: Sat Apr  6 07:00:53 2024, max compression
+gzip compressed data, was "glhf-0.0a1.tar", last modified: Sat Mar 16 16:21:46 2024, max compression
```

## Comparing `glhf-0.0.1.dev5.tar` & `glhf-0.0a1.tar`

### file list

```diff
@@ -1,31 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 07:00:53.261387 glhf-0.0.1.dev5/
--rw-rw-rw-   0        0        0    18429 2024-03-16 14:03:23.000000 glhf-0.0.1.dev5/LICENSE
--rw-rw-rw-   0        0        0    22768 2024-04-06 07:00:53.255616 glhf-0.0.1.dev5/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-03-16 14:08:37.000000 glhf-0.0.1.dev5/README.md
--rw-rw-rw-   0        0        0     1006 2024-04-06 06:57:15.000000 glhf-0.0.1.dev5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 07:00:53.261387 glhf-0.0.1.dev5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-06 07:00:53.133123 glhf-0.0.1.dev5/src/
-drwxrwxrwx   0        0        0        0 2024-04-06 07:00:53.195355 glhf-0.0.1.dev5/src/glhf/
--rw-rw-rw-   0        0        0      113 2024-03-18 16:20:13.000000 glhf-0.0.1.dev5/src/glhf/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-06 06:49:20.000000 glhf-0.0.1.dev5/src/glhf/__main__.py
--rw-rw-rw-   0        0        0     5568 2024-03-26 15:12:32.000000 glhf-0.0.1.dev5/src/glhf/base.py
--rw-rw-rw-   0        0        0     2657 2024-03-20 15:53:49.000000 glhf-0.0.1.dev5/src/glhf/bot.py
--rw-rw-rw-   0        0        0     4548 2024-04-06 06:48:51.000000 glhf-0.0.1.dev5/src/glhf/cli.py
--rw-rw-rw-   0        0        0     7736 2024-03-30 06:23:34.000000 glhf-0.0.1.dev5/src/glhf/client.py
--rw-rw-rw-   0        0        0    12402 2024-03-22 15:21:49.000000 glhf-0.0.1.dev5/src/glhf/gui.py
--rw-rw-rw-   0        0        0     2212 2024-03-20 06:04:54.000000 glhf-0.0.1.dev5/src/glhf/helper.py
-drwxrwxrwx   0        0        0        0 2024-04-06 07:00:53.246868 glhf-0.0.1.dev5/src/glhf/resource/
--rw-rw-rw-   0        0        0    78596 2023-09-14 22:27:18.000000 glhf-0.0.1.dev5/src/glhf/resource/Quicksand-Bold.ttf
--rw-rw-rw-   0        0        0     1813 2024-01-17 15:21:51.000000 glhf-0.0.1.dev5/src/glhf/resource/city.png
--rw-rw-rw-   0        0        0     2121 2024-01-17 15:22:12.000000 glhf-0.0.1.dev5/src/glhf/resource/crown.png
--rw-rw-rw-   0        0        0     1789 2024-01-17 15:21:15.000000 glhf-0.0.1.dev5/src/glhf/resource/mountain.png
--rw-rw-rw-   0        0        0     1252 2024-01-17 15:22:35.000000 glhf-0.0.1.dev5/src/glhf/resource/obstacle.png
--rw-rw-rw-   0        0        0    16731 2024-03-30 06:21:17.000000 glhf-0.0.1.dev5/src/glhf/server.py
--rw-rw-rw-   0        0        0     1039 2024-03-24 12:48:33.000000 glhf-0.0.1.dev5/src/glhf/typing_.py
--rw-rw-rw-   0        0        0     8331 2024-03-26 08:43:46.000000 glhf-0.0.1.dev5/src/glhf/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 07:00:53.251511 glhf-0.0.1.dev5/src/glhf.egg-info/
--rw-rw-rw-   0        0        0    22768 2024-04-06 07:00:53.000000 glhf-0.0.1.dev5/src/glhf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2024-04-06 07:00:53.000000 glhf-0.0.1.dev5/src/glhf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 07:00:53.000000 glhf-0.0.1.dev5/src/glhf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2024-04-06 07:00:53.000000 glhf-0.0.1.dev5/src/glhf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-06 07:00:53.000000 glhf-0.0.1.dev5/src/glhf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-16 16:21:46.961485 glhf-0.0a1/
+-rw-rw-rw-   0        0        0    18429 2024-03-16 14:03:23.000000 glhf-0.0a1/LICENSE
+-rw-rw-rw-   0        0        0    22690 2024-03-16 16:21:46.946765 glhf-0.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-03-16 14:08:37.000000 glhf-0.0a1/README.md
+drwxrwxrwx   0        0        0        0 2024-03-16 16:21:46.883462 glhf-0.0a1/glhf/
+-rw-rw-rw-   0        0        0      113 2024-03-16 14:56:01.000000 glhf-0.0a1/glhf/__init__.py
+-rw-rw-rw-   0        0        0     5436 2024-03-16 12:58:47.000000 glhf-0.0a1/glhf/base.py
+-rw-rw-rw-   0        0        0     9450 2024-03-16 14:55:30.000000 glhf-0.0a1/glhf/bot.py
+-rw-rw-rw-   0        0        0     7751 2024-03-16 13:03:33.000000 glhf-0.0a1/glhf/client.py
+-rw-rw-rw-   0        0        0    12152 2024-03-15 14:56:03.000000 glhf-0.0a1/glhf/gui.py
+-rw-rw-rw-   0        0        0     8872 2024-03-16 13:25:48.000000 glhf-0.0a1/glhf/helper.py
+-rw-rw-rw-   0        0        0    13990 2024-03-16 13:14:52.000000 glhf-0.0a1/glhf/server.py
+-rw-rw-rw-   0        0        0     1019 2024-02-20 08:32:19.000000 glhf-0.0a1/glhf/typing_.py
+drwxrwxrwx   0        0        0        0 2024-03-16 16:21:46.935977 glhf-0.0a1/glhf.egg-info/
+-rw-rw-rw-   0        0        0    22690 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-03-16 16:21:46.000000 glhf-0.0a1/glhf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      889 2024-03-16 14:46:16.000000 glhf-0.0a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-16 16:21:46.961485 glhf-0.0a1/setup.cfg
```

### Comparing `glhf-0.0.1.dev5/LICENSE` & `glhf-0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `glhf-0.0.1.dev5/PKG-INFO` & `glhf-0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glhf
-Version: 0.0.1.dev5
+Version: 0.0a1
 Summary: Good luck, have fun! A generals.io bot framework.
 Author-email: Hong-Chang Huang <seer852741@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -349,19 +349,17 @@
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygame-ce==2.4.1
-Requires-Dist: python-socketio[asyncio_client]==5.11.1
+Requires-Dist: python-socketio==5.11.1
 Requires-Dist: ortools==9.9.3963
 Requires-Dist: igraph==0.11.4
-Requires-Dist: fire==0.6.0
-Requires-Dist: rich==13.7.1
 
 # GLHF | Generals.io Bot Framework
 
 :warning: **NOTE: This is a template README and the code is still a work in progress.**
 
 Short description of the repository.
```

### Comparing `glhf-0.0.1.dev5/README.md` & `glhf-0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `glhf-0.0.1.dev5/pyproject.toml` & `glhf-0.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [build-system]
 requires = ["setuptools>=69.1.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glhf"
-version = "0.0.1.dev5"
+version = "0.0a1"
 dependencies = [
   "pygame-ce==2.4.1",
-  "python-socketio[asyncio_client]==5.11.1",
+  "python-socketio==5.11.1",
   "ortools==9.9.3963",
   "igraph==0.11.4",
-  "fire==0.6.0",
-  "rich==13.7.1",
 ]
 requires-python = ">= 3.12"
 authors = [{ name = "Hong-Chang Huang", email = "seer852741@gmail.com" }]
 description = "Good luck, have fun! A generals.io bot framework."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
@@ -23,10 +21,7 @@
   "Development Status :: 2 - Pre-Alpha",
   "Topic :: Software Development :: Libraries",
   "Topic :: Games/Entertainment :: Real Time Strategy",
   "Topic :: Games/Entertainment :: Simulation",
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Programming Language :: Python :: 3.12",
 ]
-
-[tool.setuptools.package-data]
-"glhf.resource" = ["*"]
```

### Comparing `glhf-0.0.1.dev5/src/glhf/base.py` & `glhf-0.0a1/glhf/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 from abc import abstractmethod
 from typing import Any, Protocol
 
+from glhf.helper import methodlike
 from glhf.typing_ import GameStartDict, GameUpdateDict, QueueUpdateDict
-from glhf.utils import methodlike
 
 __all__ = "ServerProtocol", "ClientProtocol", "BotProtocol"
 
 
 class ServerProtocol(Protocol):
     # ============================================================
     # send
@@ -67,24 +67,25 @@
     # run
     # ============================================================
 
     @abstractmethod
     async def connect(
         self,
         client: ClientProtocol,
-        user_id: str,
     ) -> None: ...
 
     @abstractmethod
     async def disconnect(
         self,
         client: ClientProtocol,
-        user_id: str,
     ) -> None: ...
 
+    @abstractmethod
+    async def run(self) -> None: ...
+
 
 class ClientProtocol(Protocol):
     # ============================================================
     # recieve
     # ============================================================
 
     @abstractmethod
@@ -141,21 +142,14 @@
 
     @abstractmethod
     def surrender(self) -> asyncio.Task[None]: ...
 
     @abstractmethod
     def attack(self, start: int, end: int, is50: bool) -> asyncio.Task[None]: ...
 
-    # ============================================================
-    # run
-    # ============================================================
-
-    @abstractmethod
-    async def run(self) -> None: ...
-
 
 class BotProtocol(Protocol):
     # ============================================================
     # recieve
     # ============================================================
 
     @methodlike
@@ -203,11 +197,14 @@
     def game_over(self) -> Any: ...
 
     # ============================================================
     # run
     # ============================================================
 
     @abstractmethod
-    async def run(self, client: ClientProtocol) -> None: ...
+    def set_client(self, client: ClientProtocol) -> None: ...
+
+    @abstractmethod
+    async def run(self) -> None: ...
 
 
 class GUIProtocol(Protocol): ...
```

### Comparing `glhf-0.0.1.dev5/src/glhf/client.py` & `glhf-0.0a1/glhf/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+from __future__ import annotations
 import asyncio
+
 from typing import Any
+from uuid import uuid4
 
 from socketio import AsyncClient
 
 from glhf.base import BotProtocol, ClientProtocol, ServerProtocol
 from glhf.gui import PygameGUI
 from glhf.typing_ import GameStartDict, GameUpdateDict, QueueUpdateDict
 
@@ -22,14 +25,16 @@
     ) -> None:
         self.userid = userid
         self.username = username
         self.queue_id = ""
         self.server = server
         self.bot = bot
         self.gui = gui
+        bot.set_client(self)
+        self.uuid = uuid4()
 
     # ============================================================
     # recieve
     # ============================================================
 
     def stars(self, data: dict[str, float]) -> None:
         self.bot.stars(data)
@@ -47,15 +52,15 @@
         self.bot.queue_update(data)
 
     def pre_game_start(self) -> None:
         self.bot.pre_game_start()
 
     def game_start(self, data: GameStartDict, _: Any = None) -> None:
         self.bot.game_start(data)
-        self.gui.game_start(data)
+        self.gui.game_start.set()
 
     def game_update(self, data: GameUpdateDict, _: Any = None) -> None:
         self.bot.game_update(data)
         self.gui.game_update(data)
 
     def game_won(self, _1: Any = None, _2: Any = None) -> None:
         self.bot.game_won()
@@ -94,27 +99,26 @@
         return self.server.attack(self, start, end, is50)
 
     # ============================================================
     # run
     # ============================================================
 
     def __hash__(self) -> int:
-        return hash(self.userid)
+        return hash(self.uuid)
 
     async def __aenter__(self) -> None:
-        self.gui.__enter__()
-        await self.server.connect(self, self.userid)
+        await self.server.connect(self)
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
-        self.gui.__exit__(exc_type, exc_val, exc_tb)
-        await self.server.disconnect(self, self.userid)
+        await self.server.disconnect(self)
 
     async def run(self) -> None:
         async with self:
-            await self.bot.run(self)
+            with self.gui:
+                await self.bot.run()
 
 
 class SocketioClient(AsyncClient, ClientProtocol):
     def __init__(
         self,
         userid: str,
         username: str,
@@ -127,14 +131,15 @@
 
         self.userid = userid
         self.username = username
         self.queue_id = ""
         self.bot = bot
         self.gui = gui
 
+        bot.set_client(self)
         self.event(self.stars)
         self.event(self.rank)
         self.event(self.chat_message)
         self.event(self.notify)
         self.event(self.queue_update)
         self.event(self.pre_game_start)
         self.event(self.game_start)
@@ -163,15 +168,15 @@
         self.bot.queue_update(data)
 
     def pre_game_start(self) -> None:
         self.bot.pre_game_start()
 
     def game_start(self, data: GameStartDict, _: Any = None) -> None:
         self.bot.game_start(data)
-        self.gui.game_start(data)
+        self.gui.game_start.set()
 
     def game_update(self, data: GameUpdateDict, _: Any = None) -> None:
         self.bot.game_update(data)
         self.gui.game_update(data)
 
     def game_won(self, _1: Any = None, _2: Any = None) -> None:
         self.bot.game_won()
@@ -208,27 +213,26 @@
         )
 
     def leave_game(self) -> asyncio.Task[None]:
         return asyncio.create_task(self.emit("leave_game"))
 
     def surrender(self) -> asyncio.Task[None]:
         return asyncio.create_task(self.emit("surrender"))
-
+    
     def attack(self, start: int, end: int, is50: bool) -> asyncio.Task[None]:
         return asyncio.create_task(self.emit("attack", (start, end, is50)))
 
     # ============================================================
     # run
     # ============================================================
 
     async def __aenter__(self) -> None:
-        self.gui.__enter__()
         await self.connect(WSURL, transports=["websocket"])
 
     async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
-        self.gui.__exit__(exc_type, exc_val, exc_tb)
         await self.disconnect()
         await self.wait()
 
     async def run(self) -> None:
         async with self:
-            await self.bot.run(self)
+            with self.gui:
+                await self.bot.run()
```

### Comparing `glhf-0.0.1.dev5/src/glhf/gui.py` & `glhf-0.0a1/glhf/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from functools import lru_cache
 from itertools import product
 from os import PathLike
-from pathlib import Path
 from threading import Event, Thread
 from typing import IO, Sequence
 
 import pygame
 from pygame import (
     Color,
     Rect,
@@ -18,17 +17,16 @@
     image,
     mouse,
     sprite,
     time,
     transform,
 )
 
-from glhf.helper import patch
-from glhf.typing_ import GameStartDict, GameUpdateDict
-from glhf.utils import signalize, streamify
+from glhf.helper import event_method, patch, queue_method
+from glhf.typing_ import GameUpdateDict
 
 __all__ = ("PygameGUI",)
 
 type AnyPath = str | bytes | PathLike[str] | PathLike[bytes]
 type FileArg = AnyPath | IO[bytes] | IO[str]
 type Coordinate = Sequence[float]
 
@@ -52,27 +50,25 @@
     0x483D8BFF,
 )
 PALETTE = tuple(map(Color, PALETTE))
 ARROWS = "↑↓←→"
 WHITE = Color("white")
 BLACK = Color("black")
 
-path = Path(__file__).parent
-
 
 class CachedResource:
     __slots__ = "font_", "city", "crown", "mountain", "obstacle"
 
     def __init__(
         self,
-        font_: FileArg = path / "resource/Quicksand-Bold.ttf",
-        city: FileArg = path / "resource/city.png",
-        crown: FileArg = path / "resource/crown.png",
-        mountain: FileArg = path / "resource/mountain.png",
-        obstacle: FileArg = path / "resource/obstacle.png",
+        font_: FileArg = "glhf/resource/Quicksand-Bold.ttf",
+        city: FileArg = "glhf/resource/city.png",
+        crown: FileArg = "glhf/resource/crown.png",
+        mountain: FileArg = "glhf/resource/mountain.png",
+        obstacle: FileArg = "glhf/resource/obstacle.png",
     ) -> None:
         self.font_ = font_
         load = image.load
         self.city = load(city).convert_alpha()
         self.crown = load(crown).convert_alpha()
         self.mountain = load(mountain).convert_alpha()
         self.obstacle = load(obstacle).convert_alpha()
@@ -334,28 +330,20 @@
 
         self.dirty = 1
 
 
 class PygameGUI(Thread):
     WINDOWSIZE = 800, 600
 
-    @streamify
-    def game_start(self, data: GameStartDict) -> GameStartDict:
-        return data
-
-    @streamify
-    def game_update(self, data: GameUpdateDict) -> GameUpdateDict:
-        return data
-
-    @signalize
-    def game_over(self) -> None:
-        self.game_update.close()
+    game_update = queue_method()
+    game_start = event_method()
+    game_over = event_method()
 
     def __init__(self, **kwargs) -> None:
-        super().__init__(name=f"{type(self).__name__}-{id(self):X}", **kwargs)
+        super().__init__(name=f"{type(self).__name__}({id(self):X})", **kwargs)
         self.quit = Event()
 
     def __enter__(self) -> None:
         self.start()
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         if exc_type is None:
@@ -392,33 +380,35 @@
                         move += e.rel
 
             bg.fast_update(window_resize)
             map_.fast_update(zoom, move, self.game_update.get())
 
             rects = group.draw(window)
             if rects:
-                display.update(rects)
+                pygame.display.update(rects)
 
             clock.tick(60)
             # print(f"\r{clock.get_fps():0>7.1f}", end="")
 
     def run(self) -> None:
         pygame.init()
         # pygame.RESIZABLE | pygame.SCALED
+        quit = self.quit
+        game_start = self.game_start
         try:
             window = display.set_mode(self.WINDOWSIZE)
-            while not self.quit.is_set():
+            while not quit.is_set():
                 for e in event.get():
                     if e.type == pygame.QUIT:
                         return
-                if self.game_start.get() is not None:
+                if game_start.wait():
                     self.main(window)
         finally:
             pygame.quit()
-            self.quit.set()
+            quit.set()
 
 
 if __name__ == "__main__":
 
     def main() -> None:
         pass
```

### Comparing `glhf-0.0.1.dev5/src/glhf/server.py` & `glhf-0.0a1/glhf/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import asyncio
 import time
 from collections import deque
-from dataclasses import dataclass, field
 from itertools import combinations as C
 from itertools import product as P
 from random import Random
 from typing import Any
 
 import igraph as ig
 import ortools.sat.python.cp_model as cp
-from bidict import KeyDuplicationError, ValueDuplicationError, bidict
 from socketio import AsyncClient
 
 from glhf.base import ClientProtocol, ServerProtocol
-from glhf.helper import make_diff
-from glhf.utils import to_task
+from glhf.helper import make_diff, to_task
 
 WSURL = "wss://ws.generals.io"
 BOTKEY = "sd09fjd203i0ejwi_changeme"
 
 
 def make_2d_grid(
     row: int,
@@ -36,16 +33,14 @@
     g = ig.Graph.Lattice((col, row), circular=False)
     coords = [(x, y) for y, x in P(range(row), range(col))]
     vs = g.vs
     vs["coord"] = coords
     vs["name"] = [f"{x},{y}" for x, y in coords]
     vs["army"] = 0
     vs["terrain"] = -1
-    # vs["is_city"] = False
-    # vs["is_general"] = False
     return g
 
 
 def make_complete_map(
     row: int,
     col: int,
 ) -> tuple[list[int], ig.Graph]:
@@ -148,333 +143,227 @@
                 else:
                     v["army"] = army - v_army
                     v["terrain"] = u_terrain
             return True
     return False
 
 
-@dataclass(slots=True)
-class Queue:
-    id: str = ""
-    force_start: bool = False
-
-    def clear(self) -> None:
-        self.id = ""
-        self.force_start = False
-
-
-@dataclass(slots=True)
-class Game:
-    id: str = ""
-    left: bool = False
-    surrendered: bool = False
-    attacks: deque[tuple[int, int, bool]] = field(default_factory=deque)
-
-
-@dataclass(slots=True)
-class User:
-    id: str
-    name: str = "Anonymous"
-
-
-@dataclass(slots=True)
-class Player:
-    client: ClientProtocol
-    user: User
-    queue: Queue = field(default_factory=Queue)
-    game: Game = field(default_factory=Game)
-
-
 class LocalServer(ServerProtocol):
-    def __init__(
-        self,
-        row: int,
-        col: int,
-        moves_per_turn: int = 2,
-        turns_per_round: int = 25,
-        turns_per_sec: float = 1.0,
-    ) -> None:
+    def __init__(self, row: int, col: int) -> None:
+        self.clients: dict[ClientProtocol, str] = {}
         self.row = row
         self.col = col
-
-        self.user_ids: bidict[ClientProtocol, str] = bidict()
-        self.clients: bidict[str, ClientProtocol] = self.user_ids.inverse
-
-        self.users: dict[str, User] = {}
-        self.players: dict[str, Player] = {}
-        self.game_queues: dict[str, list[Player]] = {}
-
-        # settings
-        self.mpt = moves_per_turn
-        self.tpr = turns_per_round
-        self.tps = turns_per_sec
+        self.map_ = []
+        self.graph = make_2d_grid(row, col)
+        self.turn = 0
+        self.generals: list[int] = []
+        self.cities: list[int] = []
+        self.usernames: dict[str, str] = {}
+        self.player_ids: list[str] = []
+        self.queue_id = ""
+        self.move_queues: list[deque[tuple[int, int, bool]]] = []
 
     def random_connected_map(
         self,
-        graph: ig.Graph,
         seed: Any = None,
     ) -> None:
-        es = graph.es
-        vs = graph.vs
+        g = self.graph
+        es = g.es
+        vs = g.vs
         rng = Random(seed)
-        es["weight"] = [rng.random() for _ in range(graph.ecount())]
-        mst = graph.spanning_tree("weight")
+        es["weight"] = [rng.random() for _ in range(g.ecount())]
+        mst = g.spanning_tree("weight")
         leaves = mst.vs.select(_degree_le=1).indices
-        graph.delete_edges(_source=leaves)
+        g.delete_edges(_source=leaves)
         vs[leaves]["terrain"] = -2
 
-    def set_generals(self, graph: ig.Graph, generals: list[int]) -> None:
+    def set_generals(self, generals: list[int]) -> None:
+        """Sets the generals on the map.
+
+        Args:
+            generals: The list of generals.
+
+        Returns:
+            None
+        """
+        graph = self.graph
         vs = graph.vs
         for i, v in enumerate(vs[generals]):
             v["terrain"] = i
+        self.generals = generals
+        self.move_queues = [deque() for _ in generals]
 
     def dispersion_generals(
         self,
         n: int,
-        row: int,
-        col: int,
-        graph: ig.Graph,
         *,
         d_min: int = 9,
         seed: Any = None,
         verbose: bool = False,
-    ) -> list[int]:
-        vs = graph.vs
+    ) -> None:
+        """Randomly selects generals on the map.
+
+        Args:
+            n: The number of generals to select.
+
+        Keyword Args:
+            d_min: The minimum distance between any two generals.
+            seed: The seed for the random number generator.
+            verbose: A flag indicating whether to print the solver status.
+
+        Returns:
+            None
+        """
+        g = self.graph
+        vs = g.vs
 
         # sample vertices
         rng = Random(seed)
         indices = vs.select(_degree_gt=0).indices
         k = min(max(24, n * 12), len(indices))
         selects = rng.sample(indices, k)
 
         # update generals
-        d_max = row + col - 2
+        d_max = self.row + self.col - 2
         coords = vs[selects]["coord"]
         generals = p_dispersion(n, d_min, d_max, selects, coords, verbose)
-        self.set_generals(graph, generals)
-        return generals
+        self.set_generals(generals)
 
     # ============================================================
     # send
     # ============================================================
 
     @to_task
     async def stars_and_rank(self, client: ClientProtocol, user_id: str) -> None:
         pass
 
     @to_task
     async def set_username(
         self, client: ClientProtocol, user_id: str, username: str
     ) -> None:
-        if self.user_ids[client] != user_id:
-            raise
-        self.users[user_id].name = username
+        self.usernames[user_id] = username
 
     @to_task
     async def join_private(
         self, client: ClientProtocol, queue_id: str, user_id: str
     ) -> None:
-        if self.user_ids[client] != user_id:
-            raise
-        game_queue = self.game_queues.setdefault(queue_id, [])
-        player = self.players[user_id]
-        player.queue.id = queue_id
-        game_queue.append(player)
-        self._queue_update(queue_id)
+        self.queue_id = queue_id
+        self.clients[client] = user_id
+        self.player_ids.append(user_id)
+        asyncio.create_task(self.run())
 
     @to_task
     async def set_force_start(
         self, client: ClientProtocol, queue_id: str, do_force: bool
     ) -> None:
-        try:
-            user_id = self.user_ids[client]
-        except KeyError:
-            raise
-        players = self.game_queues[queue_id]
-        for player in players:
-            if player.user.id == user_id:
-                player.queue.force_start = do_force
-                break
-        else:
-            raise
-        self._queue_update(queue_id)
+        pass
 
     @to_task
     async def leave_game(self, client: ClientProtocol) -> None:
-        try:
-            user_id = self.user_ids[client]
-        except KeyError:
-            raise
-        player = self.players[user_id]
-        if player.game.id:
-            player.game.left = True
-        else:
-            raise
+        user_id = self.clients[client]
+        self.player_ids.remove(user_id)
 
     @to_task
     async def surrender(self, client: ClientProtocol) -> None:
-        try:
-            user_id = self.user_ids[client]
-        except KeyError:
-            raise
-        player = self.players[user_id]
-        if player.game.id:
-            player.game.surrendered = True
-        else:
-            raise
+        pass
 
     @to_task
     async def attack(
         self, client: ClientProtocol, start: int, end: int, is50: bool
     ) -> None:
         try:
-            user_id = self.user_ids[client]
-        except KeyError:
-            raise
-        player = self.players[user_id]
-        player.game.attacks.append((start, end, is50))
+            user_id = self.clients[client]
+            i = self.player_ids.index(user_id)
+        except (KeyError, ValueError):
+            pass
+        else:
+            self.move_queues[i].append((start, end, is50))
 
     # ============================================================
     # recieve
     # ============================================================
 
-    def _queue_update(self, queue_id: str) -> None:
-        try:
-            players = self.game_queues[queue_id]
-        except KeyError:
-            raise
-
-        for i, player in enumerate(players):
-            data = {
-                "playerIndices": i,
-                "isForcing": player.queue.force_start,
-                "usernames": [player.user.name for player in players],
-            }
-            player.client.queue_update(data)  # type: ignore
-
-        if sum(user_data.queue.force_start for user_data in players) >= 1:
-            del self.game_queues[queue_id]
-            for player in players:
-                player.queue.clear()
-                player.game.id = queue_id
-            asyncio.create_task(self.run(players))
-
-    def _game_start(self, players: list[Player]) -> None:
-        for i, player in enumerate(players):
-            player.client.game_start({"playerIndex": i})  # type: ignore
-
-    def _game_update(self, players: list[Player], turn, generals, map_diff) -> None:
-        for player in players:
-            player.client.game_update(
-                {
-                    "scores": [],
-                    "turn": turn,
-                    "stars": [],
-                    "attackIndex": 0,
-                    "generals": generals,
-                    "map_diff": map_diff,
-                    "cities_diff": [],
-                }
-            )
+    async def game_update(self) -> None:
+        g = self.graph
+        vs = g.vs
 
-    def _game_over(self, players: list[Player]) -> None:
-        for player in players:
-            player.client.game_over()
-
-    def _map_update(
-        self,
-        players: list[Player],
-        row: int,
-        col: int,
-        turn: int,
-        map_old: list[int],
-        generals: list[int],
-        cities: list[int],
-        graph: ig.Graph,
-    ) -> tuple[list[int], list[int]]:
-        vs = graph.vs
+        turn = self.turn + 1
 
         # move armies
-        for i, player in enumerate(players):
-            attacks = player.game.attacks
-            while attacks:
-                start, end, is50 = attacks.popleft()
-                if move_army(graph, i, start, end, is50):
+        for i, q in enumerate(self.move_queues):
+            while q:
+                start, end, is50 = q.popleft()
+                if move_army(g, i, start, end, is50):
                     break
 
         # update generals and cities
         if turn % 2 == 1:
-            for v in vs[generals]:
+            for v in vs[self.generals]:
                 v["army"] += 1
-            for v in vs[cities]:
+            for v in vs[self.cities]:
                 v["army"] += 1
 
         # update lands
         if turn > 1 and turn % 50 == 1:
             for v in vs.select(terrain_ge=0):
                 v["army"] += 1
 
-        map_new = [col, row]
-        map_new += vs["army"]
-        map_new += vs["terrain"]
+        map_ = [self.col, self.row]
+        map_ += vs["army"]
+        map_ += vs["terrain"]
+
+        map_diff = make_diff(map_, self.map_)
+        self.map_ = map_
+        self.turn = turn
 
-        map_diff = make_diff(map_new, map_old)
+        for c in self.clients.keys():
+            c.game_update(
+                {
+                    "scores": [],
+                    "turn": turn,
+                    "stars": [],
+                    "attackIndex": 0,
+                    "generals": self.generals,
+                    "map_diff": map_diff,
+                    "cities_diff": [],
+                }
+            )
 
-        return map_new, map_diff
+    # ============================================================
+    # recieve
+    # ============================================================
 
     # ============================================================
     # run
     # ============================================================
 
-    async def connect(self, client: ClientProtocol, user_id: str) -> None:
-        try:
-            self.user_ids.put(client, user_id)
-        except ValueDuplicationError:
-            raise
-        except KeyDuplicationError:
-            raise
-        if user_id not in self.users:
-            self.users[user_id] = User(user_id)
-        user = self.users[user_id]
-        self.players[user_id] = Player(client, user)
-
-    async def disconnect(self, client: ClientProtocol, user_id: str) -> None:
-        if self.user_ids[client] != user_id:
-            raise
-        del self.user_ids[client]
-
-    async def run(self, players: list[Player]) -> None:
-        row = self.row
-        col = self.col
-
-        graph = make_2d_grid(row, col)
-        self.random_connected_map(graph, 0)
-
-        map_: list[int] = []
-        generals: list[int] = self.dispersion_generals(2, row, col, graph)
-        cities: list[int] = []
-
-        t_start = time.monotonic()
-        secs_per_move = self.tps / self.mpt
-
-        self._game_start(players)
-
-        for turn in range(1, 52):
-            map_, map_diff = self._map_update(
-                players, row, col, turn, map_, generals, cities, graph
-            )
-            t_start += secs_per_move
-            t_end = time.monotonic()
-            await asyncio.sleep(max(0, t_start - t_end))
-            self._game_update(players, turn, generals, map_diff)
+    async def connect(self, client: ClientProtocol) -> None:
+        self.clients[client] = ""
+
+    async def disconnect(self, client: ClientProtocol) -> None:
+        del self.clients[client]
 
-            if __debug__:
-                pass
+    async def run(self) -> None:
+        self.random_connected_map(0)
+        self.dispersion_generals(2)
+
+        for c in self.clients.keys():
+            c.game_start({})  # type: ignore
+
+        start = time.monotonic()
+
+        for _ in range(51):
+            await self.game_update()
 
-        self._game_over(players)
+            end = time.monotonic()
+            await asyncio.sleep(max(0, 0.5 - (end - start)))
+            start = end
+
+        for c in self.clients.keys():
+            c.game_over()
 
 
 class SocketioServer:
     def __init__(self) -> None:
         self.sockets: dict[ClientProtocol, AsyncClient] = {}
 
     # ============================================================
@@ -521,15 +410,15 @@
             self.sockets[client].emit("attack", (start, end, is50))
         )
 
     # ============================================================
     # run
     # ============================================================
 
-    async def connect(self, client: ClientProtocol, user_id: str) -> None:
+    async def connect(self, client: ClientProtocol) -> None:
         c = AsyncClient(ssl_verify=False)
         self.sockets[client] = c
         c.event(client.stars)
         c.event(client.rank)
         c.event(client.chat_message)
         c.event(client.notify)
         c.event(client.queue_update)
@@ -537,15 +426,40 @@
         c.event(client.game_start)
         c.event(client.game_update)
         c.event(client.game_won)
         c.event(client.game_lost)
         c.event(client.game_over)
         await c.connect(WSURL, transports=["websocket"])
 
-    async def disconnect(self, client: ClientProtocol, user_id: str) -> None:
+    async def disconnect(self, client: ClientProtocol) -> None:
         c = self.sockets[client]
         del self.sockets[client]
         await c.disconnect()
         await c.wait()
 
     async def run(self) -> None:
         pass
+
+    # def draw_graph(self):
+    #     """Draws the graph representation of the map.
+
+    #     Returns:
+    #         A tuple containing the figure and axis objects.
+    #     """
+    #     import matplotlib.pyplot as plt
+
+    #     c, r = self.map_[:2]
+    #     g = self.graph
+    #     vs = g.vs
+    #     fig, ax = plt.subplots(
+    #         figsize=(c * 0.5, r * 0.5),
+    #         layout="tight",
+    #     )
+    #     ax.invert_yaxis()
+    #     ig.plot(
+    #         g,
+    #         ax,
+    #         layout=vs["coord"],
+    #         vertex_label=vs["name"],
+    #         vertex_label_size=4,
+    #     )
+    #     return fig, ax
```

### Comparing `glhf-0.0.1.dev5/src/glhf/typing_.py` & `glhf-0.0a1/glhf/typing_.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, NamedTuple, TypedDict
+from typing import Literal, TypedDict, NamedTuple, Any
 
 __all__ = "QueueUpdateDict", "GameStartDict", "GameUpdateDict", "GameUpdateTuple"
 
 
 class QueueUpdateDict(TypedDict):
     playerIndices: list[int]
     playerColors: list[int]
@@ -19,17 +19,17 @@
     playerIndex: int
     playerColors: list[int]
     replay_id: str
     chat_room: str
     usernames: list[str]
     teams: list[int]
     game_type: Literal["ffa", "1v1", "custom"]
-    swamps: list[Any]
-    lights: list[Any]
-    options: dict[str, Any]
+    swamps: list
+    lights: list
+    options: list
 
 
 class GameUpdateDict(TypedDict):
     scores: list[dict]
     turn: int
     stars: list[int]
     attackIndex: int
```

### Comparing `glhf-0.0.1.dev5/src/glhf/utils.py` & `glhf-0.0a1/glhf/helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,332 +1,361 @@
-from asyncio import Event as AEvent
-from asyncio import Queue as AQueue
-from asyncio import QueueEmpty, Task, create_task
+from __future__ import annotations
+
+from asyncio import Event as _AsyncioEvent
+from asyncio import Queue as _AsyncioQueue
+from asyncio import Task, create_task
+from collections import deque
 from functools import partial, update_wrapper, wraps
-from queue import Empty, Queue
-from threading import Event
 from typing import Any, Callable, Concatenate, Coroutine, Protocol, Self, overload
 
 __all__ = (
-    "methodlike",
-    "streamify",
-    "signalize",
-    "astreamify",
-    "asignalize",
-    "to_coro",
+    "patch",
+    "make_diff",
     "to_task",
+    "to_coro",
+    "asyncio_queueify",
+    "asyncio_eventify",
+    "queue_method",
+    "event_method",
 )
 
 
-# ============================================================
-# typing
-# ============================================================
+def coord_to_name(coord: tuple[int, int]) -> str:
+    """Converts a coordinate to a string representation."""
+    return f"{coord[0]},{coord[1]}"
+
+
+def coord_to_index(coord: tuple[int, int], col: int) -> int:
+    """Converts a coordinate to an index in a 1D list representation."""
+    return coord[0] * col + coord[1]
+
+
+def patch(old: list[int], diff: list[int]) -> list[int]:
+    new = []
+    i = 0
+    len_diff = len(diff)
+    while i < len_diff:
+        n = diff[i]
+        if n:
+            j = len(new)
+            new += old[j : j + n]
+        i += 1
+        if i == len_diff:
+            break
+        n = diff[i]
+        if n:
+            j = i + 1
+            new += diff[j : j + n]
+            i += n
+        i += 1
+    return new
+
+
+def make_diff(new: list[int], old: list[int]) -> list[int]:
+    diff = []
+    i = 0
+    j = 0
+    len_new = len(new)
+    len_old = len(old)
+    len_min = min(len_new, len_old)
+    while True:
+        while j < len_min and new[j] == old[j]:
+            j += 1
+        diff.append(j - i)
+        i = j
+        if j == len_min:
+            if len_new > len_old:
+                diff.append(len_new - len_old)
+                diff += new[len_old:]
+            break
+        while j < len_min and new[j] != old[j]:
+            j += 1
+        if j < len_min:
+            diff.append(j - i)
+            diff += new[i:j]
+            i = j
+        else:
+            diff.append(len_new - i)
+            diff += new[i:len_new]
+            break
+    return diff
+
+
+def to_task[**P, R](
+    wrapped: Callable[P, Coroutine[Any, Any, R]],
+) -> Callable[P, Task[R]]:
+    @wraps(wrapped)
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> Task[R]:
+        return create_task(wrapped(*args, **kwargs))
+
+    return wrapper
+
+
+def to_coro[**P, R](wrapped: Callable[P, R]) -> Callable[P, Coroutine[Any, Any, R]]:
+    @wraps(wrapped)
+    async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
+        return wrapped(*args, **kwargs)
+
+    return wrapper
+
 
-type _MethodType[T, **P, R] = Callable[Concatenate[T, P], R]
+type MethodType[T, **P, R] = Callable[Concatenate[T, P], R]
 
 
-class _MethodLike[T, **P, R](Protocol):
+class MethodLikeProtocol[T, **P, R](Protocol):
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
         /,
-    ) -> _MethodType[T, P, R]: ...
+    ) -> MethodType[T, P, R]: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
         /,
     ) -> Callable[P, R]: ...
 
 
-class _MethodDescriptor[T, **P, R](_MethodLike[T, P, R]):
-    def __set_name__(self, owner: type[T], name: str) -> None:
-        self.name = "_" + name
-
-    def __init__(self, wrapped: _MethodType[T, P, R]) -> None:
-        self.wrapped = wrapped
+def methodlike[T, **P, R](m: MethodType[T, P, R]) -> MethodLikeProtocol[T, P, R]:
+    return m
 
 
-def methodlike[T, **P, R](m: _MethodType[T, P, R]) -> _MethodLike[T, P, R]:
-    return m
+class MethodLike[T, **P, R](MethodLikeProtocol[T, P, R]):
+    def __set_name__(self, owner: type[T], name: str) -> None:
+        self.name = "_" + name
 
 
-# ============================================================
-# synchronous
-# ============================================================
+class _wrappedmethod[T, **P, R](MethodLike[T, P, R]):
+    def __init__(self, wrapped: MethodType[T, P, R]) -> None:
+        self.wrapped = wrapped
 
 
-class _Stream[**P, R]:
+class AsyncioQueue[**P, R](_AsyncioQueue[R | None]):
     __wrapped__: Callable[P, R]
 
     def __init__(self, wrapped: Callable[P, R]) -> None:
+        super().__init__()
         update_wrapper(self, wrapped)
-        self._queue: Queue[R | None] = Queue()
+        self._tasks: set[Task] = set()
+        self._close = _AsyncioEvent()
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
         item = self.__wrapped__(*args, **kwargs)
-        self._queue.put_nowait(item)
+        task = create_task(self.put(item))
+        self._tasks.add(task)
+        task.add_done_callback(self._tasks.remove)
         return item
 
-    def __iter__(self) -> Self:
+    def __aiter__(self) -> Self:
         return self
 
-    def __next__(self) -> R:
-        q = self._queue
-        item = q.get()
-        q.task_done()
+    async def __anext__(self) -> R:
+        item = await self.get()
+        self.task_done()
         if item is None:
-            raise StopIteration()
-        return item
-
-    def wait(self) -> R | None:
-        q = self._queue
-        item = q.get()
-        q.task_done()
+            raise StopAsyncIteration()
         return item
 
-    def get(self) -> R | None:
-        q = self._queue
-        try:
-            item = q.get_nowait()
-        except Empty:
-            return None
-        else:
-            q.task_done()
-            return item
-
-    def close(self) -> None:
-        self._queue.put_nowait(None)
+    def close(self) -> Task[None]:
+        return create_task(self.put(None))
 
 
-class _Signal[**P, R]:
-    __wrapped__: Callable[P, R]
-
-    def __init__(self, wrapped: Callable[P, R]) -> None:
-        update_wrapper(self, wrapped)
-        self.event = Event()
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        self.event.set()
-        return self.__wrapped__(*args, **kwargs)
-
-    def get(self) -> bool:
-        s = self.event.is_set()
-        if s:
-            self.event.clear()
-        return s
-
-    def wait(self) -> None:
-        self.event.wait()
-        self.event.clear()
-
-
-class streamify[T, **P, R](_MethodDescriptor[T, P, R]):
+class asyncio_queueify[T, **P, R](_wrappedmethod[T, P, R]):
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
-    ) -> _MethodType[T, P, R]: ...
+    ) -> MethodType[T, P, R]: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
-    ) -> _Stream[P, R]: ...
+    ) -> AsyncioQueue[P, R]: ...
 
     def __get__(
         self,
         instance: T | None,
         owner: type[T] | None = None,
     ) -> Any:
         if instance is None:
             return self.wrapped
         try:
             x = getattr(instance, self.name)
         except AttributeError:
-            x = _Stream(partial(self.wrapped, instance))
+            x = AsyncioQueue(partial(self.wrapped, instance))
             setattr(instance, self.name, x)
         return x
 
 
-class signalize[T, **P, R](_MethodDescriptor[T, P, R]):
+class AsyncioEvent[**P, R](_AsyncioEvent):
+    __wrapped__: Callable[P, R]
+
+    def __init__(self, wrapped: Callable[P, R]) -> None:
+        super().__init__()
+        update_wrapper(self, wrapped)
+
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
+        res = self.__wrapped__(*args, **kwargs)
+        self.set()
+        return res
+
+
+class asyncio_eventify[T, **P, R](_wrappedmethod[T, P, R]):
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
-    ) -> _MethodType[T, P, R]: ...
+    ) -> MethodType[T, P, R]: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
-    ) -> _Signal[P, R]: ...
+    ) -> AsyncioEvent[P, R]: ...
 
     def __get__(
         self,
         instance: T | None,
         owner: type[T] | None = None,
     ) -> Any:
         if instance is None:
             return self.wrapped
         try:
             x = getattr(instance, self.name)
         except AttributeError:
-            x = _Signal(partial(self.wrapped, instance))
+            x = AsyncioEvent(partial(self.wrapped, instance))
             setattr(instance, self.name, x)
         return x
 
 
-# ============================================================
-# asynchronous
-# ============================================================
-
-
-class _AStream[**P, R]:
-    __wrapped__: Callable[P, R]
-
-    def __init__(self, wrapped: Callable[P, R]) -> None:
-        update_wrapper(self, wrapped)
-        self._queue: AQueue[R | None] = AQueue()
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        item = self.__wrapped__(*args, **kwargs)
-        self._queue.put_nowait(item)
-        return item
-
-    def __aiter__(self) -> Self:
-        return self
-
-    async def __anext__(self) -> R:
-        q = self._queue
-        item = await q.get()
-        q.task_done()
-        if item is None:
-            raise StopAsyncIteration()
-        return item
-
-    async def wait(self) -> R | None:
-        q = self._queue
-        item = await q.get()
-        q.task_done()
+class _Queue[R](deque[R]):
+    def __call__(self, item: R) -> R:
+        self.append(item)
         return item
 
     def get(self) -> R | None:
-        q = self._queue
         try:
-            item = q.get_nowait()
-        except QueueEmpty:
+            return self.popleft()
+        except IndexError:
             return None
-        else:
-            q.task_done()
-            return item
-
-    def close(self) -> None:
-        self._queue.put_nowait(None)
-
-
-class _ASignal[**P, R]:
-    __wrapped__: Callable[P, R]
 
-    def __init__(self, wrapped: Callable[P, R]) -> None:
-        update_wrapper(self, wrapped)
-        self.event = AEvent()
-
-    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> R:
-        self.event.set()
-        return self.__wrapped__(*args, **kwargs)
 
-    def get(self) -> bool:
-        s = self.event.is_set()
-        if s:
-            self.event.clear()
-        return s
+class queue_method[T, R](MethodLike[T, [R], R]):
+    def __call__(self, instance: T, item: R) -> R:
+        return self.__get__(instance)(item)
 
-    async def wait(self) -> None:
-        await self.event.wait()
-        self.event.clear()
-
-
-class astreamify[T, **P, R](_MethodDescriptor[T, P, R]):
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
-    ) -> _MethodType[T, P, R]: ...
+    ) -> Self: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
-    ) -> _AStream[P, R]: ...
+    ) -> _Queue[R]: ...
 
     def __get__(
         self,
         instance: T | None,
         owner: type[T] | None = None,
     ) -> Any:
         if instance is None:
-            return self.wrapped
+            return self
         try:
             x = getattr(instance, self.name)
         except AttributeError:
-            x = _AStream(partial(self.wrapped, instance))
+            x = _Queue()
             setattr(instance, self.name, x)
         return x
 
 
-class asignalize[T, **P, R](_MethodDescriptor[T, P, R]):
+class _Event:
+    def __init__(self) -> None:
+        self._set = False
+
+    def __call__(self) -> None:
+        self.set()
+
+    def set(self) -> None:
+        self._set = True
+
+    def clear(self) -> None:
+        self._set = False
+
+    def wait(self) -> bool:
+        x = self._set
+        if self._set:
+            self.clear()
+        return x
+
+
+class event_method[T](MethodLike[T, [], None]):
+    def __call__(self, instance: T) -> None:
+        return self.__get__(instance)()
+
     @overload
     def __get__(
         self,
         instance: None,
         owner: type[T],
-    ) -> _MethodType[T, P, R]: ...
+    ) -> Self: ...
 
     @overload
     def __get__(
         self,
         instance: T,
         owner: type[T] | None = None,
-    ) -> _ASignal[P, R]: ...
+    ) -> _Event: ...
 
     def __get__(
         self,
         instance: T | None,
         owner: type[T] | None = None,
     ) -> Any:
         if instance is None:
-            return self.wrapped
+            return self
         try:
             x = getattr(instance, self.name)
         except AttributeError:
-            x = _ASignal(partial(self.wrapped, instance))
+            x = _Event()
             setattr(instance, self.name, x)
         return x
 
 
-def to_coro[**P, R](wrapped: Callable[P, R]) -> Callable[P, Coroutine[Any, Any, R]]:
-    @wraps(wrapped)
-    async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
-        return wrapped(*args, **kwargs)
-
-    return wrapper
-
-
-def to_task[**P, R](
-    wrapped: Callable[P, Coroutine[Any, Any, R]],
-) -> Callable[P, Task[R]]:
-    @wraps(wrapped)
-    def wrapper(*args: P.args, **kwargs: P.kwargs) -> Task[R]:
-        return create_task(wrapped(*args, **kwargs))
-
-    return wrapper
+class Map(list[int]):
+    @property
+    def shape(self) -> list[int]:
+        return self[:2:-1]
+
+    @property
+    def armies(self) -> list[list[int]]:
+        m = self
+        c, r = m[:2]
+        stop = 2 + c * r
+        return [m[i : i + r] for i in range(2, stop, r)]
+
+    @property
+    def terrain(self) -> list[list[int]]:
+        m = self
+        c, r = m[:2]
+        n = c * r
+        start = 2 + n
+        return [m[i : i + r] for i in range(start, start + n, r)]
+
+
+class Cities(list[int]):
+    @property
+    def cities(self) -> list[int]:
+        return self.copy()
```

### Comparing `glhf-0.0.1.dev5/src/glhf.egg-info/PKG-INFO` & `glhf-0.0a1/glhf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glhf
-Version: 0.0.1.dev5
+Version: 0.0a1
 Summary: Good luck, have fun! A generals.io bot framework.
 Author-email: Hong-Chang Huang <seer852741@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
@@ -349,19 +349,17 @@
 Classifier: Topic :: Games/Entertainment :: Simulation
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygame-ce==2.4.1
-Requires-Dist: python-socketio[asyncio_client]==5.11.1
+Requires-Dist: python-socketio==5.11.1
 Requires-Dist: ortools==9.9.3963
 Requires-Dist: igraph==0.11.4
-Requires-Dist: fire==0.6.0
-Requires-Dist: rich==13.7.1
 
 # GLHF | Generals.io Bot Framework
 
 :warning: **NOTE: This is a template README and the code is still a work in progress.**
 
 Short description of the repository.
```

