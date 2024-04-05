# Comparing `tmp/auto-sdk-0.1.2.tar.gz` & `tmp/auto-sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-sdk-0.1.2.tar", last modified: Fri Apr  5 14:23:12 2024, max compression
+gzip compressed data, was "auto-sdk-0.1.3.tar", last modified: Fri Apr  5 23:30:57 2024, max compression
```

## Comparing `auto-sdk-0.1.2.tar` & `auto-sdk-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      274 2024-03-20 21:08:12.000000 auto-sdk-0.1.2/README.md
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/auto_identity/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1101 2024-04-05 14:22:16.000000 auto-sdk-0.1.2/auto_identity/__init__.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     2544 2024-04-04 00:32:25.000000 auto-sdk-0.1.2/auto_identity/certificate_management.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4845 2024-04-05 14:15:46.000000 auto-sdk-0.1.2/auto_identity/key_management.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4040 2024-04-04 00:32:25.000000 auto-sdk-0.1.2/auto_identity/registry.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1232 2024-04-04 00:32:25.000000 auto-sdk-0.1.2/auto_identity/utils.py
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/auto_sdk.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      324 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       84 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/requires.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2024-04-05 14:23:12.000000 auto-sdk-0.1.2/auto_sdk.egg-info/top_level.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-05 14:23:12.192119 auto-sdk-0.1.2/setup.cfg
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      389 2024-04-05 14:22:23.000000 auto-sdk-0.1.2/setup.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      274 2024-03-20 21:08:12.000000 auto-sdk-0.1.3/README.md
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/auto_identity/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      960 2024-04-05 23:30:32.000000 auto-sdk-0.1.3/auto_identity/__init__.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     5558 2024-04-05 23:26:06.000000 auto-sdk-0.1.3/auto_identity/certificate_manager.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     5822 2024-04-05 22:29:31.000000 auto-sdk-0.1.3/auto_identity/key_management.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4040 2024-04-04 00:32:25.000000 auto-sdk-0.1.3/auto_identity/registry.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1232 2024-04-04 00:32:25.000000 auto-sdk-0.1.3/auto_identity/utils.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/auto_sdk.egg-info/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      321 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       84 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/requires.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2024-04-05 23:30:57.000000 auto-sdk-0.1.3/auto_sdk.egg-info/top_level.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-05 23:30:57.607017 auto-sdk-0.1.3/setup.cfg
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      389 2024-04-05 23:30:40.000000 auto-sdk-0.1.3/setup.py
```

### Comparing `auto-sdk-0.1.2/auto_identity/__init__.py` & `auto-sdk-0.1.3/auto_identity/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,31 +12,28 @@
     key_to_hex,
     key_to_pem,
     pem_to_private_key,
     load_private_key,
     pem_to_public_key,
     load_public_key,
     save_key)
-from .certificate_management import create_csr, issue_certificate, self_issue_certificate, get_subject_common_name
+from .certificate_manager import CertificateManager
 from .registry import Registry
 from .utils import der_encode_signature_algorithm_oid
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 __all__ = [
     "generate_rsa_key_pair",
     "generate_ed25519_key_pair",
     "key_to_hex",
     "load_private_key",
     "load_public_key",
     "save_key",
     "pem_to_private_key",
     "pem_to_public_key",
     "key_to_pem",
-    "create_csr",
-    "issue_certificate",
-    "self_issue_certificate",
-    "get_subject_common_name",
+    "CertificateManager",
     "der_encode_signature_algorithm_oid",
     "Registry",
     "Keypair",
 ]
```

### Comparing `auto-sdk-0.1.2/auto_identity/key_management.py` & `auto-sdk-0.1.3/auto_identity/key_management.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,14 +37,17 @@
 def key_to_pem(key, password: str = None) -> str:
     """
     Converts a private or public key to a PEM string.
 
     Args:
         key: The key to convert (private or public).
         password (str): The password used to encrypt the key.
+
+    Returns:
+            str: The PEM string representation of the key.
     """
     if hasattr(key, 'private_bytes'):
         encoding = serialization.Encoding.PEM
         format = serialization.PrivateFormat.PKCS8
         encryption_algorithm = (serialization.BestAvailableEncryption(password.encode())
                                 if password else serialization.NoEncryption())
         key_data = key.private_bytes(encoding, format, encryption_algorithm)
@@ -75,15 +78,21 @@
 def pem_to_private_key(pem_data: str, password: str = None):
     """
     Converts a PEM string to a private or public key. If the PEM string is encrypted, a password must be provided.
 
     Args:
         pem_data (str): The PEM string to convert.
         password (str): The password used to encrypt the key.
+
+    Returns:
+        The private key.
     """
+    # Ensure pem_data is a bytes object
+    if isinstance(pem_data, str):
+        pem_data = pem_data.encode()
 
     private_key = serialization.load_pem_private_key(
         pem_data,
         password=password.encode() if password else None,
         backend=default_backend()
     )
     return private_key
@@ -107,14 +116,17 @@
 
 def pem_to_public_key(pem_data: str):
     """
     Converts a PEM string to a public key.
 
     Args:
         pem_data (str): The PEM string to convert.
+
+    Returns:
+        The public key.
     """
     public_key = serialization.load_pem_public_key(
         pem_data,
         backend=default_backend()
     )
     return public_key
 
@@ -156,7 +168,31 @@
         encoding = serialization.Encoding.DER
         format = serialization.PublicFormat.SubjectPublicKeyInfo
         key_data = key.public_bytes(encoding, format)
     else:
         raise ValueError("Unsupported key type")
 
     return key_data.hex()
+
+
+def do_public_keys_match(public_key_1, public_key_2):
+    """
+    Checks if two public keys match.
+
+    Args:
+        public_key_1: The first public key.
+        public_key_2: The second public key.
+
+    Returns:
+            bool: True if the keys match, False otherwise.
+    """
+    # Serialize public keys to DER format for comparison
+    public_key_1_der = public_key_1.public_bytes(
+        encoding=serialization.Encoding.DER,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo
+    )
+
+    public_key_2_der = public_key_2.public_bytes(
+        encoding=serialization.Encoding.DER,
+        format=serialization.PublicFormat.SubjectPublicKeyInfo
+    )
+    return public_key_1_der == public_key_2_der
```

### Comparing `auto-sdk-0.1.2/auto_identity/registry.py` & `auto-sdk-0.1.3/auto_identity/registry.py`

 * *Files identical despite different names*

### Comparing `auto-sdk-0.1.2/auto_identity/utils.py` & `auto-sdk-0.1.3/auto_identity/utils.py`

 * *Files identical despite different names*

