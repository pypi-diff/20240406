# Comparing `tmp/promplate-0.3.3.post1.tar.gz` & `tmp/promplate-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate-0.3.3.post1.tar", max compression
+gzip compressed data, was "promplate-0.3.4.tar", max compression
```

## Comparing `promplate-0.3.3.post1.tar` & `promplate-0.3.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.3.post1/promplate/__init__.py
--rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.3.post1/promplate/chain/__init__.py
--rw-r--r--   0        0        0     2417 2024-02-05 15:21:12.418993 promplate-0.3.3.post1/promplate/chain/callback.py
--rw-r--r--   0        0        0    17779 2024-02-05 15:21:12.418993 promplate-0.3.3.post1/promplate/chain/node.py
--rw-r--r--   0        0        0     1333 2024-02-05 15:21:12.420965 promplate-0.3.3.post1/promplate/chain/utils.py
--rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.3.post1/promplate/llm/__init__.py
--rw-r--r--   0        0        0     1074 2024-02-05 15:21:12.421366 promplate-0.3.3.post1/promplate/llm/base.py
--rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.3.post1/promplate/llm/openai/__init__.py
--rw-r--r--   0        0        0     4368 2024-02-05 15:21:12.421366 promplate-0.3.3.post1/promplate/llm/openai/v0.py
--rw-r--r--   0        0        0     5449 2024-02-05 15:21:12.421366 promplate-0.3.3.post1/promplate/llm/openai/v1.py
--rw-r--r--   0        0        0       87 2024-02-05 14:52:39.252076 promplate-0.3.3.post1/promplate/prompt/__init__.py
--rw-r--r--   0        0        0     1590 2023-12-15 15:04:40.204809 promplate-0.3.3.post1/promplate/prompt/builder.py
--rw-r--r--   0        0        0     2976 2024-02-05 15:21:12.423189 promplate-0.3.3.post1/promplate/prompt/chat.py
--rw-r--r--   0        0        0     6839 2024-02-05 15:21:12.423189 promplate-0.3.3.post1/promplate/prompt/template.py
--rw-r--r--   0        0        0     3216 2024-02-05 15:21:12.423189 promplate-0.3.3.post1/promplate/prompt/utils.py
--rw-r--r--   0        0        0      214 2024-02-05 15:21:12.425491 promplate-0.3.3.post1/promplate/typing.py
--rw-r--r--   0        0        0     1631 2024-02-05 15:21:12.426021 promplate-0.3.3.post1/pyproject.toml
--rw-r--r--   0        0        0     1918 2024-02-05 15:12:05.370855 promplate-0.3.3.post1/README.md
--rw-r--r--   0        0        0     3247 1970-01-01 00:00:00.000000 promplate-0.3.3.post1/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.4/promplate/__init__.py
+-rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.4/promplate/chain/__init__.py
+-rw-r--r--   0        0        0     2309 2024-04-05 09:30:17.923274 promplate-0.3.4/promplate/chain/callback.py
+-rw-r--r--   0        0        0    17320 2024-04-06 09:47:54.814935 promplate-0.3.4/promplate/chain/node.py
+-rw-r--r--   0        0        0     1308 2024-02-06 11:24:26.943042 promplate-0.3.4/promplate/chain/utils.py
+-rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.4/promplate/llm/__init__.py
+-rw-r--r--   0        0        0     1043 2024-02-06 11:24:26.944273 promplate-0.3.4/promplate/llm/base.py
+-rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.4/promplate/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4125 2024-02-06 11:24:26.945287 promplate-0.3.4/promplate/llm/openai/v0.py
+-rw-r--r--   0        0        0     6002 2024-02-28 11:45:48.661575 promplate-0.3.4/promplate/llm/openai/v1.py
+-rw-r--r--   0        0        0       87 2024-04-06 09:45:04.214579 promplate-0.3.4/promplate/prompt/__init__.py
+-rw-r--r--   0        0        0     1633 2024-04-06 09:41:46.823783 promplate-0.3.4/promplate/prompt/builder.py
+-rw-r--r--   0        0        0     3216 2024-02-06 11:24:26.947313 promplate-0.3.4/promplate/prompt/chat.py
+-rw-r--r--   0        0        0     7301 2024-04-06 09:35:41.637869 promplate-0.3.4/promplate/prompt/template.py
+-rw-r--r--   0        0        0     3386 2024-04-06 08:33:51.420912 promplate-0.3.4/promplate/prompt/utils.py
+-rw-r--r--   0        0        0     1598 2024-04-06 10:40:23.943401 promplate-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1995 2024-04-06 10:35:03.295230 promplate-0.3.4/README.md
+-rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 promplate-0.3.4/PKG-INFO
```

### Comparing `promplate-0.3.3.post1/promplate/chain/callback.py` & `promplate-0.3.4/promplate/chain/callback.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-from typing import TYPE_CHECKING, Awaitable, Callable, Optional, Protocol, Tuple, Union
+from typing import TYPE_CHECKING, Awaitable, Callable, Protocol
 
 from ..prompt import Context
 
 if TYPE_CHECKING:
     from .node import AsyncProcess, ChainContext, Interruptable, Process
 
 
 class BaseCallback(Protocol):
-    def pre_process(self, context: "ChainContext") -> Optional[Union[Context, Awaitable[Optional[Context]]]]:
-        pass
+    def pre_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
 
-    def mid_process(self, context: "ChainContext") -> Optional[Union[Context, Awaitable[Optional[Context]]]]:
-        pass
+    def mid_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
 
-    def end_process(self, context: "ChainContext") -> Optional[Union[Context, Awaitable[Optional[Context]]]]:
-        pass
+    def end_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
 
-    def on_enter(self, node: "Interruptable", context: Optional[Context], config: Context) -> Tuple[Optional[Context], Context]:
+    def on_enter(self, node: "Interruptable", context: Context | None, config: Context) -> tuple[Context | None, Context]:
         return context, config
 
-    def on_leave(self, node: "Interruptable", context: "ChainContext", config: Context) -> Tuple["ChainContext", Context]:
+    def on_leave(self, node: "Interruptable", context: "ChainContext", config: Context) -> tuple["ChainContext", Context]:
         return context, config
 
 
 class Callback(BaseCallback):
     def __init__(
         self,
         *,
         pre_process: "Process | AsyncProcess | None" = None,
         mid_process: "Process | AsyncProcess | None" = None,
         end_process: "Process | AsyncProcess | None" = None,
-        on_enter: Optional[Callable[["Interruptable", Optional[Context], Context], Tuple[Optional[Context], Context]]] = None,
-        on_leave: Optional[Callable[["Interruptable", "ChainContext", Context], Tuple["ChainContext", Context]]] = None,
+        on_enter: Callable[["Interruptable", Context | None, Context], tuple[Context | None, Context]] | None = None,
+        on_leave: Callable[["Interruptable", "ChainContext", Context], tuple["ChainContext", Context]] | None = None,
     ):
         self._pre_process = pre_process
         self._mid_process = mid_process
         self._end_process = end_process
         self._on_enter = on_enter
         self._on_leave = on_leave
```

### Comparing `promplate-0.3.3.post1/promplate/chain/node.py` & `promplate-0.3.4/promplate/chain/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from inspect import isclass
 from itertools import accumulate
 from typing import Callable, Mapping, MutableMapping, overload
 
-from ..llm.base import LLM, AsyncComplete, AsyncGenerate, Complete, Generate
+from ..llm.base import *
 from ..prompt.template import Context, Loader, SafeChainMapContext, Template
-from ..typing import AsyncIterable, Awaitable, Callable, Iterable, List, Mapping, MutableMapping, Optional, Protocol, Type, Union, cast, overload
 from .callback import BaseCallback, Callback
 from .utils import accumulate_any, resolve
 
 
 class ChainContext(SafeChainMapContext):
     @overload
     def __init__(self): ...
 
     @overload
-    def __init__(self, least: Optional[MutableMapping] = None): ...
+    def __init__(self, least: MutableMapping | None = None): ...
 
     @overload
-    def __init__(self, least: Optional[MutableMapping] = None, *maps: Mapping): ...
+    def __init__(self, least: MutableMapping | None = None, *maps: Mapping): ...
 
-    def __init__(self, least: Optional[MutableMapping] = None, *maps: Mapping):
+    def __init__(self, least: MutableMapping | None = None, *maps: Mapping):
         super().__init__({} if least is None else least, *maps)  # type: ignore
 
     @classmethod
     def ensure(cls, context):
         return context if isinstance(context, cls) else cls(context)
 
     @property
@@ -35,177 +34,177 @@
         self.__setitem__("__result__", result)
 
     @result.deleter
     def result(self):
         self.__delitem__("__result__")
 
 
-Process = Callable[[ChainContext], Optional[Context]]
+Process = Callable[[ChainContext], Context | None]
 
-AsyncProcess = Callable[[ChainContext], Awaitable[Optional[Context]]]
+AsyncProcess = Callable[[ChainContext], Awaitable[Context | None]]
 
 
 class AbstractNode(Protocol):
     def invoke(
         self,
-        context: Optional[Context] = None,
+        context: Context | None = None,
         /,
-        complete: Optional[Complete] = None,
+        complete: Complete | None = None,
         **config,
     ) -> ChainContext: ...
 
     async def ainvoke(
         self,
-        context: Optional[Context] = None,
+        context: Context | None = None,
         /,
-        complete: Union[Complete, Optional[AsyncComplete]] = None,
+        complete: Complete | AsyncComplete | None = None,
         **config,
     ) -> ChainContext: ...
 
     def stream(
         self,
-        context: Optional[Context] = None,
+        context: Context | None = None,
         /,
-        generate: Optional[Generate] = None,
+        generate: Generate | None = None,
         **config,
     ) -> Iterable[ChainContext]: ...
 
     def astream(
         self,
-        context: Optional[Context] = None,
+        context: Context | None = None,
         /,
-        generate: Union[Generate, Optional[AsyncGenerate]] = None,
+        generate: Generate | AsyncGenerate | None = None,
         **config,
     ) -> AsyncIterable[ChainContext]: ...
 
     @classmethod
     def _get_chain_type(cls):
         return Chain
 
     def __add__(self, chain: "AbstractNode"):
         if isinstance(chain, Chain):
             return self._get_chain_type()(self, *chain)
         return self._get_chain_type()(self, chain)
 
 
-def ensure_callbacks(callbacks: List[Union[BaseCallback, Type[BaseCallback]]]) -> List[BaseCallback]:
+def ensure_callbacks(callbacks: list[BaseCallback | type[BaseCallback]]) -> list[BaseCallback]:
     return [i() if isclass(i) else i for i in callbacks]
 
 
 class Interruptable(AbstractNode, Protocol):
     def _invoke(
         self,
         context: ChainContext,
         /,
-        complete: Optional[Complete],
-        callbacks: List[BaseCallback],
+        complete: Complete | None,
+        callbacks: list[BaseCallback],
         **config,
     ): ...
 
     async def _ainvoke(
         self,
         context: ChainContext,
         /,
-        complete: Union[Complete, Optional[AsyncComplete]],
-        callbacks: List[BaseCallback],
+        complete: Complete | AsyncComplete | None,
+        callbacks: list[BaseCallback],
         **config,
     ): ...
 
     def _stream(
         self,
         context: ChainContext,
         /,
-        generate: Optional[Generate],
-        callbacks: List[BaseCallback],
+        generate: Generate | None,
+        callbacks: list[BaseCallback],
         **config,
     ) -> Iterable: ...
 
     def _astream(
         self,
         context: ChainContext,
         /,
-        generate: Union[Generate, Optional[AsyncGenerate]],
-        callbacks: List[BaseCallback],
+        generate: Generate | AsyncGenerate | None,
+        callbacks: list[BaseCallback],
         **config,
     ) -> AsyncIterable: ...
 
-    callbacks: List[Union[BaseCallback, Type[BaseCallback]]]
+    callbacks: list[BaseCallback | type[BaseCallback]]
 
-    def enter(self, context: Optional[Context], config: Context):
-        callbacks: List[BaseCallback] = ensure_callbacks(self.callbacks)
+    def enter(self, context: Context | None, config: Context):
+        callbacks: list[BaseCallback] = ensure_callbacks(self.callbacks)
         for callback in callbacks:
             context, config = callback.on_enter(self, context, config)
         return context, config, callbacks
 
-    def leave(self, context: ChainContext, config: Context, callbacks: List[BaseCallback]):
+    def leave(self, context: ChainContext, config: Context, callbacks: list[BaseCallback]):
         for callback in reversed(callbacks):
             context, config = callback.on_leave(self, context, config)
         return context, config
 
-    def add_pre_processes(self, *processes: Union[Process, AsyncProcess]):
+    def add_pre_processes(self, *processes: Process | AsyncProcess):
         self.callbacks.extend(Callback(pre_process=i) for i in processes)
         return self
 
-    def add_mid_processes(self, *processes: Union[Process, AsyncProcess]):
+    def add_mid_processes(self, *processes: Process | AsyncProcess):
         self.callbacks.extend(Callback(mid_process=i) for i in processes)
         return self
 
-    def add_end_processes(self, *processes: Union[Process, AsyncProcess]):
+    def add_end_processes(self, *processes: Process | AsyncProcess):
         self.callbacks.extend(Callback(end_process=i) for i in processes)
         return self
 
-    def add_callbacks(self, *callbacks: Union[BaseCallback, Type[BaseCallback]]):
+    def add_callbacks(self, *callbacks: BaseCallback | type[BaseCallback]):
         self.callbacks.extend(callbacks)
         return self
 
-    def pre_process(self, process: Union[Process, AsyncProcess]):
+    def pre_process(self, process: Process | AsyncProcess):
         self.add_pre_processes(process)
         return process
 
-    def mid_process(self, process: Union[Process, AsyncProcess]):
+    def mid_process(self, process: Process | AsyncProcess):
         self.add_mid_processes(process)
         return process
 
-    def end_process(self, process: Union[Process, AsyncProcess]):
+    def end_process(self, process: Process | AsyncProcess):
         self.add_end_processes(process)
         return process
 
-    def callback(self, callback: Union[BaseCallback, Type[BaseCallback]]):
+    def callback(self, callback: BaseCallback | type[BaseCallback]):
         self.add_callbacks(callback)
         return callback
 
     @staticmethod
-    def _apply_pre_processes(context: ChainContext, callbacks: List[BaseCallback]):
+    def _apply_pre_processes(context: ChainContext, callbacks: list[BaseCallback]):
         for callback in callbacks:
-            context.update(cast(Context, callback.pre_process(context) or {}))
+            context |= cast(Context, callback.pre_process(context) or {})
 
     @staticmethod
-    def _apply_mid_processes(context: ChainContext, callbacks: List[BaseCallback]):
+    def _apply_mid_processes(context: ChainContext, callbacks: list[BaseCallback]):
         for callback in callbacks:
-            context.update(cast(Context, callback.mid_process(context) or {}))
+            context |= cast(Context, callback.mid_process(context) or {})
 
     @staticmethod
-    def _apply_end_processes(context: ChainContext, callbacks: List[BaseCallback]):
+    def _apply_end_processes(context: ChainContext, callbacks: list[BaseCallback]):
         for callback in reversed(callbacks):
-            context.update(cast(Context, callback.end_process(context) or {}))
+            context |= cast(Context, callback.end_process(context) or {})
 
     @staticmethod
-    async def _apply_async_pre_processes(context: ChainContext, callbacks: List[BaseCallback]):
+    async def _apply_async_pre_processes(context: ChainContext, callbacks: list[BaseCallback]):
         for callback in callbacks:
-            context.update(cast(Context, await resolve(callback.pre_process(context)) or {}))
+            context |= cast(Context, await resolve(callback.pre_process(context)) or {})
 
     @staticmethod
-    async def _apply_async_mid_processes(context: ChainContext, callbacks: List[BaseCallback]):
+    async def _apply_async_mid_processes(context: ChainContext, callbacks: list[BaseCallback]):
         for callback in callbacks:
-            context.update(cast(Context, await resolve(callback.mid_process(context)) or {}))
+            context |= cast(Context, await resolve(callback.mid_process(context)) or {})
 
     @staticmethod
-    async def _apply_async_end_processes(context: ChainContext, callbacks: List[BaseCallback]):
+    async def _apply_async_end_processes(context: ChainContext, callbacks: list[BaseCallback]):
         for callback in reversed(callbacks):
-            context.update(cast(Context, await resolve(callback.end_process(context)) or {}))
+            context |= cast(Context, await resolve(callback.end_process(context)) or {})
 
     def invoke(self, context=None, /, complete=None, **config) -> ChainContext:
         context, config, callbacks = self.enter(context, config)
         context = ChainContext.ensure(context)
 
         try:
             self._invoke(ChainContext(context, self.context), complete, callbacks, **config)
@@ -266,118 +265,118 @@
                 raise jump from None
             if jump.into is not None:
                 async for i in jump.into.astream(context, generate, **config):
                     yield i
         else:
             context, config = self.leave(context, config, callbacks)
 
-    _context: Optional[Context]
+    _context: Context | None
 
     @property
     def context(self):
         if self._context is None:
             self._context = {}
         return self._context
 
     @context.setter
-    def context(self, context: Optional[Context]):
+    def context(self, context: Context | None):
         self._context = context
 
     @context.deleter
     def context(self):
         self._context = None
 
 
 class Node(Loader, Interruptable):
     def __init__(
         self,
-        template: Union[Template, str],
-        partial_context: Optional[Context] = None,
-        llm: Optional[LLM] = None,
+        template: Template | str,
+        partial_context: Context | None = None,
+        llm: LLM | None = None,
         **config,
     ):
         self.template = Template(template) if isinstance(template, str) else template
         self._context = partial_context
-        self.callbacks: List[Union[BaseCallback, Type[BaseCallback]]] = []
+        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
         self.llm = llm
         self.run_config = config
 
     def _invoke(self, context, /, complete, callbacks, **config):
         complete = cast(Complete, self.llm.complete if self.llm else complete)
         assert complete is not None
 
         prompt = self.render(context, callbacks)
 
-        context.result = complete(prompt, **({**self.run_config, **config}))
+        context.result = complete(prompt, **(self.run_config | config))
 
         self._apply_mid_processes(context, callbacks)
 
         self._apply_end_processes(context, callbacks)
 
     def _stream(self, context, /, generate, callbacks, **config):
         generate = cast(Generate, self.llm.generate if self.llm else generate)
         assert generate is not None
 
         prompt = self.render(context, callbacks)
 
-        for result in accumulate(generate(prompt, **({**self.run_config, **config}))):
+        for result in accumulate(generate(prompt, **(self.run_config | config))):
             context.result = result
             self._apply_mid_processes(context, callbacks)
             yield
 
         self._apply_end_processes(context, callbacks)
 
     async def _ainvoke(self, context, /, complete, callbacks, **config):
-        complete = cast(Union[Complete, AsyncComplete], self.llm.complete if self.llm else complete)
+        complete = cast(Complete | AsyncComplete, self.llm.complete if self.llm else complete)
         assert complete is not None
 
         prompt = await self.arender(context, callbacks)
 
-        context.result = await resolve(complete(prompt, **({**self.run_config, **config})))
+        context.result = await resolve(complete(prompt, **(self.run_config | config)))
 
         await self._apply_async_mid_processes(context, callbacks)
 
         await self._apply_async_end_processes(context, callbacks)
 
     async def _astream(self, context, /, generate, callbacks, **config):
-        generate = cast(Union[Generate, AsyncGenerate], self.llm.generate if self.llm else generate)
+        generate = cast(Generate | AsyncGenerate, self.llm.generate if self.llm else generate)
         assert generate is not None
 
         prompt = await self.arender(context, callbacks)
 
-        async for result in accumulate_any(generate(prompt, **({**self.run_config, **config}))):
+        async for result in accumulate_any(generate(prompt, **(self.run_config | config))):
             context.result = result
             await self._apply_async_mid_processes(context, callbacks)
             yield
 
         await self._apply_async_end_processes(context, callbacks)
 
-    def render(self, context: Optional[Context] = None, callbacks: Optional[List[BaseCallback]] = None):
+    def render(self, context: Context | None = None, callbacks: list[BaseCallback] | None = None):
         if callbacks is None:
             callbacks = ensure_callbacks(self.callbacks)
         context = ChainContext(context, self.context)
         self._apply_pre_processes(context, callbacks)
         return self.template.render(context)
 
-    async def arender(self, context: Optional[Context] = None, callbacks: Optional[List[BaseCallback]] = None):
+    async def arender(self, context: Context | None = None, callbacks: list[BaseCallback] | None = None):
         if callbacks is None:
             callbacks = ensure_callbacks(self.callbacks)
         context = ChainContext(context, self.context)
         await self._apply_async_pre_processes(context, callbacks)
         return await self.template.arender(context)
 
     def __str__(self):
         return f"</{self.name}/>"
 
 
 class Loop(Interruptable):
-    def __init__(self, chain: AbstractNode, partial_context: Optional[Context] = None):
+    def __init__(self, chain: AbstractNode, partial_context: Context | None = None):
         self.chain = chain
         self._context = partial_context
-        self.callbacks: List[Union[BaseCallback, Type[BaseCallback]]] = []
+        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
 
     def _invoke(self, context, /, complete, callbacks, **config):
         while True:
             self._apply_pre_processes(context, callbacks)
             self.chain.invoke(context, complete, **config)
             self._apply_mid_processes(context, callbacks)
             self._apply_end_processes(context, callbacks)
@@ -403,64 +402,64 @@
             async for _ in self.chain.astream(context, generate, **config):
                 await self._apply_async_mid_processes(context, callbacks)
                 yield
             await self._apply_async_end_processes(context, callbacks)
 
 
 class Chain(Interruptable):
-    def __init__(self, *nodes: AbstractNode, partial_context: Optional[Context] = None):
+    def __init__(self, *nodes: AbstractNode, partial_context: Context | None = None):
         self.nodes = list(nodes)
         self._context = partial_context
-        self.callbacks: List[Union[BaseCallback, Type[BaseCallback]]] = []
+        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
 
     @classmethod
     def _get_chain_type(cls):
         return cls
 
     def __iadd__(self, chain: AbstractNode):
         self.nodes.append(chain)
         return self
 
     def __iter__(self):
         return iter(self.nodes)
 
-    def _invoke(self, context, /, complete, callbacks: List[BaseCallback], **config):
+    def _invoke(self, context, /, complete, callbacks: list[BaseCallback], **config):
         self._apply_pre_processes(context, callbacks)
         for node in self.nodes:
             node.invoke(context, complete, **config)
             self._apply_mid_processes(context, callbacks)
         self._apply_end_processes(context, callbacks)
 
-    async def _ainvoke(self, context, /, complete, callbacks: List[BaseCallback], **config):
+    async def _ainvoke(self, context, /, complete, callbacks: list[BaseCallback], **config):
         await self._apply_async_pre_processes(context, callbacks)
         for node in self.nodes:
             await node.ainvoke(context, complete, **config)
             await self._apply_async_mid_processes(context, callbacks)
         await self._apply_async_end_processes(context, callbacks)
 
-    def _stream(self, context, /, generate, callbacks: List[BaseCallback], **config):
+    def _stream(self, context, /, generate, callbacks: list[BaseCallback], **config):
         self._apply_pre_processes(context, callbacks)
         for node in self.nodes:
             for _ in node.stream(context, generate, **config):
                 self._apply_mid_processes(context, callbacks)
                 yield
         self._apply_end_processes(context, callbacks)
 
-    async def _astream(self, context, /, generate, callbacks: List[BaseCallback], **config):
+    async def _astream(self, context, /, generate, callbacks: list[BaseCallback], **config):
         await self._apply_async_pre_processes(context, callbacks)
         for node in self.nodes:
             async for _ in node.astream(context, generate, **config):
                 await self._apply_async_mid_processes(context, callbacks)
                 yield
         await self._apply_async_end_processes(context, callbacks)
 
     def __repr__(self):
         return " + ".join(map(str, self.nodes))
 
 
 class Jump(Exception):
-    def __init__(self, into: Optional[Interruptable] = None, out_of: Optional[Interruptable] = None):
+    def __init__(self, into: Interruptable | None = None, out_of: Interruptable | None = None):
         self.into = into
         self.out_of = out_of
 
     def __str__(self):
         return f"{self.out_of} does not exist in the chain hierarchy"
```

### Comparing `promplate-0.3.3.post1/promplate/chain/utils.py` & `promplate-0.3.4/promplate/chain/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from inspect import Parameter, isasyncgen, isawaitable, signature
 from itertools import accumulate
-from typing import AsyncIterable, Awaitable, Callable, Iterable, List, TypeVar, Union, cast
+from typing import AsyncIterable, Awaitable, Callable, Iterable, TypeVar, cast
 
 T = TypeVar("T")
 
 
-def appender(to_append: List[T]) -> Callable[[T], T]:
+def appender(to_append: list[T]) -> Callable[[T], T]:
     def append_processer(func: T) -> T:
         to_append.append(func)
 
         return func
 
     return append_processer
 
@@ -18,29 +18,29 @@
     return p.kind is Parameter.POSITIONAL_OR_KEYWORD or p.kind is Parameter.KEYWORD_ONLY
 
 
 def count_position_parameters(func):
     return sum(map(is_positional_parameter, signature(func).parameters.values()))
 
 
-async def resolve(maybe_awaitable: Union[T, Awaitable[T]], /) -> T:
+async def resolve(maybe_awaitable: T | Awaitable[T], /) -> T:
     while isawaitable(maybe_awaitable):
         maybe_awaitable = await maybe_awaitable
 
     return maybe_awaitable  # type: ignore
 
 
 async def async_accumulate(async_iterable: AsyncIterable[str]):
     result = ""
     async for delta in async_iterable:
         result += delta
         yield result
 
 
-def accumulate_any(any_iterable: Union[Iterable[str], AsyncIterable[str]]):
+def accumulate_any(any_iterable: Iterable[str] | AsyncIterable[str]):
     if isasyncgen(any_iterable):
         return async_accumulate(any_iterable)
 
     async def _():
         for i in accumulate(cast(Iterable[str], any_iterable)):
             yield i
```

### Comparing `promplate-0.3.3.post1/promplate/llm/base.py` & `promplate-0.3.4/promplate/llm/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import AsyncIterable, Awaitable, Iterable, Protocol, Union, cast
+from typing import AsyncIterable, Awaitable, Iterable, Protocol, cast
 
 
 class Configurable:
     def __init__(self, **config):
         for key, val in config.items():
             setattr(self, key, val)
 
@@ -25,12 +25,12 @@
 
 
 class AsyncGenerate(Protocol):
     def __call__(self, prompt, /, **config) -> AsyncIterable[str]: ...
 
 
 class LLM(Protocol):
-    @partial(cast, Union[Complete, AsyncComplete])
-    def complete(self, prompt, /, **config) -> Union[str, Awaitable[str]]: ...
+    @partial(cast, Complete | AsyncComplete)
+    def complete(self, prompt, /, **config) -> str | Awaitable[str]: ...
 
-    @partial(cast, Union[Generate, AsyncGenerate])
-    def generate(self, prompt, /, **config) -> Union[Iterable[str], AsyncIterable[str]]: ...
+    @partial(cast, Generate | AsyncGenerate)
+    def generate(self, prompt, /, **config) -> Iterable[str] | AsyncIterable[str]: ...
```

### Comparing `promplate-0.3.3.post1/promplate/llm/openai/v0.py` & `promplate-0.3.4/promplate/llm/openai/v0.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 from importlib.metadata import metadata
-from typing import TYPE_CHECKING, Any, List, Optional, Union
+from typing import TYPE_CHECKING, Any
 
 import openai
 from openai import ChatCompletion, Completion  # type: ignore
 
 from ...prompt.chat import Message, ensure
-from ..base import AsyncComplete, AsyncGenerate, Complete, Configurable, Generate
+from ..base import *
 
 meta = metadata("promplate")
 
 if openai.api_key is None:
     openai.api_key = ""
 
-openai.app_info = {  # type: ignore
-    **(openai.app_info or {}),  # type: ignore
-    **{
-        "name": "Promplate",
-        "version": meta["version"],
-        "url": meta["home-page"],
-    },
+openai.app_info = (openai.app_info or {}) | {  # type: ignore
+    "name": "Promplate",
+    "version": meta["version"],
+    "url": meta["home-page"],
 }
 
 
 if TYPE_CHECKING:
 
     class Config(Configurable):
         def __init__(
             self,
             model: str,
-            temperature: Optional[Union[float, int]] = None,
-            top_p: Optional[Union[float, int]] = None,
-            stop: Optional[Union[str, List[str]]] = None,
-            max_tokens: Optional[int] = None,
-            api_key: Optional[str] = None,
-            api_base: Optional[str] = None,
+            temperature: float | int | None = None,
+            top_p: float | int | None = None,
+            stop: str | list[str] | None = None,
+            max_tokens: int | None = None,
+            api_key: str | None = None,
+            api_base: str | None = None,
             **other_config,
         ):
             self.model = model
             self.temperature = temperature
             self.top_p = top_p
             self.stop = stop
             self.max_tokens = max_tokens
@@ -53,69 +50,69 @@
 
 else:
     Config = Configurable
 
 
 class TextComplete(Config, Complete):
     def __call__(self, text: str, /, **config):
-        config = {**self._config, **config, **{"stream": False, "prompt": text}}
+        config = self._config | config | {"stream": False, "prompt": text}
         result: Any = Completion.create(**config)
         return result["choices"][0]["text"]
 
 
 class AsyncTextComplete(Config, AsyncComplete):
     async def __call__(self, text: str, /, **config):
-        config = {**self._config, **config, **{"stream": False, "prompt": text}}
+        config = self._config | config | {"stream": False, "prompt": text}
         result: Any = await Completion.acreate(**config)
         return result["choices"][0]["text"]
 
 
 class TextGenerate(Config, Generate):
     def __call__(self, text: str, /, **config):
-        config = {**self._config, **config, **{"stream": True, "prompt": text}}
+        config = self._config | config | {"stream": True, "prompt": text}
         stream: Any = Completion.create(**config)
         for event in stream:
             yield event["choices"][0]["text"]
 
 
 class AsyncTextGenerate(Config, AsyncGenerate):
     async def __call__(self, text: str, /, **config):
-        config = {**self._config, **config, **{"stream": True, "prompt": text}}
+        config = self._config | config | {"stream": True, "prompt": text}
         stream: Any = await Completion.acreate(**config)
         async for event in stream:
             yield event["choices"][0]["text"]
 
 
 class ChatComplete(Config, Complete):
-    def __call__(self, messages: Union[List[Message], str], /, **config):
+    def __call__(self, messages: list[Message] | str, /, **config):
         messages = ensure(messages)
-        config = {**self._config, **config, **{"stream": False, "messages": messages}}
+        config = self._config | config | {"stream": False, "messages": messages}
         result: Any = ChatCompletion.create(**config)
         return result["choices"][0]["message"]["content"]
 
 
 class AsyncChatComplete(Config, AsyncComplete):
-    async def __call__(self, messages: Union[List[Message], str], /, **config):
+    async def __call__(self, messages: list[Message] | str, /, **config):
         messages = ensure(messages)
-        config = {**self._config, **config, **{"stream": False, "messages": messages}}
+        config = self._config | config | {"stream": False, "messages": messages}
         result: Any = await ChatCompletion.acreate(**config)
         return result["choices"][0]["message"]["content"]
 
 
 class ChatGenerate(Config, Generate):
-    def __call__(self, messages: Union[List[Message], str], /, **config):
+    def __call__(self, messages: list[Message] | str, /, **config):
         messages = ensure(messages)
-        config = {**self._config, **config, **{"stream": True, "messages": messages}}
+        config = self._config | config | {"stream": True, "messages": messages}
         stream: Any = ChatCompletion.create(**config)
         for event in stream:
             delta: dict = event["choices"][0]["delta"]
             yield delta.get("content", "")
 
 
 class AsyncChatGenerate(Config, AsyncGenerate):
-    async def __call__(self, messages: Union[List[Message], str], /, **config):
+    async def __call__(self, messages: list[Message] | str, /, **config):
         messages = ensure(messages)
-        config = {**self._config, **config, **{"stream": True, "messages": messages}}
+        config = self._config | config | {"stream": True, "messages": messages}
         stream: Any = await ChatCompletion.acreate(**config)
         async for event in stream:
             delta: dict = event["choices"][0]["delta"]
             yield delta.get("content", "")
```

### Comparing `promplate-0.3.3.post1/promplate/llm/openai/v1.py` & `promplate-0.3.4/promplate/llm/openai/v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from copy import copy
 from functools import cached_property
 from types import MappingProxyType
+from typing import TYPE_CHECKING, Any, Callable, ParamSpec, TypeVar
 
 from openai import AsyncClient, Client  # type: ignore
 
 from ...prompt.chat import Message, ensure
 from ...prompt.utils import _get_aclient, _get_client, get_user_agent
-from ...typing import TYPE_CHECKING, Any, Callable, List, ParamSpec, TypeVar, Union
-from ..base import LLM, Configurable
+from ..base import *
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def same_params_as(_: Callable[P, Any]):
     def func(__init__: Callable[..., None]) -> Callable[P, None]:
@@ -23,26 +23,28 @@
 class Config(Configurable):
     def __init__(self, **config):
         super().__init__(**config)
         self._run_config = {}
 
     def bind(self, **run_config):
         obj = copy(self)
-        obj._run_config = {**self._run_config, **run_config}
+        obj._run_config = self._run_config | run_config
         return obj
 
     @cached_property
     def _user_agent(self):
-        return get_user_agent(self, ("OpenAI", "openai"))
+        from openai.version import VERSION
+
+        return get_user_agent(self, ("OpenAI", VERSION))
 
     @property
     def _config(self):  # type: ignore
         ua_header = {"User-Agent": self._user_agent}
         config = dict(super()._config)
-        config["default_headers"] = {**config.get("default_headers", {}), **ua_header}
+        config["default_headers"] = config.get("default_headers", {}) | ua_header
         return MappingProxyType(config)
 
     @cached_property
     def _client(self):
         if "http_client" in self._config:
             return Client(**self._config)
         else:
@@ -68,74 +70,86 @@
 
 else:
     ClientConfig = AsyncClientConfig = Config
 
 
 class TextComplete(ClientConfig):
     def __call__(self, text: str, /, **config):
-        config = {**self._run_config, **config, **{"stream": False, "prompt": text}}
+        config = self._run_config | config | {"stream": False, "prompt": text}
         result = self._client.completions.create(**config)
         return result.choices[0].text
 
 
 class AsyncTextComplete(AsyncClientConfig):
     async def __call__(self, text: str, /, **config):
-        config = {**self._run_config, **config, **{"stream": False, "prompt": text}}
+        config = self._run_config | config | {"stream": False, "prompt": text}
         result = await self._aclient.completions.create(**config)
         return result.choices[0].text
 
 
 class TextGenerate(ClientConfig):
     def __call__(self, text: str, /, **config):
-        config = {**self._run_config, **config, **{"stream": True, "prompt": text}}
+        config = self._run_config | config | {"stream": True, "prompt": text}
         stream = self._client.completions.create(**config)
         for event in stream:
-            yield event.choices[0].text
+            try:
+                yield event.choices[0].text
+            except AttributeError:
+                pass
 
 
 class AsyncTextGenerate(AsyncClientConfig):
     async def __call__(self, text: str, /, **config):
-        config = {**self._run_config, **config, **{"stream": True, "prompt": text}}
+        config = self._run_config | config | {"stream": True, "prompt": text}
         stream = await self._aclient.completions.create(**config)
         async for event in stream:
-            yield event.choices[0].text
+            try:
+                yield event.choices[0].text
+            except AttributeError:
+                pass
 
 
 class ChatComplete(ClientConfig):
-    def __call__(self, messages: Union[List[Message], str], /, **config):
+    def __call__(self, messages: list[Message] | str, /, **config):
         messages = ensure(messages)
-        config = {**self._run_config, **config, **{"stream": False, "messages": messages}}
+        config = self._run_config | config | {"stream": False, "messages": messages}
         result = self._client.chat.completions.create(**config)
         return result.choices[0].message.content
 
 
 class AsyncChatComplete(AsyncClientConfig):
-    async def __call__(self, messages: Union[List[Message], str], /, **config):
+    async def __call__(self, messages: list[Message] | str, /, **config):
         messages = ensure(messages)
-        config = {**self._run_config, **config, **{"stream": False, "messages": messages}}
+        config = self._run_config | config | {"stream": False, "messages": messages}
         result = await self._aclient.chat.completions.create(**config)
         return result.choices[0].message.content
 
 
 class ChatGenerate(ClientConfig):
-    def __call__(self, messages: Union[List[Message], str], /, **config):
+    def __call__(self, messages: list[Message] | str, /, **config):
         messages = ensure(messages)
-        config = {**self._run_config, **config, **{"stream": True, "messages": messages}}
+        config = self._run_config | config | {"stream": True, "messages": messages}
         stream = self._client.chat.completions.create(**config)
         for event in stream:
-            yield event.choices[0].delta.content or ""
+            try:
+                yield event.choices[0].delta.content or ""
+            except AttributeError:
+                pass
 
 
 class AsyncChatGenerate(AsyncClientConfig):
-    async def __call__(self, messages: Union[List[Message], str], /, **config):
+    async def __call__(self, messages: list[Message] | str, /, **config):
         messages = ensure(messages)
-        config = {**self._run_config, **config, **{"stream": True, "messages": messages}}
+        config = self._run_config | config | {"stream": True, "messages": messages}
         stream = await self._aclient.chat.completions.create(**config)
         async for event in stream:
-            yield event.choices[0].delta.content or ""
+            try:
+                yield event.choices[0].delta.content or ""
+            except AttributeError:
+                pass
 
 
 class SyncTextOpenAI(ClientConfig, LLM):
     complete = TextComplete.__call__  # type: ignore
     generate = TextGenerate.__call__  # type: ignore
 
 
@@ -148,7 +162,23 @@
     complete = ChatComplete.__call__  # type: ignore
     generate = ChatGenerate.__call__  # type: ignore
 
 
 class AsyncChatOpenAI(AsyncClientConfig, LLM):
     complete = AsyncChatComplete.__call__  # type: ignore
     generate = AsyncChatGenerate.__call__  # type: ignore
+
+
+__all__ = (
+    "TextComplete",
+    "AsyncTextComplete",
+    "TextGenerate",
+    "AsyncTextGenerate",
+    "ChatComplete",
+    "AsyncChatComplete",
+    "ChatGenerate",
+    "AsyncChatGenerate",
+    "SyncTextOpenAI",
+    "AsyncTextOpenAI",
+    "SyncChatOpenAI",
+    "AsyncChatOpenAI",
+)
```

### Comparing `promplate-0.3.3.post1/promplate/prompt/chat.py` & `promplate-0.3.4/promplate/prompt/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,36 @@
-from ..typing import List, Literal, NotRequired, Optional, TypedDict, Union
+from sys import version_info
+from typing import Literal
+
 from .utils import is_message_start
 
 Role = Literal["user", "assistant", "system"]
 
+if version_info >= (3, 12):
+    from typing import NotRequired, TypedDict
 
-class Message(TypedDict):
-    role: Role
-    content: str
-    name: NotRequired[str]
+    class Message(TypedDict):  # type: ignore
+        role: Role
+        content: str
+        name: NotRequired[str]
+
+else:
+    from typing_extensions import NotRequired, TypedDict
+
+    class Message(TypedDict):
+        role: Role
+        content: str
+        name: NotRequired[str]
 
 
 class MessageBuilder:
     _initializing = True
     __slots__ = ("role", "content", "name")
 
-    def __init__(self, role: Role, /, content: str = "", name: Optional[str] = None):
+    def __init__(self, role: Role, /, content: str = "", name: str | None = None):
         self.role: Role = role
         self.content = content
         self.name = name
 
     def __repr__(self):
         if self.name is not None:
             return f"<| {self.role} {self.name} |>"
@@ -54,19 +66,19 @@
 
 U = user = MessageBuilder("user")
 A = assistant = MessageBuilder("assistant")
 S = system = MessageBuilder("system")
 MessageBuilder._initializing = False
 
 
-def ensure(text_or_list: Union[List[Message], str]) -> List[Message]:
+def ensure(text_or_list: list[Message] | str) -> list[Message]:
     return parse_chat_markup(text_or_list) if isinstance(text_or_list, str) else text_or_list
 
 
-def parse_chat_markup(text: str) -> List[Message]:
+def parse_chat_markup(text: str) -> list[Message]:
     messages = []
     current_message = None
     buffer = []
 
     for line in text.splitlines():
         match = is_message_start.match(line)
         if match:
@@ -88,9 +100,9 @@
     if current_message:
         current_message["content"] = "\n".join(buffer)
         messages.append(current_message)
 
     if messages:
         return messages
     elif text and text != "\n":
-        return [{"role": "user", "content": text[:-1] if text[-1] == "\n" else text}]
+        return [{"role": "user", "content": text.removesuffix("\n")}]
     return []
```

### Comparing `promplate-0.3.3.post1/promplate/prompt/template.py` & `promplate-0.3.4/promplate/prompt/template.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from ast import Expr, parse, unparse
 from collections import ChainMap
 from functools import cached_property
 from pathlib import Path
-from sys import version_info
+from textwrap import dedent
+from typing import TYPE_CHECKING, Any, Protocol
 
-from ..typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Protocol, Self, Union
-from .builder import get_base_builder
-from .utils import AutoNaming, get_user_agent, split_template_tokens
+from .builder import *
+from .utils import *
 
-Context = Dict[str, Any]  # globals must be a real dict
+Context = dict[str, Any]  # globals must be a real dict
 
 
 class Component(Protocol):
     def render(self, context: Context) -> str: ...
 
     async def arender(self, context: Context) -> str: ...
 
@@ -29,33 +30,40 @@
     def _flush(self):
         for line in self._buffer:
             self._builder.add_line(line)
         self._buffer.clear()
 
     @staticmethod
     def _unwrap_token(token: str):
-        return token.strip()[2:-2].strip("-").strip()
+        return dedent(token[2:-2].strip("-")).strip()
 
     def _on_literal_token(self, token: str):
         self._buffer.append(f"__append__({repr(token)})")
 
     def _on_eval_token(self, token):
-        exp = self._unwrap_token(token)
+        token = self._unwrap_token(token)
+        if "\n" in token:
+            mod = parse(token)
+            [*rest, last] = mod.body
+            assert isinstance(last, Expr), "{{ }} block must end with an expression, or you should use {# #} block"
+            self._buffer.extend(unparse(rest).splitlines())  # type: ignore
+            exp = unparse(last)
+        else:
+            exp = token
         self._buffer.append(f"__append__({exp})")
 
     def _on_exec_token(self, token):
-        exp = self._unwrap_token(token)
-        self._buffer.append(exp)
+        self._buffer.extend(self._unwrap_token(token).splitlines())
 
     def _on_special_token(self, token, sync: bool):
-        inner: str = self._unwrap_token(token)
+        inner = self._unwrap_token(token)
 
         if inner.startswith("end"):
             last = self._ops_stack.pop()
-            assert last == inner[3:]
+            assert last == inner.removeprefix("end")
             self._flush()
             self._builder.dedent()
 
         else:
             op = inner.split(" ", 1)[0]
 
             if op == "if" or op == "for" or op == "while":
@@ -76,28 +84,27 @@
                     self._buffer.append(f"__append__({op}.render({params}))")
                 else:
                     self._buffer.append(f"__append__(await {op}.arender({params}))")
 
     @staticmethod
     def _make_context(text: str):
         """generate context parameter if specified otherwise use locals() by default"""
-        if version_info >= (3, 10):
-            return f"(__l__:=locals().copy(), __l__.update(dict({text[text.index(' ') + 1:]})))[0]" if " " in text else "locals()"
-        return f"(__l__:=globals().copy(), __l__.update(dict({text[text.index(' ') + 1:]})))[0]" if " " in text else "globals()"
 
-    def compile(self, sync=True):
-        self._builder = get_base_builder(sync)
+        return f"locals() | dict({text[text.index(' ') + 1:]})" if " " in text else "locals()"
+
+    def compile(self, sync=True, indent_str="\t"):
+        self._builder = get_base_builder(sync, indent_str)
 
         for token in split_template_tokens(self.text):
             s_token = token.strip()
-            if s_token.startswith("{{"):
+            if s_token.startswith("{{") and s_token.endswith("}}"):
                 self._on_eval_token(token)
-            elif s_token.startswith("{#"):
+            elif s_token.startswith("{#") and s_token.endswith("#}"):
                 self._on_exec_token(token)
-            elif s_token.startswith("{%"):
+            elif s_token.startswith("{%") and s_token.endswith("%}") and "\n" not in s_token:
                 self._on_special_token(token, sync)
             else:
                 self._on_literal_token(token)
 
         if self._ops_stack:
             raise SyntaxError(self._ops_stack)
 
@@ -117,90 +124,97 @@
     def _arender_code(self):
         self.compile(sync=False)
         return self._builder.get_render_function().__code__.replace(co_filename=str(self), co_name="arender")
 
     async def arender(self, context: Context) -> str:
         return await eval(self._arender_code, context)
 
-    def get_script(self, sync=True):
+    def get_script(self, sync=True, indent_str="    "):
         """compile template string into python script"""
-        self.compile(sync)
+        self.compile(sync, indent_str)
         return str(self._builder)
 
 
 class Loader(AutoNaming):
     @classmethod
-    def read(cls, path: Union[str, Path], encoding="utf-8"):
+    def read(cls, path: str | Path, encoding="utf-8"):
         path = Path(path)
         obj = cls(path.read_text(encoding))
         obj.name = path.stem
         return obj
 
     @classmethod
-    async def aread(cls, path: Union[str, Path], encoding="utf-8"):
+    async def aread(cls, path: str | Path, encoding="utf-8"):
         from aiofiles import open
 
         async with open(path, encoding=encoding) as f:
             content = await f.read()
 
         path = Path(path)
         obj = cls(content)
         obj.name = path.stem
         return obj
 
     @classmethod
-    def _patch_kwargs(cls, kwargs: dict):
-        return {
-            **{
-                "follow_redirects": True,
-                "base_url": "https://promplate.dev/",
-                "headers": {"User-Agent": get_user_agent(cls)},
-            },
-            **kwargs,
-        }
+    def _patch_kwargs(cls, kwargs: dict) -> dict:
+        return {"headers": {"User-Agent": get_user_agent(cls)}} | kwargs
+
+    @staticmethod
+    def _join_url(url: str):
+        if url.startswith("http"):
+            return url
+
+        from urllib.parse import urljoin
+
+        return urljoin("https://promplate.dev/", url)
 
     @classmethod
     def fetch(cls, url: str, **kwargs):
         from .utils import _get_client
 
-        response = _get_client().get(url, **cls._patch_kwargs(kwargs))
+        response = _get_client().get(cls._join_url(url), **cls._patch_kwargs(kwargs))
         obj = cls(response.raise_for_status().text)
         obj.name = Path(url).stem
         return obj
 
     @classmethod
     async def afetch(cls, url: str, **kwargs):
         from .utils import _get_aclient
 
-        response = await _get_aclient().get(url, **cls._patch_kwargs(kwargs))
+        response = await _get_aclient().get(cls._join_url(url), **cls._patch_kwargs(kwargs))
         obj = cls(response.raise_for_status().text)
         obj.name = Path(url).stem
         return obj
 
 
 class SafeChainMapContext(ChainMap, dict):
     if TYPE_CHECKING:  # fix type from `collections.ChainMap`
         from sys import version_info
 
+        if version_info >= (3, 11):
+            from typing_extensions import Self
+        else:
+            from typing import Self
+
         copy: Callable[[Self], Self]
 
 
 class Template(TemplateCore, Loader):
-    def __init__(self, text: str, /, context: Optional[Context] = None):
+    def __init__(self, text: str, /, context: Context | None = None):
         super().__init__(text)
         self.context = {} if context is None else context
 
-    def render(self, context: Optional[Context] = None):
+    def render(self, context: Context | None = None):
         if context is None:
             context = SafeChainMapContext({}, self.context)
         else:
             context = SafeChainMapContext({}, context, self.context)
 
         return super().render(context)
 
-    async def arender(self, context: Optional[Context] = None):
+    async def arender(self, context: Context | None = None):
         if context is None:
             context = SafeChainMapContext({}, self.context)
         else:
             context = SafeChainMapContext({}, context, self.context)
 
         return await super().arender(context)
```

### Comparing `promplate-0.3.3.post1/promplate/prompt/utils.py` & `promplate-0.3.4/promplate/prompt/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from functools import cached_property, wraps
+from functools import cache, cached_property, wraps
 from inspect import currentframe, isclass
 from re import compile
-from typing import Dict, Tuple
-
-from ..typing import Any, Callable, ParamSpec, TypeVar
+from typing import Any, Callable, ParamSpec, TypeVar
 
 split_template_tokens = compile(
-    r"(\s{%-.*?-%}\s|\s{{-.*?-}}\s|\s{#-.*?-#}\s|\s{%-.*?%}|\s{{-.*?}}|\s{#-.*?#}|{%.*?-%}\s|{{.*?-}}\s|{#.*?-#}\s|{%.*?%}|{{.*?}}|{#.*?#})"
+    r"(\s{%-.*?-%}\s|\s{{-[\s\S]*?-}}\s|\s{#-[\s\S]*?-#}\s"
+    r"|\s{%-.*?%}|\s{{-[\s\S]*?}}|\s{#-[\s\S]*?#}"
+    r"|{%.*?-%}\s|{{[\s\S]*?-}}\s|{#[\s\S]*?-#}\s"
+    r"|{%.*?%}|{{[\s\S]*?}}|{#[\s\S]*?#})"
 ).split
 
 
 var_name_checker = compile(r"[_a-zA-Z]\w*$")
 
 is_message_start = compile(r"<\|\s?(user|system|assistant)\s?(\w{1,64})?\s?\|>")
 
@@ -84,28 +85,37 @@
             result = func(*args, **kwargs)
         return result
 
     return wrapper
 
 
 @cache_once
-def get_builtins() -> Dict[str, Any]:
+def get_builtins() -> dict[str, Any]:
     return __builtins__ if isinstance(__builtins__, dict) else __builtins__.__dict__
 
 
+@cache
+def version(package: str):
+    from importlib.metadata import PackageNotFoundError, version
+
+    try:
+        return version(package)
+    except PackageNotFoundError:
+        return None
+
+
 @cache_once
-def get_user_agent(self, *additional_packages: Tuple[str, str]):
-    from importlib.metadata import version
+def get_user_agent(self, *additional_packages: tuple[str, str]):
     from sys import version as py_version
 
     return " ".join(
         (
             f"Promplate/{version('promplate')} ({self.__name__ if isclass(self) else self.__class__.__name__})",
-            *(f"{display_name}/{version(package)}" for display_name, package in additional_packages),
-            f"HTTPX/{version('httpx')}",
+            *(f"{name}/{v}" for name, v in additional_packages),
+            f"HTTPX/{version('httpx') or '-'}",
             f"Python/{py_version.split()[0]}",
         )
     )
 
 
 @cache_once
 def _is_http2_available():
```

### Comparing `promplate-0.3.3.post1/pyproject.toml` & `promplate-0.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "promplate"
-version = "0.3.3.post1"
-description = "cross-language prompt engineering framework"
+version = "0.3.4"
+description = "Prompt engineering framework for humans"
 homepage = "https://promplate.dev/"
 documentation = "https://docs.py.promplate.dev/"
 repository = "https://github.com/promplate/core"
-authors = ["Muspi Merol <admin@muspimerol.site>"]
+authors = ["Muspi Merol <me@promplate.dev>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["prompt", "template", "nlp", "llm"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Text Processing :: Markup",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 typing-extensions = { version = "^4", python = "<3.12" }
 aiofiles = { version = "^23.2", optional = true }
 httpx = { version = ">=0.24, <1.0", optional = true }
 openai = { version = ">=0.27, <2.0", optional = true }
 
 [tool.poetry.extras]
 aiofiles = ["aiofiles"]
@@ -39,18 +39,17 @@
 [tool.pdm.scripts]
 format = { composite = ["isort ./{args}", "black ./{args}"] }
 test = "pytest"
 cov = { composite = ["coverage run -m pytest", "coverage report"] }
 
 [tool.isort]
 profile = "black"
-line_length = 150
 
 [tool.black]
-line-length = 150
+line-length = 130
 
 [tool.coverage.run]
 source = ["promplate"]
 branch = true
 
 [tool.coverage.report]
 fail_under = 45
```

### Comparing `promplate-0.3.3.post1/README.md` & `promplate-0.3.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Promplate
 
 ```text
 </Promplate/> = <template> // prompt
 ```
 
-**Promplate** is a prompting framework focusing on developing experience. However, it can also be a super-convenient SDK for simple LLM calls. Promplate progressively enhance your prompting workflow. And it values flexibility as well as perfect conventions. [Learn more](https://promplate.dev/py)
+**Promplate** is a prompting framework focusing on developing experience. However, it can also be a super-convenient SDK for simple LLM calls. Promplate progressively enhance your prompting workflow. And it values flexibility as well as perfect conventions. [Try online](https://promplate.dev/py)
 
 ## Installation
 
 ```shell
 pip install promplate
 ```
 
-**Promplate** supports both CPython and PyPy, from `3.8` to `3.12`.
+**Promplate** supports both CPython and PyPy, from `3.8` to `3.12`. It even supports running in browsers through wasm implementations of python.
 
 ## Documentation
 
 You can visit our official docs site at [docs.py.promplate.dev](https://docs.py.promplate.dev/).
 
 ## IDE Support 🌹
```

### Comparing `promplate-0.3.3.post1/PKG-INFO` & `promplate-0.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: promplate
-Version: 0.3.3.post1
-Summary: cross-language prompt engineering framework
+Version: 0.3.4
+Summary: Prompt engineering framework for humans
 Home-page: https://promplate.dev/
 License: MIT
 Keywords: prompt,template,nlp,llm
 Author: Muspi Merol
-Author-email: admin@muspimerol.site
-Requires-Python: >=3.8,<4.0
+Author-email: me@promplate.dev
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Typing :: Typed
 Provides-Extra: aiofiles
@@ -33,23 +31,23 @@
 
 # Promplate
 
 ```text
 </Promplate/> = <template> // prompt
 ```
 
-**Promplate** is a prompting framework focusing on developing experience. However, it can also be a super-convenient SDK for simple LLM calls. Promplate progressively enhance your prompting workflow. And it values flexibility as well as perfect conventions. [Learn more](https://promplate.dev/py)
+**Promplate** is a prompting framework focusing on developing experience. However, it can also be a super-convenient SDK for simple LLM calls. Promplate progressively enhance your prompting workflow. And it values flexibility as well as perfect conventions. [Try online](https://promplate.dev/py)
 
 ## Installation
 
 ```shell
 pip install promplate
 ```
 
-**Promplate** supports both CPython and PyPy, from `3.8` to `3.12`.
+**Promplate** supports both CPython and PyPy, from `3.8` to `3.12`. It even supports running in browsers through wasm implementations of python.
 
 ## Documentation
 
 You can visit our official docs site at [docs.py.promplate.dev](https://docs.py.promplate.dev/).
 
 ## IDE Support 🌹
```

