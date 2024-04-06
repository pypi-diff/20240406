# Comparing `tmp/vertex_protocol-2.0.0.tar.gz` & `tmp/vertex_protocol-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_protocol-2.0.0.tar", max compression
+gzip compressed data, was "vertex_protocol-2.0.1.tar", max compression
```

## Comparing `vertex_protocol-2.0.0.tar` & `vertex_protocol-2.0.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     3345 2024-03-12 17:08:19.382212 vertex_protocol-2.0.0/README.md
--rw-r--r--   0        0        0     1663 2024-03-12 17:08:19.382212 vertex_protocol-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/__init__.py
--rw-r--r--   0        0        0     8199 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/__init__.py
--rw-r--r--   0        0        0      580 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/__init__.py
--rw-r--r--   0        0        0     1394 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/base.py
--rw-r--r--   0        0        0     1108 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/market/__init__.py
--rw-r--r--   0        0        0     5441 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/market/execute.py
--rw-r--r--   0        0        0    10937 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/market/query.py
--rw-r--r--   0        0        0      746 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/perp/__init__.py
--rw-r--r--   0        0        0     1438 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/perp/query.py
--rw-r--r--   0        0        0     1027 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/spot/__init__.py
--rw-r--r--   0        0        0     1191 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/spot/base.py
--rw-r--r--   0        0        0     4782 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/spot/execute.py
--rw-r--r--   0        0        0     2964 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/spot/query.py
--rw-r--r--   0        0        0     1307 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/subaccount/__init__.py
--rw-r--r--   0        0        0     2023 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/subaccount/execute.py
--rw-r--r--   0        0        0     4599 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/apis/subaccount/query.py
--rw-r--r--   0        0        0     2895 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/client/context.py
--rw-r--r--   0        0        0     9059 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/__init__.py
--rw-r--r--   0        0        0    12130 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/Endpoint.json
--rw-r--r--   0        0        0    55374 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/FQuerier.json
--rw-r--r--   0        0        0    18751 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IClearinghouse.json
--rw-r--r--   0        0        0     3385 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IERC20.json
--rw-r--r--   0        0        0     4796 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IEndpoint.json
--rw-r--r--   0        0        0    13112 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IOffchainBook.json
--rw-r--r--   0        0        0    19746 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IPerpEngine.json
--rw-r--r--   0        0        0     6836 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IProductEngine.json
--rw-r--r--   0        0        0    17284 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/ISpotEngine.json
--rw-r--r--   0        0        0     5698 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/abis/MockERC20.json
--rw-r--r--   0        0        0     1000 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
--rw-r--r--   0        0        0      773 2024-03-12 17:08:19.386212 vertex_protocol-2.0.0/vertex_protocol/contracts/deployments/deployment.arbitrumSepolia.json
--rw-r--r--   0        0        0      544 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/contracts/deployments/deployment.blastMainnet.json
--rw-r--r--   0        0        0      950 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/contracts/deployments/deployment.test.json
--rw-r--r--   0        0        0      426 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/contracts/eip712/__init__.py
--rw-r--r--   0        0        0     1189 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/contracts/eip712/domain.py
--rw-r--r--   0        0        0     2484 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/contracts/eip712/sign.py
--rw-r--r--   0        0        0     4636 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/contracts/eip712/types.py
--rw-r--r--   0        0        0     1526 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/contracts/loader.py
--rw-r--r--   0        0        0     2859 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/contracts/types.py
--rw-r--r--   0        0        0     1127 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/engine_client/__init__.py
--rw-r--r--   0        0        0    23900 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/engine_client/execute.py
--rw-r--r--   0        0        0    13499 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/engine_client/query.py
--rw-r--r--   0        0        0     5802 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/engine_client/types/__init__.py
--rw-r--r--   0        0        0    21336 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/engine_client/types/execute.py
--rw-r--r--   0        0        0     4021 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/engine_client/types/models.py
--rw-r--r--   0        0        0    10384 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/engine_client/types/query.py
--rw-r--r--   0        0        0      926 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/indexer_client/__init__.py
--rw-r--r--   0        0        0    12949 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/indexer_client/query.py
--rw-r--r--   0        0        0     3231 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/indexer_client/types/__init__.py
--rw-r--r--   0        0        0     5732 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/indexer_client/types/models.py
--rw-r--r--   0        0        0    14250 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/indexer_client/types/query.py
--rw-r--r--   0        0        0      933 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/__init__.py
--rw-r--r--   0        0        0      691 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/backend.py
--rw-r--r--   0        0        0     5301 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/bytes32.py
--rw-r--r--   0        0        0       99 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/enum.py
--rw-r--r--   0        0        0     1136 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/exceptions.py
--rw-r--r--   0        0        0     1094 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/expiration.py
--rw-r--r--   0        0        0     1290 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/math.py
--rw-r--r--   0        0        0     2089 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/model.py
--rw-r--r--   0        0        0      863 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/nonce.py
--rw-r--r--   0        0        0      503 2024-03-12 17:08:19.390212 vertex_protocol-2.0.0/vertex_protocol/utils/subaccount.py
--rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 vertex_protocol-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3345 2024-04-06 18:48:27.551685 vertex_protocol-2.0.1/README.md
+-rw-r--r--   0        0        0     1663 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/__init__.py
+-rw-r--r--   0        0        0     8199 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/__init__.py
+-rw-r--r--   0        0        0      580 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/__init__.py
+-rw-r--r--   0        0        0     1394 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/base.py
+-rw-r--r--   0        0        0     1108 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/market/__init__.py
+-rw-r--r--   0        0        0     5441 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/market/execute.py
+-rw-r--r--   0        0        0    10937 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/market/query.py
+-rw-r--r--   0        0        0      746 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/perp/__init__.py
+-rw-r--r--   0        0        0     1438 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/perp/query.py
+-rw-r--r--   0        0        0     1027 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/spot/__init__.py
+-rw-r--r--   0        0        0     1191 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/spot/base.py
+-rw-r--r--   0        0        0     4782 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/spot/execute.py
+-rw-r--r--   0        0        0     2964 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/spot/query.py
+-rw-r--r--   0        0        0     1307 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/subaccount/__init__.py
+-rw-r--r--   0        0        0     2023 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/subaccount/execute.py
+-rw-r--r--   0        0        0     4599 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/apis/subaccount/query.py
+-rw-r--r--   0        0        0     2895 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/client/context.py
+-rw-r--r--   0        0        0     9059 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/contracts/__init__.py
+-rw-r--r--   0        0        0    12130 2024-04-06 18:48:27.555685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/Endpoint.json
+-rw-r--r--   0        0        0    55374 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/FQuerier.json
+-rw-r--r--   0        0        0    18751 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IClearinghouse.json
+-rw-r--r--   0        0        0     3385 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IERC20.json
+-rw-r--r--   0        0        0     4796 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IEndpoint.json
+-rw-r--r--   0        0        0    13112 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IOffchainBook.json
+-rw-r--r--   0        0        0    19746 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IPerpEngine.json
+-rw-r--r--   0        0        0     6836 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IProductEngine.json
+-rw-r--r--   0        0        0    17284 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/ISpotEngine.json
+-rw-r--r--   0        0        0     5698 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/abis/MockERC20.json
+-rw-r--r--   0        0        0     1000 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
+-rw-r--r--   0        0        0      773 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/deployments/deployment.arbitrumSepolia.json
+-rw-r--r--   0        0        0      544 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/deployments/deployment.blastMainnet.json
+-rw-r--r--   0        0        0      950 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/deployments/deployment.test.json
+-rw-r--r--   0        0        0      426 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/eip712/__init__.py
+-rw-r--r--   0        0        0     1189 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/eip712/domain.py
+-rw-r--r--   0        0        0     2484 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/eip712/sign.py
+-rw-r--r--   0        0        0     4636 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/eip712/types.py
+-rw-r--r--   0        0        0     1526 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/loader.py
+-rw-r--r--   0        0        0     2859 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/contracts/types.py
+-rw-r--r--   0        0        0     1127 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/engine_client/__init__.py
+-rw-r--r--   0        0        0    23900 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/engine_client/execute.py
+-rw-r--r--   0        0        0    13499 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/engine_client/query.py
+-rw-r--r--   0        0        0     5802 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/engine_client/types/__init__.py
+-rw-r--r--   0        0        0    21336 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/engine_client/types/execute.py
+-rw-r--r--   0        0        0     4021 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/engine_client/types/models.py
+-rw-r--r--   0        0        0    10384 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/engine_client/types/query.py
+-rw-r--r--   0        0        0      926 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/indexer_client/__init__.py
+-rw-r--r--   0        0        0    13190 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/indexer_client/query.py
+-rw-r--r--   0        0        0     3259 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/indexer_client/types/__init__.py
+-rw-r--r--   0        0        0     5732 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/indexer_client/types/models.py
+-rw-r--r--   0        0        0    14902 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/indexer_client/types/query.py
+-rw-r--r--   0        0        0      933 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/__init__.py
+-rw-r--r--   0        0        0      691 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/backend.py
+-rw-r--r--   0        0        0     5301 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/bytes32.py
+-rw-r--r--   0        0        0       99 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/enum.py
+-rw-r--r--   0        0        0     1136 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/exceptions.py
+-rw-r--r--   0        0        0     1094 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/expiration.py
+-rw-r--r--   0        0        0     1290 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/math.py
+-rw-r--r--   0        0        0     2089 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/model.py
+-rw-r--r--   0        0        0      863 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/nonce.py
+-rw-r--r--   0        0        0      503 2024-04-06 18:48:27.559685 vertex_protocol-2.0.1/vertex_protocol/utils/subaccount.py
+-rw-r--r--   0        0        0     4178 1970-01-01 00:00:00.000000 vertex_protocol-2.0.1/PKG-INFO
```

### Comparing `vertex_protocol-2.0.0/README.md` & `vertex_protocol-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/pyproject.toml` & `vertex_protocol-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vertex-protocol"
-version = "2.0.0"
+version = "2.0.1"
 description = "Vertex Protocol SDK"
 authors = ["Jeury Mejia <jeury@vertexprotocol.com>"]
 homepage = "https://vertexprotocol.com/"
 maintainers = [
   "Frank Jia <frank@vertexprotocol.com>",
   "Clark Oh-Willeke <clark@vertexprotocol.com>"
 ]
```

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/base.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/market/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/market/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/market/execute.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/market/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/market/query.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/market/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/perp/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/perp/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/perp/query.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/perp/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/spot/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/spot/base.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/spot/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/spot/execute.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/spot/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/spot/query.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/spot/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/subaccount/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/subaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/subaccount/execute.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/subaccount/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/apis/subaccount/query.py` & `vertex_protocol-2.0.1/vertex_protocol/client/apis/subaccount/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/client/context.py` & `vertex_protocol-2.0.1/vertex_protocol/client/context.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/Endpoint.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/Endpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/FQuerier.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/FQuerier.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IClearinghouse.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IClearinghouse.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IERC20.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IEndpoint.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IEndpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IOffchainBook.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IOffchainBook.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IPerpEngine.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IPerpEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/IProductEngine.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/IProductEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/ISpotEngine.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/ISpotEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/abis/MockERC20.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/abis/MockERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/deployments/deployment.arbitrumSepolia.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/deployments/deployment.arbitrumSepolia.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/deployments/deployment.blastMainnet.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/deployments/deployment.blastMainnet.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/deployments/deployment.test.json` & `vertex_protocol-2.0.1/vertex_protocol/contracts/deployments/deployment.test.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/eip712/domain.py` & `vertex_protocol-2.0.1/vertex_protocol/contracts/eip712/domain.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/eip712/sign.py` & `vertex_protocol-2.0.1/vertex_protocol/contracts/eip712/sign.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/eip712/types.py` & `vertex_protocol-2.0.1/vertex_protocol/contracts/eip712/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/loader.py` & `vertex_protocol-2.0.1/vertex_protocol/contracts/loader.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/contracts/types.py` & `vertex_protocol-2.0.1/vertex_protocol/contracts/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/engine_client/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/engine_client/execute.py` & `vertex_protocol-2.0.1/vertex_protocol/engine_client/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/engine_client/query.py` & `vertex_protocol-2.0.1/vertex_protocol/engine_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/engine_client/types/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/engine_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/engine_client/types/execute.py` & `vertex_protocol-2.0.1/vertex_protocol/engine_client/types/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/engine_client/types/models.py` & `vertex_protocol-2.0.1/vertex_protocol/engine_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/engine_client/types/query.py` & `vertex_protocol-2.0.1/vertex_protocol/engine_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/indexer_client/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/indexer_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/indexer_client/query.py` & `vertex_protocol-2.0.1/vertex_protocol/indexer_client/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     IndexerResponse,
     IndexerSubaccountSummaryParams,
     IndexerSubaccountSummaryData,
     IndexerSubaccountsData,
     IndexerSubaccountsParams,
     IndexerTokenRewardsData,
     IndexerTokenRewardsParams,
+    IndexerUsdcPriceParams,
+    IndexerUsdcPriceData,
     to_indexer_request,
 )
 from vertex_protocol.utils.model import (
     VertexBaseModel,
     ensure_data_type,
     is_instance_of_union,
 )
@@ -365,7 +367,13 @@
         Returns:
             IndexerSubaccountsData: List of subaccounts found.
         """
         return ensure_data_type(
             self.query(params).data,
             IndexerSubaccountsData,
         )
+
+    def get_usdc_price(self) -> IndexerUsdcPriceData:
+        return ensure_data_type(
+            self.query(IndexerUsdcPriceParams()).data,
+            IndexerUsdcPriceData,
+        )
```

### Comparing `vertex_protocol-2.0.0/vertex_protocol/indexer_client/types/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/indexer_client/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,8 +104,9 @@
     "IndexerAddressReward",
     "IndexerGlobalRewards",
     "IndexerTokenReward",
     "IndexerMarketMakerData",
     "IndexerMarketMaker",
     "IndexerLiquidatableAccount",
     "IndexerSubaccount",
+    "IndexerUsdcPriceData",
 ]
```

### Comparing `vertex_protocol-2.0.0/vertex_protocol/indexer_client/types/models.py` & `vertex_protocol-2.0.1/vertex_protocol/indexer_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/indexer_client/types/query.py` & `vertex_protocol-2.0.1/vertex_protocol/indexer_client/types/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     ORACLE_PRICES = "oracle_price"
     REWARDS = "rewards"
     MAKER_STATISTICS = "maker_statistics"
     LIQUIDATION_FEED = "liquidation_feed"
     LINKED_SIGNER_RATE_LIMIT = "linked_signer_rate_limit"
     REFERRAL_CODE = "referral_code"
     SUBACCOUNTS = "subaccounts"
+    USDC_PRICE = "usdc_price"
 
 
 class IndexerBaseParams(VertexBaseModel):
     """
     Base parameters for the indexer queries.
     """
 
@@ -221,14 +222,22 @@
     """
 
     address: Optional[str]
     limit: Optional[int]
     start: Optional[int]
 
 
+class IndexerUsdcPriceParams(VertexBaseModel):
+    """
+    Parameters for querying usdc price.
+    """
+
+    pass
+
+
 IndexerParams = Union[
     IndexerSubaccountHistoricalOrdersParams,
     IndexerHistoricalOrdersByDigestParams,
     IndexerMatchesParams,
     IndexerEventsParams,
     IndexerSubaccountSummaryParams,
     IndexerProductSnapshotsParams,
@@ -238,14 +247,15 @@
     IndexerOraclePricesParams,
     IndexerTokenRewardsParams,
     IndexerMakerStatisticsParams,
     IndexerLiquidationFeedParams,
     IndexerLinkedSignerRateLimitParams,
     IndexerReferralCodeParams,
     IndexerSubaccountsParams,
+    IndexerUsdcPriceParams,
 ]
 
 
 class IndexerHistoricalOrdersRequest(VertexBaseModel):
     """
     Request object for querying historical orders.
     """
@@ -371,14 +381,22 @@
     """
     Request object for querying subaccounts.
     """
 
     subaccounts: IndexerSubaccountsParams
 
 
+class IndexerUsdcPriceRequest(VertexBaseModel):
+    """
+    Request object for querying usdc price.
+    """
+
+    usdc_price: IndexerUsdcPriceParams
+
+
 IndexerRequest = Union[
     IndexerHistoricalOrdersRequest,
     IndexerMatchesRequest,
     IndexerEventsRequest,
     IndexerSubaccountSummaryRequest,
     IndexerProductSnapshotsRequest,
     IndexerCandlesticksRequest,
@@ -387,14 +405,15 @@
     IndexerOraclePricesRequest,
     IndexerTokenRewardsRequest,
     IndexerMakerStatisticsRequest,
     IndexerLiquidationFeedRequest,
     IndexerLinkedSignerRateLimitRequest,
     IndexerReferralCodeRequest,
     IndexerSubaccountsRequest,
+    IndexerUsdcPriceRequest,
 ]
 
 
 class IndexerHistoricalOrdersData(VertexBaseModel):
     """
     Data object for historical orders.
     """
@@ -519,14 +538,22 @@
     """
     Data object for subaccounts response from the indexer.
     """
 
     subaccounts: list[IndexerSubaccount]
 
 
+class IndexerUsdcPriceData(VertexBaseModel):
+    """
+    Data object for the usdc price response from the indexer.
+    """
+
+    price_x18: str
+
+
 IndexerLiquidationFeedData = list[IndexerLiquidatableAccount]
 
 
 IndexerResponseData = Union[
     IndexerHistoricalOrdersData,
     IndexerMatchesData,
     IndexerEventsData,
@@ -537,14 +564,15 @@
     IndexerPerpPricesData,
     IndexerOraclePricesData,
     IndexerTokenRewardsData,
     IndexerMakerStatisticsData,
     IndexerLinkedSignerRateLimitData,
     IndexerReferralCodeData,
     IndexerSubaccountsData,
+    IndexerUsdcPriceData,
     IndexerLiquidationFeedData,
     IndexerFundingRatesData,
 ]
 
 
 class IndexerResponse(VertexBaseModel):
     """
@@ -626,11 +654,15 @@
             IndexerReferralCodeRequest,
             IndexerQueryType.REFERRAL_CODE.value,
         ),
         IndexerSubaccountsParams: (
             IndexerSubaccountsRequest,
             IndexerQueryType.SUBACCOUNTS.value,
         ),
+        IndexerUsdcPriceParams: (
+            IndexerUsdcPriceRequest,
+            IndexerQueryType.USDC_PRICE.value,
+        ),
     }
 
     RequestClass, field_name = indexer_request_mapping[type(params)]
     return RequestClass(**{field_name: params})
```

### Comparing `vertex_protocol-2.0.0/vertex_protocol/utils/__init__.py` & `vertex_protocol-2.0.1/vertex_protocol/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/utils/backend.py` & `vertex_protocol-2.0.1/vertex_protocol/utils/backend.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/utils/bytes32.py` & `vertex_protocol-2.0.1/vertex_protocol/utils/bytes32.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/utils/exceptions.py` & `vertex_protocol-2.0.1/vertex_protocol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/utils/expiration.py` & `vertex_protocol-2.0.1/vertex_protocol/utils/expiration.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/utils/math.py` & `vertex_protocol-2.0.1/vertex_protocol/utils/math.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/utils/model.py` & `vertex_protocol-2.0.1/vertex_protocol/utils/model.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/vertex_protocol/utils/nonce.py` & `vertex_protocol-2.0.1/vertex_protocol/utils/nonce.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-2.0.0/PKG-INFO` & `vertex_protocol-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertex-protocol
-Version: 2.0.0
+Version: 2.0.1
 Summary: Vertex Protocol SDK
 Home-page: https://vertexprotocol.com/
 Keywords: vertex protocol,vertex sdk,vertex protocol api
 Author: Jeury Mejia
 Author-email: jeury@vertexprotocol.com
 Maintainer: Frank Jia
 Maintainer-email: frank@vertexprotocol.com
```

