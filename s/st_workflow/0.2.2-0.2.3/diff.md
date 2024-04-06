# Comparing `tmp/st_workflow-0.2.2.tar.gz` & `tmp/st_workflow-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_workflow-0.2.2.tar", max compression
+gzip compressed data, was "st_workflow-0.2.3.tar", max compression
```

## Comparing `st_workflow-0.2.2.tar` & `st_workflow-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    17491 2024-02-03 14:36:59.062198 st_workflow-0.2.2/README.md
--rw-r--r--   0        0        0      457 2024-02-19 08:45:17.634857 st_workflow-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7275 2024-02-19 08:44:29.274861 st_workflow-0.2.2/st_workflow/__init__.py
--rw-r--r--   0        0        0    18149 1970-01-01 00:00:00.000000 st_workflow-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    17491 2024-02-03 14:36:59.062198 st_workflow-0.2.3/README.md
+-rw-r--r--   0        0        0      457 2024-04-06 19:17:20.859484 st_workflow-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7250 2024-04-06 19:05:38.199522 st_workflow-0.2.3/st_workflow/__init__.py
+-rw-r--r--   0        0        0    18149 1970-01-01 00:00:00.000000 st_workflow-0.2.3/PKG-INFO
```

### Comparing `st_workflow-0.2.2/README.md` & `st_workflow-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `st_workflow-0.2.2/st_workflow/__init__.py` & `st_workflow-0.2.3/st_workflow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from dataclasses import dataclass
 from enum import Enum
+from itertools import chain
 from typing import Callable, List, Optional
 from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 
 import inspect
 import asyncio
 
 
@@ -13,22 +15,35 @@
 
 
 class ExecutionMode(Enum):
     THREAD = "thread"
     PROCESS = "process"
 
 
+@dataclass
+class Step:
+    func: Callable
+    name: Optional[str] = None
+    timeout: Optional[int] = None
+    retries: int = 0
+    cont_on_err: bool = False
+    err_step: Optional["Step"] = None
+
+
+type CondSteps = Callable | Step | List[Callable] | List[Step]
+
+
 class Workflow:
     def __init__(self, ctx: dict) -> None:
         self.ctx = ctx
         self.ctx["cancel"] = False
         self.ctx["error"] = False
         self.thread_executor = ThreadPoolExecutor()
         self.process_executor = ProcessPoolExecutor()
-        self.steps = {
+        self.steps: dict[str, list[Step]] = {
             Scope.NORMAL.value: [],
             Scope.ERROR.value: [],
             Scope.EXIT.value: [],
         }
 
     def __exit__(self, _exc_type, _exc_value, _traceback):
         self.thread_executor.shutdown(wait=True)
@@ -38,105 +53,83 @@
         self,
         func: Callable,
         scope=Scope.NORMAL,
         name: Optional[str] = None,
         timeout: Optional[int] = None,
         retries: int = 0,
         cont_on_err: bool = False,
-        err_step: Optional[dict] = None,
+        err_step: Optional[Step] = None,
     ):
         if name is None:
             name = func.__name__
+
         self.steps[scope.value].append(
-            {
-                "name": name,
-                "func": func,
-                "err_step": err_step,
-                "timeout": timeout,
-                "retries": retries,
-                "cont_on_err": cont_on_err,
-            }
+            Step(
+                func=func,
+                name=name,
+                err_step=err_step,
+                timeout=timeout,
+                retries=retries,
+                cont_on_err=cont_on_err,
+            )
         )
 
     def add_error_step(
         self,
         func: Callable,
         name: Optional[str] = None,
         timeout: Optional[int] = None,
         step_func: Optional[Callable] = None,
         retries: int = 0,
     ):
         if step_func:
-            step_func_name = step_func.__name__
-            step = next(
-                filter(
-                    lambda x: x["name"] == step_func_name,
-                    self.steps[Scope.NORMAL.value],
-                )
+            steps = filter(
+                lambda s: s.name == step_func.__name__, self.steps[Scope.NORMAL.value]
+            )
+            step = next(steps)
+            step.err_step = Step(
+                name=func.__name__, func=func, timeout=timeout, retries=retries
             )
-            step["err_step"] = {
-                "name": func.__name__,
-                "func": func,
-                "timeout": timeout,
-                "retries": retries,
-            }
         else:
             self.add_step(func, Scope.ERROR, name, timeout, retries)
 
     def add_exit_step(
         self,
         func: Callable,
         name: Optional[str] = None,
         timeout: Optional[int] = None,
         retries: int = 0,
     ):
         self.add_step(func, Scope.EXIT, name, timeout, retries)
 
     def add_cond_step(
         self,
-        name: str,
-        on_true_steps: Callable | List[Callable],
-        on_false_steps: Callable | List[Callable],
+        on_true_steps: CondSteps,
+        on_false_steps: CondSteps,
         scope=Scope.NORMAL,
-        timeout: Optional[int] = None,
-        retries: int = 0,
     ):
+        prev_step = self.steps[scope.value][-1]
+
         async def cond_step():
-            index = next(
-                (
-                    index
-                    for index, step in enumerate(self.steps[scope.value])
-                    if step["name"] == name
-                )
-            )
-            index -= 1
-            prev_result = (
-                self.ctx.get(self.steps[scope.value][index]["name"])
-                if self.steps[scope.value]
-                else None
-            )
+            prev_result = self.ctx.get(prev_step.name)
 
             next_steps = on_true_steps if prev_result else on_false_steps
 
             if not isinstance(next_steps, List):
                 next_steps = [next_steps]
 
-            results = []
-
             for step in next_steps:
-                result = await self._run_step(
-                    {"func": step, "timeout": timeout, "retries": retries}
-                )
-
-                if result:
-                    results.append(result[1])
+                if isinstance(step, Callable):
+                    step = Step(func=step, name=step.__name__)
+                results = await self._run_step(step)
 
-            return results[-1]
+                if results:
+                    self.ctx[results[0]] = results[1]
 
-        self.add_step(cond_step, scope, name, timeout, retries)
+        self.add_step(cond_step, scope)
 
     def add_parallel_steps(
         self,
         name: str,
         steps: list[Callable],
         execution_mode=ExecutionMode.THREAD,
         scope=Scope.NORMAL,
@@ -173,21 +166,23 @@
                     break
 
                 results = await self._run_step(step)
                 if results:
                     step_name = results[0]
                     result = results[1]
                     self.ctx[step_name] = result
-                    err_step = step.get("err_step") or {}
-                    err_step_name = err_step.get("name")
-                    if step_name == err_step_name and not step.get("cont_on_err"):
+                    if (
+                        step.err_step
+                        and step_name == step.err_step.name
+                        and not step.cont_on_err
+                    ):
                         break
             except Exception as e:
-                self.ctx[f"{scope.value}_error"] = {"step": step["name"], "error": e}
-                if not step["cont_on_err"]:
+                self.ctx[f"{scope.value}_error"] = {"step": step.name, "error": e}
+                if not step.cont_on_err:
                     raise e
 
     async def run(self, **kwargs):
         self.ctx.update(kwargs)
         try:
             await self.run_steps(Scope.NORMAL)
         except Exception as e:
@@ -201,38 +196,44 @@
                 await self.run_steps(Scope.ERROR)
         finally:
             await self.run_steps(Scope.EXIT)
 
     def cancel(self):
         self.ctx["cancel"] = True
 
+    def get_step_value(self, func: Callable):
+        try:
+            steps = list(chain.from_iterable(self.steps.values()))
+            steps = filter(lambda s: s.func.__name__ == func.__name__, steps)
+            step = next(steps)
+            return self.ctx[step.name]
+        except StopIteration:
+            return None
+
     def _get_step_args(self, func: Callable):
         func_args = inspect.signature(func).parameters
         if "ctx" in func_args:
             return [self.ctx]
         else:
             return [self.ctx[arg] for arg in func_args]
 
-    async def _run_step(self, step: dict):
-        name = step.get("name")
-        func = step["func"]
-        timeout = step.get("timeout")
-        retries = step.get("retries", 0)
-        err_step = step.get("err_step")
-        args = self._get_step_args(func)
+    async def _run_step(self, step: Step):
+        args = self._get_step_args(step.func)
 
-        for i in range(retries + 1):
+        for i in range(step.retries + 1):
             try:
-                if asyncio.iscoroutinefunction(func):
-                    if timeout is not None:
-                        result = await asyncio.wait_for(func(*args), timeout=timeout)
-                        return (name, result)
+                if asyncio.iscoroutinefunction(step.func):
+                    if step.timeout is not None:
+                        result = await asyncio.wait_for(
+                            step.func(*args), timeout=step.timeout
+                        )
+                        return (step.name, result)
                     else:
-                        result = await func(*args)
-                        return (name, result)
+                        result = await step.func(*args)
+                        return (step.name, result)
                 else:
-                    return (name, func(*args))
+                    return (step.name, step.func(*args))
             except Exception as e:
-                if err_step:
-                    return await self._run_step(err_step)
-                if i == retries:
+                if step.err_step:
+                    return await self._run_step(step.err_step)
+                if i == step.retries:
                     raise e
```

### Comparing `st_workflow-0.2.2/PKG-INFO` & `st_workflow-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_workflow
-Version: 0.2.2
+Version: 0.2.3
 Summary: Library for creating complex workflows in Python
 Home-page: https://github.com/safari12/st_workflow
 License: MIT
 Author: Reza Safari
 Author-email: rsafari.s@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

