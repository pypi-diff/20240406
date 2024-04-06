# Comparing `tmp/Liara-2.5.4.tar.gz` & `tmp/Liara-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Liara-2.5.4.tar", last modified: Sun Apr 16 12:43:42 2023, max compression
+gzip compressed data, was "Liara-2.6.0.tar", last modified: Sat Apr  6 18:43:08 2024, max compression
```

## Comparing `Liara-2.5.4.tar` & `Liara-2.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1332 2023-01-02 13:55:30.000000 Liara-2.5.4/LICENSE.txt
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/Liara.egg-info/
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/PKG-INFO
--rw-r--r--   0 anteru    (1000) anteru    (1000)      729 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/SOURCES.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)        1 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/dependency_links.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)       45 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/entry_points.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)      376 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/requires.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)        6 2023-04-16 12:43:42.000000 Liara-2.5.4/Liara.egg-info/top_level.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-16 12:43:42.778083 Liara-2.5.4/PKG-INFO
--rw-r--r--   0 anteru    (1000) anteru    (1000)      441 2023-01-01 11:59:39.000000 Liara-2.5.4/README.md
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/liara/
--rwxr-xr-x   0 anteru    (1000) anteru    (1000)    29291 2023-04-16 12:43:28.000000 Liara-2.5.4/liara/__init__.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4975 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/actions.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     9328 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/cache.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    10367 2023-04-15 11:41:10.000000 Liara-2.5.4/liara/cmdline.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2675 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/config.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4540 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/feeds.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    12471 2023-04-16 12:43:28.000000 Liara-2.5.4/liara/md.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    32036 2023-04-16 12:43:28.000000 Liara-2.5.4/liara/nodes.py
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/liara/plugins/
--rw-r--r--   0 anteru    (1000) anteru    (1000)      132 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/plugins/__init__.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      889 2023-04-15 11:41:10.000000 Liara-2.5.4/liara/plugins/has_pending_document.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1326 2023-04-15 11:41:10.000000 Liara-2.5.4/liara/plugins/series_schedule.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     5349 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/publish.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     8046 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/query.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    11574 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/quickstart.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     5236 2023-01-22 13:57:52.000000 Liara-2.5.4/liara/server.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1953 2023-02-11 11:15:23.000000 Liara-2.5.4/liara/signals.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    28210 2023-04-15 11:41:10.000000 Liara-2.5.4/liara/site.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    11215 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/template.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4116 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/util.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      888 2023-01-01 11:59:39.000000 Liara-2.5.4/liara/yaml.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      190 2023-01-01 11:59:39.000000 Liara-2.5.4/pyproject.toml
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1457 2023-04-16 12:43:42.778083 Liara-2.5.4/setup.cfg
--rw-r--r--   0 anteru    (1000) anteru    (1000)       38 2023-01-01 11:59:39.000000 Liara-2.5.4/setup.py
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 12:43:42.778083 Liara-2.5.4/test/
--rw-r--r--   0 anteru    (1000) anteru    (1000)      141 2023-01-01 11:59:39.000000 Liara-2.5.4/test/test_cache.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     3708 2023-04-16 11:43:18.000000 Liara-2.5.4/test/test_md.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1363 2023-02-11 11:15:23.000000 Liara-2.5.4/test/test_nodes.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2498 2023-02-11 11:15:23.000000 Liara-2.5.4/test/test_query.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     6064 2023-01-01 11:59:39.000000 Liara-2.5.4/test/test_site.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2391 2023-01-01 11:59:39.000000 Liara-2.5.4/test/test_template.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1031 2023-01-01 11:59:39.000000 Liara-2.5.4/test/test_util.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2024-04-06 18:43:08.492517 Liara-2.6.0/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1332 2024-04-06 18:42:49.000000 Liara-2.6.0/LICENSE.txt
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2024-04-06 18:43:08.492517 Liara-2.6.0/Liara.egg-info/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2176 2024-04-06 18:43:08.000000 Liara-2.6.0/Liara.egg-info/PKG-INFO
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      729 2024-04-06 18:43:08.000000 Liara-2.6.0/Liara.egg-info/SOURCES.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)        1 2024-04-06 18:43:08.000000 Liara-2.6.0/Liara.egg-info/dependency_links.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)       45 2024-04-06 18:43:08.000000 Liara-2.6.0/Liara.egg-info/entry_points.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      381 2024-04-06 18:43:08.000000 Liara-2.6.0/Liara.egg-info/requires.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)        6 2024-04-06 18:43:08.000000 Liara-2.6.0/Liara.egg-info/top_level.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2176 2024-04-06 18:43:08.492517 Liara-2.6.0/PKG-INFO
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      441 2023-01-01 11:59:39.000000 Liara-2.6.0/README.md
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2024-04-06 18:43:08.482517 Liara-2.6.0/liara/
+-rwxr-xr-x   0 anteru    (1000) anteru    (1000)    29580 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/__init__.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5067 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/actions.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     9326 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/cache.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    10600 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/cmdline.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2675 2023-02-11 11:15:23.000000 Liara-2.6.0/liara/config.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4655 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/feeds.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    13195 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/md.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    32361 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/nodes.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2024-04-06 18:43:08.482517 Liara-2.6.0/liara/plugins/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      132 2023-01-01 11:59:39.000000 Liara-2.6.0/liara/plugins/__init__.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      889 2023-04-15 11:41:10.000000 Liara-2.6.0/liara/plugins/has_pending_document.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1326 2023-04-15 11:41:10.000000 Liara-2.6.0/liara/plugins/series_schedule.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5403 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/publish.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     8045 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/query.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    11574 2023-01-01 11:59:39.000000 Liara-2.6.0/liara/quickstart.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5680 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/server.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1953 2023-02-11 11:15:23.000000 Liara-2.6.0/liara/signals.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    28238 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/site.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    11267 2024-04-06 18:42:49.000000 Liara-2.6.0/liara/template.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4116 2023-01-01 11:59:39.000000 Liara-2.6.0/liara/util.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      888 2023-01-01 11:59:39.000000 Liara-2.6.0/liara/yaml.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      190 2023-01-01 11:59:39.000000 Liara-2.6.0/pyproject.toml
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1426 2024-04-06 18:43:08.492517 Liara-2.6.0/setup.cfg
+-rw-r--r--   0 anteru    (1000) anteru    (1000)       38 2023-01-01 11:59:39.000000 Liara-2.6.0/setup.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2024-04-06 18:43:08.492517 Liara-2.6.0/test/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      409 2024-04-06 18:42:49.000000 Liara-2.6.0/test/test_cache.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4037 2024-04-06 18:42:49.000000 Liara-2.6.0/test/test_md.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1363 2023-02-11 11:15:23.000000 Liara-2.6.0/test/test_nodes.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2498 2023-02-11 11:15:23.000000 Liara-2.6.0/test/test_query.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     6287 2024-04-06 18:42:49.000000 Liara-2.6.0/test/test_site.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2413 2024-04-06 18:42:49.000000 Liara-2.6.0/test/test_template.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1031 2023-01-01 11:59:39.000000 Liara-2.6.0/test/test_util.py
```

### Comparing `Liara-2.5.4/LICENSE.txt` & `Liara-2.6.0/LICENSE.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2012-2023 Matthäus G. Chajdas
+Copyright (c) 2012-2024 Matthäus G. Chajdas
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `Liara-2.5.4/Liara.egg-info/SOURCES.txt` & `Liara-2.6.0/Liara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/liara/__init__.py` & `Liara-2.6.0/liara/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import time
 import multiprocessing
 
 from typing import (
         IO,
         ChainMap,
         List,
-        Callable,
         Dict,
         Optional,
         Text,
         Union,
     )
 
 import collections
@@ -30,15 +29,15 @@
     _process_node_sync
 )
 
 from .cache import Cache, FilesystemCache, NullCache, Sqlite3Cache, RedisCache
 from .util import FilesystemWalker, flatten_dictionary
 from .yaml import load_yaml
 
-__version__ = '2.5.4'
+__version__ = '2.6.0'
 __all__ = [
     'actions',
     'cache',
     'cmdline',
     'config',
     'feeds',
     'md',
@@ -79,31 +78,30 @@
 def _process_resource_task(t):
     return t.process()
 
 
 def _setup_multiprocessing_worker(log_level):
     from .cmdline import _setup_logging
     if log_level == logging.DEBUG:
-        _setup_logging(True, False)
+        _setup_logging(debug=True, verbose=False)
     elif log_level == logging.INFO:
-        _setup_logging(False, True)
+        _setup_logging(debug=False, verbose=True)
     else:
-        _setup_logging(False, False)
+        _setup_logging(debug=False, verbose=False)
 
 
 class Liara:
     """Main entry point for Liara. This class handles all the state required
     to process and build a site."""
     __site: Site
     __resource_node_factory: ResourceNodeFactory
     __document_node_factory: DocumentNodeFactory
     __redirections: List[Dict[str, str]]
     __log = logging.getLogger('liara')
     __cache: Cache
-    __document_post_processors: List[Callable]
     # When running using 'serve', this will be set to the local URL
     __base_url_override: Optional[str] = None
     __registered_plugins: Dict[object, object] = dict()
     __filesystem_walker: FilesystemWalker
     __template_repository: TemplateRepository
 
     def __init__(self,
@@ -121,15 +119,15 @@
         if configuration is None:
             project_configuration = {}
         elif isinstance(configuration, str):
             project_configuration = load_yaml(open(configuration))
         else:
             project_configuration = load_yaml(configuration)
 
-        # It's none of the YAML file is empty, for instance, when creating a
+        # It's none if the YAML file is empty, for instance, when creating a
         # new site from scratch. In this case, set it to an empty dict as
         # flatten_dictionary cannot handle None
         if project_configuration is None:
             project_configuration = dict()
 
         ignore_list = {
             'content.markdown.extensions',
@@ -168,35 +166,35 @@
 
         template_configuration = pathlib.Path(self.__configuration['template'])
         self.__setup_template_backend(template_configuration)
 
         self.__setup_content_filters(self.__configuration['content.filters'])
 
     @classmethod
-    def setup_plugins(self) -> None:
+    def setup_plugins(cls) -> None:
         import liara.plugins
         import pkgutil
         import importlib
 
         def iter_namespace(ns_pkg):
             return pkgutil.iter_modules(ns_pkg.__path__, ns_pkg.__name__ + ".")
 
         plugins = {
             name: importlib.import_module(name)
             for _, name, _ in iter_namespace(liara.plugins)
         }
 
         for name, module in plugins.items():
-            if name in self.__registered_plugins:
+            if name in cls.__registered_plugins:
                 continue
 
-            self.__log.debug(f'Initializing plugin: {name}')
+            cls.__log.debug(f'Initializing plugin: {name}')
             assert hasattr(module, 'register')
             module.register()
-            self.__registered_plugins[name] = module
+            cls.__registered_plugins[name] = module
 
     def __setup_cache(self) -> None:
         # Deprecated since version 2.2
         cache_directory = self.__configuration.get('build.cache_directory')
         if cache_directory:
             self.__log.warning(
                 "'build.cache_directory' is deprecated. Please "
@@ -213,39 +211,42 @@
         # Official value since 2.2
         if cache_type is None:
             # We need to check first because this is part of the default
             # config and it would overwrite the user setting if they were using
             # the deprecated value
             cache_type = self.__configuration.get('build.cache.type')
 
-        if cache_type == 'db':
-            self.__log.debug('Using Sqlite3Cache')
-            dir = self.__configuration.get('build.cache.db.directory')
-            if dir and cache_directory is None:
-                cache_directory = pathlib.Path(dir)
-            self.__cache = Sqlite3Cache(cache_directory)
-        elif cache_type == 'fs':
-            self.__log.debug('Using FilesystemCache')
-            dir = self.__configuration.get('build.cache.fs.directory')
-            if dir and cache_directory is None:
-                cache_directory = pathlib.Path(dir)
-            self.__cache = FilesystemCache(cache_directory)
-        elif cache_type == 'redis':
-            self.__log.debug('Using RedisCache')
-            self.__cache = RedisCache(
-                self.__configuration['build.cache.redis.host'],
-                self.__configuration['build.cache.redis.port'],
-                self.__configuration['build.cache.redis.db'],
-                datetime.timedelta(minutes=self.__configuration[
-                    'build.cache.redis.expiration_time'])
-            )
-        elif cache_type == 'none':
-            self.__log.debug('Not using any cache')
-        else:
-            self.__log.warning('No cache backend configured')
+        match cache_type:
+            case 'db':
+                self.__log.debug('Using Sqlite3Cache')
+                dir = self.__configuration.get('build.cache.db.directory')
+                if dir and cache_directory is None:
+                    cache_directory = pathlib.Path(dir)
+                assert cache_directory
+                self.__cache = Sqlite3Cache(cache_directory)
+            case 'fs':
+                self.__log.debug('Using FilesystemCache')
+                dir = self.__configuration.get('build.cache.fs.directory')
+                if dir and cache_directory is None:
+                    cache_directory = pathlib.Path(dir)
+                assert cache_directory
+                self.__cache = FilesystemCache(cache_directory)
+            case 'redis':
+                self.__log.debug('Using RedisCache')
+                self.__cache = RedisCache(
+                    self.__configuration['build.cache.redis.host'],
+                    self.__configuration['build.cache.redis.port'],
+                    self.__configuration['build.cache.redis.db'],
+                    datetime.timedelta(minutes=self.__configuration[
+                        'build.cache.redis.expiration_time'])
+                )
+            case 'none':
+                self.__log.debug('Not using any cache')
+            case _:
+                self.__log.warning('No cache backend configured')
 
     def __setup_content_filters(self, filters: List[str]) -> None:
         content_filter_factory = ContentFilterFactory()
         for f in filters:
             self.__site.register_content_filter(
                 content_filter_factory.create_filter(f)
             )
@@ -489,35 +490,36 @@
                 if metadata_path.exists():
                     node = resource_factory.create_node(src.suffix, src, path,
                                                         metadata_path)
                 else:
                     node = resource_factory.create_node(src.suffix, src, path)
                 site.add_resource(node)
 
-    def __discover_feeds(self, site: Site, feeds: pathlib.Path) -> None:
+    def __discover_feeds(self, site: Site, feed_definition: pathlib.Path) -> None:
         from .feeds import JsonFeedNode, RSSFeedNode, SitemapXmlFeedNode
 
-        if not feeds.exists():
+        if not feed_definition.exists():
             return
 
-        for key, options in load_yaml(feeds.open()).items():
+        for key, options in load_yaml(feed_definition.open()).items():
             path = pathlib.PurePosixPath(options['path'])
             del options['path']
 
-            if key == 'rss':
-                feed = RSSFeedNode(path, site, **options)
-                site.add_generated(feed)
-            elif key == 'json':
-                feed = JsonFeedNode(path, site, **options)
-                site.add_generated(feed)
-            elif key == 'sitemap':
-                feed = SitemapXmlFeedNode(path, site, **options)
-                site.add_generated(feed)
-            else:
-                self.__log.warning(f'Unknown feed type: "{key}", ignored')
+            match key:
+                case 'rss':
+                    feed = RSSFeedNode(path, site, **options)
+                    site.add_generated(feed)
+                case 'json':
+                    feed = JsonFeedNode(path, site, **options)
+                    site.add_generated(feed)
+                case 'sitemap':
+                    feed = SitemapXmlFeedNode(path, site, **options)
+                    site.add_generated(feed)
+                case _:
+                    self.__log.warning(f'Unknown feed type: "{key}", ignored')
 
     def __discover_metadata(self, site: Site, metadata: pathlib.Path) -> None:
         if not metadata.exists():
             return
 
         site.set_metadata(load_yaml(metadata.open()))
 
@@ -733,23 +735,28 @@
             module = self._load_module(plugin)
             if hasattr(module, 'register'):
                 module.register()
                 # Keep it around to prevent garbage collection
                 self.__registered_plugins[plugin] = module
 
     def _load_module(self, path, name=''):
-        import importlib
+        import importlib.util
         self.__log.debug(f'Initializing plugin from module: "{path}"')
         # Prevent modules from being loaded twice
         if module := self.__registered_plugins.get(path):
             self.__log.debug(f'Module "{path}" already registered, skipping')
             return module
 
         if not name:
             name = path.stem
         spec = importlib.util.spec_from_file_location(name, path)
+        assert spec
+        assert spec.loader
+        
         module = importlib.util.module_from_spec(spec)
+        assert module
+
         spec.loader.exec_module(module)
         return module
 
     def _get_cache(self) -> Cache:
         return self.__cache
```

### Comparing `Liara-2.5.4/liara/actions.py` & `Liara-2.6.0/liara/actions.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 
 def _extract_links(document: DocumentNode):
     """Extract all links from ``<a>`` and ``<img>`` tags in a document.
 
     This assumes the document has been already processed into valid Html.
     """
     from bs4 import BeautifulSoup
+    assert document.content
     soup = BeautifulSoup(document.content, 'lxml')
 
     for item in soup.find_all(['img', 'a']):
+        target = None
+
         if item.name == 'img':
             target = item.attrs.get('src', None)
         elif item.name == 'a':
             target = item.attrs.get('href', None)
 
         if target and not target.startswith('#'):
             yield target
@@ -100,14 +103,16 @@
     import requests
     try:
         ok = False
 
         if url.startswith('mailto'):
             return (True, url, None,)
 
+        error = 'Unknown error'
+        
         try:
             r = requests.get(url, timeout=5)
             if r.status_code == 200:
                 ok = True
             else:
                 error = f'got {r.status_code}, expected 200'
         except requests.exceptions.ConnectTimeout:
```

### Comparing `Liara-2.5.4/liara/cache.py` & `Liara-2.6.0/liara/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 @dataclass
 class CacheInfo:
     """Information about a cache. Note that the information can be approximated
     as getting the exact numbers may be costly."""
 
     size: int = 0
-    """Approximate number of objects stored in the cache."""
+    """Approximate number of bytes stored in the cache."""
 
     entry_count: int = 0
     """Approximate number of objects stored in the cache."""
 
     name: str = ""
     """A human-friendly name for this cache."""
 
@@ -230,15 +230,15 @@
         self.__index = {}
 
     def inspect(self):
         import sys
         size = sys.getsizeof(self.__index)
 
         size += sum([sys.getsizeof(k) + sys.getsizeof(v)
-                     for k, v in self.__index.value()])
+                     for k, v in self.__index.items()])
 
         count = len(self.__index)
 
         return CacheInfo(size, count, 'In-Memory')
 
 
 class RedisCache(Cache):
```

### Comparing `Liara-2.5.4/liara/cmdline.py` & `Liara-2.6.0/liara/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,32 +9,34 @@
 
 
 class Environment:
     """The command line environment.
 
     This provides access to global variables that are useful for command line
     commands, as well as a global liara instance."""
+    __liara : Liara | None
+
     def __init__(self):
         self.verbose = False
         self.debug = False
         self.config = None
         self.__liara = None
         self.log = logging.getLogger('liara.cmdline')
 
     @property
-    def liara(self):
+    def liara(self) -> Liara:
         if not self.__liara:
             self.__liara = _create_liara(self.config)
         return self.__liara
 
 
 pass_environment = click.make_pass_decorator(Environment, ensure=True)
 
 
-def _setup_logging(debug, verbose):
+def _setup_logging(*, debug: bool, verbose: bool):
     if debug:
         logging.basicConfig(
             level=logging.DEBUG,
             format='%(asctime)s %(levelname)-7s %(name)s %(message)s')
         # Unfortunately PIL writes a lot of debug output, so we're disabling it
         # manually here to make debug output useful
         # This doesn't remove critical debug output -- PIL writes things like
@@ -57,21 +59,25 @@
 @click.option('--debug/--no-debug', default=False, help='Enable debug output.')
 @click.option('--verbose', is_flag=True, help='Enable verbose output.')
 @click.option('--config', default='config.yaml', type=click.Path(),
               help='Set the path to the configuration file.')
 @click.option('--date', default=None, help='Override the current date.')
 @click.version_option()
 @pass_environment
-def cli(env, debug, verbose, config, date):
-    _setup_logging(debug, verbose)
+def cli(env, debug: bool, verbose: bool, config, date: str):
+    _setup_logging(debug=debug, verbose=verbose)
 
     if date:
         from .util import set_local_now
         import dateparser
-        set_local_now(dateparser.parse(date))
+        now = dateparser.parse(date)
+        if now:
+            set_local_now(now)
+        else:
+            env.log.error(f'Could not parse date {date}, ignoring it for this build')
 
     env.config = config
 
 
 def main():
     from .signals import commandline_prepared
 
@@ -92,15 +98,15 @@
 @click.option('--profile-file', type=click.Path(writable=True),
               default='build.prof')
 @click.option('--cache/--no-cache', default=True,
               help='Enable or disable the configured cache')
 @click.option('--parallel/--no-parallel', default=True,
               help='Enable or disable parallel processing.')
 @pass_environment
-def build(env, profile, profile_file, cache, parallel):
+def build(env, profile, profile_file, cache: bool, parallel: bool):
     """Build a site."""
     if profile:
         pr = cProfile.Profile()
         pr.enable()
     env.liara.build(disable_cache=not cache,
                     parallel_build=parallel)
     if profile:
```

### Comparing `Liara-2.5.4/liara/config.py` & `Liara-2.6.0/liara/config.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/liara/feeds.py` & `Liara-2.6.0/liara/feeds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .nodes import GeneratedNode, NodeKind
+from .nodes import GeneratedNode, NodeKind, DocumentNode
 from .site import Site
 from . import __version__
 from .util import local_now
 import datetime
 import email.utils
 
 
@@ -46,14 +46,15 @@
             E.language(meta['language']),
             E.copyright(meta['copyright']),
             E.lastBuildDate(email.utils.format_datetime(
                 local_now())),
         )
 
         for item in items:
+            assert isinstance(item, DocumentNode)
             e = E.item(
                 E.title(item.metadata['title']),
                 E.link(meta['base_url'] + str(item.path)),
                 E.pubDate(email.utils.format_datetime(item.metadata['date'])),
                 E.guid(meta['base_url'] + str(item.path)),
                 E.description(item.content)
             )
@@ -85,14 +86,15 @@
             'home_page_url': meta['base_url'],
             'feed_url': meta['base_url'] + str(self.path),
             'description': meta['description']
         }
 
         result_items = []
         for item in items:
+            assert isinstance(item, DocumentNode)
             result_items.append({
                 'id': meta['base_url'] + str(item.path),
                 'title': item.metadata['title'],
                 'date_published': item.metadata['date'].isoformat('T'),
                 'url': meta['base_url'] + str(item.path),
                 'content_html': item.content
             })
@@ -128,12 +130,13 @@
             url = E.url()
             url.append(E.loc(metadata['base_url'] + str(node.path)))
 
             if 'date' in node.metadata:
                 url.append(E.lastmod(node.metadata['date'].isoformat()))
             else:
                 url.append(E.lastmod(now.isoformat()))
+
             if node.kind == NodeKind.Index:
                 # This is machine generated, so reduce priority
                 url.append(E.priority('0'))
             urlset.append(url)
         self.content = etree.tostring(urlset)
```

### Comparing `Liara-2.5.4/liara/md.py` & `Liara-2.6.0/liara/md.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from markdown.extensions import Extension
 from markdown.treeprocessors import Treeprocessor
 from markdown.preprocessors import Preprocessor
 import re
 import logging
 from typing import (
-    List, Optional
+    Optional, Sequence
 )
 
 
 class HeadingLevelFixupProcessor(Treeprocessor):
     """This processor demotes headings by one level.
 
     By default, Markdown starts headings with ``<h1>``, but in general the
@@ -55,15 +55,15 @@
         if line_offset is not None:
             return f'Line {line_number + line_offset}: {error_message}'
         else:
             return error_message
 
 
 class _ParseBuffer:
-    def __init__(self, first_line: int, lines: List[str]):
+    def __init__(self, first_line: int, lines: Sequence[str]):
         self.__current_line = first_line
         self.__lines = lines
         self.__line_start = 0
 
     def get_current_line(self) -> str:
         return self.__lines[self.__current_line][self.__line_start:]
 
@@ -245,15 +245,15 @@
     functions before the markup processing starts.
 
     Shortcodes are delimited by ``<%`` and ``/%>``. The content must start with
     the function name, followed by ``key=value`` pairs. The values are passed
     as strings, the calling function must do the type conversion.
 
     Values without quotation marks must consist of alphanumeric characters and
-    ``-``,``_`` only.
+    ``-``, ``_`` only.
 
     .. note::
       Freestanding keys are not supported as it's ambiguous whether this should
       be a considered a plain argument (i.e. passed as a non-named argument) or
       a defaulted argument (i.e. named, but set to ``True`` or some other
       value.) For example, you can't write a shortcode like this::
 
@@ -291,15 +291,15 @@
             raise Exception(f'Cannot register function "{name}" as a '
                             'shortcode handler as the function signature '
                             'is missing a **kwargs parameter.')
 
         assert name and name[0] != '$'
         self.__functions[name] = function
 
-    def run(self, lines):
+    def run(self, lines: list[str]):
         i = 0
         line_count = len(lines)
 
         # We can't use for ... in range or for ... enumerate here, as we have
         # to skip lines based on the shortcode parser
         while i < line_count:
             line = lines[i]
@@ -314,14 +314,29 @@
                 lines[i] = line[tag_start:]
 
                 parse_buffer = _ParseBuffer(i, lines)
                 shortcode_parser = _ShortcodeParser(parse_buffer)
                 rest, next_line, func_name, args = shortcode_parser.parse()
 
                 args['$page'] = self.__page
+
+                def pretty_print_args(d):
+                    for k, v in d.items():
+                        # Skip internal arguments as they can't be
+                        # pretty-printed anyways
+                        if k[0] == '$':
+                            continue
+                        yield f'{k}={repr(v)}'
+
+                # Skip the text processing if logging is disabled
+                if self.__log.isEnabledFor(logging.DEBUG):
+                    self.__log.debug('Calling shortcode handler: "%s" with '
+                                     'arguments: %s',
+                                     func_name,
+                                     ', '.join(pretty_print_args(args)))
                 yield from self.__functions[func_name](**args).splitlines()
 
                 # Another shortcode in the same line, so we need to resume
                 # parsing there and cannot simply emit the rest
                 if '<%' in rest:
                     assert next_line >= 1
                     lines[next_line-1] = rest
```

### Comparing `Liara-2.5.4/liara/nodes.py` & `Liara-2.6.0/liara/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,39 +37,39 @@
     needed.
     """
     def publish_document(self, document: 'DocumentNode') -> pathlib.Path:
         """Publish a document node.
 
         :return: The path of the generated file.
         """
-        pass
+        ...
 
     def publish_index(self, index: 'IndexNode') -> pathlib.Path:
         """Publish an index node.
 
         :return: The path of the generated file."""
-        pass
+        ...
 
     def publish_resource(self, resource: 'ResourceNode') -> pathlib.Path:
         """Publish a resource node.
 
         :return: The path of the generated file."""
-        pass
+        ...
 
     def publish_static(self, static: 'StaticNode') -> pathlib.Path:
         """Publish a static node.
 
         :return: The path of the generated file."""
-        pass
+        ...
 
     def publish_generated(self, generated: 'GeneratedNode') -> pathlib.Path:
         """Publish a generated node.
 
         :return: The path of the generated file."""
-        pass
+        ...
 
 
 class NodeKind(Enum):
     Resource = auto()
     Index = auto()
     Document = auto()
     Data = auto()
@@ -85,22 +85,22 @@
 
     The function must return the new content of the node.
     """
     def process(self) -> object:
         """
         Process the task and return the new content for the node.
         """
-        pass
+        ...
 
     def update_cache(self, content: object, cache: Cache):
         """
         After processing, an async task may update the cache in a separate
         step.
         """
-        pass
+        ...
 
 
 class Node:
     kind: NodeKind
     """The node kind, must be set in the constructor."""
     src: Optional[pathlib.Path]
     """The full path to the source file.
@@ -186,15 +186,15 @@
         operation.
 
         By convention this method should populate ``self.content`` if executed
         synchronously. If asynchronous execution is supported, this method
         must return an ``_AsyncTask`` which is then executed later. In this
         case, ``self.content`` will be populated by the task runner.
         """
-        pass
+        ...
 
 
 _metadata_marker = re.compile(r'(---|\+\+\+)\n')
 
 
 class MetadataKind(Enum):
     Unknown = auto()
@@ -261,14 +261,17 @@
     # +1 because we start counting at 1
     return metadata, content, text[meta_start:meta_end].count('\n') + 3
 
 
 def fixup_relative_links(document: 'DocumentNode'):
     """Replace relative links in the document with links relative to the
     site root."""
+    if not document.content:
+        return
+
     # early out if there's no relative link in here, as the parsing is
     # very expensive
     if "href=\"." not in document.content:
         return
 
     from bs4 import BeautifulSoup
     soup = BeautifulSoup(document.content, 'lxml')
@@ -316,14 +319,16 @@
     (These should be called before :py:meth:`load`/:py:meth:`reload`
     returns.)"""
 
     _process_fixups: List[Callable]
     """These functions are called after a document has been processed
     (These should be called before :py:meth:`process` returns)."""
 
+    content: str | None
+
     def __init__(self, src, path: pathlib.PurePosixPath,
                  metadata_path: Optional[pathlib.Path] = None):
         super().__init__()
         self.kind = NodeKind.Document
         self.src = src
         self.path = path
         self.metadata_path = metadata_path
@@ -361,14 +366,16 @@
             fixup(self)
 
     def _apply_process_fixups(self):
         for fixup in self._process_fixups:
             fixup(self)
 
     def _load(self):
+        assert self.src
+
         if self.metadata_path:
             self.metadata = load_yaml(self.metadata_path.read_text())
             self._raw_content = self.src.read_text('utf-8')
             self._content_line_start = 1
         else:
             self.metadata, self._raw_content, self._content_line_start = \
                 extract_metadata_content(self.src.read_text('utf-8'))
@@ -410,23 +417,24 @@
         ] + configuration['content.markdown.extensions']
 
         extension_configs = configuration['content.markdown.config']
         output = configuration['content.markdown.output']
 
         return Markdown(extensions=extensions,
                         extension_configs=extension_configs,
-                        output=output)
+                        output_format=output)
 
     def process(self, cache: Cache):
         import hashlib
         from .md import ShortcodeException
 
         byte_content = self._raw_content.encode('utf-8')
         content_hash = hashlib.sha256(byte_content).digest()
         if content := cache.get(content_hash):
+            assert isinstance(content, str)
             self.content = content
             return
 
         # We re-raise shortcode exceptions to adjust the line number to
         # make debugging easier
         try:
             self.content = self.__md.convert(self._raw_content)
@@ -789,15 +797,15 @@
             # is the only one with ordering issues.
             self.__load_fixups.insert(0, fixup_date)
         if configuration['allow_relative_links']:
             self.__process_fixups.append(fixup_relative_links)
 
     def __init__(self, configuration):
         super().__init__()
-        self.__load_fixups = [FixupDateTimezone()]
+        self.__load_fixups: List[Callable] = [FixupDateTimezone()]
         self.__process_fixups = []
 
         self.__setup_fixups(configuration)
 
         self.register_type(
             ['.md'], MarkdownDocumentNode,
             extra_args={
@@ -815,15 +823,19 @@
 
 class StaticNode(Node):
     """A static data node.
 
     Static nodes are suitable for large static data which never changes, for
     instance, binary files, videos, images etc.
     """
-    def __init__(self, src, path: pathlib.PurePosixPath, metadata_path=None):
+    src: pathlib.Path   # Unlike a generic Node, a StaticNode always has a
+                        # source
+
+    def __init__(self, src: pathlib.Path, path: pathlib.PurePosixPath,
+                 metadata_path=None):
         super().__init__()
         self.kind = NodeKind.Static
         self.src = src
         self.path = path
         if metadata_path:
             self.metadata = load_yaml(open(metadata_path, 'r'))
 
@@ -849,15 +861,15 @@
         """Publish this node using the provided publisher."""
         return publisher.publish_static(self)
 
 
 class _AsyncThumbnailTask(_AsyncTask):
     __log = logging.getLogger(f'{__name__}.{__qualname__}')
 
-    def __init__(self, cache_key, src: pathlib.Path,
+    def __init__(self, cache_key: bytes, src: pathlib.Path,
                  size: Dict[str, int],
                  format: Optional[str]):
         self.__src = src
         self.__size = size
         self.__cache_key = cache_key
         assert format != 'original'
         self.__format = format
@@ -873,15 +885,15 @@
         if 'height' in self.__size:
             scale = min(self.__size['height'] / height, scale)
         if 'width' in self.__size:
             scale = min(self.__size['width'] / width, scale)
         width *= scale
         height *= scale
 
-        image.thumbnail((width, height,))
+        image.thumbnail((int(width), int(height),))
         storage = io.BytesIO()
         assert self.__src
         result = None
 
         format_from_suffix = {
             '.jpg': 'JPEG',
             '.png': 'PNG',
@@ -904,15 +916,15 @@
 
     def update_cache(self, content: object, cache: Cache):
         cache.put(self.__cache_key, bytes(content))
 
 
 class ThumbnailNode(ResourceNode):
     def __init__(self, src, path: pathlib.PurePosixPath, size: Dict[str, int],
-                 format: str = 'original'):
+                 format: str | None = 'original'):
         super().__init__(src, path)
         self.__size = size
         self.__format = format
 
     def __get_cache_key(self) -> bytes:
         import hashlib
         assert self.src
@@ -929,15 +941,15 @@
             cache_key += bytes([0, 0, 0, 0])
 
         if self.__format:
             cache_key += self.__format.encode('utf-8')
 
         return cache_key
 
-    def process(self, cache: Cache) -> _AsyncThumbnailTask:
+    def process(self, cache: Cache) -> _AsyncThumbnailTask | None:
         cache_key = self.__get_cache_key()
         if content := cache.get(cache_key):
             self.content = content
             return None
 
         async_task = _AsyncThumbnailTask(cache_key, self.src,
                                          self.__size,
```

### Comparing `Liara-2.5.4/liara/plugins/has_pending_document.py` & `Liara-2.6.0/liara/plugins/has_pending_document.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/liara/plugins/series_schedule.py` & `Liara-2.6.0/liara/plugins/series_schedule.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/liara/publish.py` & `Liara-2.6.0/liara/publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
                 'Generated node "%s" has no content, skipping', generated.path)
             return
         file_path = pathlib.Path(str(self._output_path) + str(generated.path))
         os.makedirs(file_path.parent, exist_ok=True)
         if isinstance(generated.content, bytes):
             file_path.write_bytes(generated.content)
         else:
+            assert isinstance(generated.content, str)
             file_path.write_text(generated.content, encoding='utf-8')
         return file_path
 
     def publish_static(self, static: StaticNode):
         import shutil
         import os
         from contextlib import suppress
```

### Comparing `Liara-2.5.4/liara/query.py` & `Liara-2.6.0/liara/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 
 
 class SelectionFilter:
     """Base class for query selection filters."""
     def match(self, node: Node) -> bool:
         """Return ``True`` if the node should be kept, else ``False``."""
-        pass
+        ...
 
 
 class MetadataFilter(SelectionFilter):
     """Filter items which contain a specific metadata field and optionally
     check if that field matches the provided value.
     """
     def __init__(self, name, value=None):
```

### Comparing `Liara-2.5.4/liara/quickstart.py` & `Liara-2.6.0/liara/quickstart.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/liara/server.py` & `Liara-2.6.0/liara/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,27 @@
 from .template import TemplateRepository
 from .publish import TemplatePublisher
 from .cache import Cache
 import sys
 import logging
 import webbrowser
 import mimetypes
+import http.server
+
+
+class _HttpServer(http.server.HTTPServer):
+    def __init__(self, address, request_handler_class,
+                 server: 'HttpServer',
+                 log: logging.Logger):
+        self.server = server
+        self.log = log
+        self.cache = {}
+        super().__init__(address, request_handler_class)
+
+    pass
 
 
 class HttpServer:
     __log = logging.getLogger('liara.HttpServer')
 
     def get_url(self):
         return f'http://127.0.0.1:{self.__port}'
@@ -51,29 +64,30 @@
         node = self.__site.get_node(path)
 
         if node is None:
             self.__log.warning(f'Could not find node for path: "{path}"')
             return (None, None,)
 
         # We always regenerate the content
-        if node.kind in {NodeKind.Document, NodeKind.Resource}:
-            assert isinstance(node, DocumentNode) \
-                   or isinstance(node, ResourceNode)
-            node.reload()
-            _process_node_sync(node, self.__cache)
-            cache = False
-        elif node.kind in {NodeKind.Generated}:
-            assert isinstance(node, GeneratedNode)
-            node.generate()
-            cache = False
-        # We don't cache index nodes so templates get re-applied
-        elif node.kind == NodeKind.Index:
-            cache = False
-        else:
-            cache = True
+        match node.kind:
+            case NodeKind.Document | NodeKind.Resource:
+                assert isinstance(node, DocumentNode) \
+                    or isinstance(node, ResourceNode)
+                node.reload()
+                _process_node_sync(node, self.__cache)
+                cache = False
+            case NodeKind.Generated:
+                assert isinstance(node, GeneratedNode)
+                node.generate()
+                cache = False
+            # We don't cache index nodes so templates get re-applied
+            case NodeKind.Index:
+                cache = False
+            case _:
+                cache = True
 
         if node.kind == NodeKind.Document:
             self._reload_template_paths()
 
         assert isinstance(node, StaticNode) \
                or isinstance(node, DocumentNode) \
                or isinstance(node, GeneratedNode) \
@@ -106,17 +120,19 @@
         class RequestHandler(http.server.BaseHTTPRequestHandler):
             def do_GET(self):
                 path = pathlib.PurePosixPath(self.path)
 
                 if path.name == 'index.html':
                     path = path.parent
 
+                assert isinstance(self.server, _HttpServer)
+
                 if path not in self.server.cache:
                     node_path, cache = \
-                        self.server.http_server._build_single_node(path)
+                        self.server.server._build_single_node(path)
 
                     if node_path is None:
                         return
 
                     if cache:
                         self.server.cache[path] = node_path
                 else:
@@ -127,21 +143,20 @@
                 content_type, _ = mimetypes.guess_type(path.name)
                 if content_type:
                     self.send_header('Content-Type', content_type)
                 self.end_headers()
                 self.wfile.write(node_path.open('rb').read())
 
             def log_message(self, f, *args):
+                assert isinstance(self.server, _HttpServer)
                 self.server.log.info(f, *args)
 
         server_address = ('', self.__port)
-        server = http.server.HTTPServer(server_address, RequestHandler)
-        server.http_server = self
-        server.log = self.__log
-        server.cache = {}
+        server = _HttpServer(server_address, RequestHandler,
+                             self, self.__log)
         url = self.get_url()
         self.__log.info(f'Listening on {url}')
 
         if self.__open_browser:
             webbrowser.open(url)
         else:
             print(f'Listening on {url}')
```

### Comparing `Liara-2.5.4/liara/signals.py` & `Liara-2.6.0/liara/signals.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/liara/site.py` & `Liara-2.6.0/liara/site.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,32 +34,32 @@
     an accessor ``foo.bar.baz`` will access ``foo['bar']['baz]`` and
     ``foo.bar.baz``, and any combination thereof. Attributes will be preferred
     over dictionary access.
 
     If the field is not present, this function returns ``None``.
     """
     if '.' in field_name:
-        def key_fun(o):
+        def dict_key_fun(o):
             field = field_name.split('.')
             o = o.metadata.get(field[0])
             if o is None:
                 return None
             for f in field[1:]:
                 if hasattr(o, f):
                     o = getattr(o, f)
                 elif f in o:
                     o = o[f]
                 else:
                     return None
             return o
-        return key_fun
+        return dict_key_fun
     else:
-        def key_fun(o):
+        def metadata_key_fun(o):
             return o.metadata.get(field_name)
-        return key_fun
+        return metadata_key_fun
 
 
 def _create_metadata_filter(exclude_without:
                             List[Union[str, Tuple[str, Any]]]):
     """Create a function to filter out nodes based on metadata fields.
 
     The filter function will check if the specified fields are present,
```

### Comparing `Liara-2.5.4/liara/template.py` & `Liara-2.6.0/liara/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,27 +54,27 @@
         self._template_path = template_path
 
     @property
     def path(self):
         return self._template_path
 
     def render(self, **kwargs):
-        pass
+        ...
 
 
 class TemplateRepository:
     def __init__(self, paths: Dict[str, str]):
         self.__paths = paths
 
     def update_paths(self, paths: Dict[str, str]):
         self.__paths = paths
 
     def find_template(self, url: pathlib.PurePosixPath, site: 'Site') \
             -> Template:
-        pass
+        ...
 
     def _match_template(self, url: pathlib.PurePosixPath, site: 'Site') -> str:
         best_match = None
         best_score = None
         longest_matching_pattern_length = -1
         for pattern, template in self.__paths.items():
             score = _match_url(url, pattern, site)
@@ -166,14 +166,15 @@
 
             def clear(self):
                 pass
 
             def load_bytecode(self, bucket):
                 key = bucket.key.encode('utf-8')
                 if content := self.__cache.get(key):
+                    assert isinstance(content, bytes)
                     s = io.BytesIO(content)
                     bucket.load_bytecode(s)
 
             def dump_bytecode(self, bucket):
                 key = bucket.key.encode('utf-8')
                 s = io.BytesIO()
                 bucket.write_bytecode(s)
```

### Comparing `Liara-2.5.4/liara/util.py` & `Liara-2.6.0/liara/util.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/liara/yaml.py` & `Liara-2.6.0/liara/yaml.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/setup.cfg` & `Liara-2.6.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -13,43 +13,42 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: End Users/Desktop
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Internet :: WWW/HTTP
 
 [options]
-python_requires = >= 3.8
+python_requires = >= 3.10
 packages = find:
 install_requires = 
-	beautifulsoup4~=4.7
-	blinker~=1.5
-	click~=8.0
-	dateparser~=1.0
+	beautifulsoup4~=4.12
+	blinker~=1.7
+	click~=8.1
+	dateparser~=1.2
 	humanfriendly~=10.0
-	Jinja2~=3.0
+	Jinja2~=3.1
 	libsass~=0.21
-	lxml~=4.6
-	Mako~=1.2
-	Markdown~=3.3
-	Pillow~=9.2
-	Pygments~=2.10
-	pymdown-extensions~=9.0
-	python-slugify~=7.0
+	lxml~=5.1
+	Mako~=1.3
+	Markdown~=3.5
+	Pillow~=10.2
+	Pygments~=2.17
+	pymdown-extensions~=10.0
+	python-slugify~=8.0
 	PyYAML~=6.0
-	requests~=2.25
+	requests~=2.31
 	tomli~=2.0; python_version < "3.11"
-	treelib~=1.5
-	tzlocal~=4.2
+	treelib~=1.7
+	tzlocal~=5.2
 
 [options.packages.find]
 where = .
 exclude = 
 	*.test
 	test.*
 	*.test.*
@@ -58,17 +57,18 @@
 console_scripts = 
 	liara = liara.cmdline:main
 
 [options.extras_require]
 dev = 
 	flake8
 	flake8-mypy
+	tox
 redis = 
-	redis~=3.5.3
+	redis~=5.0
 docs = 
-	Sphinx~=6.0
+	Sphinx~=7.0
 	furo
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `Liara-2.5.4/test/test_md.py` & `Liara-2.6.0/test/test_md.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from liara.md import ShortcodePreprocessor, _ParseBuffer, _ShortcodeParser
 import pytest
 
+def _get_lines(document: str) -> list[str]:
+    # document.splitlines() returns a list of string literals, so you shouldn't
+    # modify it, but our pre-processor does actually replace things. This makes
+    # sure everything is type safe (by "type casting" LiteralString to str in
+    # the input)
+    return document.splitlines()
+
 
 def test_shortcode_parse():
     document = r"""<% code arg1="23" arg2=52 /%>"""
     sp = ShortcodePreprocessor()
 
     def code(arg1, arg2, **kwargs):
         return f"*{arg1}*\n_{arg2}_"
 
     sp.register('code', code)
 
-    output = list(sp.run(document.splitlines()))
+    output = list(sp.run(_get_lines(document)))
 
     assert len(output) == 2
     assert output[0] == '*23*'
     assert output[1] == '_52_'
 
 
 def test_shortcode_embedded_tag_end_in_string():
@@ -23,30 +30,30 @@
     sp = ShortcodePreprocessor()
 
     def code(arg1, **kwargs):
         return arg1
 
     sp.register('code', code)
 
-    output = list(sp.run(document.splitlines()))
+    output = list(sp.run(_get_lines(document)))
 
     assert len(output) == 1
     assert output[0] == '/%>'
 
 
 def test_shortcode_two_codes_in_one_line():
     document = r"""<% code arg1="a" /%><% code arg1="b"/%>"""
     sp = ShortcodePreprocessor()
 
     def code(arg1, **kwargs):
         return arg1
 
     sp.register('code', code)
 
-    output = list(sp.run(document.splitlines()))
+    output = list(sp.run(_get_lines(document)))
 
     assert len(output) == 2
     assert output[0] == 'a'
     assert output[1] == 'b'
 
 
 def test_parse_buffer():
@@ -156,10 +163,10 @@
 def test_shortcode_preprocessor_preserves_empty_lines():
     document = r"""Header
 ======
 
 Body"""
 
     sp = ShortcodePreprocessor()
-    output = '\n'.join(sp.run(document.splitlines()))
+    output = '\n'.join(sp.run(_get_lines(document)))
 
     assert output == document
```

### Comparing `Liara-2.5.4/test/test_nodes.py` & `Liara-2.6.0/test/test_nodes.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/test/test_query.py` & `Liara-2.6.0/test/test_query.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.4/test/test_site.py` & `Liara-2.6.0/test/test_site.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,22 +13,24 @@
         item({'a': 'key_a_1', 'b': 'key_b_1', 'c': 'key_c_2'}, 3),
         item({'a': 'key_a_1', 'b': 'key_b_2', 'c': 'key_c_1'}, 4),
         item({'a': 'key_a_1', 'b': 'key_b_1', 'c': 'key_c_1'}, 5),
         item({'a': 'key_a_2', 'b': 'key_b_2', 'c': 'key_c_1'}, 6)
     ]
 
     groups = site._group_recursive(items, ['a', 'b', 'c'])
+    assert isinstance(groups, dict)
     assert len(groups) == 2
     assert 'key_a_1' in groups
     assert 'key_a_2' in groups
 
     group_1 = groups['key_a_1']
     assert 'key_b_1' in group_1
     assert 'key_b_2' in group_1
 
+    assert isinstance(group_1, dict)
     group_1_1 = group_1['key_b_1']
     # c_1 and c_2
     assert len(group_1_1) == 2
 
     group_1_1_1 = group_1_1['key_c_1']
     # c_1, 1; c_1, 2; c_1, 5
     assert len(group_1_1_1) == 3
@@ -41,14 +43,15 @@
         item({'tags': ['a', 'd']}, 3),
         item({'tags': ['e', 'b']}, 4),
         item({'tags': ['f', 'b']}, 5),
         item({'tags': ['g', 'b']}, 6)
     ]
 
     groups = site._group_recursive(items, ['*tags'])
+    assert isinstance(groups, dict)
     # 6 tags
     assert len(groups) == 7
     assert len(groups['a']) == 3
     assert items[0] in groups['a']
     assert items[1] in groups['a']
     assert items[2] in groups['a']
 
@@ -109,15 +112,15 @@
     root.add_index(MockIndexNode('/'))
     root.add_document(n1)
     root.add_document(n2)
     root.add_document(n3)
     root.create_links()
 
     collection = site.Collection(root, 'test', '/*')
-    nodes = collection.nodes
+    nodes = list(collection.nodes)
 
     assert len(nodes) == 3
 
 
 def test_collection_group_by_fails_on_missing_metadata():
     n1 = MockDocumentNode('/a', {'title': 'A'})
     n2 = MockDocumentNode('/b', {'title': 'B'})
@@ -144,15 +147,15 @@
     root.add_document(n1)
     root.add_document(n2)
     root.add_document(n3)
     root.create_links()
 
     collection = site.Collection(root, 'test', '/*',
                                  exclude_without=['title'], order_by=['title'])
-    nodes = collection.nodes
+    nodes = list(collection.nodes)
 
     assert len(nodes) == 2
 
 
 def test_index_group_by_fails_on_missing_metadata():
     n1 = MockDocumentNode('/a', {'title': 'A'})
     n2 = MockDocumentNode('/b', {'title': 'B'})
@@ -186,14 +189,15 @@
 
     index = site.Index(collection, '/index/%1', group_by=['title'],
                        exclude_without=['title'],
                        create_top_level_index=True)
     index.create_nodes(root)
 
     index_node = root.get_node('/index')
+    assert isinstance(index_node, nodes.IndexNode)
     assert len(index_node.references) == 2
 
 
 def test_index_exclude_without_key_matching_removes_items():
     n1 = MockDocumentNode('/a', {'year': 2022, 'title': 'A'})
     n2 = MockDocumentNode('/b', {'year': 2022, 'title': 'B'})
     n3 = MockDocumentNode('/c', {'year': 2023, 'title': 'C'})
@@ -209,8 +213,9 @@
 
     index = site.Index(collection, '/index/%1', group_by=['title'],
                        exclude_without=[('year', 2022,)],
                        create_top_level_index=True)
     index.create_nodes(root)
 
     index_node = root.get_node('/index')
+    assert isinstance(index_node, nodes.IndexNode)
     assert len(index_node.references) == 2
```

### Comparing `Liara-2.5.4/test/test_template.py` & `Liara-2.6.0/test/test_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     assert score0 < score1
 
 
 def test_match_url_exact(default_site):
     score = _match_url('/blog', '/blog', default_site)
     assert score == 0
     score = _match_url('/blog/', '/blog/*', default_site)
-    assert score > 0
+    assert score is not None and score > 0
 
 
 def test_match_fail(default_site):
     score = _match_url('/2014/02/16/2297', '/research/*', default_site)
     assert score is None
```

### Comparing `Liara-2.5.4/test/test_util.py` & `Liara-2.6.0/test/test_util.py`

 * *Files identical despite different names*

