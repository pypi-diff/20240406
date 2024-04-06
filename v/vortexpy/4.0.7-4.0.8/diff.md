# Comparing `tmp/vortexpy-4.0.7.tar.gz` & `tmp/vortexpy-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vortexpy-4.0.7.tar", last modified: Fri Feb  2 03:48:53 2024, max compression
+gzip compressed data, was "vortexpy-4.0.8.tar", last modified: Tue Feb  6 12:32:36 2024, max compression
```

## Comparing `vortexpy-4.0.7.tar` & `vortexpy-4.0.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.766800 vortexpy-4.0.7/
--rw-r--r--   0 jchesney   (501) staff       (20)     1057 2021-09-22 06:19:17.000000 vortexpy-4.0.7/LICENSE
--rw-r--r--   0 jchesney   (501) staff       (20)      735 2024-02-02 03:48:53.766649 vortexpy-4.0.7/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     4607 2021-09-22 06:19:17.000000 vortexpy-4.0.7/README.md
--rw-r--r--   0 jchesney   (501) staff       (20)      915 2024-02-02 03:48:46.000000 vortexpy-4.0.7/pyproject.toml
--rw-r--r--   0 jchesney   (501) staff       (20)       79 2024-02-02 03:48:53.767436 vortexpy-4.0.7/setup.cfg
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.739655 vortexpy-4.0.7/vortex/
--rw-r--r--   0 jchesney   (501) staff       (20)      551 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/DataWrapTuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4476 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/DeferUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)     9286 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/Jsonable.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3674 2023-02-13 09:01:49.000000 vortexpy-4.0.7/vortex/Payload.py
--rw-r--r--   0 jchesney   (501) staff       (20)     6602 2022-09-10 02:45:31.000000 vortexpy-4.0.7/vortex/PayloadEndpoint.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4636 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/PayloadEndpointTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4911 2023-02-13 09:01:49.000000 vortexpy-4.0.7/vortex/PayloadEnvelope.py
--rw-r--r--   0 jchesney   (501) staff       (20)      319 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/PayloadFilterKeys.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4500 2023-01-11 02:41:19.000000 vortexpy-4.0.7/vortex/PayloadIO.py
--rw-r--r--   0 jchesney   (501) staff       (20)      213 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/PayloadPriority.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5356 2023-01-10 04:54:31.000000 vortexpy-4.0.7/vortex/PayloadResponse.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1290 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/PayloadResponseTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4360 2024-01-14 05:02:15.000000 vortexpy-4.0.7/vortex/PayloadTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)      713 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/PerformTestActionTuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     6185 2023-12-19 01:42:46.000000 vortexpy-4.0.7/vortex/SerialiseUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1597 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/TestTuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)    29613 2024-02-02 03:47:56.000000 vortexpy-4.0.7/vortex/Tuple.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1956 2023-01-10 11:24:51.000000 vortexpy-4.0.7/vortex/TupleAction.py
--rw-r--r--   0 jchesney   (501) staff       (20)      187 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/TupleActionVortex.py
--rw-r--r--   0 jchesney   (501) staff       (20)      606 2024-01-14 05:02:12.000000 vortexpy-4.0.7/vortex/TupleDataForTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1623 2024-01-26 06:04:56.000000 vortexpy-4.0.7/vortex/TuplePerfTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2207 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/TuplePolymorphicTupleTypeFieldArgTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3978 2024-01-26 06:04:56.000000 vortexpy-4.0.7/vortex/TupleRestfulTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2997 2024-01-20 02:51:40.000000 vortexpy-4.0.7/vortex/TupleSelector.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3866 2024-01-26 06:04:56.000000 vortexpy-4.0.7/vortex/TupleTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1350 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/VortexABC.py
--rw-r--r--   0 jchesney   (501) staff       (20)     8710 2023-12-23 00:40:49.000000 vortexpy-4.0.7/vortex/VortexClientHttp.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1790 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/VortexClientHttpTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)    10800 2023-01-07 04:45:16.000000 vortexpy-4.0.7/vortex/VortexClientTcp.py
--rw-r--r--   0 jchesney   (501) staff       (20)    11639 2023-01-08 09:38:46.000000 vortexpy-4.0.7/vortex/VortexClientWebsocketFactory.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2057 2022-09-08 04:32:19.000000 vortexpy-4.0.7/vortex/VortexConnectionABC.py
--rw-r--r--   0 jchesney   (501) staff       (20)    33022 2024-01-26 06:04:56.000000 vortexpy-4.0.7/vortex/VortexFactory.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5620 2022-12-31 04:15:27.000000 vortexpy-4.0.7/vortex/VortexPayloadProtocol.py
--rw-r--r--   0 jchesney   (501) staff       (20)    11557 2023-02-13 22:21:32.000000 vortexpy-4.0.7/vortex/VortexServer.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3758 2023-01-05 06:06:13.000000 vortexpy-4.0.7/vortex/VortexServerConnection.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5834 2023-01-08 09:01:52.000000 vortexpy-4.0.7/vortex/VortexServerHttpResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3081 2023-01-08 09:00:29.000000 vortexpy-4.0.7/vortex/VortexServerTcp.py
--rw-rw-rw-   0 jchesney   (501) staff       (20)     7700 2023-01-10 07:21:05.000000 vortexpy-4.0.7/vortex/VortexServerWebsocket.py
--rw-r--r--   0 jchesney   (501) staff       (20)    19710 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/VortexTcpMemoryLeakPayloadTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2327 2024-01-14 05:02:15.000000 vortexpy-4.0.7/vortex/VortexTcpMemoryLeakRawTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)      548 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/VortexTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     9717 2023-01-11 12:46:46.000000 vortexpy-4.0.7/vortex/VortexUtil.py
--rw-r--r--   0 jchesney   (501) staff       (20)    10495 2023-01-01 11:44:30.000000 vortexpy-4.0.7/vortex/VortexWritePushProducer.py
--rw-r--r--   0 jchesney   (501) staff       (20)      194 2024-02-02 03:48:46.000000 vortexpy-4.0.7/vortex/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.742972 vortexpy-4.0.7/vortex/data_loader/
--rw-r--r--   0 jchesney   (501) staff       (20)     8816 2024-01-28 11:53:44.000000 vortexpy-4.0.7/vortex/data_loader/TupleDataLiveLockManager.py
--rw-r--r--   0 jchesney   (501) staff       (20)    11416 2024-01-28 13:48:15.000000 vortexpy-4.0.7/vortex/data_loader/TupleDataLoader.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2609 2024-01-27 11:13:30.000000 vortexpy-4.0.7/vortex/data_loader/TupleDataLoaderDelegate.py
--rw-r--r--   0 jchesney   (501) staff       (20)      177 2023-04-18 11:21:17.000000 vortexpy-4.0.7/vortex/data_loader/TupleDataLoaderTupleABC.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1593 2024-01-27 11:58:44.000000 vortexpy-4.0.7/vortex/data_loader/TupleDataLoaderTuples.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-04-01 05:32:56.000000 vortexpy-4.0.7/vortex/data_loader/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.750661 vortexpy-4.0.7/vortex/handler/
--rw-r--r--   0 jchesney   (501) staff       (20)     8353 2023-04-01 02:00:03.000000 vortexpy-4.0.7/vortex/handler/TupleActionProcessor.py
--rw-r--r--   0 jchesney   (501) staff       (20)     7290 2023-01-11 11:42:42.000000 vortexpy-4.0.7/vortex/handler/TupleActionProcessorProxy.py
--rw-r--r--   0 jchesney   (501) staff       (20)      933 2024-01-26 06:04:56.000000 vortexpy-4.0.7/vortex/handler/TupleActionProcessorTestHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5202 2024-01-26 06:04:56.000000 vortexpy-4.0.7/vortex/handler/TupleChangeEventBus.py
--rw-r--r--   0 jchesney   (501) staff       (20)      270 2024-01-14 06:19:33.000000 vortexpy-4.0.7/vortex/handler/TupleChangeEventBusObserverABC.py
--rw-r--r--   0 jchesney   (501) staff       (20)     2112 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/handler/TupleDataActionClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     6202 2023-11-28 05:57:35.000000 vortexpy-4.0.7/vortex/handler/TupleDataObservableCache.py
--rw-r--r--   0 jchesney   (501) staff       (20)    12671 2024-01-23 09:32:14.000000 vortexpy-4.0.7/vortex/handler/TupleDataObservableHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)    11648 2023-01-10 12:12:02.000000 vortexpy-4.0.7/vortex/handler/TupleDataObservableProxyHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1969 2024-01-26 06:04:56.000000 vortexpy-4.0.7/vortex/handler/TupleDataObservableTestHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5552 2023-11-28 05:57:35.000000 vortexpy-4.0.7/vortex/handler/TupleDataObserverClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1438 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/handler/VortexJSTupleLoaderTestHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/handler/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.757136 vortexpy-4.0.7/vortex/restful/
--rw-r--r--   0 jchesney   (501) staff       (20)     5153 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/restful/GzippedDataHttpClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3304 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/restful/GzippedDataHttpClientTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     5636 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/restful/GzippedPayloadHttpClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3007 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/restful/RestfulHttpClient.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1662 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/restful/RestfulHttpClientTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)     4958 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/restful/RestfulResource.py
--rw-r--r--   0 jchesney   (501) staff       (20)     3292 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/restful/RestfulResourceTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/restful/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.759270 vortexpy-4.0.7/vortex/rpc/
--rw-r--r--   0 jchesney   (501) staff       (20)    13497 2022-09-08 03:30:59.000000 vortexpy-4.0.7/vortex/rpc/RPC.py
--rw-r--r--   0 jchesney   (501) staff       (20)      387 2022-09-12 02:58:12.000000 vortexpy-4.0.7/vortex/rpc/RPCTest.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/rpc/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.762031 vortexpy-4.0.7/vortex/sqla_orm/
--rw-r--r--   0 jchesney   (501) staff       (20)    13698 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/sqla_orm/OrmCrudHandler.py
--rw-r--r--   0 jchesney   (501) staff       (20)     1414 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/sqla_orm/TupleProviderForDb.py
--rw-r--r--   0 jchesney   (501) staff       (20)      636 2023-12-23 23:31:45.000000 vortexpy-4.0.7/vortex/sqla_orm/VortexTupleJson.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-4.0.7/vortex/sqla_orm/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.763190 vortexpy-4.0.7/vortex/storage/
--rw-r--r--   0 jchesney   (501) staff       (20)    11237 2022-09-11 13:08:55.000000 vortexpy-4.0.7/vortex/storage/TupleStorageSqlite.py
--rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-09-10 22:39:53.000000 vortexpy-4.0.7/vortex/storage/__init__.py
-drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-02 03:48:53.765966 vortexpy-4.0.7/vortexpy.egg-info/
--rw-r--r--   0 jchesney   (501) staff       (20)      735 2024-02-02 03:48:53.000000 vortexpy-4.0.7/vortexpy.egg-info/PKG-INFO
--rw-r--r--   0 jchesney   (501) staff       (20)     2761 2024-02-02 03:48:53.000000 vortexpy-4.0.7/vortexpy.egg-info/SOURCES.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        1 2024-02-02 03:48:53.000000 vortexpy-4.0.7/vortexpy.egg-info/dependency_links.txt
--rw-r--r--   0 jchesney   (501) staff       (20)      139 2024-02-02 03:48:53.000000 vortexpy-4.0.7/vortexpy.egg-info/requires.txt
--rw-r--r--   0 jchesney   (501) staff       (20)        7 2024-02-02 03:48:53.000000 vortexpy-4.0.7/vortexpy.egg-info/top_level.txt
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.149836 vortexpy-4.0.8/
+-rw-r--r--   0 jchesney   (501) staff       (20)     1057 2021-09-22 06:19:17.000000 vortexpy-4.0.8/LICENSE
+-rw-r--r--   0 jchesney   (501) staff       (20)      735 2024-02-06 12:32:36.149634 vortexpy-4.0.8/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     4607 2021-09-22 06:19:17.000000 vortexpy-4.0.8/README.md
+-rw-r--r--   0 jchesney   (501) staff       (20)      915 2024-02-06 12:32:22.000000 vortexpy-4.0.8/pyproject.toml
+-rw-r--r--   0 jchesney   (501) staff       (20)       79 2024-02-06 12:32:36.150582 vortexpy-4.0.8/setup.cfg
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.123391 vortexpy-4.0.8/vortex/
+-rw-r--r--   0 jchesney   (501) staff       (20)      551 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/DataWrapTuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4476 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/DeferUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     9286 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/Jsonable.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3674 2023-02-13 09:01:49.000000 vortexpy-4.0.8/vortex/Payload.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     6602 2022-09-10 02:45:31.000000 vortexpy-4.0.8/vortex/PayloadEndpoint.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4636 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/PayloadEndpointTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4911 2023-02-13 09:01:49.000000 vortexpy-4.0.8/vortex/PayloadEnvelope.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      319 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/PayloadFilterKeys.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4500 2023-01-11 02:41:19.000000 vortexpy-4.0.8/vortex/PayloadIO.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      213 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/PayloadPriority.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5356 2023-01-10 04:54:31.000000 vortexpy-4.0.8/vortex/PayloadResponse.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1290 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/PayloadResponseTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4360 2024-01-14 05:02:15.000000 vortexpy-4.0.8/vortex/PayloadTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      713 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/PerformTestActionTuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     6185 2023-12-19 01:42:46.000000 vortexpy-4.0.8/vortex/SerialiseUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1597 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/TestTuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    29613 2024-02-02 03:47:56.000000 vortexpy-4.0.8/vortex/Tuple.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1956 2023-01-10 11:24:51.000000 vortexpy-4.0.8/vortex/TupleAction.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      187 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/TupleActionVortex.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      606 2024-01-14 05:02:12.000000 vortexpy-4.0.8/vortex/TupleDataForTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1623 2024-01-26 06:04:56.000000 vortexpy-4.0.8/vortex/TuplePerfTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2207 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/TuplePolymorphicTupleTypeFieldArgTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3978 2024-01-26 06:04:56.000000 vortexpy-4.0.8/vortex/TupleRestfulTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2997 2024-02-06 03:44:33.000000 vortexpy-4.0.8/vortex/TupleSelector.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3866 2024-01-26 06:04:56.000000 vortexpy-4.0.8/vortex/TupleTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1350 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/VortexABC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     8710 2023-12-23 00:40:49.000000 vortexpy-4.0.8/vortex/VortexClientHttp.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1790 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/VortexClientHttpTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    10800 2023-01-07 04:45:16.000000 vortexpy-4.0.8/vortex/VortexClientTcp.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    11639 2023-01-08 09:38:46.000000 vortexpy-4.0.8/vortex/VortexClientWebsocketFactory.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2057 2022-09-08 04:32:19.000000 vortexpy-4.0.8/vortex/VortexConnectionABC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    33022 2024-01-26 06:04:56.000000 vortexpy-4.0.8/vortex/VortexFactory.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5620 2022-12-31 04:15:27.000000 vortexpy-4.0.8/vortex/VortexPayloadProtocol.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    11557 2023-02-13 22:21:32.000000 vortexpy-4.0.8/vortex/VortexServer.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3758 2023-01-05 06:06:13.000000 vortexpy-4.0.8/vortex/VortexServerConnection.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5834 2023-01-08 09:01:52.000000 vortexpy-4.0.8/vortex/VortexServerHttpResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3081 2023-01-08 09:00:29.000000 vortexpy-4.0.8/vortex/VortexServerTcp.py
+-rw-rw-rw-   0 jchesney   (501) staff       (20)     7700 2023-01-10 07:21:05.000000 vortexpy-4.0.8/vortex/VortexServerWebsocket.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    19710 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/VortexTcpMemoryLeakPayloadTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2327 2024-01-14 05:02:15.000000 vortexpy-4.0.8/vortex/VortexTcpMemoryLeakRawTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      548 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/VortexTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     9717 2023-01-11 12:46:46.000000 vortexpy-4.0.8/vortex/VortexUtil.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    10495 2023-01-01 11:44:30.000000 vortexpy-4.0.8/vortex/VortexWritePushProducer.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      194 2024-02-06 12:32:22.000000 vortexpy-4.0.8/vortex/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.127459 vortexpy-4.0.8/vortex/data_loader/
+-rw-r--r--   0 jchesney   (501) staff       (20)     8816 2024-01-28 11:53:44.000000 vortexpy-4.0.8/vortex/data_loader/TupleDataLiveLockManager.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    11416 2024-01-28 13:48:15.000000 vortexpy-4.0.8/vortex/data_loader/TupleDataLoader.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2609 2024-01-27 11:13:30.000000 vortexpy-4.0.8/vortex/data_loader/TupleDataLoaderDelegate.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      177 2023-04-18 11:21:17.000000 vortexpy-4.0.8/vortex/data_loader/TupleDataLoaderTupleABC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1593 2024-01-27 11:58:44.000000 vortexpy-4.0.8/vortex/data_loader/TupleDataLoaderTuples.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2023-04-01 05:32:56.000000 vortexpy-4.0.8/vortex/data_loader/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.134973 vortexpy-4.0.8/vortex/handler/
+-rw-r--r--   0 jchesney   (501) staff       (20)     8353 2023-04-01 02:00:03.000000 vortexpy-4.0.8/vortex/handler/TupleActionProcessor.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     7290 2023-01-11 11:42:42.000000 vortexpy-4.0.8/vortex/handler/TupleActionProcessorProxy.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      933 2024-01-26 06:04:56.000000 vortexpy-4.0.8/vortex/handler/TupleActionProcessorTestHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5278 2024-02-06 12:30:59.000000 vortexpy-4.0.8/vortex/handler/TupleChangeEventBus.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      270 2024-01-14 06:19:33.000000 vortexpy-4.0.8/vortex/handler/TupleChangeEventBusObserverABC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     2112 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/handler/TupleDataActionClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     6202 2023-11-28 05:57:35.000000 vortexpy-4.0.8/vortex/handler/TupleDataObservableCache.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    12671 2024-01-23 09:32:14.000000 vortexpy-4.0.8/vortex/handler/TupleDataObservableHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)    11648 2023-01-10 12:12:02.000000 vortexpy-4.0.8/vortex/handler/TupleDataObservableProxyHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1969 2024-01-26 06:04:56.000000 vortexpy-4.0.8/vortex/handler/TupleDataObservableTestHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5552 2023-11-28 05:57:35.000000 vortexpy-4.0.8/vortex/handler/TupleDataObserverClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1438 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/handler/VortexJSTupleLoaderTestHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/handler/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.140321 vortexpy-4.0.8/vortex/restful/
+-rw-r--r--   0 jchesney   (501) staff       (20)     5153 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/restful/GzippedDataHttpClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3304 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/restful/GzippedDataHttpClientTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     5636 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/restful/GzippedPayloadHttpClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3007 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/restful/RestfulHttpClient.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1662 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/restful/RestfulHttpClientTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     4958 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/restful/RestfulResource.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     3292 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/restful/RestfulResourceTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/restful/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.142228 vortexpy-4.0.8/vortex/rpc/
+-rw-r--r--   0 jchesney   (501) staff       (20)    13497 2022-09-08 03:30:59.000000 vortexpy-4.0.8/vortex/rpc/RPC.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      387 2022-09-12 02:58:12.000000 vortexpy-4.0.8/vortex/rpc/RPCTest.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/rpc/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.144877 vortexpy-4.0.8/vortex/sqla_orm/
+-rw-r--r--   0 jchesney   (501) staff       (20)    13698 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/sqla_orm/OrmCrudHandler.py
+-rw-r--r--   0 jchesney   (501) staff       (20)     1414 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/sqla_orm/TupleProviderForDb.py
+-rw-r--r--   0 jchesney   (501) staff       (20)      636 2023-12-23 23:31:45.000000 vortexpy-4.0.8/vortex/sqla_orm/VortexTupleJson.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-06-07 01:35:57.000000 vortexpy-4.0.8/vortex/sqla_orm/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.146030 vortexpy-4.0.8/vortex/storage/
+-rw-r--r--   0 jchesney   (501) staff       (20)    11237 2022-09-11 13:08:55.000000 vortexpy-4.0.8/vortex/storage/TupleStorageSqlite.py
+-rw-r--r--   0 jchesney   (501) staff       (20)        0 2022-09-10 22:39:53.000000 vortexpy-4.0.8/vortex/storage/__init__.py
+drwxr-xr-x   0 jchesney   (501) staff       (20)        0 2024-02-06 12:32:36.148932 vortexpy-4.0.8/vortexpy.egg-info/
+-rw-r--r--   0 jchesney   (501) staff       (20)      735 2024-02-06 12:32:36.000000 vortexpy-4.0.8/vortexpy.egg-info/PKG-INFO
+-rw-r--r--   0 jchesney   (501) staff       (20)     2761 2024-02-06 12:32:36.000000 vortexpy-4.0.8/vortexpy.egg-info/SOURCES.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        1 2024-02-06 12:32:36.000000 vortexpy-4.0.8/vortexpy.egg-info/dependency_links.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)      139 2024-02-06 12:32:36.000000 vortexpy-4.0.8/vortexpy.egg-info/requires.txt
+-rw-r--r--   0 jchesney   (501) staff       (20)        7 2024-02-06 12:32:36.000000 vortexpy-4.0.8/vortexpy.egg-info/top_level.txt
```

### Comparing `vortexpy-4.0.7/LICENSE` & `vortexpy-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/PKG-INFO` & `vortexpy-4.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortexpy
-Version: 4.0.7
+Version: 4.0.8
 Summary: Synertys observable, routable, data serialisation and transport code.
 Author-email: Synerty <contact@synerty.com>
 Project-URL: Homepage, https://github.com/Synerty/vortexpy
 Project-URL: Download, https://github.com/Synerty/vortexpy/tarball/3.4.6
 Keywords: vortex,observable,http,compressed,synerty
 Classifier: Programming Language :: Python :: 3.5
 License-File: LICENSE
```

### Comparing `vortexpy-4.0.7/README.md` & `vortexpy-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/pyproject.toml` & `vortexpy-4.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vortexpy"
-version = "4.0.7"
+version = "4.0.8"
 authors = [{name = "Synerty", email = "contact@synerty.com"}]
 description = "Synertys observable, routable, data serialisation and transport code."
 keywords = [
     "vortex",
     "observable",
     "http",
     "compressed",
```

### Comparing `vortexpy-4.0.7/vortex/DataWrapTuple.py` & `vortexpy-4.0.8/vortex/DataWrapTuple.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/DeferUtil.py` & `vortexpy-4.0.8/vortex/DeferUtil.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/Jsonable.py` & `vortexpy-4.0.8/vortex/Jsonable.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/Payload.py` & `vortexpy-4.0.8/vortex/Payload.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/PayloadEndpoint.py` & `vortexpy-4.0.8/vortex/PayloadEndpoint.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/PayloadEndpointTest.py` & `vortexpy-4.0.8/vortex/PayloadEndpointTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/PayloadEnvelope.py` & `vortexpy-4.0.8/vortex/PayloadEnvelope.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/PayloadIO.py` & `vortexpy-4.0.8/vortex/PayloadIO.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/PayloadResponse.py` & `vortexpy-4.0.8/vortex/PayloadResponse.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/PayloadResponseTest.py` & `vortexpy-4.0.8/vortex/PayloadResponseTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/PayloadTest.py` & `vortexpy-4.0.8/vortex/PayloadTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/PerformTestActionTuple.py` & `vortexpy-4.0.8/vortex/PerformTestActionTuple.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/SerialiseUtil.py` & `vortexpy-4.0.8/vortex/SerialiseUtil.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/TestTuple.py` & `vortexpy-4.0.8/vortex/TestTuple.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/Tuple.py` & `vortexpy-4.0.8/vortex/Tuple.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/TupleAction.py` & `vortexpy-4.0.8/vortex/TupleAction.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/TupleDataForTest.py` & `vortexpy-4.0.8/vortex/TupleDataForTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/TuplePerfTest.py` & `vortexpy-4.0.8/vortex/TuplePerfTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/TuplePolymorphicTupleTypeFieldArgTest.py` & `vortexpy-4.0.8/vortex/TuplePolymorphicTupleTypeFieldArgTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/TupleRestfulTest.py` & `vortexpy-4.0.8/vortex/TupleRestfulTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/TupleSelector.py` & `vortexpy-4.0.8/vortex/TupleSelector.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         # no arguments
         if nameOrTuple is None:
             return None
 
         if isinstance(nameOrTuple, str):
             name = nameOrTuple
 
-        elif issubclass(nameOrTuple, Tuple):
+        elif isinstance(nameOrTuple, Tuple):
             name = nameOrTuple.tupleType()
 
-        elif isinstance(nameOrTuple, Tuple):
+        elif issubclass(nameOrTuple, Tuple):
             name = nameOrTuple.tupleType()
 
         else:
             raise Exception(
                 "Argument should be of type Union[str, Type[Tuple], Tuple]"
             )
```

### Comparing `vortexpy-4.0.7/vortex/TupleTest.py` & `vortexpy-4.0.8/vortex/TupleTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexABC.py` & `vortexpy-4.0.8/vortex/VortexABC.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexClientHttp.py` & `vortexpy-4.0.8/vortex/VortexClientHttp.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexClientHttpTest.py` & `vortexpy-4.0.8/vortex/VortexClientHttpTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexClientTcp.py` & `vortexpy-4.0.8/vortex/VortexClientTcp.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexClientWebsocketFactory.py` & `vortexpy-4.0.8/vortex/VortexClientWebsocketFactory.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexConnectionABC.py` & `vortexpy-4.0.8/vortex/VortexConnectionABC.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexFactory.py` & `vortexpy-4.0.8/vortex/VortexFactory.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexPayloadProtocol.py` & `vortexpy-4.0.8/vortex/VortexPayloadProtocol.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexServer.py` & `vortexpy-4.0.8/vortex/VortexServer.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexServerConnection.py` & `vortexpy-4.0.8/vortex/VortexServerConnection.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexServerHttpResource.py` & `vortexpy-4.0.8/vortex/VortexServerHttpResource.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexServerTcp.py` & `vortexpy-4.0.8/vortex/VortexServerTcp.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexServerWebsocket.py` & `vortexpy-4.0.8/vortex/VortexServerWebsocket.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexTcpMemoryLeakPayloadTest.py` & `vortexpy-4.0.8/vortex/VortexTcpMemoryLeakPayloadTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexTcpMemoryLeakRawTest.py` & `vortexpy-4.0.8/vortex/VortexTcpMemoryLeakRawTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexTest.py` & `vortexpy-4.0.8/vortex/VortexTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexUtil.py` & `vortexpy-4.0.8/vortex/VortexUtil.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/VortexWritePushProducer.py` & `vortexpy-4.0.8/vortex/VortexWritePushProducer.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/data_loader/TupleDataLiveLockManager.py` & `vortexpy-4.0.8/vortex/data_loader/TupleDataLiveLockManager.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/data_loader/TupleDataLoader.py` & `vortexpy-4.0.8/vortex/data_loader/TupleDataLoader.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/data_loader/TupleDataLoaderDelegate.py` & `vortexpy-4.0.8/vortex/data_loader/TupleDataLoaderDelegate.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/data_loader/TupleDataLoaderTuples.py` & `vortexpy-4.0.8/vortex/data_loader/TupleDataLoaderTuples.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleActionProcessor.py` & `vortexpy-4.0.8/vortex/handler/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleActionProcessorProxy.py` & `vortexpy-4.0.8/vortex/handler/TupleActionProcessorProxy.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleActionProcessorTestHandler.py` & `vortexpy-4.0.8/vortex/handler/TupleActionProcessorTestHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleChangeEventBus.py` & `vortexpy-4.0.8/vortex/handler/TupleChangeEventBus.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,19 @@
         :param tupleSelector: The tuple selector that describes the tuple
         that has been changed. This change might be created, updated, or
         deleted.
         :return:
         """
         weakSets = [self._weakObserversForAllTupleSelectorNames]
 
-        if tupleSelector.name in self._weakObserversBySelectorName:
+        tupleSelectorName = TupleSelector.nameFromTuple(tupleSelector)
+
+        if tupleSelectorName in self._weakObserversBySelectorName:
             weakSets.append(
-                self._weakObserversBySelectorName[tupleSelector.name]
+                list(self._weakObserversBySelectorName[tupleSelectorName])
             )
 
         for weakSet in weakSets:
             for item in weakSet:
                 if not item:
                     continue
```

### Comparing `vortexpy-4.0.7/vortex/handler/TupleDataActionClient.py` & `vortexpy-4.0.8/vortex/handler/TupleDataActionClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleDataObservableCache.py` & `vortexpy-4.0.8/vortex/handler/TupleDataObservableCache.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleDataObservableHandler.py` & `vortexpy-4.0.8/vortex/handler/TupleDataObservableHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleDataObservableProxyHandler.py` & `vortexpy-4.0.8/vortex/handler/TupleDataObservableProxyHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleDataObservableTestHandler.py` & `vortexpy-4.0.8/vortex/handler/TupleDataObservableTestHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/TupleDataObserverClient.py` & `vortexpy-4.0.8/vortex/handler/TupleDataObserverClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/handler/VortexJSTupleLoaderTestHandler.py` & `vortexpy-4.0.8/vortex/handler/VortexJSTupleLoaderTestHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/restful/GzippedDataHttpClient.py` & `vortexpy-4.0.8/vortex/restful/GzippedDataHttpClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/restful/GzippedDataHttpClientTest.py` & `vortexpy-4.0.8/vortex/restful/GzippedDataHttpClientTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/restful/GzippedPayloadHttpClient.py` & `vortexpy-4.0.8/vortex/restful/GzippedPayloadHttpClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/restful/RestfulHttpClient.py` & `vortexpy-4.0.8/vortex/restful/RestfulHttpClient.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/restful/RestfulHttpClientTest.py` & `vortexpy-4.0.8/vortex/restful/RestfulHttpClientTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/restful/RestfulResource.py` & `vortexpy-4.0.8/vortex/restful/RestfulResource.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/restful/RestfulResourceTest.py` & `vortexpy-4.0.8/vortex/restful/RestfulResourceTest.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/rpc/RPC.py` & `vortexpy-4.0.8/vortex/rpc/RPC.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/sqla_orm/OrmCrudHandler.py` & `vortexpy-4.0.8/vortex/sqla_orm/OrmCrudHandler.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/sqla_orm/TupleProviderForDb.py` & `vortexpy-4.0.8/vortex/sqla_orm/TupleProviderForDb.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/sqla_orm/VortexTupleJson.py` & `vortexpy-4.0.8/vortex/sqla_orm/VortexTupleJson.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortex/storage/TupleStorageSqlite.py` & `vortexpy-4.0.8/vortex/storage/TupleStorageSqlite.py`

 * *Files identical despite different names*

### Comparing `vortexpy-4.0.7/vortexpy.egg-info/PKG-INFO` & `vortexpy-4.0.8/vortexpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortexpy
-Version: 4.0.7
+Version: 4.0.8
 Summary: Synertys observable, routable, data serialisation and transport code.
 Author-email: Synerty <contact@synerty.com>
 Project-URL: Homepage, https://github.com/Synerty/vortexpy
 Project-URL: Download, https://github.com/Synerty/vortexpy/tarball/3.4.6
 Keywords: vortex,observable,http,compressed,synerty
 Classifier: Programming Language :: Python :: 3.5
 License-File: LICENSE
```

### Comparing `vortexpy-4.0.7/vortexpy.egg-info/SOURCES.txt` & `vortexpy-4.0.8/vortexpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

