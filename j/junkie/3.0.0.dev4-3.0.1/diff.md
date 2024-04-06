# Comparing `tmp/junkie-3.0.0.dev4.tar.gz` & `tmp/junkie-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/junkie-3.0.0.dev4.tar", last modified: Mon Nov 14 21:28:54 2022, max compression
+gzip compressed data, was "/home/runner/work/junkie/junkie/dist/.tmp-qtm89409/junkie-3.0.1.tar", last modified: Sat Apr  6 20:08:44 2024, max compression
```

## Comparing `junkie-3.0.0.dev4.tar` & `junkie-3.0.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/junkie/
--rw-r--r--   0 runner    (1001) docker     (121)     9114 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/junkie/_junkie.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/junkie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/junkie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/junkie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/junkie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/junkie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/junkie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/test/
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/test/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/test/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/test/test_bugfix.py
--rw-r--r--   0 runner    (1001) docker     (121)    14669 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/test/test_junkie.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-11-14 21:28:42.000000 junkie-3.0.0.dev4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-14 21:28:54.000000 junkie-3.0.0.dev4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:44.000000 junkie-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 20:08:38.000000 junkie-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-06 20:08:44.000000 junkie-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9087 2024-04-06 20:08:38.000000 junkie-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-06 20:08:38.000000 junkie-3.0.1/junkie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-04-06 20:08:38.000000 junkie-3.0.1/junkie/_junkie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 20:08:44.000000 junkie-3.0.1/junkie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:08:44.000000 junkie-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-06 20:08:38.000000 junkie-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:44.000000 junkie-3.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 20:08:38.000000 junkie-3.0.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_bugfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_junkie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-06 20:08:38.000000 junkie-3.0.1/test/test_readme.py
```

### Comparing `junkie-3.0.0.dev4/junkie/_junkie.py` & `junkie-3.0.1/junkie/_junkie.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,33 +17,33 @@
 
 class JunkieError(RuntimeError):
     pass
 
 
 class Junkie(Mapping[str, Any]):
     def __init__(self, instances_and_factories: Mapping[str, Any] = None):
-        self._mapping = instances_and_factories or {}
+        self._context = instances_and_factories or {}
         self._exit_stack: Optional[ExitStack] = None
 
         self._instances_by_name: dict = {}
         self._instances_by_name_stack: Junkie._Stack = Junkie._Stack()
         self._instances_by_name_stack.push(self._instances_by_name)
 
         self._instantiation_stack: Junkie._InstantiationStack = Junkie._InstantiationStack()
         self._cycle_detection_instance_set = set()
 
-        self._mapping["_junkie"] = self
+        self._context["_junkie"] = self
 
     def __getitem__(self, item):
         return self._instances_by_name[item]
 
     def __setitem__(self, key, value):
         if key in self._instances_by_name:
             raise JunkieError(f'Instance for "{key}" already exists')
-        if key in self._mapping:
+        if key in self._context:
             raise JunkieError(f'Instance for "{key}" already exists in context')
 
         self._instances_by_name[key] = value
 
     def __len__(self) -> int:
         return self._instances_by_name.__len__()
 
@@ -65,15 +65,15 @@
                 yield self._build_instance(names_and_factories[0])
             else:
                 yield self._build_tuple(*names_and_factories)
 
             self._instances_by_name_stack.pop()
             self._instances_by_name = self._instances_by_name_stack.peek()
 
-    def _build_tuple(self, *names_and_factories: Union[str, Callable]) -> Tuple[Any]:
+    def _build_tuple(self, *names_and_factories: Union[str, Callable]) -> Tuple[Any, ...]:
         instances = []
 
         for name_or_factory in names_and_factories:
             instance = self._build_instance(name_or_factory)
             instances.append(instance)
 
         return tuple(instances)
@@ -82,61 +82,54 @@
         if isinstance(name_or_factory, str):
             return self._build_by_instance_name(name_or_factory)
 
         elif callable(name_or_factory):
             return self._build_by_factory_function(name_or_factory, None)
 
         raise JunkieError(
-            f"{self._instantiation_stack}" +
-            f'Unknown type "{name_or_factory}" (str, type or Callable expected)'
+            f"{self._instantiation_stack}" + f'Unknown type "{name_or_factory}" (str, type or Callable expected)'
         )
 
-    def _build_by_instance_name(self, instance_name: str, default=None) -> Any:
+    def _build_by_instance_name(self, instance_name: str) -> Any:
         if instance_name in self._instances_by_name:
             return self._instances_by_name[instance_name]
 
-        if instance_name in self._mapping:
-            value = self._mapping[instance_name]
+        if instance_name in self._context:
+            value = self._context[instance_name]
 
             if callable(value):
                 return self._build_by_factory_function(value, instance_name)
             else:
                 return value
 
-        if default is not None:
-            return default
-
-        raise JunkieError(
-            f"{self._instantiation_stack}" +
-            f'Unable to find "{instance_name}"'
-        )
+        raise JunkieError(f"{self._instantiation_stack}" + f'Unable to find "{instance_name}"')
 
     def _build_by_factory_function(self, factory_function: Callable, instance_name: Union[str, None]) -> Any:
         if factory_function in BUILTINS:
             raise JunkieError(
-                f"{self._instantiation_stack}" +
-                f'Mapping for "{instance_name}" of builtin type "{get_factory_name(factory_function)}" is missing'
+                f"{self._instantiation_stack}"
+                + f'Mapping for "{instance_name}" of builtin type "{get_factory_name(factory_function)}" is missing'
             )
 
         if factory_function in self._cycle_detection_instance_set:
             raise JunkieError(
-                f"{self._instantiation_stack}" +
-                f'Dependency cycle detected with "{get_factory_name(factory_function)}()"'
+                f"{self._instantiation_stack}"
+                + f'Dependency cycle detected with "{get_factory_name(factory_function)}()"'
             )
 
         self._cycle_detection_instance_set.add(factory_function)
         self._instantiation_stack.push(factory_function)
 
-        parameters, args, kwargs = self._build_parameters(factory_function)
+        positional_params, args, keyword_params, kwargs = self._build_parameters(factory_function)
 
         if LOGGER.isEnabledFor(logging.DEBUG):
-            log_params = Junkie._LogParams(*parameters.keys(), *args, **kwargs)
+            log_params = Junkie._LogParams(*positional_params.keys(), *args, **keyword_params, **kwargs)
             LOGGER.debug("%s = %s(%s)", instance_name or "_", get_factory_name(factory_function), log_params)
 
-        instance = factory_function(*parameters.values(), *args, **kwargs)
+        instance = factory_function(*positional_params.values(), *args, **keyword_params, **kwargs)
 
         if hasattr(instance, "__enter__"):
             if LOGGER.isEnabledFor(logging.DEBUG):
                 LOGGER.debug("%s.__enter__()", instance_name or "_")
                 self._exit_stack.push(lambda *exception_details: LOGGER.debug("%s.__exit__()", instance_name or "_"))
 
             instance = self._exit_stack.enter_context(instance)
@@ -146,52 +139,76 @@
 
         self._instantiation_stack.pop()
         self._cycle_detection_instance_set.remove(factory_function)
 
         return instance
 
     def _build_parameters(self, factory_function: Callable) -> (OrderedDict, tuple, dict):
-        parameters = OrderedDict()
+        positional_params = OrderedDict()
         args = ()
+        keyword_params = OrderedDict()
         kwargs = {}
+        positional_params_finished = False
 
         try:
             signature = inspect.signature(factory_function)
         except Exception as e:
             raise JunkieError(
-                f"{self._instantiation_stack}" +
-                f'Unable to inspect signature for "{get_factory_name(factory_function)}()"'
+                f"{self._instantiation_stack}"
+                + f'Unable to inspect signature for "{get_factory_name(factory_function)}()"'
             ) from e
 
         for instance_name, annotation in signature.parameters.items():
-            if annotation.kind is inspect.Parameter.VAR_POSITIONAL:
-                args = self._build_by_instance_name(instance_name, args)
+            if instance_name in self._instances_by_name or instance_name in self._context:
+                value = self._build_by_instance_name(instance_name)
 
-            elif annotation.kind is inspect.Parameter.VAR_KEYWORD:
-                kwargs = self._build_by_instance_name(instance_name, kwargs)
+            # *args
+            elif annotation.kind is inspect.Parameter.VAR_POSITIONAL:
+                continue
 
-            elif instance_name in self._instances_by_name:
-                parameters[instance_name] = self._instances_by_name[instance_name]
-
-            elif instance_name in self._mapping:
-                parameters[instance_name] = self._build_by_instance_name(instance_name)
+            # **kwargs
+            elif annotation.kind is inspect.Parameter.VAR_KEYWORD:
+                continue
 
+            # arg="value"
             elif annotation.default is not inspect.Parameter.empty:
-                parameters[instance_name] = annotation.default
+                positional_params_finished = True
+                continue
 
             elif isinstance(annotation.annotation, Callable) and annotation.annotation != inspect.Parameter.empty:
-                parameters[instance_name] = self._build_by_factory_function(annotation.annotation, instance_name)
+                value = self._build_by_factory_function(annotation.annotation, instance_name)
 
             else:
                 raise JunkieError(
-                    f"{self._instantiation_stack}" +
-                    f'Unable to find "{instance_name}" for "{get_factory_name(factory_function)}()"'
+                    f"{self._instantiation_stack}"
+                    + f'Unable to find "{instance_name}" for "{get_factory_name(factory_function)}()"'
                 )
 
-        return parameters, args, kwargs
+            if annotation.kind is inspect.Parameter.POSITIONAL_ONLY:
+                positional_params[instance_name] = value
+
+            elif annotation.kind is inspect.Parameter.POSITIONAL_OR_KEYWORD:
+                if positional_params_finished:
+                    keyword_params[instance_name] = value
+                else:
+                    positional_params[instance_name] = value
+
+            elif annotation.kind is inspect.Parameter.VAR_POSITIONAL:
+                args = value
+
+            elif annotation.kind is inspect.Parameter.KEYWORD_ONLY:
+                keyword_params[instance_name] = value
+
+            elif annotation.kind is inspect.Parameter.VAR_KEYWORD:
+                kwargs = value
+
+            else:
+                raise NotImplementedError(f'Unknown parameter type "{annotation.kind}"')
+
+        return positional_params, args, keyword_params, kwargs
 
     class _LogParams:
         def __init__(self, *args, **kwargs):
             self.args = args
             self.kwargs = kwargs
 
         def __str__(self):
```

### Comparing `junkie-3.0.0.dev4/test/test_error.py` & `junkie-3.0.1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `junkie-3.0.0.dev4/test/test_dict.py` & `junkie-3.0.1/test/test_dict.py`

 * *Files identical despite different names*

### Comparing `junkie-3.0.0.dev4/test/test_bugfix.py` & `junkie-3.0.1/test/test_bugfix.py`

 * *Files identical despite different names*

### Comparing `junkie-3.0.0.dev4/test/test_junkie.py` & `junkie-3.0.1/test/test_junkie.py`

 * *Files identical despite different names*

### Comparing `junkie-3.0.0.dev4/setup.py` & `junkie-3.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='junkie',
-    version='3.0.0.dev4',
+    version='3.0.1',
     packages=setuptools.find_packages(exclude="test"),
     author='Stefan Richter',
-    description='A dependency injection library for beginners',
+    description='A dependency injection library for beginners and professionals',
     url="https://github.com/sealor/junkie",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

