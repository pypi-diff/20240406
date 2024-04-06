# Comparing `tmp/ring-attention-pytorch-0.3.1.tar.gz` & `tmp/ring-attention-pytorch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.3.1.tar", last modified: Sat Apr  6 15:45:38 2024, max compression
+gzip compressed data, was "ring-attention-pytorch-0.3.2.tar", last modified: Sat Apr  6 15:50:18 2024, max compression
```

## Comparing `ring-attention-pytorch-0.3.1.tar` & `ring-attention-pytorch-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 15:45:38.000000 ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:45:38.808471 ring-attention-pytorch-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-06 15:45:35.000000 ring-attention-pytorch-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:50:18.764027 ring-attention-pytorch-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:50:18.764027 ring-attention-pytorch-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:50:18.764027 ring-attention-pytorch-0.3.2/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25494 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch/ring_flash_attention_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:50:18.764027 ring-attention-pytorch-0.3.2/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:50:18.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 15:50:18.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:50:18.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:50:18.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 15:50:18.000000 ring-attention-pytorch-0.3.2/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:50:18.764027 ring-attention-pytorch-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-06 15:50:14.000000 ring-attention-pytorch-0.3.2/setup.py
```

### Comparing `ring-attention-pytorch-0.3.1/LICENSE` & `ring-attention-pytorch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.1/PKG-INFO` & `ring-attention-pytorch-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.1/README.md` & `ring-attention-pytorch-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.1/ring_attention_pytorch/distributed.py` & `ring-attention-pytorch-0.3.2/ring_attention_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring.py` & `ring-attention-pytorch-0.3.2/ring_attention_pytorch/ring.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_attention.py` & `ring-attention-pytorch-0.3.2/ring_attention_pytorch/ring_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_flash_attention.py` & `ring-attention-pytorch-0.3.2/ring_attention_pytorch/ring_flash_attention.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.3.1/ring_attention_pytorch/ring_flash_attention_cuda.py` & `ring-attention-pytorch-0.3.2/ring_attention_pytorch/ring_flash_attention_cuda.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,14 @@
 # flash attention v2 - https://tridao.me/publications/flash2/flash2.pdf
 # ring attention - https://arxiv.org/abs/2310.01889
 
 class RingFlashAttentionCUDAFunction(Function):
 
     @staticmethod
     @torch.no_grad()
-    @autocast(enabled = False)
     def forward(
         ctx,
         q: Tensor,
         k: Tensor,
         v: Tensor,
         mask: Optional[Tensor],
         causal: bool,
@@ -627,15 +626,14 @@
         # cast back to original dtype
 
         o = o.type(dtype)
         return o
 
     @staticmethod
     @torch.no_grad()
-    @autocast(enabled = False)
     def backward(ctx, do):
         """ Algorithm 2 in the v2 paper """
 
         (
             causal,
             softmax_scale,
             mask,
@@ -832,14 +830,15 @@
 
         dq, dk, dv = map(lambda t: t.to(dtype), (dq, dk, dv))
 
         return dq, dk, dv, None, None, None, None, None, None, None
 
 ring_flash_attn_cuda_ = RingFlashAttentionCUDAFunction.apply
 
+@autocast(enabled = False)
 @beartype
 def ring_flash_attn_cuda(
     q: Tensor,
     k: Tensor,
     v: Tensor,
     mask: Optional[Tensor] = None,
     causal: bool = False,
```

### Comparing `ring-attention-pytorch-0.3.1/ring_attention_pytorch.egg-info/PKG-INFO` & `ring-attention-pytorch-0.3.2/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.3.1/setup.py` & `ring-attention-pytorch-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.1',
+  version = '0.3.2',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

