# Comparing `tmp/abses-0.5.4.tar.gz` & `tmp/abses-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.5.4.tar", max compression
+gzip compressed data, was "abses-0.5.5.tar", max compression
```

## Comparing `abses-0.5.4.tar` & `abses-0.5.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.5.4/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.5.4/LICENSES/
--rw-r--r--   0        0        0     4422 2024-03-28 05:44:10.771243 abses-0.5.4/README.md
--rw-r--r--   0        0        0      978 2024-03-28 05:52:54.350080 abses-0.5.4/abses/__init__.py
--rw-r--r--   0        0        0    11158 2024-03-26 10:47:24.064157 abses-0.5.4/abses/actor.py
--rw-r--r--   0        0        0     2648 2024-03-12 14:08:50.243373 abses-0.5.4/abses/bases.py
--rw-r--r--   0        0        0     5095 2024-03-26 03:03:31.433042 abses-0.5.4/abses/cells.py
--rw-r--r--   0        0        0     2939 2024-03-12 14:08:50.244255 abses-0.5.4/abses/components.py
--rw-r--r--   0        0        0    16185 2024-03-26 03:06:50.063640 abses-0.5.4/abses/container.py
--rw-r--r--   0        0        0     8728 2024-03-11 13:48:46.402196 abses-0.5.4/abses/decision.py
--rw-r--r--   0        0        0     2814 2024-03-12 14:08:50.245365 abses-0.5.4/abses/dynamic.py
--rw-r--r--   0        0        0      298 2024-01-11 09:19:35.315645 abses-0.5.4/abses/errors.py
--rw-r--r--   0        0        0     3901 2024-03-12 14:08:50.245695 abses-0.5.4/abses/human.py
--rw-r--r--   0        0        0    13802 2024-03-25 07:03:37.716715 abses-0.5.4/abses/links.py
--rw-r--r--   0        0        0      347 2024-01-11 09:19:35.316189 abses-0.5.4/abses/logging.py
--rw-r--r--   0        0        0    10446 2024-03-20 04:34:35.990347 abses-0.5.4/abses/main.py
--rw-r--r--   0        0        0     4225 2024-03-12 14:08:50.246915 abses-0.5.4/abses/modules.py
--rw-r--r--   0        0        0     7694 2024-03-26 10:47:24.064623 abses-0.5.4/abses/move.py
--rw-r--r--   0        0        0    20336 2024-03-20 09:23:32.734956 abses-0.5.4/abses/nature.py
--rw-r--r--   0        0        0     2945 2024-03-12 12:58:25.607010 abses-0.5.4/abses/objects.py
--rw-r--r--   0        0        0     5941 2024-03-25 08:27:14.810207 abses-0.5.4/abses/random.py
--rw-r--r--   0        0        0     1611 2024-03-12 14:08:50.248566 abses-0.5.4/abses/selection.py
--rw-r--r--   0        0        0    10634 2024-03-26 03:21:16.283820 abses-0.5.4/abses/sequences.py
--rw-r--r--   0        0        0     1085 2024-03-12 14:08:50.249165 abses-0.5.4/abses/states.py
--rw-r--r--   0        0        0    14355 2024-03-12 14:08:50.249446 abses-0.5.4/abses/time.py
--rw-r--r--   0        0        0     3206 2024-03-12 14:08:50.249724 abses-0.5.4/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-03-12 14:08:50.250006 abses-0.5.4/abses/tools/regex.py
--rw-r--r--   0        0        0     2294 2024-03-28 05:52:54.348536 abses-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     5390 1970-01-01 00:00:00.000000 abses-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.5.5/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.5.5/LICENSES/
+-rw-r--r--   0        0        0     4422 2024-04-04 10:58:12.162255 abses-0.5.5/README.md
+-rw-r--r--   0        0        0      978 2024-04-06 01:08:35.022686 abses-0.5.5/abses/__init__.py
+-rw-r--r--   0        0        0     9396 2024-04-06 01:06:25.258369 abses-0.5.5/abses/actor.py
+-rw-r--r--   0        0        0     2651 2024-04-06 01:06:25.259012 abses-0.5.5/abses/bases.py
+-rw-r--r--   0        0        0     5608 2024-04-06 01:06:25.259525 abses-0.5.5/abses/cells.py
+-rw-r--r--   0        0        0     2967 2024-04-06 01:06:25.259964 abses-0.5.5/abses/components.py
+-rw-r--r--   0        0        0    16509 2024-04-06 01:06:25.260683 abses-0.5.5/abses/container.py
+-rw-r--r--   0        0        0     8957 2024-04-06 01:06:25.261273 abses-0.5.5/abses/decision.py
+-rw-r--r--   0        0        0     2814 2024-04-04 10:58:12.165326 abses-0.5.5/abses/dynamic.py
+-rw-r--r--   0        0        0      298 2024-01-11 09:19:35.315645 abses-0.5.5/abses/errors.py
+-rw-r--r--   0        0        0     3956 2024-04-06 01:06:25.261907 abses-0.5.5/abses/human.py
+-rw-r--r--   0        0        0    18110 2024-04-06 01:06:25.262363 abses-0.5.5/abses/links.py
+-rw-r--r--   0        0        0      347 2024-01-11 09:19:35.316189 abses-0.5.5/abses/logging.py
+-rw-r--r--   0        0        0    11515 2024-04-06 01:06:25.262785 abses-0.5.5/abses/main.py
+-rw-r--r--   0        0        0     4389 2024-04-06 01:06:25.263178 abses-0.5.5/abses/modules.py
+-rw-r--r--   0        0        0     8216 2024-04-06 01:06:25.263593 abses-0.5.5/abses/move.py
+-rw-r--r--   0        0        0    21209 2024-04-06 01:06:25.263971 abses-0.5.5/abses/nature.py
+-rw-r--r--   0        0        0     2942 2024-04-06 01:06:25.264485 abses-0.5.5/abses/objects.py
+-rw-r--r--   0        0        0     5962 2024-04-06 01:06:25.265050 abses-0.5.5/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.5.5/abses/selection.py
+-rw-r--r--   0        0        0    11402 2024-04-06 01:06:25.265385 abses-0.5.5/abses/sequences.py
+-rw-r--r--   0        0        0     1098 2024-04-06 01:06:25.265815 abses-0.5.5/abses/states.py
+-rw-r--r--   0        0        0    14591 2024-04-06 01:06:25.266235 abses-0.5.5/abses/time.py
+-rw-r--r--   0        0        0     3216 2024-04-06 01:06:25.266508 abses-0.5.5/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-04 10:58:12.169839 abses-0.5.5/abses/tools/regex.py
+-rw-r--r--   0        0        0     2469 2024-04-06 01:08:35.022744 abses-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     5390 1970-01-01 00:00:00.000000 abses-0.5.5/PKG-INFO
```

### Comparing `abses-0.5.4/LICENSE` & `abses-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.5.4/README.md` & `abses-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.5.4/abses/__init__.py` & `abses-0.5.5/abses/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Decision",
     "ActorsList",
     "PatchCell",
     "perception",
     "alive_required",
     "time_condition",
 ]
-__version__ = "v0.5.4"
+__version__ = "v0.5.5"
 
 from .actor import Actor, alive_required, perception
 from .container import ActorsList
 from .decision import Decision
 from .human import BaseHuman
 from .main import MainModel
 from .nature import BaseNature, PatchCell, PatchModule
```

### Comparing `abses-0.5.4/abses/actor.py` & `abses-0.5.5/abses/actor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,51 +10,49 @@
 
 在 abses 中，主体也叫做 Actor（行动者）。
 """
 
 from __future__ import annotations
 
 from functools import cached_property, wraps
-from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Optional,
+    Union,
+    cast,
+)
 
 try:
-    from typing import Self, TypeAlias
+    from typing import TypeAlias
 except ImportError:
-    from typing_extensions import TypeAlias, Self
+    from typing_extensions import TypeAlias
 
 import mesa_geo as mg
 
 from abses.decision import _DecisionFactory
 from abses.errors import ABSESpyError
-from abses.links import _LinkNode, _LinkProxy
+from abses.links import TargetName, _LinkNode
 from abses.move import _Movements
 from abses.objects import _BaseObj
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
-    from abses.human import LinkContainer
+    from abses.human import _LinkContainer
     from abses.main import MainModel
-    from abses.nature import PatchCell
+    from abses.nature import PatchCell, PatchModule
     from abses.sequences import ActorsList
 
 
 Selection: TypeAlias = Union[str, Iterable[bool]]
 Trigger: TypeAlias = Union[Callable, str]
-Targets: TypeAlias = Union["ActorsList", "Self", "PatchCell", "str"]
 Breeds: TypeAlias = Optional[Union[str, Iterable[str]]]
 
-TARGET_KEYWORDS = {
-    "at": "at",
-    "world": "at",
-    "nature": "at",
-    "me": "self",
-    "actor": "self",
-    "agent": "self",
-}
-
 
 def alive_required(method):
     """
     A decorator that only executes the method when the object's alive attribute is True.
     """
 
     @wraps(method)
@@ -79,38 +77,44 @@
         raise ValueError(
             f"Perception result of '{name}' got type {type(result)} as return."
         )
     return nodata if result is None else result
 
 
 def perception(
-    decorated_func: Optional[Callable] = None, *, nodata: Optional[Any] = None
-) -> Callable:
+    decorated_func: Optional[Callable[..., Any]] = None,
+    *,
+    nodata: Optional[Any] = None,
+) -> Callable[..., Any]:
     """Change the decorated function into a perception attribute.
 
     Parameters:
         decorated_func:
             The decorated function.
         nodata:
             The value to return if the result is None.
 
     Returns:
         The decorated perception attribute or a decorator.
     """
 
-    def decorator(func) -> Callable:
+    def decorator(func) -> Callable[..., Any]:
         @wraps(func)
-        def wrapper(self: Actor, *args, **kwargs):
+        def wrapper(self: Actor, *args, **kwargs) -> Callable[..., Any]:
             result = func(self, *args, **kwargs)
             return perception_result(func.__name__, result, nodata=nodata)
 
         return wrapper
 
     # 检查是否有参数传递给装饰器，若没有则返回装饰器本身
-    return decorator(decorated_func) if decorated_func else decorator
+    return (
+        decorator(decorated_func)
+        if decorated_func
+        else cast(Callable[..., Any], decorator)
+    )
 
 
 class Actor(mg.GeoAgent, _BaseObj, _LinkNode):
     """
     An actor in a social-ecological system (or "Agent" in an agent-based model.)
 
     Attributes:
@@ -141,36 +145,41 @@
     """
 
     # when checking the rules
     __decisions__ = None
 
     def __init__(
         self,
-        model: MainModel,
+        model: MainModel[Any, Any],
         observer: bool = True,
         unique_id: Optional[int] = None,
         **kwargs,
     ) -> None:
         _BaseObj.__init__(self, model, observer=observer)
         if not unique_id:
             unique_id = self.model.next_id()
         crs = kwargs.pop("crs", model.nature.crs)
         geometry = kwargs.pop("geometry", None)
         mg.GeoAgent.__init__(
             self, unique_id, model=model, geometry=geometry, crs=crs
         )
         _LinkNode.__init__(self)
-        self._cell: PatchCell = None
+        self._cell: Optional[PatchCell] = None
         self._decisions: _DecisionFactory = self._setup_decisions()
         self._alive: bool = True
         self._setup()
 
     def __repr__(self) -> str:
         return f"<{self.breed} [{self.unique_id}]>"
 
+    def _default_redirection(
+        self, target: Optional[TargetName]
+    ) -> Optional[PatchCell]:
+        return self if target == "actor" else self._cell
+
     def _setup_decisions(self) -> _DecisionFactory:
         """Decisions that this actor makes."""
         decisions = make_list(getattr(self, "__decisions__", None))
         return _DecisionFactory(self, decisions)
 
     @property
     def alive(self) -> bool:
@@ -182,15 +191,15 @@
         """The decisions that this actor makes."""
         return self._decisions
 
     # alias of decisions
     d = decisions
 
     @property
-    def layer(self) -> mg.RasterLayer | None:
+    def layer(self) -> Optional[PatchModule]:
         """Get the layer where the actor is located."""
         return None if self._cell is None else self._cell.layer
 
     @property
     def on_earth(self) -> bool:
         """Whether agent stands on a cell."""
         return bool(self._cell)
@@ -211,15 +220,16 @@
             )
         self._cell = cell
         self.pos = cell.pos
 
     @at.deleter
     def at(self) -> None:
         """Remove the agent from the located cell."""
-        if self.on_earth and self in self.at.agents:
+        cell = cast("PatchCell", self.at)
+        if self.on_earth and cell.agents is not None and self in cell.agents:
             raise ABSESpyError(
                 "Cannot remove location directly because the actor is still on earth."
             )
         self._cell = None
 
     @cached_property
     def move(self) -> _Movements:
@@ -228,50 +238,19 @@
         1. `move.to()`: moves the actor to another cell.
         2. `move.off()`: removes the actor from the current layer.
         3. `move.by()`: moves the actor by a distance.
         4. `move.random()`: moves the actor to a random cell.
         """
         return _Movements(self)
 
-    @cached_property
-    def link(self) -> _LinkProxy:
-        """A proxy which can be used to manipulate the links:
-
-        1. `link.to()`: creates a new link from this actor to another.
-        2. `link.by()`: creates a new link from another to this actor.
-        3. `link.get()`: gets the links of this actor.
-        4. `link.has()`: checks if there is a link between this actor and another.
-        5. `link.unlink()`: removes a link between this actor and another.
-        6. `link.clean()`: removes all links of this actor.
-        """
-        return _LinkProxy(self, self.model)
-
-    def _get_correct_target(self, target: Targets, attr: str) -> Targets:
-        """Which targets should be used when getting or setting."""
-        # If the target is not None, get the target from dict.
-        if target is not None:
-            if isinstance(target, str):
-                target = TARGET_KEYWORDS.get(target, target)
-                target = {"self": self, "at": self.at}[target]
-            return target
-        # If the attribute is in the agent, the agent is the target.
-        if hasattr(self, attr):
-            return self
-        # If the attribute is in the cell, the cell is the target.
-        if self.on_earth and hasattr(self.at, attr):
-            return self._cell
-        # If the attribute is not found, raise an error.
-        warn = "Set a new attribute outside '__init__' is not allowed."
-        raise AttributeError(f"Attribute '{attr}' not found in {self}. {warn}")
-
     @alive_required
     def get(
         self,
         attr: str,
-        target: Optional[Self | PatchCell] = None,
+        target: Optional[TargetName] = None,
     ) -> Any:
         """Gets attribute value from target.
 
         Parameters:
             attr:
                 The name of the attribute to get.
             target:
@@ -279,19 +258,20 @@
                 If None, the agent itself is the target.
                 If the target is an agent, get the attribute from the agent.
                 If the target is a cell, get the attribute from the cell.
 
         Returns:
             The value of the attribute.
         """
-        target = self._get_correct_target(target, attr=attr)
-        return getattr(self, attr) if target is self else target.get(attr)
+        return super().get(attr=attr, target=target)
 
     @alive_required
-    def set(self, attr: str, value: Any, target: Targets) -> None:
+    def set(
+        self, attr: str, value: Any, target: Optional[TargetName] = None
+    ) -> None:
         """Sets the value of an attribute.
 
         Parameters:
             attr:
                 The name of the attribute to set.
             value:
                 The value to set the attribute to.
@@ -302,23 +282,15 @@
 
         Raises:
             TypeError:
                 If the attribute is not a string.
             ABSESpyError:
                 If the attribute is protected.
         """
-        # If the attribute is not a string, raise an error.
-        if not isinstance(attr, str):
-            raise TypeError("The attribute must be a string.")
-        # If the attribute is protected, raise an error
-        if attr.startswith("_"):
-            raise ABSESpyError(f"Attribute '{attr}' is protected.")
-        # Set the attribute on the target.
-        target = self._get_correct_target(target=target, attr=attr)
-        setattr(target, attr, value)
+        super().set(attr=attr, value=value, target=target)
 
     @alive_required
     def die(self) -> None:
         """Kills the agent (self)"""
         self.link.clean()  # 从链接中移除
         if self.on_earth:  # 如果在地上，那么从地块上移除
             self.move.off()
```

### Comparing `abses-0.5.4/abses/bases.py` & `abses-0.5.5/abses/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 class _Notice:
     """Notice class for the observer pattern."""
 
-    __glob_vars__: Set[str] = []
+    __glob_vars__: Set[str] = set()
 
     def __init__(self, observer: Optional[_Observer] = None):
         self.observers: Set[_Observer] = set()
         self._glob_vars = set(self.__glob_vars__)
         if observer is not None:
             self.attach(observer)
```

### Comparing `abses-0.5.4/abses/cells.py` & `abses-0.5.5/abses/cells.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,30 +7,37 @@
 
 """
 每一个世界里的斑块
 """
 
 from __future__ import annotations
 
-from functools import cached_property
-from typing import TYPE_CHECKING, Any, Optional
+from numbers import Number
+from typing import TYPE_CHECKING, Any, Callable, Optional, Tuple, Union
 
 import mesa_geo as mg
 
 from abses import ActorsList
 from abses.container import _CellAgentsContainer
 from abses.errors import ABSESpyError
-from abses.links import _LinkNode, _LinkProxy
+from abses.links import TargetName, _LinkNode
 
 if TYPE_CHECKING:
-    from abses.main import MainModel
+    from abses.main import H, MainModel, N
     from abses.nature import PatchModule
 
+try:
+    from typing import Self, TypeAlias
+except ImportError:
+    from typing_extensions import Self, TypeAlias
 
-def raster_attribute(func):
+Pos: TypeAlias = Tuple[int, int]
+
+
+def raster_attribute(func: Callable[..., Union[Number, str]]) -> property:
     """Turn the method into a property that the patch can extract.
     Examples:
         ```
         class TestCell(Cell):
             @raster_attribute
             def test:
                 return 1
@@ -51,15 +58,15 @@
         >>> np.array([
             [1, 1, 1],
             [1, 1, 1],
             [1, 1, 1],
         ])
         ```
     """
-    func.is_decorated = True
+    setattr(func, "is_decorated", True)
     return property(func)
 
 
 class PatchCell(mg.Cell, _LinkNode):
     """A patch cell of a `RasterLayer`.
     Subclassing this class to create a custom cell.
     When class attribute `max_agents` is assigned,
@@ -70,19 +77,21 @@
             The agents located at here.
         layer:
             The `RasterLayer` where this `PatchCell` belongs.
     """
 
     max_agents: Optional[int] = None
 
-    def __init__(self, pos=None, indices=None):
+    def __init__(
+        self, pos: Optional[Pos] = None, indices: Optional[Pos] = None
+    ):
         mg.Cell.__init__(self, pos, indices)
         _LinkNode.__init__(self)
         self._agents: Optional[_CellAgentsContainer] = None
-        self._layer: Optional[mg.RasterLayer] = None
+        self._layer: Optional[PatchModule] = None
 
     def __repr__(self) -> str:
         return f"<Cell at {self.layer}[{self.pos}]>"
 
     @classmethod
     def __attribute_properties__(cls) -> set[str]:
         """Properties that should be found in the `RasterLayer`.
@@ -95,42 +104,48 @@
             if isinstance(method, property)
             and getattr(method.fget, "is_decorated", False)
         }
 
     @property
     def layer(self) -> PatchModule:
         """`RasterLayer` where this `PatchCell` belongs."""
+        if self._layer is None:
+            raise ABSESpyError(
+                "PatchCell must belong to a layer."
+                f"However, {self} has no layer."
+                "Did you create this cell in the correct way?"
+            )
         return self._layer
 
     @layer.setter
     def layer(self, layer: PatchModule) -> None:
         if not isinstance(layer, mg.RasterLayer):
             raise TypeError(f"{type(layer)} is not valid layer.")
-        if self.layer is not None:
+        if self._layer is not None:
             raise ABSESpyError("PatchCell can only belong to one layer.")
         # set layer property
         self._layer = layer
         # set layer's model as the model
-        self.model = layer.model
+        self.model: MainModel[Any, Any] = layer.model
         # set agents container
         self._agents = _CellAgentsContainer(
             layer.model, cell=self, max_len=getattr(self, "max_agents", None)
         )
 
     @property
-    def agents(self) -> _CellAgentsContainer:
+    def agents(self) -> Optional[_CellAgentsContainer]:
         """The agents located at here."""
         return self._agents
 
-    @cached_property
-    def link(self) -> _LinkProxy:
-        """The link to the patch."""
-        return _LinkProxy(node=self, model=self.layer.model)
+    def _default_redirection(
+        self, target: Optional[TargetName]
+    ) -> _CellAgentsContainer | None:
+        return self if target == "cell" else self.agents
 
-    def get(self, attr: str) -> Any:
+    def get(self, attr: str, target: Optional[TargetName] = None) -> Any:
         """Gets the value of an attribute or registered property.
         Automatically update the value if it is the dynamic variable of the layer.
 
         Parameters:
             attr:
                 The name of attribute to get.
 
@@ -140,25 +155,23 @@
 
         Raises:
             AttributeError:
                 Attribute value of the associated patch cell.
         """
         if attr in self.layer.dynamic_variables:
             self.layer.dynamic_var(attr_name=attr)
-        if not hasattr(self, attr):
-            raise AttributeError(f"{attr} not exists in {self.layer}.")
-        return getattr(self, attr)
+        return super().get(attr=attr, target=target)
 
     def neighboring(
         self,
         moore: bool = False,
         radius: int = 1,
         include_center: bool = False,
         annular: bool = False,
-    ) -> ActorsList:
+    ) -> ActorsList[Self]:
         """Get the grid around the patch."""
         cells = self.layer.get_neighboring_cells(
             self.pos, moore=moore, radius=radius, include_center=include_center
         )
         if annular:
             interiors = self.layer.get_neighboring_cells(
                 self.pos, moore=moore, radius=radius - 1, include_center=False
```

### Comparing `abses-0.5.4/abses/components.py` & `abses-0.5.5/abses/components.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 3. TimeDriver 时间驱动器
 4. DataCollector 数据收集器
 """
 
 from __future__ import annotations
 
 import re
-from typing import TYPE_CHECKING, Iterable, Optional, Set, Union
+from typing import TYPE_CHECKING, Any, Iterable, Optional, Set, Union
 
 from omegaconf import DictConfig
 
 from abses.tools.func import make_list
 from abses.tools.regex import MODULE_NAME
 
 if TYPE_CHECKING:
@@ -35,37 +35,37 @@
 class _Component:
     """
     Class _Component is used to represent a component of the model.
     Components are foundational pieces in constructing the model's entities.
     It is initialized with a model and a optional name.
     """
 
-    __args__ = []
+    __args__: Iterable[str] = []
 
-    def __init__(self, model: MainModel, name: Optional[str] = None):
+    def __init__(self, model: MainModel[Any, Any], name: Optional[str] = None):
         self._args: Set[str] = set()
-        self._model: MainModel = model
-        self.name: str = name
+        self._model: MainModel[Any, Any] = model
+        if name is None:
+            name = self.__class__.__name__.lower()
+        self.name = name
         self.add_args(self.__args__)
 
     @property
     def name(self) -> str:
         """Get the name of the component"""
         return self._name
 
     @name.setter
-    def name(self, value: Optional[str]) -> None:
+    def name(self, value: str) -> None:
         """Set the name of the component"""
-        if value is None:
-            value = self.__class__.__name__.lower()
         if not isinstance(value, str):
             raise TypeError(f"Name must be a string, not {type(value)}.")
         if not re.match(MODULE_NAME, value):
             raise ValueError(f"Name '{value}' is not a valid name.")
-        self._name = value
+        self._name: str = value
 
     @property
     def params(self) -> DictConfig:
         """Returns read-only model's parameters.
 
         Returns:
             dict:
```

### Comparing `abses-0.5.4/abses/container.py` & `abses-0.5.5/abses/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,36 @@
 """
 行动者容器，集中保存行动者。
 Container for actors.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Iterable, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Iterable,
+    Optional,
+    Type,
+    Union,
+)
+
+import numpy as np
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 from loguru import logger
 
 from abses.actor import Actor, Breeds
 from abses.errors import ABSESpyError
-from abses.sequences import ActorsList, Selection
+from abses.sequences import HOW, ActorsList, Selection
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
     from abses.cells import PatchCell
     from abses.main import MainModel
 
 ActorTypes: TypeAlias = Union[Type[Actor], Iterable[Type[Actor]]]
@@ -35,40 +45,42 @@
 
 
 class _AgentsContainer(dict):
     """AgentsContainer for the main model."""
 
     def __init__(
         self,
-        model: MainModel,
+        model: MainModel[Any, Any],
         max_len: None | int = None,
     ):
         super().__init__({b: set() for b in model.breeds})
         self._model: MainModel = model
         model._containers.append(self)
-        self._max_length: int = max_len
+        self._max_length: Optional[int] = max_len
 
     def __len__(self) -> int:
         return len(self.get())
 
     def __str__(self) -> str:
         return "ModelAgents"
 
     def __repr__(self) -> str:
         strings = [f"({len(v)}){k}" for k, v in self.items()]
         return f"<{str(self)}: {'; '.join(strings)}>"
 
-    def __contains__(self, name) -> bool:
-        return name in self.get()
+    def __contains__(self, actor: object) -> bool:
+        if not isinstance(actor, Actor):
+            raise TypeError(f"{type(actor)} is not a Actor.")
+        return actor in self.get()
 
-    def __call__(self, *args, **kwargs) -> ActorsList[Actor]:
+    def __call__(self, *args: Breeds, **kwargs: Breeds) -> ActorsList[Actor]:
         return self.get(*args, **kwargs)
 
     @property
-    def model(self) -> MainModel:
+    def model(self) -> MainModel[Any, Any]:
         """The ABSESpy model where the container belongs to."""
         return self._model
 
     @property
     def is_full(self) -> bool:
         """Whether the container is full."""
         return (
@@ -138,15 +150,15 @@
             self._model.breeds = a_cls
 
     def new(
         self,
         breed_cls: Type[Actor],
         num: int = 1,
         singleton: bool = False,
-        **kwargs: dict[str, Any],
+        **kwargs: Any,
     ) -> Union[Actor, ActorsList[Actor]]:
         """Create one or more actors of the given breed class.
 
         Parameters:
             breed_cls:
                 The breed class of the actor(s) to create.
             num:
@@ -179,17 +191,20 @@
         objs = [breed_cls(self._model, **kwargs) for _ in range(num)]
         logger.info(f"Created {num} actors of breed {breed_cls.__name__}")
         # add actors to the container and the schedule.
         for agent in objs:
             self.add(agent)
             self.model.schedule.add(agent)
         # return the created actor(s).
+        actors_list: ActorsList[Actor] = ActorsList(
+            model=self.model, objs=objs
+        )
         if singleton:
-            return objs[0] if num == 1 else objs
-        return ActorsList(model=self.model, objs=objs)
+            return objs[0] if num == 1 else actors_list
+        return actors_list
 
     def get(self, breeds: Breeds = None) -> ActorsList[Actor]:
         """Get all entities of specified breeds to a list.
 
         Parameters:
             breeds:
                 The breed(s) of entities to convert to a list.
@@ -383,24 +398,24 @@
             >>> 2
             model.agents.has(['Actor1', 'Actor2'])
             >>> 5
             ```
         """
         return len(self.get(breeds=breeds))
 
-    def apply(self, func: callable, *args, **kwargs) -> None:
+    def apply(self, func: Callable, *args: Any, **kwargs: Any) -> np.ndarray:
         """Apply a function to all agents in the container.
 
         Parameters:
             func:
                 The function to apply to all agents in the container.
         """
         return self.get().apply(func, *args, **kwargs)
 
-    def item(self, how: str = "item", index: int = 0) -> Actor | None:
+    def item(self, how: HOW = "item", index: int = 0) -> Actor | None:
         """Retrieve one agent if possible.
 
         Parameters:
             how:
                 The method to use to retrieve the agent.
                 Can be either "only", "item", or "random".
                 If "only", it will return the only agent in the container.
@@ -417,25 +432,26 @@
         return self.get().item(how=how, index=index)
 
 
 class _CellAgentsContainer(_AgentsContainer):
     """Container for agents located at cells."""
 
     def __init__(
-        self, model: MainModel, cell: PatchCell, max_len: int | None = None
+        self,
+        model: MainModel[Any, Any],
+        cell: PatchCell,
+        max_len: int | None = None,
     ):
         super().__init__(model, max_len)
         self._cell = cell
 
     def __str__(self) -> str:
         return "CellAgents"
 
-    def _add_one(
-        self, agent: Actor, register: TYPE_CHECKING = False
-    ) -> TYPE_CHECKING:
+    def _add_one(self, agent: Actor, register: bool = False) -> None:
         if agent.on_earth and agent not in self:
             e1 = f"{agent} is on another cell thus cannot be added."
             e2 = "You may use 'actor.move.to()' to change its location."
             e3 = "Or you may use 'actor.move.off()' before adding it."
             raise ABSESpyError(e1 + e2 + e3)
         super()._add_one(agent, register)
         agent.at = self._cell
@@ -457,17 +473,17 @@
         if agent.at is not self._cell:
             raise ABSESpyError(f"{agent} is not on this cell.")
         self[agent.breed].remove(agent)
         del agent.at
 
     def new(
         self,
-        breed_cls: Actor,
+        breed_cls: Type[Actor],
         num: int = 1,
-        singleton: TYPE_CHECKING = False,
+        singleton: bool = False,
         **kwargs: Any,
     ) -> Actor | ActorsList:
         """Creates a new actor or a list of actors of the given breed class.
         The created actors are added to both the cell and the model's global container.
 
         Parameters:
             breed_cls:
```

### Comparing `abses-0.5.4/abses/decision.py` & `abses-0.5.5/abses/decision.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
     Type,
     Union,
+    cast,
 )
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
@@ -34,24 +35,24 @@
 
 Strategy: TypeAlias = Union[str, None, bool, Number]
 
 
 class Decision:
     """Decision class of actor."""
 
-    __strategies__: Optional[Dict] = None
-    _strategies: Optional[Dict] = None
+    __strategies__: Dict[str, Strategy] = {}
+    _strategies: Dict[str, Strategy] = {}
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         cls.validate_strategies(cls.__strategies__)
         cls.set_strategies(cls.__strategies__)
 
-    def __init__(self, agent: Actor = None) -> None:
-        self._agent: Actor = agent
+    def __init__(self, agent: Optional[Actor] = None) -> None:
+        self._agent: Optional[Actor] = agent
         self._strategy: Any = self._setup()
 
     def __repr__(self) -> str:
         return f"<{self.name}: {self.now}>"
 
     @classmethod
     @property
@@ -83,41 +84,40 @@
         """Check if the strategies valid."""
         if not isinstance(strategies, Dict):
             raise TypeError(
                 f"So far, only discrete strategies are supported, you should set '__strategies__' class attribute with a dictionary of strategies when subclassing 'Decision', got {type(strategies)} instead."
             )
 
     @classmethod
-    def set_strategies(cls, strategies: Strategy) -> None:
+    def set_strategies(cls, strategies: Dict[str, Strategy]) -> None:
         """Parsing strategies and save into properties."""
         cls._strategies = strategies
 
-    @classmethod
     @property
-    def strategies(cls) -> Dict:
-        """Possible strategies."""
-        return cls._strategies
+    def strategies(self) -> Dict[str, Strategy]:
+        """Get all strategies."""
+        return self._strategies
 
     @property
-    def agent(self) -> Actor:
+    def agent(self) -> Optional[Actor]:
         """Decision-maker."""
         return self._agent
 
     @classmethod
     def making(cls, method: Callable) -> Callable:
         """A decorator makes this decision."""
 
         @wraps(method)
         def decorated(self: Actor, *args, **kwargs):
             cls.validate_decision_maker(self)
             result = method(self, *args, **kwargs)
             cls.validate_strategy(result)
             return result
 
-        decorated.__making__ = cls
+        setattr(decorated, "__making__", cls)
         return decorated
 
     @classmethod
     def response(cls, strategy: Strategy) -> Callable:
         """Change the decorated function into a response methods."""
 
         def decorator(func) -> Callable:
@@ -127,23 +127,23 @@
                     raise AttributeError(
                         f"{self.breed} doesn't have an attribute 'decisions'"
                     )
                 if not isinstance(
                     getattr(self, "decisions"), _DecisionFactory
                 ):
                     raise TypeError("Type of a decision must be decision.")
-                decision_obj = self.decisions.get(cls.name)
+                decision_obj = self.decisions.get(cast(str, cls.name))
                 if not decision_obj.has_strategy(strategy):
                     raise TypeError(
                         f"Decision '{cls.name}' doesn't have strategy {strategy}."
                     )
                 return func(self, *args, **kwargs)
 
-            wrapper.__response__ = cls
-            wrapper.__expected__ = strategy
+            setattr(wrapper, "__response__", cls)
+            setattr(wrapper, "__expected__", strategy)
             return wrapper
 
         # decorator.__response__ = cls
         return decorator
 
     @classmethod
     def validate_decision_maker(cls, agent: Actor):
@@ -179,23 +179,23 @@
         Parameters:
             strategy:
                 The strategy to validate.
 
         Returns:
             If the strategy exists, return True, otherwise returns False.
         """
-        return strategy in cls.strategies.keys()
+        return strategy in cls._strategies.keys()
 
     @property
     def now(self) -> Any:
         """The strategy now."""
         return self._strategy
 
     def _setup(self) -> Any:
-        if init_strategy := self.setup():
+        if init_strategy := self.setup():  # type: ignore[error-code, func-returns-value]
             self.validate_strategy(init_strategy)
         return init_strategy
 
     def setup(self) -> None:
         """Overwrite to setup an initial strategy for this decision."""
 
     def _find_methods(self, symbol="making") -> Any:
@@ -216,18 +216,22 @@
         """Overwrite this method to do something else after make decision."""
 
 
 class _DecisionFactory:
     """Creating and containing decisions of an agent."""
 
     def __init__(
-        self, agent: Actor, decisions: Optional[Iterable[Decision]] = None
+        self,
+        agent: Actor,
+        decisions: Optional[Iterable[Type[Decision]]] = None,
     ) -> None:
         self.agent: Actor = agent
         self._decisions: Dict[str, Decision] = {}
+        if decisions is None:
+            decisions = []
         self.parse_decisions(decisions)
 
     @property
     def agent(self) -> Actor:
         """Decision-maker, who has these decisions."""
         return self._agent
```

### Comparing `abses-0.5.4/abses/dynamic.py` & `abses-0.5.5/abses/dynamic.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.4/abses/human.py` & `abses-0.5.5/abses/human.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @Author  : Shuang Song
 # @Contact   : SongshGeo@gmail.com
 # GitHub   : https://github.com/SongshGeo
 # Website: https://cv.songshgeo.com/
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, Dict, Optional, Set, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Set, Union
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 from loguru import logger
@@ -21,16 +21,16 @@
 from abses.links import _LinkContainer
 
 from .cells import PatchCell
 from .container import _AgentsContainer
 from .modules import CompositeModule, Module
 from .sequences import ActorsList, Selection
 
-Actors: TypeAlias = Union[ActorsList, Selection, Actor]
-Trigger: TypeAlias = Union[str, Callable]
+Actors: TypeAlias = Union[ActorsList[Actor], Selection, Actor]
+Trigger: TypeAlias = Union[str, Callable[..., Any]]
 if TYPE_CHECKING:
     from abses import MainModel
 
 
 class HumanModule(Module):
     """The `Human` sub-module base class.
 
@@ -40,18 +40,18 @@
     Attributes:
         agents:
             The agents container of this ABSESpy model.
         collections:
             Actor collections defined.
     """
 
-    def __init__(self, model: MainModel, name: Optional[str] = None):
+    def __init__(self, model: MainModel[Any, Any], name: Optional[str] = None):
         Module.__init__(self, model, name)
         logger.info("Initializing a new Human Module...")
-        self._collections: Dict[str, Selection] = DictConfig({})
+        self._collections: Dict[str, Selection] = {}
 
     @property
     def agents(self) -> _AgentsContainer:
         """The agents container of this ABSESpy model."""
         return self.model.agents
 
     @property
@@ -76,15 +76,15 @@
 
     def _must_be_cell(self, cell: PatchCell) -> None:
         if not isinstance(cell, PatchCell):
             raise TypeError(
                 f"Cell must be a subclass of Cell, instead of {type(cell)}."
             )
 
-    def define(self, name: str, selection: Selection) -> ActorsList:
+    def define(self, name: str, selection: Selection) -> ActorsList[Actor]:
         """Define a query of actors and save it into collections.
 
         Parameters:
             name:
                 defined name of this group of actors.
             selection:
                 Selection query of `Actor`.
@@ -117,11 +117,11 @@
         self._collections[name] = selection
         return selected
 
 
 class BaseHuman(CompositeModule, HumanModule, _LinkContainer):
     """The Base Human Module."""
 
-    def __init__(self, model, name="human"):
+    def __init__(self, model: MainModel[Any, Any], name: str = "human"):
         HumanModule.__init__(self, model, name)
         CompositeModule.__init__(self, model, name=name)
         _LinkContainer.__init__(self)
```

### Comparing `abses-0.5.4/abses/main.py` & `abses-0.5.5/abses/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,28 @@
 """
 The main modelling framework of ABSESpy.
 """
 
 from __future__ import annotations
 
 import sys
-from typing import Dict, Generic, List, Optional, Tuple, Type, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 from loguru import logger
@@ -36,21 +49,34 @@
 from .time import TimeDriver
 
 # Logging configuration
 logger.remove(0)
 logger.add(
     sys.stderr,
     format="[{time:YYYY-MM-DD HH:mm:ss}][{module:<15}] | {message}",
-    level="INFO",
+    level="WARNING",
+)
+# 'w' mode in add() method will clean the contents of the logging.log file before writing to it
+logger.add(
+    "logging.log",
+    format="[{time:YYYY-MM-DD HH:mm:ss}][{module:<15}] | {message}",
+    level="DEBUG",
+    mode="w",
 )
 
 # Dynamically load type hints from users' input type
-N = TypeVar("N")
-H = TypeVar("H")
-Reporter: TypeAlias = Dict[str, Union[str, callable]]
+N = TypeVar("N", bound=BaseNature)
+H = TypeVar("H", bound=BaseHuman)
+Reporter: TypeAlias = Union[str, Callable[..., Any]]
+SubSystemType: TypeAlias = Literal["model", "nature", "human"]
+SubSystem = Union[
+    SubSystemType,
+    Tuple[SubSystemType, SubSystemType],
+    Tuple[SubSystemType, SubSystemType, SubSystemType],
+]
 
 
 class MainModel(Generic[H, N], Model, _Notice, _States):
     """
     Base class of a main ABSESpy model.
 
     Attributes:
@@ -76,51 +102,65 @@
             All agents on the earth (added to a specific PatchCell) as a list.
             A model can create multiple lists referring different actors.
     """
 
     def __init__(
         self,
         parameters: DictConfig = DictConfig({}),
-        human_class: Type[H] = BaseHuman,
-        nature_class: Type[N] = BaseNature,
+        human_class: Optional[Type[H]] = None,
+        nature_class: Optional[Type[N]] = None,
         run_id: Optional[int] = None,
-        **kwargs,
+        **kwargs: Optional[Any],
     ) -> None:
         Model.__init__(self, **kwargs)
         _Notice.__init__(self)
         _States.__init__(self)
 
-        self._breeds: dict[str, Type[Actor]] = {}
+        self.running: bool = True
+        self._breeds: Dict[str, Type[Actor]] = {}
         self._containers: List[_AgentsContainer] = []
         self._settings = DictConfig(parameters)
         self._version: str = __version__
-        if not issubclass(human_class, BaseHuman):
-            raise TypeError(f"{human_class} is not a subclass of BaseHuman.")
-        if not issubclass(nature_class, BaseNature):
-            raise TypeError(f"{nature_class} is not a subclass of BaseNature.")
-        self._human = human_class(self)
-        self._nature = nature_class(self)
+        self._check_subsystems(h_cls=human_class, n_cls=nature_class)
         self._agents = _AgentsContainer(
             model=self, max_len=kwargs.get("max_agents")
         )
         self._time = TimeDriver(model=self)
         self._run_id: int | None = run_id
         self.schedule = BaseScheduler(model=self)
         self.initialize_data_collector()
         self._do_each("initialize", order=("nature", "human"))
         self._do_each("set_state", code=1)  # initial state
 
     def __repr__(self) -> str:
         version = self._version
         return f"<{self.name}-{version}({self.state})>"
 
-    def _do_each(self, _func: str, order: Tuple[str] = None, **kwargs) -> None:
+    def _check_subsystems(
+        self, h_cls: Optional[Type[H]], n_cls: Optional[Type[N]]
+    ) -> None:
+        """Check if the subsystems are correctly set."""
+        if h_cls is None:
+            h_cls = cast(Type[H], BaseHuman)
+        else:
+            assert issubclass(h_cls, BaseHuman)
+        if n_cls is None:
+            n_cls = cast(Type[N], BaseNature)
+        else:
+            assert issubclass(n_cls, BaseNature)
+        self._human = h_cls(self)
+        self._nature = n_cls(self)
+
+    def _do_each(
+        self,
+        _func: str,
+        order: SubSystem = ("model", "nature", "human"),
+        **kwargs: Any,
+    ) -> None:
         _obj = {"model": self, "nature": self.nature, "human": self.human}
-        if order is None:
-            order = ("model", "nature", "human")
         for name in order:
             if name not in _obj:
                 raise ValueError(f"{name} is not a valid component.")
             getattr(_obj[name], _func)(**kwargs)
 
     @property
     def run_id(self) -> int | None:
@@ -165,15 +205,15 @@
         2. `model.agents.new(Actor, num=3)` to create 3 agents of Actor.
         3. `model.agents.register(Actor)` to register a new breed of agents to the whole model.
         4. `model.agents.trigger()` to trigger a specific event to all agents.
         """
         return self._agents
 
     @property
-    def actors(self) -> ActorsList:
+    def actors(self) -> ActorsList[Actor]:
         """All agents on the earth as an `ActorList`.
         A model can create multiple lists referring different actors.
         """
         return self.agents.get().select({"on_earth": True})
 
     @property
     def human(self) -> Union[H, BaseHuman]:
@@ -195,15 +235,15 @@
         """The global parameters of this model."""
         return self.settings.get("model", DictConfig({}))
 
     # alias for model's parameters
     p = params
 
     @property
-    def breeds(self) -> Tuple[str]:
+    def breeds(self) -> Tuple[str, ...]:
         """All breeds in the model."""
         return tuple(self._breeds.keys())
 
     @breeds.setter
     def breeds(self, breed: Type[Actor]) -> None:
         """Register a new breed of agents in the model."""
         if not issubclass(breed, Actor):
@@ -218,15 +258,15 @@
         In order, the model will go through the following steps:
         1. Call `model.setup()` method.
         2. Call `model.step()` method.
         3. Repeating steps, until the end situation is triggered
         4. Call `model.end()` method.
         """
         self._setup()
-        while self.running:
+        while self.running is True:
             logger.debug(f"Current tick: {self.time.tick}")
             self._step()
             self.time.go()
             if self.time.tick == steps:
                 self.running = False
         self._end()
 
@@ -252,16 +292,16 @@
     def _end(self) -> None:
         self._do_each("end", order=("nature", "human", "model"))
         self._do_each("set_state", code=3)
         logger.info(f"Ending {self.name}")
 
     def initialize_data_collector(
         self,
-        model_reporters: Optional[Reporter] = None,
-        agent_reporters: Optional[Reporter] = None,
+        model_reporters: Optional[Dict[str, Reporter]] = None,
+        agent_reporters: Optional[Dict[str, Reporter]] = None,
         tables: Optional[Reporter] = None,
     ) -> None:
         """Initialize data collector for this ABSESpy Model.
         This method overrides the default `DataCollector` of `mesa.Model`.
         When initializing, users can set the model-level reporters, agent-level reporters,
         and tables not only by parameters but also by config file.
 
@@ -271,33 +311,38 @@
             agent_reporters:
                 A dictionary of agent-level reporters.
             tables:
                 A list of tables to collect data.
 
         Example:
         """
-        to_reports: DictConfig = self.settings.get(
-            "reports", OmegaConf.create({})
+        cfg: DictConfig = self.settings.get("reports", OmegaConf.create({}))
+        to_reports = cast(
+            Dict[str, Dict[str, Reporter]],
+            OmegaConf.to_container(cfg, resolve=True),
         )
-        to_reports = OmegaConf.to_container(to_reports, resolve=True)
-        reporting_model: DictConfig = to_reports.get("model", {})
-        reporting_agents: DictConfig = to_reports.get("agents", {})
+        reporting_model: Dict[str, Reporter] = to_reports.get("model", {})
+        reporting_agents: Dict[str, Reporter] = to_reports.get("agents", {})
         if model_reporters is not None:
-            reporting_model.update(model_reporters)
+            reporting_model |= model_reporters
         if agent_reporters is not None:
-            reporting_agents.update(agent_reporters)
+            reporting_agents |= agent_reporters
         _convert_to_python_expression(reporting_model)
         _convert_to_python_expression(reporting_agents)
         self.datacollector = DataCollector(
             model_reporters=reporting_model,
             agent_reporters=reporting_agents,
             tables=tables,
         )
 
 
 def _convert_to_python_expression(
-    expression_dict: dict[str, str]
-) -> dict[str, any]:
+    expression_dict: Dict[str, Reporter]
+) -> None:
     """Convert a Python expression string to a Python expression."""
     for key, value in expression_dict.items():
+        if not isinstance(value, str):
+            continue
         if value.startswith(":"):
-            expression_dict[key] = eval(value[1:])  # pylint: disable=eval-used
+            func = eval(value[1:])  # pylint: disable=eval-used
+            assert callable(func), f"{value} is not a callable function."
+            expression_dict[key] = func
```

### Comparing `abses-0.5.4/abses/modules.py` & `abses-0.5.5/abses/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 模型的基本模块。
 Basic implementation of the model's module.
 """
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List, Optional, Type
+from typing import TYPE_CHECKING, Any, List, Optional, Type
 
 from loguru import logger
 
 from abses.tools.func import iter_func
 
 from .bases import _Notice
 from .objects import _BaseObj
@@ -25,15 +25,15 @@
 if TYPE_CHECKING:
     from .main import MainModel
 
 
 class Module(_BaseObj):
     """Basic module for the model."""
 
-    def __init__(self, model: MainModel, name: Optional[str] = None):
+    def __init__(self, model: MainModel[Any, Any], name: Optional[str] = None):
         _BaseObj.__init__(self, model, observer=True, name=name)
         self._open: bool = True
 
     def __repr__(self) -> str:
         flag = "open" if self.opening else "closed"
         return f"<{self.name}: {flag}>"
 
@@ -71,34 +71,40 @@
         """
 
 
 # Composite
 class CompositeModule(Module, _States, _Notice):
     """基本的组合模块，可以创建次级模块"""
 
-    def __init__(self, model: MainModel, name: str = None) -> None:
+    def __init__(
+        self, model: MainModel[Any, Any], name: Optional[str] = None
+    ) -> None:
         Module.__init__(self, model, name=name)
         _States.__init__(self)
         _Notice.__init__(self)
         self._modules: List[Module] = []
 
     @property
     def modules(self) -> List[Module]:
         """All attached sub-modules."""
         return self._modules
 
-    @Module.opening.setter
+    @property
+    def opening(self) -> bool:
+        return self._open
+
+    @opening.setter
     def opening(self, value: bool) -> None:
         for module in self.modules:
             module.opening = value
-        Module.opening.fset(self, value)
+        self._open = value
 
     def create_module(
         self,
-        module_class: Type[Module] = Module,
+        module_class: Optional[Type[Module]] = None,
         how: Optional[str] = None,
         **kwargs,
     ) -> Module:
         """Create a module and attach it to the model.
 
         Parameters:
             module_class:
@@ -116,18 +122,20 @@
                 If the module class is not a subclass of Module.
             ValueError:
                 If the creating method is not valid.
 
         Returns:
             The created module.
         """
-        if not issubclass(module_class, Module):
-            raise TypeError(
-                f"Module {module_class} not inherited from a module."
-            )
+        if module_class is None:
+            module_class = Module
+        else:
+            assert issubclass(
+                module_class, Module
+            ), f"Module {module_class} not inherited from a module."
         if not how:
             module = module_class(model=self._model, **kwargs)
         elif hasattr(module_class, how):
             creating_method = getattr(module_class, how)
             module = creating_method(model=self.model, **kwargs)
         else:
             raise ValueError(f"{how} is not a valid creating method.")
```

### Comparing `abses-0.5.4/abses/move.py` & `abses-0.5.5/abses/move.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "down left",
     "down right",
 ]
 
 
 def _get_layer_and_position(
     pos: Coordinate | PatchCell, layer: Optional[PatchModule] = None
-) -> Tuple[Coordinate, PatchModule]:
+) -> Tuple[Optional[PatchModule], Coordinate]:
     if isinstance(pos, mg.Cell):
         if layer is not None and layer is not pos.layer:
             raise ABSESpyError(
                 "The input layer is not consistent with the cell's layer."
             )
         return pos.layer, pos.pos
     if isinstance(pos, tuple) and len(pos) == 2:
@@ -75,15 +75,15 @@
     # self.geometry = Point(cell.layer.transform * cell.indices)
 
 
 def move_agent_to(
     agent: Actor,
     layer: PatchModule,
     pos: Coordinate | mg.Cell,
-) -> bool:
+) -> None:
     """Move an Actor to another position of this layer.
 
     Parameters:
         agent:
             The actor to operate.
         position:
             The position to put on.
@@ -115,19 +115,21 @@
 
     def __init__(self, actor: Actor) -> None:
         self.actor = actor
         self.model = actor.model
         # self.direction = actor.direction
 
     @property
-    def layer(self) -> PatchModule:
+    def layer(self) -> Optional[PatchModule]:
         """The current layer of the operating actor."""
         return self.actor.layer
 
-    def _operating_layer(self, layer: PatchModule) -> PatchModule:
+    def _operating_layer(
+        self, layer: Optional[PatchModule]
+    ) -> Optional[PatchModule]:
         """
         This method is used to check if the input layer is consistent with the actor's layer.
         """
         if self.layer is None and layer is None:
             raise ABSESpyError("No operating layer is specified.")
         if self.layer is layer or self.layer is None:
             return layer
@@ -159,25 +161,32 @@
                 If the input layer is not consistent with the actor's layer.
                 If the position is out of bounds.
                 Or, if the pos is coordinate without layer.
         """
         if isinstance(pos, str) and pos == "random":
             # 随机分配一个该图层的位置
             operating_layer = self._operating_layer(layer=layer)
+            assert operating_layer is not None
             pos = operating_layer.select().random.choice()
         else:
             # 检查这个位置的类型，返回图层和位置
             layer, pos = _get_layer_and_position(pos, layer=layer)
             operating_layer = self._operating_layer(layer=layer)
+            assert operating_layer is not None
         move_agent_to(self.actor, layer=operating_layer, pos=pos)
 
     def off(self) -> None:
         """Remove the actor from the world."""
+        if self.actor.at is None:
+            raise ABSESpyError("The actor is not located on a cell.")
         if self.actor.on_earth:
-            self.actor.at.agents.remove(self.actor)
+            container = self.actor.at.agents
+            if container is None:
+                raise ABSESpyError("The actor is not located on a cell.")
+            container.remove(self.actor)
         del self.actor.at
 
     def by(self, direction: MovingDirection, distance: int = 1) -> None:
         """Move the actor by a specific distance.
 
         Parameters:
             direction:
@@ -189,15 +198,15 @@
 
         Raises:
             ABSESpyError:
                 If the actor is not located on a cell, thus cannot move.
             ValueError:
                 If the direction is invalid.
         """
-        if not self.actor.on_earth:
+        if (self.actor.at is None) or (self.layer is None):
             raise ABSESpyError(
                 "The actor is not located on a cell, thus cannot move."
             )
         old_row, old_col = self.actor.at.indices
         if direction == "left":
             new_indices = (old_row, old_col - distance)
         elif direction == "right":
@@ -225,9 +234,11 @@
         Parameters:
             prob:
                 The probability to select a cell.
             kwargs:
                 Passing keyword args to `PatchCell.neighboring`,
                 used to select neighboring cells.
         """
+        if self.actor.at is None:
+            raise ABSESpyError("The actor is not located on a cell.")
         cells = self.actor.at.neighboring(**kwargs)
         self.actor.move.to(cells.random.choice(prob=prob))
```

### Comparing `abses-0.5.4/abses/nature.py` & `abses-0.5.5/abses/nature.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,25 @@
 """
 The spatial module.
 """
 
 from __future__ import annotations
 
 import functools
-from numbers import Number
-from typing import TYPE_CHECKING, Any, Callable, Dict, Optional
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Type,
+    Union,
+    cast,
+)
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 import geopandas
@@ -80,23 +89,28 @@
         coords:
             Coordinate system of the raster data.
             This is useful when working with `xarray.DataArray`.
         random:
             A random proxy by calling the cells as an `ActorsList`.
     """
 
-    def __init__(self, model, name=None, **kwargs):
+    def __init__(
+        self,
+        model: MainModel[Any, Any],
+        name: Optional[str] = None,
+        **kwargs: Any,
+    ):
         Module.__init__(self, model, name=name)
         mg.RasterLayer.__init__(self, **kwargs)
         logger.info("Initializing a new Model Layer...")
         logger.info(f"Using rioxarray version: {rioxarray.__version__}")
 
         for cell in self:
             cell.layer = self
-        self._updated_ticks = []
+        self._updated_ticks: List[int] = []
 
     @property
     def cell_properties(self) -> set[str]:
         """The accessible attributes of cells stored in this layer.
         All `PatchCell` methods decorated by `raster_attribute` should be appeared here.
         """
         return self.cell_cls.__attribute_properties__()
@@ -140,19 +154,19 @@
             "y": y_arr,
             "x": x_arr,
         }
 
     @classmethod
     def from_resolution(
         cls,
-        model: MainModel,
-        name: str = None,
+        model: MainModel[Any, Any],
+        name: Optional[str] = None,
         shape: Coordinate = (10, 10),
         crs: Optional[pyproj.CRS | str] = CRS,
-        resolution: Number = 1,
+        resolution: Union[int, float] = 1,
         cell_cls: type[PatchCell] = PatchCell,
     ) -> Self:
         """Create a layer from resolution.
 
         Parameters:
             model:
                 ABSESpy Model that the new module belongs.
@@ -190,18 +204,18 @@
             total_bounds=total_bounds,
             cell_cls=cell_cls,
         )
 
     @classmethod
     def copy_layer(
         cls,
-        model: MainModel,
+        model: MainModel[Any, Any],
         layer: Self,
         name: Optional[str] = None,
-        cell_cls: PatchCell = PatchCell,
+        cell_cls: Type[PatchCell] = PatchCell,
     ) -> Self:
         """Copy an existing layer to create a new layer.
 
         Parameters:
             model:
                 ABSESpy Model that the new module belongs.
             layer:
@@ -233,15 +247,15 @@
 
     @classmethod
     def from_file(
         cls,
         raster_file: str,
         cell_cls: type[Cell] = PatchCell,
         attr_name: str | None = None,
-        model: None | MainModel = None,
+        model: Optional[MainModel[Any, Any]] = None,
         name: str | None = None,
     ) -> Self:
         """Create a raster layer module from a file.
 
         Parameters:
             raster_file:
                 File path of a geo-tiff dataset.
@@ -253,14 +267,16 @@
                 Name of the new module.
                 If None (by default), using lowercase of the '__class__.__name__'.
                 E.g., class Module -> module.
             cell_cls:
                 Class type of `PatchCell` to create.
 
         """
+        if model is None:
+            raise ABSESpyError("No `model` module defined for module.")
         with rio.open(raster_file, "r") as dataset:
             values = dataset.read()
             _, height, width = values.shape
             total_bounds = [
                 dataset.bounds.left,
                 dataset.bounds.bottom,
                 dataset.bounds.right,
@@ -275,18 +291,22 @@
             total_bounds=total_bounds,
             cell_cls=cell_cls,
         )
         obj._transform = dataset.transform
         obj.apply_raster(values, attr_name=attr_name)
         return obj
 
-    def _attr_or_array(self, data: None | str | np.ndarray) -> np.ndarray:
+    def _attr_or_array(
+        self, data: None | str | np.ndarray | xr.DataArray
+    ) -> np.ndarray:
         """Determine the incoming data type and turn it into a reasonable array."""
         if data is None:
             return np.ones(self.shape2d)
+        if isinstance(data, xr.DataArray):
+            data = data.to_numpy()
         if isinstance(data, np.ndarray):
             if data.shape == self.shape2d:
                 return data
             raise ABSESpyError(
                 f"Shape mismatch: {data.shape} [input] != {self.shape2d} [expected]."
             )
         if isinstance(data, str) and data in self.attributes:
@@ -386,15 +406,18 @@
 
     @property
     def random(self) -> ListRandom:
         """Randomly"""
         return self.select().random
 
     def _select_by_geometry(
-        self, geometry: Geometry, refer_layer: Optional[str] = None, **kwargs
+        self,
+        geometry: Geometry,
+        refer_layer: Optional[str] = None,
+        **kwargs: Dict[str, Any],
     ) -> np.ndarray:
         """Gets all the cells that intersect the given geometry.
 
         Parameters:
             geometry:
                 Shapely Geometry to search intersected cells.
             refer_layer:
@@ -414,15 +437,16 @@
                 f"The refer layer {refer_layer} is not available in the attributes"
             )
         data = self.get_rasterio(attr_name=refer_layer)
         out_image, _ = mask.mask(data, [geometry], **kwargs)
         return out_image.reshape(self.shape2d)
 
     def select(
-        self, where: Optional[str | np.ndarray | Geometry] = None
+        self,
+        where: Optional[str | np.ndarray | xr.DataArray | Geometry] = None,
     ) -> ActorsList[PatchCell]:
         """Select cells from this layer.
 
         Parameters:
             where:
                 The condition to select cells.
                 If None (by default), select all cells.
@@ -443,17 +467,20 @@
             isinstance(where, (np.ndarray, str, xr.DataArray)) or where is None
         ):
             mask_ = self._attr_or_array(where).reshape(self.shape2d)
         else:
             raise TypeError(
                 f"{type(where)} is not supported for selecting cells."
             )
-        return ActorsList(self.model, self.array_cells[mask_.astype(bool)])
+        mask_ = np.nan_to_num(mask_, nan=0.0).astype(bool)
+        return ActorsList(self.model, self.array_cells[mask_])
 
-    def apply(self, ufunc: Callable, *args: Any, **kwargs: Any) -> np.ndarray:
+    def apply(
+        self, ufunc: Callable[..., Any], *args: Any, **kwargs: Any
+    ) -> np.ndarray:
         """Apply a function to array cells.
 
         Parameters:
             ufunc:
                 A function to apply.
             *args:
                 Positional arguments to pass to the function.
@@ -478,31 +505,33 @@
     Attributes:
         major_layer:
             The major layer of nature module. By default, it's the first layer that user created.
         total_bounds:
             The spatial scope of the model's concern. By default, uses the major layer of this model.
     """
 
-    def __init__(self, model, name="nature"):
+    def __init__(
+        self, model: MainModel[Any, Any], name: str = "nature"
+    ) -> None:
         CompositeModule.__init__(self, model, name=name)
         crs = self.params.get("crs", CRS)
         mg.GeoSpace.__init__(self, crs=crs)
-        self._major_layer = None
+        self._major_layer: Optional[PatchModule] = None
 
         logger.info("Initializing a new Base Nature module...")
 
     @property
     def major_layer(self) -> PatchModule | None:
         """The major layer of nature module.
         By default, it's the first created layer.
         """
         return self._major_layer
 
     @major_layer.setter
-    def major_layer(self, layer: PatchModule):
+    def major_layer(self, layer: PatchModule) -> None:
         if not isinstance(layer, PatchModule):
             raise TypeError(f"{layer} is not PatchModule.")
         self._major_layer = layer
         self.crs = layer.crs
 
     @property
     def total_bounds(self) -> np.ndarray | None:
@@ -542,34 +571,43 @@
         agents = creator.from_GeoDataFrame(gdf=gdf, unique_id=unique_id)
         self.model.agents.register(agent_cls)
         self.model.agents.add(agents)
         return ActorsList(model=self.model, objs=agents)
 
     def create_module(
         self,
-        module_class: Module = PatchModule,
-        how: str | None = None,
+        module_class: Optional[Type[Module]] = None,
+        how: Optional[str] = None,
         **kwargs: Dict[str, Any],
     ) -> PatchModule:
         """Creates a submodule of the raster layer.
 
         Parameters:
             module_class:
                 The custom module class.
             how:
-                Class method to call when creating the new sub-module (raster layer). So far, there are three options:
+                Class method to call when creating the new sub-module (raster layer).
+                So far, there are three options:
                     `from_resolution`: by selecting shape and resolution.
                     `from_file`: by input of a geo-tiff dataset.
                     `copy_layer`: by copying shape, resolution, bounds, crs, and coordinates of an existing submodule.
                 if None (by default), just simply create a sub-module without any custom methods (i.e., use the base class `PatchModule`).
             **kwargs:
-                Any other arg passed to the creation method. See corresponding method of your how option from `PatchModule` class methods.
+                Any other arg passed to the creation method.
+                See corresponding method of your how option from `PatchModule` class methods.
 
         Returns:
             the created new module.
         """
-        module = super().create_module(module_class, how, **kwargs)
+        if module_class is None:
+            module_class = PatchModule
+        assert issubclass(
+            module_class, PatchModule
+        ), "Must be a `PatchModule`."
+        module = cast(
+            PatchModule, super().create_module(module_class, how, **kwargs)
+        )
         # 如果是第一个创建的模块,则将其作为主要的图层
         if not self.layers:
             self.major_layer = module
         self.add_layer(module)
         return module
```

### Comparing `abses-0.5.4/abses/objects.py` & `abses-0.5.5/abses/objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """
     Base class for model's objects.
     Model object's have access to global model's parameters and time driver.
     """
 
     def __init__(
         self,
-        model: MainModel,
+        model: MainModel[Any, Any],
         observer: Optional[bool] = True,
         name: Optional[str] = None,
     ):
         _Component.__init__(self, model=model, name=name)
         if observer:
             model.attach(self)
         self._model = model
@@ -55,39 +55,38 @@
 
         Returns:
             MainModel:
                 ABSES model object.
         """
         return self._model
 
-    @property
-    def dynamic_variables(self) -> Dict[str, Any]:
-        """Returns read-only model's dynamic variables.
-
-        Returns:
-            Dict[str, Any]:
-                Dictionary of model's dynamic variables.
-        """
-        if not self._dynamic_variables:
-            return {}
-        for k, v in self._dynamic_variables.items():
-            return {k: v.now()}
-
     @model.setter
     def model(self, model: MainModel):
         """Sets the model object.
 
         Parameters:
             model : MainModel
                 ABSES model object.
         """
         if not isinstance(model, mesa.Model):
             raise TypeError("Model must be an instance of mesa.Model")
         self._model = model
 
+    @property
+    def dynamic_variables(self) -> Dict[str, Any]:
+        """Returns read-only model's dynamic variables.
+
+        Returns:
+            Dict[str, Any]:
+                Dictionary of model's dynamic variables.
+        """
+        if not self._dynamic_variables:
+            return {}
+        return {k: v.now() for k, v in self._dynamic_variables.items()}
+
     def add_dynamic_variable(
         self, name: str, data: Any, function: Callable
     ) -> None:
         """Adds new dynamic variable.
 
         Parameters:
             name:
```

### Comparing `abses-0.5.4/abses/random.py` & `abses-0.5.5/abses/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,24 @@
 # @Contact   : SongshGeo@gmail.com
 # GitHub   : https://github.com/SongshGeo
 # Website: https://cv.songshgeo.com/
 
 from __future__ import annotations
 
 from itertools import combinations
-from typing import TYPE_CHECKING, Iterable, List, Literal, Tuple, overload
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Iterable,
+    List,
+    Literal,
+    Optional,
+    Tuple,
+    Union,
+)
 
 import numpy as np
 
 from abses.errors import ABSESpyError
 from abses.tools.func import make_list
 
 if TYPE_CHECKING:
@@ -21,47 +30,42 @@
     from abses.sequences import ActorsList
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
-WHEN_EMPTY: TypeAlias = Literal["only", "random", "first"]
+WHEN_EMPTY: TypeAlias = Literal["raise exception", "return None"]
 
 
 class ListRandom:
     """Create a random generator from an `ActorsList`"""
 
-    def __init__(self, model: MainModel, actors: ActorsList) -> None:
+    def __init__(self, model: MainModel[Any, Any], actors: ActorsList) -> None:
         self.model = model
         self.actors = actors
         self.seed = getattr(model, "_seed", 0)
         self.generator = np.random.default_rng(seed=int(self.seed))
 
     def _to_actors_list(self, objs: Iterable) -> ActorsList:
         from abses.sequences import ActorsList
 
         return ActorsList(self.model, objs=objs)
 
-    def _when_empty(self, when_empty: WHEN_EMPTY) -> str:
+    def _when_empty(self, when_empty: WHEN_EMPTY) -> None:
         if when_empty not in ("raise exception", "return None"):
             raise ValueError(
                 f"Unknown value for `when_empty` parameter: {when_empty}"
             )
         if when_empty == "raise exception":
             raise ABSESpyError(
                 "Trying to choose an actor from an empty `ActorsList`."
             )
-        return None
 
-    @overload
-    def clean_p(self, p: str) -> np.ndarray:
-        ...
-
-    def clean_p(self, prob: np.ndarray) -> np.ndarray:
+    def clean_p(self, prob: Union[np.ndarray, str]) -> np.ndarray:
         """Clean the probabilities.
         Any negative values, NaN values, or zeros will be recognized as in-valid probabilities.
         For all valid probabilities, normalize them into a prob-array (the sum is equal to 1.0).
 
         Parameters:
             prob:
                 An array-like numbers of probabilities.
@@ -94,15 +98,15 @@
     def choice(
         self,
         size: int = 1,
         prob: np.ndarray | None | str = None,
         replace: bool = False,
         as_list: bool = False,
         when_empty: WHEN_EMPTY = "raise exception",
-    ) -> Actor | ActorsList:
+    ) -> Optional[Actor | ActorsList[Actor]]:
         """Randomly choose one or more actors from the current self object.
 
         Parameters:
             size:
                 The number of actors to choose. Defaults to 1.
             prob:
                 A list of probabilities for each actor to be chosen.
@@ -125,15 +129,16 @@
             ValueError:
                 If size is not a positive integer.
             ABSESpyError:
                 Not enough actors to choose in this `ActorsList`.
         """
         instances_num = len(self.actors)
         if instances_num == 0:
-            return self._when_empty(when_empty=when_empty)
+            self._when_empty(when_empty=when_empty)
+            return None
         if not isinstance(size, int):
             raise ValueError(f"{size} isn't an integer size.")
         if instances_num < size and not replace:
             raise ABSESpyError(
                 f"Trying to choose {size} actors from {self.actors}."
             )
         if prob is not None:
```

### Comparing `abses-0.5.4/abses/selection.py` & `abses-0.5.5/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.4/abses/sequences.py` & `abses-0.5.5/abses/sequences.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,88 +15,96 @@
 from functools import cached_property, partial
 from numbers import Number
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
+    Generic,
     List,
     Literal,
     Optional,
+    Sized,
+    TypeVar,
     Union,
+    cast,
     overload,
 )
 
 try:
-    from typing import Self, TypeAlias
+    from typing import TypeAlias
 except ImportError:
-    from typing_extensions import TypeAlias, Self
+    from typing_extensions import TypeAlias
 
 import mesa_geo as mg
 import numpy as np
+from numpy.typing import NDArray
 
 from abses.errors import ABSESpyError
 from abses.random import ListRandom
 from abses.selection import selecting
 
 from .tools.func import make_list
 
 if TYPE_CHECKING:
+    from abses.main import MainModel
+
     from .actor import Actor
 
-Selection: TypeAlias = Union[str, Iterable[bool]]
+Selection: TypeAlias = Union[str, Iterable[bool], Dict[str, bool]]
 HOW: TypeAlias = Literal["only", "random", "item"]
+ActorType = TypeVar("ActorType", bound="Actor")
 
 
 def get_only_agent(agents: ActorsList) -> Actor:
     """Select one agent"""
     if len(agents) == 0:
         raise ValueError("No agent found.")
     if len(agents) == 1:
         return agents[0]
     raise ValueError("More than one agent.")
 
 
-class ActorsList(list):
+class ActorsList(List[ActorType], Generic[ActorType]):
     """A list of actors in an agent-based model."""
 
-    def __init__(self, model, objs=()):
+    def __init__(
+        self, model: MainModel[Any, Any], objs: Iterable[Actor] = ()
+    ) -> None:
         super().__init__(objs)
         self._model = model
 
     def __repr__(self):
         results = [f"({len(v)}){k}" for k, v in self.to_dict().items()]
         return f"<ActorsList: {'; '.join(results)}>"
 
-    def __eq__(self, other: Iterable) -> bool:
+    def __eq__(self, other: Iterable[Any]) -> bool:
         return (
             all(actor in other for actor in self)
-            if self._is_same_length(other)
+            if self._is_same_length(cast(Sized, other))
             else False
         )
 
     @overload
     def __getitem__(self, other: int) -> Actor:
         ...
 
     @overload
-    def __getitem__(self, index: slice) -> Self:
+    def __getitem__(self, index: slice) -> ActorsList[Actor]:
         ...
 
     def __getitem__(self, index):
         results = super().__getitem__(index)
         return (
             ActorsList(self._model, results)
             if isinstance(index, slice)
             else results
         )
 
-    def _is_same_length(
-        self, length: Iterable[Any], rep_error: bool = False
-    ) -> bool:
+    def _is_same_length(self, length: Sized, rep_error: bool = False) -> bool:
         """Check if the length of input is as same as the number of actors."""
         if not hasattr(self, "__len__"):
             raise ValueError(f"{type(length)} object is not iterable.")
         if len(length) != len(self):
             if rep_error:
                 raise ValueError(
                     f"Length of the input {len(length)} mismatch {len(self)} actors."
@@ -105,30 +113,30 @@
         return True
 
     @cached_property
     def random(self) -> ListRandom:
         """随机模块"""
         return ListRandom(actors=self, model=self._model)
 
-    def to_dict(self) -> Dict[str, Self]:
+    def to_dict(self) -> Dict[str, ActorsList[Actor]]:
         """Convert all actors in this list to a dictionary like {breed: ActorList}.
 
         Returns:
             key is the breed of actors, and values are corresponding actors.
         """
-        dic = {}
+        dic: Dict[str, ActorsList[Actor]] = {}
         for actor in iter(self):
             breed = actor.breed
             if breed not in dic:
                 dic[breed] = ActorsList(self._model, [actor])
             else:
                 dic[breed].append(actor)
         return dic
 
-    def select(self, selection: Selection) -> Self:
+    def select(self, selection: Selection) -> ActorsList[Actor]:
         """
         Returns a new :class:`ActorList` based on `selection`.
 
         Parameters:
             selection:
                 List with same length as the agent list.
                 Positions that return True will be selected.
@@ -153,15 +161,15 @@
             ActorList: A subset of origin agents list.
         """
         ids = make_list(ids)
         return self.select([agent.unique_id in ids for agent in self])
 
     def better(
         self, metric: str, than: Optional[Union[Number, Actor]] = None
-    ) -> Self:
+    ) -> ActorsList[Actor]:
         """
         Selects the elements of the sequence that are better than a given value or actor
         based on a specified metric.
 
         Parameters:
             metric:
                 The name of the attribute to use as the metric for comparison.
@@ -190,43 +198,42 @@
         if isinstance(than, Number):
             return self.select(metrics > than)
         if isinstance(than, mg.GeoAgent):
             diff = self.array(metric) - getattr(than, metric)
             return self.select(diff > 0)
         raise ABSESpyError(f"Invalid than type {type(than)}.")
 
-    def update(self, attr: str, values: Iterable[any]) -> None:
+    def update(self, attr: str, values: Iterable[Any]) -> None:
         """Update the specified attribute of each agent in the sequence with the corresponding value in the given iterable.
 
         Parameters:
             attr:
                 The name of the attribute to update.
             values:
                 An iterable of values to update the attribute with. Must be the same length as the sequence.
 
         Raises:
             ValueError:
                 If the length of the values iterable does not match the length of the sequence.
         """
-        self._is_same_length(values, rep_error=True)
+        self._is_same_length(cast(Sized, values), rep_error=True)
         for agent, val in zip(self, values):
             setattr(agent, attr, val)
 
-    def split(self, where: Iterable[int]) -> np.ndarray:
+    def split(self, where: NDArray[Any]) -> List[NDArray[np.object_]]:
         """Split agents into N+1 groups.
 
         Parameters:
             where:
                 indexes [size=N] denotes where to split.
 
         Returns:
             np.ndarray: N+1 groups: agents array
         """
-        to_split = np.array(self)
-        return np.hsplit(to_split, where)
+        return np.hsplit(np.array(self), where)
 
     def array(self, attr: str) -> np.ndarray:
         """Convert the specified attribute of all actors to a numpy array.
 
         Parameters:
             attr:
                 The name of the attribute to convert to a numpy array.
@@ -288,15 +295,27 @@
         """
         if agent := self.item(how=how, index=0):
             return agent.get(attr)
         if default is not None:
             return default
         raise ValueError("No agent found or default value.")
 
-    def item(self, how: HOW = "item", index: int = 0) -> Actor | None:
+    def set(self, attr: str, value: Any) -> None:
+        """Set the attribute of all agents in the sequence to the specified value.
+
+        Parameters:
+            attr:
+                The name of the attribute to set.
+            value:
+                The value to set the attribute to.
+        """
+        for agent in iter(self):
+            agent.set(attr, value)
+
+    def item(self, how: HOW = "item", index: int = 0) -> Optional[Actor]:
         """Retrieve one agent if possible.
 
         Parameters:
             how:
                 The method to use to retrieve the agent.
                 Can be either "only", "item", or "random".
                 If "only", it will return the only agent in the container.
@@ -309,11 +328,12 @@
 
         Returns:
             The agent if found, otherwise None.
         """
         if how == "only":
             return get_only_agent(self)
         if how == "random":
-            return self.random.choice(when_empty="return None")
+            actor = self.random.choice(when_empty="return None")
+            return cast(Optional["Actor"], actor)
         if how == "item":
             return self[index] if len(self) > index else None
         raise ValueError(f"Invalid how method '{how}'.")
```

### Comparing `abses-0.5.4/abses/states.py` & `abses-0.5.5/abses/states.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 class _States:
     """
     模型的主要部分（自然模块和人类模块），动作将发送给 Mediator 进行记录
     """
 
     _states = STATES
 
-    def __init__(self):
-        self._state = 0  # new model
+    def __init__(self) -> None:
+        self._state: int = 0  # new model
 
     @property
     def state(self) -> str:
         """模块状态"""
         return self._states[self._state]
 
     def set_state(self, code: int) -> None:
```

### Comparing `abses-0.5.4/abses/time.py` & `abses-0.5.5/abses/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,52 @@
 
 from __future__ import annotations
 
 import threading
 from collections import deque
 from datetime import datetime
 from functools import total_ordering, wraps
-from typing import TYPE_CHECKING, Dict, List, Optional
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Union,
+    cast,
+)
 
 import pendulum
+from omegaconf import DictConfig
+from pendulum.datetime import DateTime
+from pendulum.duration import Duration
 
 from abses.components import _Component
 
 if TYPE_CHECKING:
     from .main import MainModel
 
+try:
+    from typing import Self
+except ImportError:
+    from typing_extensions import Self
 
 VALID_DT_ATTRS = (
     "years",
     "months",
     "weeks",
     "days",
     "hours",
     "minutes",
     "seconds",
 )
 
 
-def time_condition(condition: dict, when_run: bool = True) -> callable:
+def time_condition(condition: dict, when_run: bool = True) -> Callable:
     """
     A decorator to run a method based on a time condition.
 
     Parameters:
         condition:
             A dictionary containing conditions to check against the `time` attribute.
             The keys can be ['year', 'month', 'weekday', 'freqstr'].
@@ -110,47 +126,50 @@
     | hours          | int                | 0             | Time duration in hours for the duration mode. |
     | minutes        | int                | 0             | Time duration in minutes for the duration mode. |
     | seconds        | int                | 0             | Time duration in seconds for the duration mode. |
 
     See tutorial to see more.
     """
 
-    _instances = {}
+    _instances: Dict[MainModel[Any, Any], Self] = {}
     _lock = threading.Lock()
 
     def __new__(cls, model: MainModel):
         with cls._lock:
             if not cls._instances.get(model):
                 driver = super(TimeDriver, cls).__new__(cls)
                 cls._instances[model] = driver
             else:
                 driver = cls._instances[model]
         return driver
 
     def __init__(self, model: MainModel):
         super().__init__(model=model, name="time")
-        self._model: MainModel = model
+        self._model: MainModel[Any, Any] = model
         self._tick: int = 0
-        self._start_dt: Optional[datetime] = None
-        self._duration: Optional[pendulum.duration] = None
-        self._history = deque()
+        self._start_dt: DateTime = pendulum.instance(datetime.now(), tz=None)
+        self._end_dt: Optional[Union[DateTime, int]] = None
+        self._duration: Optional[Duration] = None
+        self._history: deque = deque()
         self._parse_time_settings()
 
     def __repr__(self) -> str:
         if self.ticking_mode == "tick":
             return f"<TimeDriver: tick[{self.tick}]>"
         if self.ticking_mode == "duration":
             return f"<TimeDriver: {self.strftime('%Y-%m-%d %H:%M:%S')}>"
         return f"<TimeDriver: irregular[{self.tick}] {self.strftime('%Y-%m-%d %H:%M:%S')}>"
 
     def __eq__(self, other: object) -> bool:
         return self.dt.__eq__(other)
 
     def __lt__(self, other: object) -> bool:
-        return self.dt.__lt__(other)
+        if isinstance(other, (DateTime, datetime)):
+            return self.dt < other
+        raise NotImplementedError(f"Cannot compare with {other}.")
 
     @property
     def should_end(self) -> bool:
         """Should the model end or not."""
         if not self.end_dt:
             return False
         if isinstance(self.end_dt, datetime):
@@ -211,126 +230,133 @@
     #     # logger.info(report)
     #     sys.stdout.write("\r" + report)
     #     sys.stdout.flush()
 
     def _parse_time_settings(self) -> None:
         """Setup the time driver."""
         # Parse the start time settings
-        self.start_dt = self.params.get("start")
+        self.start_dt = self.params.get("start", None)
         # logger.debug(f"start_dt: {self.start_dt}")
 
         # Parse the end time settings
-        self.end_dt = self.params.get("end")
+        self.end_dt = self.params.get("end", None)
         # logger.debug(f"end_dt: {self.end_dt}")
 
         # Parse the duration settings
         self.parse_duration(self.params)
         # logger.debug(f"duration: {self.duration}")
 
         # Parse the irregular settings
-        self._irregular = self.params.get("irregular")
+        self.irregular: bool = self.params.get("irregular", False)
         # logger.debug("irregular: {}", self._irregular)
         # logger.debug("Ticking mode: {}", self.ticking_mode)
 
         self.dt = self.start_dt
         self._history.append(self.dt)
 
     @property
-    def duration(self) -> pendulum.duration | None:
+    def irregular(self) -> bool:
+        """Returns the irregular mode of the time driver."""
+        return self._irregular
+
+    @irregular.setter
+    def irregular(self, value: bool) -> None:
+        """Set the irregular mode of the time driver."""
+        if not isinstance(value, bool):
+            raise TypeError("Irregular mode must be a boolean.")
+        self._irregular = value
+
+    @property
+    def duration(self) -> Duration | None:
         """Returns the duration of the time driver."""
         return self._duration
 
-    def parse_duration(self, duration: Dict[str, int]) -> None:
+    def parse_duration(self, duration: DictConfig) -> None:
         """Set the duration of the time driver."""
         valid_attributes = VALID_DT_ATTRS
         valid_dict = {}
         for attribute in valid_attributes:
             value = duration.get(attribute, 0)
             if not isinstance(value, int):
                 raise TypeError(f"{attribute} must be an integer.")
             valid_dict[attribute] = value
         if all(value == 0 for value in valid_dict.values()):
             self._duration = None
         else:
             self._duration = pendulum.duration(**valid_dict)
 
     @property
-    def start_dt(self) -> datetime | None:
+    def start_dt(self) -> DateTime:
         """Returns the starting time for the model."""
         return self._start_dt
 
     @start_dt.setter
-    def start_dt(self, dt: datetime | None) -> None:
+    def start_dt(self, dt: Optional[Union[datetime, DateTime, str]]) -> None:
         """Set the starting time."""
         if isinstance(dt, datetime):
             self._start_dt = pendulum.instance(dt, tz=None)
         elif dt is None:
             self._start_dt = pendulum.instance(datetime.now(), tz=None)
         elif isinstance(dt, str):
-            self._start_dt = pendulum.parse(dt, tz=None)
+            self._start_dt = cast(DateTime, pendulum.parse(dt, tz=None))
         else:
             raise TypeError(
                 "Start time must be a datetime object or a string."
             )
 
     @property
-    def end_dt(self) -> datetime | int | None:
+    def end_dt(self) -> Optional[Union[datetime, int]]:
         """The real-world time or the ticks when the model should be end."""
         return self._end_dt
 
     @end_dt.setter
-    def end_dt(self, dt: datetime | int | None) -> None:
+    def end_dt(self, dt: Optional[Union[datetime, DateTime, str]]) -> None:
         if isinstance(dt, int) and dt <= 0:
             raise ValueError("End time cannot be negative.")
         if isinstance(dt, int):
             self._end_dt = dt
         elif isinstance(dt, datetime):
             self._end_dt = pendulum.instance(dt, tz=None)
         elif dt is None:
             self._end_dt = None
         elif isinstance(dt, str):
-            self._end_dt = pendulum.parse(dt, tz=None)
+            self._end_dt = cast(DateTime, pendulum.parse(dt, tz=None))
         else:
             raise TypeError("End time must be a datetime object or a string.")
 
     @property
-    def dt(self) -> datetime:
+    def dt(self) -> DateTime:
         """The current real-world time for the model without timezone information."""
         return self._dt
 
     @dt.setter
-    def dt(self, dt: datetime) -> None:
+    def dt(self, dt: DateTime) -> None:
         """Set the current real-world time."""
-        if not isinstance(dt, datetime):
+        if not isinstance(dt, DateTime):
             raise TypeError("dt must be a datetime object.")
         self._dt = dt
 
     @property
     def day(self) -> int:
         """Returns the current day for the model."""
         return self.dt.day
 
     @property
-    def dayofweek(self) -> int:
+    def day_of_week(self) -> int:
         """Returns the number for the day of the week for the model."""
-        return self.dt.dayofweek
+        return self.dt.day_of_week
 
     @property
-    def dayofyear(self) -> int:
+    def day_of_year(self) -> int:
         """Returns the day of the year for the model."""
-        return self.dt.dayofyear
-
-    @property
-    def daysinmonth(self) -> int:
-        """Get the total number of days of the month that this period falls on for the model."""
-        return self.dt.daysinmonth
+        return self.dt.day_of_year
 
     @property
     def days_in_month(self) -> int:
-        """Get the total number of days in the month that this period falls on for the model."""
+        """Get the total number of days of the month that this period falls on for the model."""
         return self.dt.days_in_month
 
     @property
     def hour(self) -> int:
         """Get the hour of the day component of the Period."""
         return self.dt.hour
 
@@ -346,63 +372,43 @@
 
     @property
     def quarter(self) -> int:
         """Return the quarter the current model's Period falls on."""
         return self.dt.quarter
 
     @property
-    def qyear(self) -> int:
-        """Fiscal year a model's Period lies in according to its starting-quarter."""
-        return self.dt.qyear
-
-    @property
     def second(self) -> int:
         """Get the second component of a model's Period."""
         return self.dt.second
 
     @property
-    def ordinal(self) -> int:
-        """Returns period ordinal, which is the number of periods elapsed since a starting period."""
-        return self.dt.ordinal
-
-    @property
     def is_leap_year(self) -> bool:
         """Return True if the period's year is in a leap year."""
-        return self.dt.is_leap_year
+        return self.dt.is_leap_year()
 
     @property
-    def week(self) -> int:
+    def week_of_year(self) -> int:
         """Get the week of the year on the given Period."""
-        return self.dt.week
+        return self.dt.week_of_year
 
     @property
-    def weekday(self) -> int:
-        """Day of the week the period lies in, with Monday=0 and Sunday=6."""
-        return self.dt.weekday
+    def week_of_month(self) -> int:
+        """Get the week of the month on the given Period."""
+        return self.dt.week_of_month
 
     @property
-    def weekofyear(self) -> int:
-        """Get the week of the year on the given Period."""
-        return self.dt.weekofyear
+    def weekday(self) -> int:
+        """Day of the week the period lies in, with Monday=0 and Sunday=6."""
+        return self.dt.weekday()
 
     @property
     def year(self) -> int:
         """Return the year this Period falls on."""
         return self.dt.year
 
-    @property
-    def day_of_year(self) -> int:
-        """Return the day of the year."""
-        return self.dt.day_of_year
-
-    @property
-    def day_of_week(self) -> int:
-        """Day of the week the period lies in, with Monday=0 and Sunday=6."""
-        return self.dt.day_of_week
-
     def strftime(self, fmt: str) -> str:
         """Returns a string representing the current time.
 
         Parameters:
             fmt:
                 An explicit format string of datetime.
         """
```

### Comparing `abses-0.5.4/abses/tools/func.py` & `abses-0.5.5/abses/tools/func.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Website: https://cv.songshgeo.com/
 
 """
 这个模块储存一些
 """
 
 import logging
-from typing import Any, List
+from typing import Any, Callable, List
 
 import numpy as np
 from scipy import ndimage
 
 from abses.tools.regex import CAMEL_NAME
 
 logger = logging.getLogger(__name__)
@@ -71,28 +71,28 @@
         element = [element]
     elif isinstance(element, (tuple, set)):
         element = list(element)
 
     return element
 
 
-def iter_func(elements: str) -> callable:
+def iter_func(elements: str) -> Callable:
     """
     A decorator broadcasting function to all elements if available.
 
     Parameters:
         elements:
             attribute name where object store iterable elements.
             All element in this iterable object will call the decorated function.
 
     Returns:
         The decorated class method.
     """
 
-    def broadcast(func: callable) -> callable:
+    def broadcast(func: Callable) -> Callable:
         def broadcast_func(self, *args, **kwargs):
             result = func(self, *args, **kwargs)
             if not hasattr(self, elements):
                 return result
             for element in getattr(self, elements):
                 getattr(element, func.__name__)(*args, **kwargs)
             return result
```

### Comparing `abses-0.5.4/abses/tools/regex.py` & `abses-0.5.5/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.5.4/pyproject.toml` & `abses-0.5.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.5.4"
+version = "0.5.5"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
@@ -65,19 +65,20 @@
 pytest-cov = "^4.1.0"
 flake8 = "^6.1.0"
 isort = "^5.12.0"
 nbstripout = "^0.6.1"
 pydocstyle = "^6.3.0"
 pre-commit-hooks = "^4.4.0"
 interrogate = "^1.5.0"
-mypy = "^1.5.1"
+mypy = "^1.6.1"
 bandit = "^1.7.5"
 black = "^23.9.1"
 pylint = "^3.0.1"
 tox = "^4.11.3"
+lxml = "^5.2.1"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.4.2"
 mkdocs-git-revision-date-localized-plugin = "^1.2.0"
 mkdocs-minify-plugin = "^0.7.1"
@@ -98,7 +99,17 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.scriv]
 version = "literal: pyproject.toml: tool.poetry.version"
 format = "md"
+
+[tool.mypy]
+ignore_missing_imports = true
+disable_error_code = ["misc", "override"]
+
+[[tool.mypy.overrides]]
+module = [
+    "tests.*",
+]
+ignore_errors = true
```

### Comparing `abses-0.5.4/PKG-INFO` & `abses-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.5.4
+Version: 0.5.5
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: abses Version: 0.5.4 Summary: ABSESpy makes it
+Metadata-Version: 2.1 Name: abses Version: 0.5.5 Summary: ABSESpy makes it
 easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
```

