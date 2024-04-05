# Comparing `tmp/skeletonkey-0.2.0.tar.gz` & `tmp/skeletonkey-0.2.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.2.0.tar", last modified: Fri Oct 20 20:54:50 2023, max compression
+gzip compressed data, was "skeletonkey-0.2.10.tar", last modified: Fri Apr  5 23:05:54 2024, max compression
```

## Comparing `skeletonkey-0.2.0.tar` & `skeletonkey-0.2.10.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 logansizemore  (1000) logansizemore  (1000)        0 2023-10-20 20:54:50.597929 skeletonkey-0.2.0/
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)     1071 2023-10-20 17:23:04.000000 skeletonkey-0.2.0/LICENSE
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)     7530 2023-10-20 20:54:50.597929 skeletonkey-0.2.0/PKG-INFO
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)     7060 2023-10-20 20:44:58.000000 skeletonkey-0.2.0/README.md
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)       38 2023-10-20 20:54:50.597929 skeletonkey-0.2.0/setup.cfg
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)      758 2023-10-20 20:49:58.000000 skeletonkey-0.2.0/setup.py
-drwxrwxr-x   0 logansizemore  (1000) logansizemore  (1000)        0 2023-10-20 20:54:50.597929 skeletonkey-0.2.0/skeletonkey/
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)      598 2023-10-20 17:23:04.000000 skeletonkey-0.2.0/skeletonkey/__init__.py
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)    11895 2023-10-20 20:44:58.000000 skeletonkey-0.2.0/skeletonkey/config.py
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)     6209 2023-10-20 20:44:58.000000 skeletonkey-0.2.0/skeletonkey/core.py
-drwxrwxr-x   0 logansizemore  (1000) logansizemore  (1000)        0 2023-10-20 20:54:50.597929 skeletonkey-0.2.0/skeletonkey.egg-info/
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)     7530 2023-10-20 20:54:50.000000 skeletonkey-0.2.0/skeletonkey.egg-info/PKG-INFO
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)      266 2023-10-20 20:54:50.000000 skeletonkey-0.2.0/skeletonkey.egg-info/SOURCES.txt
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)        1 2023-10-20 20:54:50.000000 skeletonkey-0.2.0/skeletonkey.egg-info/dependency_links.txt
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)       14 2023-10-20 20:54:50.000000 skeletonkey-0.2.0/skeletonkey.egg-info/requires.txt
--rw-rw-r--   0 logansizemore  (1000) logansizemore  (1000)       12 2023-10-20 20:54:50.000000 skeletonkey-0.2.0/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:05:54.721673 skeletonkey-0.2.10/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 23:05:50.000000 skeletonkey-0.2.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-05 23:05:54.717673 skeletonkey-0.2.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-05 23:05:50.000000 skeletonkey-0.2.10/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:05:54.721673 skeletonkey-0.2.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-05 23:05:54.000000 skeletonkey-0.2.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:05:54.717673 skeletonkey-0.2.10/skeletonkey/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-05 23:05:50.000000 skeletonkey-0.2.10/skeletonkey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13651 2024-04-05 23:05:50.000000 skeletonkey-0.2.10/skeletonkey/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-05 23:05:50.000000 skeletonkey-0.2.10/skeletonkey/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:05:54.717673 skeletonkey-0.2.10/skeletonkey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-05 23:05:54.000000 skeletonkey-0.2.10/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 23:05:54.000000 skeletonkey-0.2.10/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:05:54.000000 skeletonkey-0.2.10/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 23:05:54.000000 skeletonkey-0.2.10/skeletonkey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 23:05:54.000000 skeletonkey-0.2.10/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.2.0/LICENSE` & `skeletonkey-0.2.10/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.2.0/PKG-INFO` & `skeletonkey-0.2.10/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,17 @@
-Metadata-Version: 2.1
-Name: skeletonkey
-Version: 0.2.0
-Summary: A bare-bones configuration managment tool.
-Home-page: https://github.com/sizemore0125/skeletonkey
-Author: Logan Sizemore
-Author-email: sizemore0125@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # SkeletonKey: A Bare-bones Configuration Management Tool
+
 <div align="center">
-<img src="./sklogo3.svg" alt="Diagram Description" width="300" >
+<picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./sklogo3.svg">
+    <img alt="SK Logo" src="./sklogo_mono.svg" width="300">
+</picture>
 </div>
 
+
 `skeletonkey` is a simple, lightweight, and flexible configuration management tool that allows you to manage complex configurations for your applications using YAML files. It dynamically loads classes and their arguments at runtime, making it easy to set up and modify your projects.
 
 ## Installation
 
 To install skeletonkey via pip, run the following command:
 
 ```bash
@@ -74,15 +64,15 @@
 
 For instance, if your configuration file has a nested YAML, you can overwrite the default values like this:
 
 ```bash
 python project.py --model.parameters.layer_size 256
 ```
 
-The resulting Namespace object will contain nested Namespace objects that can be accessed using dot notation, such as args.model.parameters.layer_size.
+The resulting Config object will contain nested Config objects that can be accessed using dot notation, such as args.model.parameters.layer_size.
 
 
 #### Defining Flags in Configuration
 
 Flags can be defined in the configuration YAML file using the `?` prefix followed by the flag name. The value of the flag is set as `true` or `false`. Flags allow a user to switch to debug mode without having to modify the configuration file or temporarily enable/disable specific features for testing without changing the configuration.
 
 For example:
@@ -150,15 +140,15 @@
 epochs: 128
 model:
   _target_: MyModel
   layer_size: 128
   activation: relu
 ```
 
-3. When you run your project, `skeletonkey` will merge the default configuration files with the main configuration file, making the values from the default configuration files available in the `args` Namespace object:
+3. When you run your project, `skeletonkey` will merge the default configuration files with the main configuration file, making the values from the default configuration files available in the `args` Config object:
 
 ```python
 print("Learning rate: ", args.learning_rate)
 print("Batch size: ", args.batch_size)
 print("Dropout: ", args.dropout)
 print("Optimizer: ", args.optimizer)
 ```
```

### Comparing `skeletonkey-0.2.0/README.md` & `skeletonkey-0.2.10/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,33 @@
+Metadata-Version: 2.1
+Name: skeletonkey
+Version: 0.2.10
+Summary: A bare-bones configuration managment tool.
+Home-page: https://github.com/sizemore0125/skeletonkey
+Author: Logan Sizemore
+Author-email: sizemore0125@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyYAML>=3.0.0
+
 # SkeletonKey: A Bare-bones Configuration Management Tool
+
 <div align="center">
-<img src="./sklogo3.svg" alt="Diagram Description" width="300" >
+<picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./sklogo3.svg">
+    <img alt="SK Logo" src="./sklogo_mono.svg" width="300">
+</picture>
 </div>
 
+
 `skeletonkey` is a simple, lightweight, and flexible configuration management tool that allows you to manage complex configurations for your applications using YAML files. It dynamically loads classes and their arguments at runtime, making it easy to set up and modify your projects.
 
 ## Installation
 
 To install skeletonkey via pip, run the following command:
 
 ```bash
@@ -59,15 +80,15 @@
 
 For instance, if your configuration file has a nested YAML, you can overwrite the default values like this:
 
 ```bash
 python project.py --model.parameters.layer_size 256
 ```
 
-The resulting Namespace object will contain nested Namespace objects that can be accessed using dot notation, such as args.model.parameters.layer_size.
+The resulting Config object will contain nested Config objects that can be accessed using dot notation, such as args.model.parameters.layer_size.
 
 
 #### Defining Flags in Configuration
 
 Flags can be defined in the configuration YAML file using the `?` prefix followed by the flag name. The value of the flag is set as `true` or `false`. Flags allow a user to switch to debug mode without having to modify the configuration file or temporarily enable/disable specific features for testing without changing the configuration.
 
 For example:
@@ -135,15 +156,15 @@
 epochs: 128
 model:
   _target_: MyModel
   layer_size: 128
   activation: relu
 ```
 
-3. When you run your project, `skeletonkey` will merge the default configuration files with the main configuration file, making the values from the default configuration files available in the `args` Namespace object:
+3. When you run your project, `skeletonkey` will merge the default configuration files with the main configuration file, making the values from the default configuration files available in the `args` Config object:
 
 ```python
 print("Learning rate: ", args.learning_rate)
 print("Batch size: ", args.batch_size)
 print("Dropout: ", args.dropout)
 print("Optimizer: ", args.optimizer)
 ```
```

### Comparing `skeletonkey-0.2.0/setup.py` & `skeletonkey-0.2.10/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version="0.2.0",
+    version='v0.2.10',
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
```

### Comparing `skeletonkey-0.2.0/skeletonkey/__init__.py` & `skeletonkey-0.2.10/skeletonkey/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 and an instantiate funtion that can dynamically instantiate classes with their configurations. 
 It facilitates the management of complex configurations for applications using YAML files and enables 
 the dynamic loading of classes and their arguments at runtime.
 """
 
 __version__ = "0.0.11"
 
-from .core import unlock, instantiate, instantiate_all
+from .core import unlock, instantiate, instantiate_all, Config
 
 # Names to import with wildcard import
-__all__ = ["unlock", "instantiate", "instantiate_all"]
+__all__ = ["unlock", "instantiate", "instantiate_all", "Config"]
```

### Comparing `skeletonkey-0.2.0/skeletonkey/config.py` & `skeletonkey-0.2.10/skeletonkey/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,90 @@
 
 import argparse
 import os
 from typing import List
 
 import yaml
 
+BASE_DEFAULT_KEYWORD: str = "defaults"
+BASE_COLLECTION_KEYWORD: str = "keyring"
+
+class Config():
+    def __init__(self, *args, **kwargs):
+        """
+        Initializes the config from a dictionary or from kwargs.\n
+
+        Args:
+            Either a single dictionary as an arg or suply a number of kwargs.
+        """
+
+        if (len(args) != 0) and (len(kwargs) != 0):
+            raise ValueError("Config should not receive args and kwargs at the same time.")
+        
+        elif not (len(args) == 0 or len(args) == 1):
+            raise ValueError("Config should not receive more than one non-keyword argument.")
+
+
+        if len(args) == 1:
+            if not isinstance(args[0], dict):
+                raise ValueError("Supplied arg must be a dictionary")
+            self._init_from_dict(args[0])
+        else:
+            self._init_from_dict(kwargs)
+
+
+    def _init_from_dict(self, dictionary: dict):
+        """
+        Initialize the config from a dictionary
+
+        Args:
+            dictionary (dict): The dictionary to be converted.
+        """
+        for key, value in dictionary.items():
+            if isinstance(value, dict):
+                value = Config(value)
+       
+            self[key] = value
+
+    def __getitem__(self, key:str):
+        return self.__getattribute__(key)
+
+    def __setitem__(self, key: str, value):
+        self.__setattr__(key, value)
+
+
+    def __delitem__(self, key: str):
+        self.__delattr__()
+
+    def __str__(self):
+        return self._subconfig_str(self, 0)[1:]
+
+    def __repr__(self):
+        return f"Config({self._subconfig_str(self, 1)})"
+
+    def _subconfig_str(self, subspace: "Config", tab_depth:int):
+        """
+        Convert a given subconfig to a string with the given tab-depth
+        
+        args:
+            subspace: A Config object
+            tab_depth: an integer representing the current tab depth
+        """
+        s = ""
+        for k, v in subspace.__dict__.items():
+            s += "\n" + "  "*tab_depth + k + ": "
+            
+            if isinstance(v, Config):
+                s+= "\n"
+                s+= self._subconfig_str(v, tab_depth+1)[1:] # [1:] gets rid of uneccesary leading \n
+            else:
+                s += str(v)
+
+        return s
+
 
 def find_yaml_path(file_path: str) -> str:
     """
     Given a file path, this function checks if a YAML file exists with either
     '.yml' or '.yaml' extension, and returns the correct path.
 
     Args:
@@ -167,15 +243,15 @@
     default_yaml = add_yaml_extension(default_yaml)
     default_config_path = os.path.join(config_path, default_yaml)
     default_config = open_yaml(default_config_path)
     return default_config
 
 
 def load_yaml_config(
-    config_path: str, config_name: str, default_keyword: str = "defaults", collection_keyword: str = "keyring"
+    config_path: str, config_name: str, default_keyword: str = BASE_DEFAULT_KEYWORD, collection_keyword: str = BASE_COLLECTION_KEYWORD
 ) -> dict:
     """
     Load a YAML configuration file and update it with default configurations.
 
     Args:
         config_path (str): The file path to the YAML configuration file.
         config_name (str): The name of the YAML configuration file.
@@ -245,28 +321,28 @@
                 subconfig = get_default_args_from_path(config_path, collection_entry)
                 config[collection_key] = subconfig
 
         del config[collection_keyword]
 
 
 def add_args_from_dict(
-    arg_parser: argparse.ArgumentParser, config: dict, prefix=""
+    arg_parser: argparse.ArgumentParser, config_dict: dict, prefix=""
 ) -> None:
     """
     Add arguments to an ArgumentParser instance using key-value pairs from a
     configuration dictionary. If the dictionary contains a nested dictionary, the
     argument will be added as --key.key value.
     Args:
         arg_parser (argparse.ArgumentParser): The ArgumentParser instance to which
                                               arguments will be added.
         config (dict): A dictionary containing key-value pairs representing
                        the arguments and their default values.
         prefix (str, optional): The prefix string for nested keys. Defaults to ''.
     """
-    for key, value in config.items():
+    for key, value in config_dict.items():
         if isinstance(value, dict):
             add_args_from_dict(arg_parser, value, f"{prefix}{key}.")
         else:
             if key.startswith("$"):
                 if key[1:] in os.environ:
                     value = os.environ[key[1:]]
                 arg_parser.add_argument(
@@ -278,44 +354,28 @@
                 )
             else:
                 arg_parser.add_argument(
                     f"--{prefix}{key}", default=value, type=type(value)
                 )
 
 
-def dict_to_namespace(dictionary: dict) -> argparse.Namespace:
-    """
-    Convert a dictionary to an argparse.Namespace object recursively.
-
-    Args:
-        dictionary (dict): The dictionary to be converted.
-
-    Returns:
-        argparse.Namespace: A Namespace object representing the input dictionary.
-    """
-    for key, value in dictionary.items():
-        if isinstance(value, dict):
-            dictionary[key] = dict_to_namespace(value)
-    return argparse.Namespace(**dictionary)
-
-
-def namespace_to_nested_namespace(namespace: argparse.Namespace) -> argparse.Namespace:
+def config_to_nested_config(config: Config) -> Config:
     """
-    Convert an argparse.Namespace object with 'key1.keyn' formatted keys into a nested Namespace object.
+    Convert an Config object with 'key1.keyn' formatted keys into a nested Config object.
 
     Args:
-        namespace (argparse.Namespace): The Namespace object to be converted.
+        config (Config): The Config object to be converted.
 
     Returns:
-        argparse.Namespace: A nested Namespace representation of the input Namespace object.
+        Config: A nested Config representation of the input Config object.
     """
     nested_dict = {}
-    for key, value in vars(namespace).items():
+    for key, value in vars(config).items():
         keys = key.split(".")
         current_dict = nested_dict
         for sub_key in keys[:-1]:
             if sub_key not in current_dict:
                 current_dict[sub_key] = {}
             current_dict = current_dict[sub_key]
         current_dict[keys[-1]] = value
 
-    return dict_to_namespace(nested_dict)
+    return Config(nested_dict)
```

### Comparing `skeletonkey-0.2.0/skeletonkey/core.py` & `skeletonkey-0.2.10/skeletonkey/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import sys
 from typing import Callable, Optional, Type, Any, Tuple
 
 from .config import (
     load_yaml_config,
     add_args_from_dict,
     add_yaml_extension,
-    namespace_to_nested_namespace,
+    config_to_nested_config,
+    Config
 )
 
+TARGET_KEYWORD: str = "_target_"
 
 def get_config_dir_path(config_path: str) -> str:
     """
     Convert a given relative or absolute config file path to its absolute directory path.
 
     Args:
         config_path (str): The path to the configuration file. Can be either relative or absolute.
@@ -69,15 +71,15 @@
 
     def _parse_config(main: Callable):
         @functools.wraps(main)
         def _inner_function():
             parser = argparse.ArgumentParser()
             add_args_from_dict(parser, config)
             args = parser.parse_args()
-            args = namespace_to_nested_namespace(args)
+            args = config_to_nested_config(args)
             return main(args)
 
         return _inner_function
 
     return _parse_config
 
 
@@ -97,36 +99,40 @@
     module_name = ".".join(parts[:-1])
     class_name = parts[-1]
     module = __import__(module_name, fromlist=[class_name])
     class_obj = getattr(module, class_name)
     return class_obj
 
 
-def instantiate(namespace: argparse.Namespace, **kwargs) -> Any:
+def instantiate(config: Config, target_keyword=TARGET_KEYWORD, _instantiate_recursive=True, **kwargs) -> Any:
     """
-    Instantiate a class object using a Namespace object.
-    The Namespace object should contain the key "_target_" to
+    Instantiate a class object using a Config object.
+    The Config object should contain the key "_target_" to
     specify the class to instantiate.
 
     Args:
-        namespace (argparse.Namespace): A Namespace object containing the key "_target_"
+        config (Config): A Config object containing the key "_target_"
             to specify the class, along with any additional keyword
             arguments for the class.
 
     Returns:
         Any: An instance of the specified class.
 
     Raises:
         TypeError: If the class is missing specific parameters.
     """
-    obj_kwargs = vars(namespace).copy()
-    target_keyword = "_target_"
+    obj_kwargs = vars(config).copy()
     class_obj = import_class(obj_kwargs[target_keyword])
     del obj_kwargs[target_keyword]
 
+    if _instantiate_recursive:
+        for k, v in obj_kwargs.items():
+            if isinstance(v, Config) and (target_keyword in vars(v)):
+                obj_kwargs[k] = instantiate(v)
+
     obj_kwargs.update(kwargs)
 
     obj_parameters = inspect.signature(class_obj).parameters
     required_parameters = [
         param_name for param_name, param in obj_parameters.items()
         if param.default == param.empty and param.kind != inspect.Parameter.VAR_KEYWORD
     ]
@@ -137,37 +143,37 @@
         raise TypeError(
             f"missing {len(missing_parameters)} required positional(s) argument: {', '.join(missing_parameters)}."
             + " Add it to your config or as a keyword argument to skeletonkey.instantiate()."
         )
     
     return class_obj(**obj_kwargs)
 
-def instantiate_all(namespace: argparse.Namespace, **kwargs) -> Tuple[Any]:
+def instantiate_all(config: Config, target_keyword=TARGET_KEYWORD, **kwargs) -> Tuple[Any]:
     """
-    Instantiate a tuple of class objects using a Namespace object.
-    The Namespace object should contain other Namespace objects where the key 
+    Instantiate a tuple of class objects using a Config object.
+    The Config object should contain other Config objects where the key 
     "_target_" is at the top level, which specifies the class to instantiate.
 
     Args:
-        namespace (argparse.Namespace): A Namespace object containing the key "_target_"
+        config (Config): A Config object containing the key "_target_"
             to specify the class , along with any additional keyword arguments for the class.
 
     Returns:
         Tuple[Any]: An tuple of instances of the specified class.
 
     Raises:
         ValueError: If any subconfig does not have "_target_" key.
     """
-    collection_dict = vars(namespace).copy()
+    collection_dict = vars(config).copy()
 
     objects = []
 
     for obj_key in collection_dict.keys():
         obj_namespace = collection_dict[obj_key]
 
-        if not hasattr(obj_namespace, "_target_"):
+        if not hasattr(obj_namespace, target_keyword):
             raise ValueError(f"subconfig ({obj_key}) in collection does not have '_target_' key at the top level.")
         
         obj = instantiate(obj_namespace, **kwargs)
         objects.append(obj)
     
     return tuple(objects)
```

### Comparing `skeletonkey-0.2.0/skeletonkey.egg-info/PKG-INFO` & `skeletonkey-0.2.10/skeletonkey.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.2.0
+Version: 0.2.10
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pyYAML>=3.0.0
 
 # SkeletonKey: A Bare-bones Configuration Management Tool
+
 <div align="center">
-<img src="./sklogo3.svg" alt="Diagram Description" width="300" >
+<picture>
+    <source media="(prefers-color-scheme: dark)" srcset="./sklogo3.svg">
+    <img alt="SK Logo" src="./sklogo_mono.svg" width="300">
+</picture>
 </div>
 
+
 `skeletonkey` is a simple, lightweight, and flexible configuration management tool that allows you to manage complex configurations for your applications using YAML files. It dynamically loads classes and their arguments at runtime, making it easy to set up and modify your projects.
 
 ## Installation
 
 To install skeletonkey via pip, run the following command:
 
 ```bash
@@ -74,15 +80,15 @@
 
 For instance, if your configuration file has a nested YAML, you can overwrite the default values like this:
 
 ```bash
 python project.py --model.parameters.layer_size 256
 ```
 
-The resulting Namespace object will contain nested Namespace objects that can be accessed using dot notation, such as args.model.parameters.layer_size.
+The resulting Config object will contain nested Config objects that can be accessed using dot notation, such as args.model.parameters.layer_size.
 
 
 #### Defining Flags in Configuration
 
 Flags can be defined in the configuration YAML file using the `?` prefix followed by the flag name. The value of the flag is set as `true` or `false`. Flags allow a user to switch to debug mode without having to modify the configuration file or temporarily enable/disable specific features for testing without changing the configuration.
 
 For example:
@@ -150,15 +156,15 @@
 epochs: 128
 model:
   _target_: MyModel
   layer_size: 128
   activation: relu
 ```
 
-3. When you run your project, `skeletonkey` will merge the default configuration files with the main configuration file, making the values from the default configuration files available in the `args` Namespace object:
+3. When you run your project, `skeletonkey` will merge the default configuration files with the main configuration file, making the values from the default configuration files available in the `args` Config object:
 
 ```python
 print("Learning rate: ", args.learning_rate)
 print("Batch size: ", args.batch_size)
 print("Dropout: ", args.dropout)
 print("Optimizer: ", args.optimizer)
 ```
```

