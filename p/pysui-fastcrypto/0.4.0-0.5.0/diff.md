# Comparing `tmp/pysui_fastcrypto-0.4.0.tar.gz` & `tmp/pysui_fastcrypto-0.5.0.tar.gz`

## Comparing `pysui_fastcrypto-0.4.0.tar` & `pysui_fastcrypto-0.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.4.0/Cargo.toml
--rw-r--r--   0      501       20       48 2023-08-26 12:21:35.000000 pysui_fastcrypto-0.4.0/.gitignore
--rw-r--r--   0      501       20     1695 2023-12-10 09:45:45.000000 pysui_fastcrypto-0.4.0/CHANGELOG.md
--rw-r--r--   0      501       20    11357 2023-07-23 20:18:01.000000 pysui_fastcrypto-0.4.0/LICENSE
--rw-r--r--   0      501       20     1413 2023-07-30 09:00:32.000000 pysui_fastcrypto-0.4.0/README.rst
--rw-r--r--   0      501       20       28 2023-10-18 08:48:40.000000 pysui_fastcrypto-0.4.0/requirements.txt
--rw-r--r--   0      501       20    20582 2023-12-10 09:32:08.000000 pysui_fastcrypto-0.4.0/src/lib.rs
--rw-r--r--   0      501       20    54555 2023-12-09 20:49:55.000000 pysui_fastcrypto-0.4.0/Cargo.lock
--rw-r--r--   0      501       20      723 2023-10-18 09:03:01.000000 pysui_fastcrypto-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1969 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.5.0/Cargo.toml
+-rw-r--r--   0      501       20       48 2023-08-26 12:21:35.000000 pysui_fastcrypto-0.5.0/.gitignore
+-rw-r--r--   0      501       20     1856 2024-04-05 10:02:16.000000 pysui_fastcrypto-0.5.0/CHANGELOG.md
+-rw-r--r--   0      501       20    11357 2023-07-23 20:18:01.000000 pysui_fastcrypto-0.5.0/LICENSE
+-rw-r--r--   0      501       20     1413 2023-07-30 09:00:32.000000 pysui_fastcrypto-0.5.0/README.rst
+-rw-r--r--   0      501       20       28 2024-04-05 08:36:52.000000 pysui_fastcrypto-0.5.0/requirements.txt
+-rw-r--r--   0      501       20    21358 2024-04-05 10:11:24.000000 pysui_fastcrypto-0.5.0/src/lib.rs
+-rw-r--r--   0      501       20    49721 2024-04-05 09:56:19.000000 pysui_fastcrypto-0.5.0/Cargo.lock
+-rw-r--r--   0      501       20      723 2023-10-18 09:03:01.000000 pysui_fastcrypto-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1969 1970-01-01 00:00:00.000000 pysui_fastcrypto-0.5.0/PKG-INFO
```

### Comparing `pysui_fastcrypto-0.4.0/Cargo.toml` & `pysui_fastcrypto-0.5.0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "pysui-fastcrypto"
-version = "0.4.0"
+version = "0.5.0"
 license = "Apache-2.0"
 edition = "2021"
 
 [lib]
 name = "pysui_fastcrypto"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
 
 [dependencies]
 anyhow = "1.0.71"
 base64ct = "1.6.0"
 bip32 = "0.5.1"
-fastcrypto = "0.1.7"
+fastcrypto = "0.1.8"
 slip10_ed25519 = "0.1.3"
 tiny-bip39 = "1.0.0"
 
 [dependencies.pyo3]
 version = "0.20.0"
 # "abi3-py37" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.10
 features = ["abi3-py310"]
```

### Comparing `pysui_fastcrypto-0.4.0/CHANGELOG.md` & `pysui_fastcrypto-0.5.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.5.0] - 2024-04-05
+
+### Added
+
+- [enhancement](https://github.com/FrankC01/pysui-fastcrypto/issues/5) - bech32 support
+
+### Fixed
+
+### Changed
+
+### Removed
+
 ## [0.4.0] - 2023-12-10
 
 ### Added
 
 - [enhancement](https://github.com/FrankC01/pysui-fastcrypto/issues/4)
 
 ### Fixed
 
 ### Changed
 
-
 ### Removed
 
 ## [0.3.0] - 2023-10-25
 
 ### Added
 
 ### Fixed
```

### Comparing `pysui_fastcrypto-0.4.0/LICENSE` & `pysui_fastcrypto-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysui_fastcrypto-0.4.0/README.rst` & `pysui_fastcrypto-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pysui_fastcrypto-0.4.0/src/lib.rs` & `pysui_fastcrypto-0.5.0/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 use anyhow::{anyhow, Result};
 use base64ct::Encoding as _;
 use bip32::{ChildNumber, DerivationPath, XPrv};
 use bip39::{Language, Mnemonic, MnemonicType, Seed};
 
 use fastcrypto::{
     ed25519::{Ed25519KeyPair, Ed25519PrivateKey, Ed25519PublicKey, Ed25519Signature},
+    encoding::Bech32,
     hash::{Blake2b256, HashFunction},
     secp256k1::{Secp256k1KeyPair, Secp256k1PrivateKey, Secp256k1PublicKey, Secp256k1Signature},
     secp256r1::{Secp256r1KeyPair, Secp256r1PrivateKey, Secp256r1PublicKey, Secp256r1Signature},
     traits::{KeyPair, Signer, ToFromBytes, VerifyingKey},
 };
 use slip10_ed25519::derive_ed25519_private_key;
 use std::{collections::VecDeque, str::FromStr};
@@ -514,21 +515,42 @@
         &Base64::decode(&sig).unwrap(),
     ) {
         Ok(_) => true,
         Err(_) => false,
     }
 }
 
+/// Decode a bech32 signature to a Sui key set (sig, pub, prv)
+#[pyfunction]
+pub fn decode_bech32(key_string: String, hrp: String) -> (u8, Vec<u8>, Vec<u8>) {
+    let kbytes = match Bech32::decode(&key_string, &hrp) {
+        Ok(v) => v,
+        Err(_e) => return (255, [].into(), [].into()),
+    };
+    // let in_str = Base64::encode(kbytes);
+    keys_from_keystring(Base64::encode(kbytes))
+}
+
+/// Enchode a key from 'sig_scheme | prv_bytes' to bech32
+#[pyfunction]
+pub fn encode_bech32(prv_bytes: Vec<u8>, hrp: String) -> String {
+    match Bech32::encode(prv_bytes, &hrp) {
+        Ok(r) => r,
+        Err(_) => String::new(),
+    }
+}
 /// The pysui_fastcrypto module implemented in Rust.  In order
 /// to import the function name must match the Cargo.toml name
 #[pymodule]
 fn pysui_fastcrypto(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(keys_from_keystring, m)?)?;
     m.add_function(wrap_pyfunction!(keys_from_mnemonics, m)?)?;
     m.add_function(wrap_pyfunction!(generate_new_keypair, m)?)?;
     m.add_function(wrap_pyfunction!(generate_mnemonic_phrase, m)?)?;
     m.add_function(wrap_pyfunction!(sign_digest, m)?)?;
     m.add_function(wrap_pyfunction!(sign_message, m)?)?;
     m.add_function(wrap_pyfunction!(verify, m)?)?;
+    m.add_function(wrap_pyfunction!(decode_bech32, m)?)?;
+    m.add_function(wrap_pyfunction!(encode_bech32, m)?)?;
 
     Ok(())
 }
```

### Comparing `pysui_fastcrypto-0.4.0/Cargo.lock` & `pysui_fastcrypto-0.5.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -14,49 +14,14 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
-name = "aead"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d122413f284cf2d62fb1b7db97e02edb8cda96d769b16e443a4f6195e35662b0"
-dependencies = [
- "crypto-common",
- "generic-array",
-]
-
-[[package]]
-name = "aes"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac1f845298e95f983ff1944b728ae08b8cebab80d684f0a832ed0fc74dfa27e2"
-dependencies = [
- "cfg-if",
- "cipher",
- "cpufeatures",
-]
-
-[[package]]
-name = "aes-gcm"
-version = "0.10.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "209b47e8954a928e1d72e86eca7000ebb6655fe1436d33eefc2201cad027e237"
-dependencies = [
- "aead",
- "aes",
- "cipher",
- "ctr",
- "ghash",
- "subtle",
-]
-
-[[package]]
 name = "ahash"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
  "cfg-if",
  "once_cell",
@@ -198,26 +163,14 @@
 checksum = "94893f1e0c6eeab764ade8dc4c0db24caf4fe7cbbaafc0eba0a9030f447b5185"
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
-name = "arrayref"
-version = "0.3.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
-
-[[package]]
-name = "arrayvec"
-version = "0.7.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
-
-[[package]]
 name = "auto_ops"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7460f7dd8e100147b82a63afca1a20eb6c231ee36b90ba7272e14951cb58af59"
 
 [[package]]
 name = "autocfg"
@@ -255,14 +208,20 @@
 [[package]]
 name = "base64ct"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c3c1a368f70d6cf7302d78f8f7093da241fb8e8807c05cc9e51a125895a6d5b"
 
 [[package]]
+name = "bech32"
+version = "0.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d86b93f97252c47b41663388e6d155714a9d0c398b99f1005cbc5f978b29f445"
+
+[[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
@@ -312,62 +271,32 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
  "digest 0.10.7",
 ]
 
 [[package]]
-name = "blake3"
-version = "1.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "199c42ab6972d92c9f8995f086273d25c42fc0f7b2a1fcefba465c1352d25ba5"
-dependencies = [
- "arrayref",
- "arrayvec",
- "cc",
- "cfg-if",
- "constant_time_eq",
- "digest 0.10.7",
-]
-
-[[package]]
 name = "block-buffer"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
 dependencies = [
- "block-padding 0.2.1",
  "generic-array",
 ]
 
 [[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
-name = "block-padding"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d696c370c750c948ada61c69a0ee2cbbb9c50b1019ddb86d9317157a99c2cae"
-
-[[package]]
-name = "block-padding"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8894febbff9f758034a5b8e12d87918f56dfc64a8e1fe757d65e29041538d93"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
 name = "blst"
 version = "0.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a30d0edd9dd1c60ddb42b80341c7852f6f985279a5c1a83659dcb65899dec99"
 dependencies = [
  "cc",
  "glob",
@@ -388,55 +317,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f5353f36341f7451062466f0b755b96ac3a9547e4d7f6b70d603fc721a7d7896"
 dependencies = [
  "sha2 0.10.7",
 ]
 
 [[package]]
-name = "bulletproofs"
-version = "4.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40e698f1df446cc6246afd823afbe2d121134d089c9102c1dd26d1264991ba32"
-dependencies = [
- "byteorder",
- "clear_on_drop",
- "curve25519-dalek-ng",
- "digest 0.9.0",
- "merlin",
- "rand",
- "rand_core",
- "serde",
- "serde_derive",
- "sha3 0.9.1",
- "subtle-ng",
- "thiserror",
-]
-
-[[package]]
 name = "bumpalo"
 version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
 [[package]]
-name = "cbc"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26b52a9543ae338f279b96b0b9fed9c8093744685043739079ce85cd58f289a6"
-dependencies = [
- "cipher",
-]
-
-[[package]]
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
@@ -454,45 +354,20 @@
  "iana-time-zone",
  "num-traits",
  "serde",
  "winapi",
 ]
 
 [[package]]
-name = "cipher"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
-dependencies = [
- "crypto-common",
- "inout",
-]
-
-[[package]]
-name = "clear_on_drop"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38508a63f4979f0048febc9966fadbd48e5dab31fd0ec6a3f151bbf4a74f7423"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "const-oid"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "795bc6e66a8e340f075fcf6227e417a2dc976b92b91f3cdc778bb858778b6747"
 
 [[package]]
-name = "constant_time_eq"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7144d30dcf0fafbce74250a3963025d8d52177934239851c917d29f1df280c2"
-
-[[package]]
 name = "convert_case"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6245d59a3e82a7fc217c5828a6692dbc6dfb63a0c8c90495621f7b9d79704a0e"
 
 [[package]]
 name = "convert_case"
@@ -533,37 +408,26 @@
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
- "rand_core",
  "typenum",
 ]
 
 [[package]]
-name = "ctr"
-version = "0.9.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0369ee1ad671834580515889b80f2ea915f23b8be8d0daa4bbaf2ac5c7590835"
-dependencies = [
- "cipher",
-]
-
-[[package]]
 name = "curve25519-dalek-ng"
 version = "4.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c359b7249347e46fb28804470d071c921156ad62b3eef5d34e2ba867533dec8"
 dependencies = [
  "byteorder",
  "digest 0.9.0",
  "rand_core",
- "serde",
  "subtle-ng",
  "zeroize",
 ]
 
 [[package]]
 name = "darling"
 version = "0.20.3"
@@ -735,61 +599,56 @@
 dependencies = [
  "indenter",
  "once_cell",
 ]
 
 [[package]]
 name = "fastcrypto"
-version = "0.1.7"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2bca1e2b84f89b70d452d426fc7d4c0354375375af31d85d677062278d5dd2fd"
+checksum = "4f9ea2139faa96e4d713803b7777b8fd2d5c245858b1644c08d3220f407149c6"
 dependencies = [
- "aes",
- "aes-gcm",
  "ark-ec",
  "ark-ff",
  "ark-secp256r1",
  "ark-serialize",
  "auto_ops",
  "base64ct",
+ "bech32",
  "bincode",
  "blake2",
- "blake3",
  "blst",
  "bs58 0.4.0",
- "bulletproofs",
- "cbc",
- "ctr",
  "curve25519-dalek-ng",
  "derive_more",
  "digest 0.10.7",
  "ecdsa",
  "ed25519-consensus",
  "elliptic-curve",
  "eyre",
  "fastcrypto-derive",
  "generic-array",
  "hex",
+ "hex-literal",
  "hkdf",
  "lazy_static",
- "merlin",
+ "num-bigint",
  "once_cell",
  "p256",
  "rand",
  "readonly",
  "rfc6979",
  "rsa",
  "schemars",
  "secp256k1",
  "serde",
- "serde_bytes",
  "serde_json",
  "serde_with",
  "sha2 0.10.7",
- "sha3 0.10.8",
+ "sha3",
  "signature",
  "static_assertions",
  "thiserror",
  "tokio",
  "typenum",
  "zeroize",
 ]
@@ -842,24 +701,14 @@
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
-name = "ghash"
-version = "0.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d930750de5717d2dd0b8c0d42c076c0e884c81a73e6cab859bbd2339c71e3e40"
-dependencies = [
- "opaque-debug",
- "polyval",
-]
-
-[[package]]
 name = "gimli"
 version = "0.27.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6c80984affa11d98d1b88b66ac8853f143217b399d3c74116778ff8fdb4ed2e"
 
 [[package]]
 name = "glob"
@@ -908,14 +757,20 @@
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
+name = "hex-literal"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fe2267d4ed49bc07b63801559be28c718ea06c4738b7a03c94df7386d2cde46"
+
+[[package]]
 name = "hkdf"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "791a029f6b9fc27657f6f188ec6e5e43f6911f6f878e0dc5501396e09809d437"
 dependencies = [
  "hmac",
 ]
@@ -984,24 +839,14 @@
 [[package]]
 name = "indoc"
 version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
 
 [[package]]
-name = "inout"
-version = "0.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
-dependencies = [
- "block-padding 0.3.3",
- "generic-array",
-]
-
-[[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
@@ -1091,39 +936,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "merlin"
-version = "3.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58c38e2799fc0978b65dfff8023ec7843e2330bb462f19198840b34b6582397d"
-dependencies = [
- "byteorder",
- "keccak",
- "rand_core",
- "zeroize",
-]
-
-[[package]]
 name = "miniz_oxide"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.3"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f93ab6289c7b344a8a9f60f88d80aa20032336fe78da341afc91c8a2341fc75f"
+checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
@@ -1162,17 +995,17 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -1318,26 +1151,14 @@
 checksum = "f950b2377845cebe5cf8b5165cb3cc1a5e0fa5cfa3e1f7f55707d8fd82e0a7b7"
 dependencies = [
  "der 0.7.7",
  "spki 0.7.2",
 ]
 
 [[package]]
-name = "polyval"
-version = "0.6.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d52cff9d1d4dee5fe6d03729099f4a310a41179e0a10dbf542039873f2e826fb"
-dependencies = [
- "cfg-if",
- "cpufeatures",
- "opaque-debug",
- "universal-hash",
-]
-
-[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "primeorder"
@@ -1416,15 +1237,15 @@
  "proc-macro2",
  "quote",
  "syn 2.0.26",
 ]
 
 [[package]]
 name = "pysui-fastcrypto"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "anyhow",
  "base64ct",
  "bip32",
  "fastcrypto",
  "pyo3",
  "slip10_ed25519",
@@ -1633,23 +1454,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "30e27d1e4fd7659406c492fd6cfaf2066ba8773de45ca75e855590f856dc34a9"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
-name = "serde_bytes"
-version = "0.11.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab33ec92f677585af6d88c65593ae2375adde54efdbf16d597f2cbc7a6d368ff"
-dependencies = [
- "serde",
-]
-
-[[package]]
 name = "serde_derive"
 version = "1.0.171"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "389894603bd18c46fa56231694f8d827779c0951a667087194cf9de94ed24682"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -1728,26 +1540,14 @@
  "cfg-if",
  "cpufeatures",
  "digest 0.10.7",
 ]
 
 [[package]]
 name = "sha3"
-version = "0.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f81199417d4e5de3f04b1e871023acea7389672c4135918f05aa9cbf2f2fa809"
-dependencies = [
- "block-buffer 0.9.0",
- "digest 0.9.0",
- "keccak",
- "opaque-debug",
-]
-
-[[package]]
-name = "sha3"
 version = "0.10.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75872d278a8f37ef87fa0ddbda7802605cb18344497949862c0d4dcb291eba60"
 dependencies = [
  "digest 0.10.7",
  "keccak",
 ]
@@ -1998,24 +1798,14 @@
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
-name = "universal-hash"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc1de2c688dc15305988b563c3854064043356019f97a4b46276fe734c4f07ea"
-dependencies = [
- "crypto-common",
- "subtle",
-]
-
-[[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "wasi"
```

### Comparing `pysui_fastcrypto-0.4.0/pyproject.toml` & `pysui_fastcrypto-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysui_fastcrypto-0.4.0/PKG-INFO` & `pysui_fastcrypto-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pysui-fastcrypto
-Version: 0.4.0
+Version: 0.5.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 License-File: LICENSE
 Summary: Python wrapper for MystenLab/fastcrypto Rust crate
 License: Apache-2.0
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst; charset=UTF-8
```

