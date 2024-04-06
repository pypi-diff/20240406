# Comparing `tmp/spiffe-0.1.1.tar.gz` & `tmp/spiffe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiffe-0.1.1.tar", max compression
+gzip compressed data, was "spiffe-0.1.2.tar", max compression
```

## Comparing `spiffe-0.1.1.tar` & `spiffe-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2024-04-01 01:10:11.588779 spiffe-0.1.1/LICENSE
--rw-r--r--   0        0        0     2550 2024-04-01 01:10:11.588779 spiffe-0.1.1/README.md
--rw-r--r--   0        0        0     1011 2024-04-01 01:10:11.588779 spiffe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      698 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/__init__.py
--rw-r--r--   0        0        0       79 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/__init__.py
--rw-r--r--   0        0        0       65 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/jwt_bundle/__init__.py
--rw-r--r--   0        0        0     1249 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/jwt_bundle/errors.py
--rw-r--r--   0        0        0     5199 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/jwt_bundle/jwt_bundle.py
--rw-r--r--   0        0        0     2885 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/jwt_bundle/jwt_bundle_set.py
--rw-r--r--   0        0        0       66 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/x509_bundle/__init__.py
--rw-r--r--   0        0        0     1477 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/x509_bundle/errors.py
--rw-r--r--   0        0        0     7730 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/x509_bundle/x509_bundle.py
--rw-r--r--   0        0        0     3088 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/bundle/x509_bundle/x509_bundle_set.py
--rw-r--r--   0        0        0     4854 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/config.py
--rw-r--r--   0        0        0      827 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/errors.py
--rw-r--r--   0        0        0        0 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/proto/__init__.py
--rw-r--r--   0        0        0     6465 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/proto/workload.proto
--rw-r--r--   0        0        0     5506 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/proto/workload_pb2.py
--rw-r--r--   0        0        0    13463 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/proto/workload_pb2.pyi
--rw-r--r--   0        0        0    10240 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/proto/workload_pb2_grpc.py
--rw-r--r--   0        0        0       70 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/spiffe_id/__init__.py
--rw-r--r--   0        0        0     6828 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/spiffe_id/spiffe_id.py
--rw-r--r--   0        0        0       55 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/svid/__init__.py
--rw-r--r--   0        0        0     2538 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/svid/errors.py
--rw-r--r--   0        0        0     7598 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/svid/jwt_svid.py
--rw-r--r--   0        0        0     5173 2024-04-01 01:10:11.588779 spiffe-0.1.1/src/spiffe/svid/jwt_svid_validator.py
--rw-r--r--   0        0        0    13724 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/svid/x509_svid.py
--rw-r--r--   0        0        0        0 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/utils/__init__.py
--rw-r--r--   0        0        0     8749 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/utils/certificate_utils.py
--rw-r--r--   0        0        0     2204 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/utils/errors.py
--rw-r--r--   0        0        0       85 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/errors.py
--rw-r--r--   0        0        0       69 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/grpc/__init__.py
--rw-r--r--   0        0        0     2505 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/grpc/generic_client_interceptor.py
--rw-r--r--   0        0        0     1664 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/grpc/header_manipulator_client_interceptor.py
--rw-r--r--   0        0        0     1595 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/handle_error.py
--rw-r--r--   0        0        0     9424 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/jwt_source.py
--rw-r--r--   0        0        0    22853 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/workload_api_client.py
--rw-r--r--   0        0        0     2321 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/x509_context.py
--rw-r--r--   0        0        0     8794 2024-04-01 01:10:11.592779 spiffe-0.1.1/src/spiffe/workloadapi/x509_source.py
--rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 spiffe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-06 17:45:28.701950 spiffe-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2595 2024-04-06 17:45:28.701950 spiffe-0.1.2/README.md
+-rw-r--r--   0        0        0     1070 2024-04-06 17:45:28.701950 spiffe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      698 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/__init__.py
+-rw-r--r--   0        0        0       79 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/jwt_bundle/__init__.py
+-rw-r--r--   0        0        0     1249 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/jwt_bundle/errors.py
+-rw-r--r--   0        0        0     5528 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/jwt_bundle/jwt_bundle.py
+-rw-r--r--   0        0        0     2885 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/jwt_bundle/jwt_bundle_set.py
+-rw-r--r--   0        0        0       66 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/x509_bundle/__init__.py
+-rw-r--r--   0        0        0     1477 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/x509_bundle/errors.py
+-rw-r--r--   0        0        0     7730 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/x509_bundle/x509_bundle.py
+-rw-r--r--   0        0        0     3088 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/bundle/x509_bundle/x509_bundle_set.py
+-rw-r--r--   0        0        0     4854 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/config.py
+-rw-r--r--   0        0        0      827 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/errors.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/proto/__init__.py
+-rw-r--r--   0        0        0     6465 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/proto/workload.proto
+-rw-r--r--   0        0        0     5506 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/proto/workload_pb2.py
+-rw-r--r--   0        0        0    13463 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/proto/workload_pb2.pyi
+-rw-r--r--   0        0        0    10240 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/proto/workload_pb2_grpc.py
+-rw-r--r--   0        0        0       70 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/spiffe_id/__init__.py
+-rw-r--r--   0        0        0     6828 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/spiffe_id/spiffe_id.py
+-rw-r--r--   0        0        0       55 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/svid/__init__.py
+-rw-r--r--   0        0        0     2538 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/svid/errors.py
+-rw-r--r--   0        0        0     7598 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/svid/jwt_svid.py
+-rw-r--r--   0        0        0     5173 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/svid/jwt_svid_validator.py
+-rw-r--r--   0        0        0    13724 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/svid/x509_svid.py
+-rw-r--r--   0        0        0        0 2024-04-06 17:45:28.701950 spiffe-0.1.2/src/spiffe/utils/__init__.py
+-rw-r--r--   0        0        0     8749 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/utils/certificate_utils.py
+-rw-r--r--   0        0        0     2204 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/utils/errors.py
+-rw-r--r--   0        0        0       85 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/errors.py
+-rw-r--r--   0        0        0       69 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/grpc/__init__.py
+-rw-r--r--   0        0        0     2505 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/grpc/generic_client_interceptor.py
+-rw-r--r--   0        0        0     1664 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/grpc/header_manipulator_client_interceptor.py
+-rw-r--r--   0        0        0     1595 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/handle_error.py
+-rw-r--r--   0        0        0     9424 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/jwt_source.py
+-rw-r--r--   0        0        0    22853 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/workload_api_client.py
+-rw-r--r--   0        0        0     2321 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/x509_context.py
+-rw-r--r--   0        0        0     8794 2024-04-06 17:45:28.705950 spiffe-0.1.2/src/spiffe/workloadapi/x509_source.py
+-rw-r--r--   0        0        0     3516 1970-01-01 00:00:00.000000 spiffe-0.1.2/PKG-INFO
```

### Comparing `spiffe-0.1.1/LICENSE` & `spiffe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/README.md` & `spiffe-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # `spiffe` package
 
 ## Overview
 
-The `spiffe` package, part of the `py-spiffe` library, provides [SPIFFE](https://spiffe.io) support and essential
+The `spiffe` package, part of the [py-spiffe library](https://github.com/HewlettPackard/py-spiffe),
+provides [SPIFFE](https://spiffe.io) support and essential
 tools for interacting with
 the [SPIFFE Workload API](https://github.com/spiffe/spiffe/blob/main/standards/SPIFFE_Workload_API.md). It simplifies
 the management and validation of SPIFFE identities,
 supporting [X509-SVIDs](https://github.com/spiffe/spiffe/blob/main/standards/X509-SVID.md), [JWT-SVIDs](https://github.com/spiffe/spiffe/blob/main/standards/JWT-SVID.md),
 and X.509 CA and JWKS Bundles.
 
 # Features
```

### Comparing `spiffe-0.1.1/pyproject.toml` & `spiffe-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "spiffe"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python library for SPIFFE support"
 authors = ["Max Lambrecht <maxlambrecht@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
+repository = "https://github.com/HewlettPackard/py-spiffe"
 
 [tool.poetry.dependencies]
 python = "^3.9" # >= 3.9, < 4.0
 grpcio = "^1.62"
 cryptography = "^42.0"
 pyjwt = { version = "^2.0", extras = ["crypto"] }
 pyasn1 = "~0.6.0"
 pyasn1-modules = "~0.4.0"
 pem = "^23.0"
 
 [tool.poetry.dev-dependencies]
 black = "^24.3"
 mypy = "^1.9"
-mypy-protobuf = "^3.0"
+mypy-protobuf = "^3.6"
 pytest = "^8.1"
 pytest-mock = "^3.0"
 pre-commit = "^3.7"
 flake8 = "^7.0"
 testutils = { path = "../testutils" }
 
 [build-system]
```

### Comparing `spiffe-0.1.1/src/spiffe/__init__.py` & `spiffe-0.1.2/src/spiffe/__init__.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/bundle/jwt_bundle/errors.py` & `spiffe-0.1.2/src/spiffe/bundle/jwt_bundle/errors.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/bundle/jwt_bundle/jwt_bundle.py` & `spiffe-0.1.2/src/spiffe/bundle/jwt_bundle/jwt_bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,32 +114,39 @@
             raise ArgumentError("Trust domain cannot be empty")
 
         if not bundle_bytes:
             raise ArgumentError('Bundle bytes cannot be empty')
 
         try:
             jwks = PyJWKSet.from_json(bundle_bytes.decode('utf-8'))
+
+            jwt_authorities = {}
+            for jwk in jwks.keys:
+                if not jwk.key_id:
+                    raise ParseJWTBundleError(
+                        'Error adding authority from JWKS: "keyID" cannot be empty'
+                    )
+
+                jwt_authorities[jwk.key_id] = jwk.key
+
+            return JwtBundle(trust_domain, jwt_authorities)
         except InvalidKeyError as err:
             raise ParseJWTBundleError(str(err)) from err
-        except (PyJWKSetError, JSONDecodeError, AttributeError) as err:
+        except PyJWKSetError as err:
+            if str(err) == "The JWK Set did not contain any keys":
+                return JwtBundle(trust_domain, {})
+            else:
+                raise ParseJWTBundleError(
+                    '"bundle_bytes" does not represent a valid jwks'
+                ) from err
+        except (JSONDecodeError, AttributeError) as err:
             raise ParseJWTBundleError(
                 '"bundle_bytes" does not represent a valid jwks'
             ) from err
 
-        jwt_authorities = {}
-        for jwk in jwks.keys:
-            if not jwk.key_id:
-                raise ParseJWTBundleError(
-                    'Error adding authority from JWKS: "keyID" cannot be empty'
-                )
-
-            jwt_authorities[jwk.key_id] = jwk.key
-
-        return JwtBundle(trust_domain, jwt_authorities)
-
     def __eq__(self, o: object) -> bool:
         if not isinstance(o, JwtBundle):
             return False
         with self.lock:
             return (
                 self._trust_domain.__eq__(o._trust_domain)
                 and self._jwt_authorities == o._jwt_authorities
```

### Comparing `spiffe-0.1.1/src/spiffe/bundle/jwt_bundle/jwt_bundle_set.py` & `spiffe-0.1.2/src/spiffe/bundle/jwt_bundle/jwt_bundle_set.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/bundle/x509_bundle/errors.py` & `spiffe-0.1.2/src/spiffe/bundle/x509_bundle/errors.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/bundle/x509_bundle/x509_bundle.py` & `spiffe-0.1.2/src/spiffe/bundle/x509_bundle/x509_bundle.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/bundle/x509_bundle/x509_bundle_set.py` & `spiffe-0.1.2/src/spiffe/bundle/x509_bundle/x509_bundle_set.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/config.py` & `spiffe-0.1.2/src/spiffe/config.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/errors.py` & `spiffe-0.1.2/src/spiffe/errors.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/proto/workload.proto` & `spiffe-0.1.2/src/spiffe/proto/workload.proto`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/proto/workload_pb2.py` & `spiffe-0.1.2/src/spiffe/proto/workload_pb2.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/proto/workload_pb2.pyi` & `spiffe-0.1.2/src/spiffe/proto/workload_pb2.pyi`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/proto/workload_pb2_grpc.py` & `spiffe-0.1.2/src/spiffe/proto/workload_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/spiffe_id/spiffe_id.py` & `spiffe-0.1.2/src/spiffe/spiffe_id/spiffe_id.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/svid/errors.py` & `spiffe-0.1.2/src/spiffe/svid/errors.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/svid/jwt_svid.py` & `spiffe-0.1.2/src/spiffe/svid/jwt_svid.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/svid/jwt_svid_validator.py` & `spiffe-0.1.2/src/spiffe/svid/jwt_svid_validator.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/svid/x509_svid.py` & `spiffe-0.1.2/src/spiffe/svid/x509_svid.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/utils/certificate_utils.py` & `spiffe-0.1.2/src/spiffe/utils/certificate_utils.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/utils/errors.py` & `spiffe-0.1.2/src/spiffe/utils/errors.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/workloadapi/errors.py` & `spiffe-0.1.2/src/spiffe/workloadapi/errors.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/workloadapi/grpc/generic_client_interceptor.py` & `spiffe-0.1.2/src/spiffe/workloadapi/grpc/generic_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/workloadapi/grpc/header_manipulator_client_interceptor.py` & `spiffe-0.1.2/src/spiffe/workloadapi/grpc/header_manipulator_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/workloadapi/handle_error.py` & `spiffe-0.1.2/src/spiffe/workloadapi/handle_error.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/workloadapi/jwt_source.py` & `spiffe-0.1.2/src/spiffe/workloadapi/jwt_source.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/workloadapi/workload_api_client.py` & `spiffe-0.1.2/src/spiffe/workloadapi/workload_api_client.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/workloadapi/x509_context.py` & `spiffe-0.1.2/src/spiffe/workloadapi/x509_context.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/src/spiffe/workloadapi/x509_source.py` & `spiffe-0.1.2/src/spiffe/workloadapi/x509_source.py`

 * *Files identical despite different names*

### Comparing `spiffe-0.1.1/PKG-INFO` & `spiffe-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: spiffe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python library for SPIFFE support
+Home-page: https://github.com/HewlettPackard/py-spiffe
 License: Apache-2.0
 Author: Max Lambrecht
 Author-email: maxlambrecht@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -14,21 +15,23 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=42.0,<43.0)
 Requires-Dist: grpcio (>=1.62,<2.0)
 Requires-Dist: pem (>=23.0,<24.0)
 Requires-Dist: pyasn1 (>=0.6.0,<0.7.0)
 Requires-Dist: pyasn1-modules (>=0.4.0,<0.5.0)
 Requires-Dist: pyjwt[crypto] (>=2.0,<3.0)
+Project-URL: Repository, https://github.com/HewlettPackard/py-spiffe
 Description-Content-Type: text/markdown
 
 # `spiffe` package
 
 ## Overview
 
-The `spiffe` package, part of the `py-spiffe` library, provides [SPIFFE](https://spiffe.io) support and essential
+The `spiffe` package, part of the [py-spiffe library](https://github.com/HewlettPackard/py-spiffe),
+provides [SPIFFE](https://spiffe.io) support and essential
 tools for interacting with
 the [SPIFFE Workload API](https://github.com/spiffe/spiffe/blob/main/standards/SPIFFE_Workload_API.md). It simplifies
 the management and validation of SPIFFE identities,
 supporting [X509-SVIDs](https://github.com/spiffe/spiffe/blob/main/standards/X509-SVID.md), [JWT-SVIDs](https://github.com/spiffe/spiffe/blob/main/standards/JWT-SVID.md),
 and X.509 CA and JWKS Bundles.
 
 # Features
```

