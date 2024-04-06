# Comparing `tmp/ring-attention-pytorch-0.3.0.tar.gz` & `tmp/ring-attention-pytorch-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.3.0.tar", last modified: Sat Apr  6 15:30:54 2024, max compression
+gzip compressed data, was "ring-attention-pytorch-0.3.1.tar", last modified: Sat Apr  6 15:45:38 2024, max compression
```

## Comparing `ring-attention-pytorch-0.3.0.tar` & `ring-attention-pytorch-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:30:54.741305 ring-attention-pytorch-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:30:54.741305 ring-attention-pytorch-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:30:54.737305 ring-attention-pytorch-0.3.0/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    25431 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:30:54.741305 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:30:54.741305 ring-attention-pytorch-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_flash_attention_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/setup.py
```

### Comparing `ring-attention-pytorch-0.3.0/LICENSE` & `ring-attention-pytorch-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.0/PKG-INFO` & `ring-attention-pytorch-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.0/README.md` & `ring-attention-pytorch-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.0/ring_attention_pytorch/distributed.py` & `ring-attention-pytorch-0.3.1/ring_attention_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring.py` & `ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_attention.py` & `ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_flash_attention.py` & `ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_flash_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_flash_attention_cuda.py` & `ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_flash_attention_cuda.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional, Tuple
 import packaging.version as pkg_version
 
 import torch
 from torch import nn, einsum, Tensor
 import torch.nn.functional as F
 from torch.autograd.function import Function
+from torch.cuda.amp import autocast
 
 from ring_attention_pytorch.ring import (
     ring_pass,
     all_ring_pass,
     null_ring_pass,
     one_ring_pass,
     get_rank,
@@ -477,14 +478,15 @@
 # flash attention v2 - https://tridao.me/publications/flash2/flash2.pdf
 # ring attention - https://arxiv.org/abs/2310.01889
 
 class RingFlashAttentionCUDAFunction(Function):
 
     @staticmethod
     @torch.no_grad()
+    @autocast(enabled = False)
     def forward(
         ctx,
         q: Tensor,
         k: Tensor,
         v: Tensor,
         mask: Optional[Tensor],
         causal: bool,
@@ -625,14 +627,15 @@
         # cast back to original dtype
 
         o = o.type(dtype)
         return o
 
     @staticmethod
     @torch.no_grad()
+    @autocast(enabled = False)
     def backward(ctx, do):
         """ Algorithm 2 in the v2 paper """
 
         (
             causal,
             softmax_scale,
             mask,
```

### Comparing `ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/PKG-INFO` & `ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.0
+Version: 0.3.1
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.0/setup.py` & `ring-attention-pytorch-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.0',
+  version = '0.3.1',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

