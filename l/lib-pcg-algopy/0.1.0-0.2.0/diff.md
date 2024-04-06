# Comparing `tmp/lib_pcg_algopy-0.1.0.tar.gz` & `tmp/lib_pcg_algopy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_pcg_algopy-0.1.0.tar", max compression
+gzip compressed data, was "lib_pcg_algopy-0.2.0.tar", max compression
```

## Comparing `lib_pcg_algopy-0.1.0.tar` & `lib_pcg_algopy-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    11636 2024-03-30 21:47:34.838689 lib_pcg_algopy-0.1.0/README.md
--rw-r--r--   0        0        0      181 2024-03-30 22:59:01.748047 lib_pcg_algopy-0.1.0/lib_pcg/__init__.py
--rw-r--r--   0        0        0     2953 2024-03-30 22:21:20.342331 lib_pcg_algopy-0.1.0/lib_pcg/xsh_rr_64_32.py
--rw-r--r--   0        0        0     2448 2024-03-30 22:46:11.403818 lib_pcg_algopy-0.1.0/lib_pcg/xsh_rr_double_64_32.py
--rw-r--r--   0        0        0     1565 2024-03-30 22:55:32.324530 lib_pcg_algopy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    12130 1970-01-01 00:00:00.000000 lib_pcg_algopy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11636 2024-03-30 21:47:34.838689 lib_pcg_algopy-0.2.0/README.md
+-rw-r--r--   0        0        0      303 2024-04-06 15:54:14.290298 lib_pcg_algopy-0.2.0/lib_pcg/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-06 13:55:27.698575 lib_pcg_algopy-0.2.0/lib_pcg/consts.py
+-rw-r--r--   0        0        0     2957 2024-04-06 13:55:57.606432 lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_64_32.py
+-rw-r--r--   0        0        0     2364 2024-04-06 13:56:18.658332 lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_double_64_32.py
+-rw-r--r--   0        0        0     4166 2024-04-06 15:39:05.592300 lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_quadruple_64_32.py
+-rw-r--r--   0        0        0     1535 2024-04-06 15:56:58.465767 lib_pcg_algopy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12130 1970-01-01 00:00:00.000000 lib_pcg_algopy-0.2.0/PKG-INFO
```

### Comparing `lib_pcg_algopy-0.1.0/README.md` & `lib_pcg_algopy-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lib_pcg_algopy-0.1.0/lib_pcg/xsh_rr_64_32.py` & `lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_64_32.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import TypeAlias
 
 from algopy import Bytes, UInt64, arc4, op, subroutine, urange
 
-PCG_DEFAULT_MULTIPLIER = 6364136223846793005
-PCG_DEFAULT_INCREMENT = 1442695040888963407
-
+from lib_pcg.consts import PCG_DEFAULT_INCREMENT, PCG_DEFAULT_MULTIPLIER
 
 PCG32_STATE: TypeAlias = UInt64
 
 
 @subroutine
 def pcg32_init(initial_state: PCG32_STATE) -> PCG32_STATE:
     return __pcg32_init(initial_state, UInt64(PCG_DEFAULT_INCREMENT))
@@ -44,15 +42,15 @@
 
             absolute_bound = upper_bound - lower_bound
         else:
             assert lower_bound < ((1 << bit_size) - 1)
 
             absolute_bound = (1 << bit_size) - lower_bound
 
-        threshold = __mask_to_32bits(__twos(absolute_bound)) % absolute_bound
+        threshold = __mask_to_32bits(__uint64_twos(absolute_bound)) % absolute_bound
 
         for i in urange(length):  # noqa: B007
             while True:
                 state, candidate = __pcg32_random(state)
                 if candidate >= threshold:
                     break
             result += op.extract(
@@ -90,19 +88,19 @@
     return __pcg32_rotation(
         __mask_to_32bits(((value >> 18) ^ value) >> 27), value >> 59
     )
 
 
 @subroutine
 def __pcg32_rotation(value: UInt64, rot: UInt64) -> UInt64:
-    return (value >> rot) | __mask_to_32bits(value << (__twos(rot) & 31))
+    return (value >> rot) | __mask_to_32bits(value << (__uint64_twos(rot) & 31))
 
 
 @subroutine
-def __twos(value: UInt64) -> UInt64:
+def __uint64_twos(value: UInt64) -> UInt64:
     addw_high, addw_low = op.addw(~value, 1)
 
     return addw_low
 
 
 @subroutine
 def __mask_to_32bits(value: UInt64) -> UInt64:
```

### Comparing `lib_pcg_algopy-0.1.0/lib_pcg/xsh_rr_double_64_32.py` & `lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_double_64_32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 from algopy import BigUInt, Bytes, UInt64, arc4, op, subroutine, urange
 
+from lib_pcg.consts import PCG_DEFAULT_INCREMENT, PCG_SECONDARY_DEFAULT_INCREMENT
 from lib_pcg.xsh_rr_64_32 import (
     __pcg32_init,
     __pcg32_output,
     __pcg32_random,
     __pcg32_step,
-    __twos,
+    __uint64_twos,
 )
 
-PCG_DEFAULT_MULTIPLIER = 6364136223846793005
-PCG_DEFAULT_INCREMENT = 1442695040888963407
-PCG_SECONDARY_DEFAULT_INCREMENT = 1442695040888963409
-
 
 @subroutine
 def pcg64_init(initial_state1: UInt64, initial_state2: UInt64) -> tuple[UInt64, UInt64]:
     return (
         __pcg32_init(initial_state1, UInt64(PCG_DEFAULT_INCREMENT)),
         __pcg32_init(initial_state2, UInt64(PCG_SECONDARY_DEFAULT_INCREMENT)),
     )
 
 
 @subroutine
 def __pcg64_random(state1: UInt64, state2: UInt64) -> tuple[UInt64, UInt64, UInt64]:
-    state1, high_prn = __pcg32_random(state1)
-    if state1 != 0:
-        new_state2 = __pcg32_step(state2, UInt64(PCG_SECONDARY_DEFAULT_INCREMENT))
-    else:
-        new_state2 = __pcg32_step(state2, UInt64(PCG_SECONDARY_DEFAULT_INCREMENT) << 1)
+    new_state1, high_prn = __pcg32_random(state1)
+
+    cond_incr = PCG_SECONDARY_DEFAULT_INCREMENT << (
+        UInt64(0) if new_state1 != 0 else UInt64(1)
+    )
+    new_state2 = __pcg32_step(state2, cond_incr)
 
     # TODO
     # This is what we would like to write. Unfortunately PuyaPy does not yet support upcasting bool to uint64.
     # new_state2 = __pcg32_step(
-    #     new_state1,
+    #     state2,
     #     UInt64(PCG_SECONDARY_DEFAULT_INCREMENT) << (state1 == 0)
     # )
 
-    return state1, new_state2, high_prn << 32 | __pcg32_output(state2)
+    return new_state1, new_state2, high_prn << 32 | __pcg32_output(state2)
 
 
 @subroutine
 def pcg64_random(
     state1: UInt64,
     state2: UInt64,
     lower_bound: UInt64,
@@ -64,15 +62,15 @@
 
             absolute_bound = upper_bound - lower_bound
         else:
             assert lower_bound < (2**64) - 1
 
             absolute_bound = op.btoi((BigUInt(2**64) - BigUInt(lower_bound)).bytes)
 
-        threshold = __twos(absolute_bound) % absolute_bound
+        threshold = __uint64_twos(absolute_bound) % absolute_bound
 
         for i in urange(length):  # noqa: B007
             while True:
                 state1, state2, candidate = __pcg64_random(state1, state2)
                 if candidate >= threshold:
                     break
             result += op.itob((candidate % absolute_bound) + lower_bound)
```

### Comparing `lib_pcg_algopy-0.1.0/pyproject.toml` & `lib_pcg_algopy-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-pcg-algopy"
-version = "0.1.0"
+version = "0.2.0"
 description = "PCG library implemented using Algorand Python"
 authors = ["CiottiGiorgio <giorgio.ciotti@algorand.foundation>"]
 readme = "README.md"
 packages = [{include = "lib_pcg"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
@@ -13,16 +13,14 @@
 algorand-python = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 algokit-client-generator = "^1.1.3"
 black = {extras = ["d"], version = "*"}
 ruff = "^0.1.6"
 mypy = "*"
-pytest = "*"
-pytest-cov = "*"
 pip-audit = "*"
 pre-commit = "*"
 puyapy = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lib_pcg_algopy-0.1.0/PKG-INFO` & `lib_pcg_algopy-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pcg-algopy
-Version: 0.1.0
+Version: 0.2.0
 Summary: PCG library implemented using Algorand Python
 Author: CiottiGiorgio
 Author-email: giorgio.ciotti@algorand.foundation
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: algokit-utils (>=2.2.0,<3.0.0)
```

