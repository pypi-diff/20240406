# Comparing `tmp/ring-attention-pytorch-0.2.9.tar.gz` & `tmp/ring-attention-pytorch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ring-attention-pytorch-0.2.9.tar", last modified: Wed Mar 20 03:40:17 2024, max compression
+gzip compressed data, was "ring-attention-pytorch-0.3.0.tar", last modified: Sat Apr  6 15:30:54 2024, max compression
```

## Comparing `ring-attention-pytorch-0.2.9.tar` & `ring-attention-pytorch-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:40:17.529554 ring-attention-pytorch-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 03:40:17.529554 ring-attention-pytorch-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:40:17.525554 ring-attention-pytorch-0.2.9/ring_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring.py
--rw-r--r--   0 runner    (1001) docker     (127)    17055 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    22903 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_flash_attention_cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 03:40:17.525554 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-20 03:40:17.000000 ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 03:40:17.529554 ring-attention-pytorch-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-20 03:40:10.000000 ring-attention-pytorch-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:30:54.741305 ring-attention-pytorch-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:30:54.741305 ring-attention-pytorch-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:30:54.737305 ring-attention-pytorch-0.3.0/ring_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25431 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_flash_attention_cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:30:54.741305 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-06 15:30:54.000000 ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:30:54.741305 ring-attention-pytorch-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-06 15:30:46.000000 ring-attention-pytorch-0.3.0/setup.py
```

### Comparing `ring-attention-pytorch-0.2.9/LICENSE` & `ring-attention-pytorch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.2.9/PKG-INFO` & `ring-attention-pytorch-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.2.9
+Version: 0.3.0
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.2.9/README.md` & `ring-attention-pytorch-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -40,16 +40,24 @@
 attended = attn(tokens)
 
 assert attended.shape == tokens.shape
 ```
 
 ## Test
 
+First install requirements
+
+```bash
+$ pip install -r requirements.txt
+```
+
+Then say testing autoregressive striped ring attention on cuda would be
+
 ```bash
-$ python assert.py
+$ python assert.py --use-cuda --causal --striped-ring-attn
 ```
 
 ## Todo
 
 - [x] make it work with derived causal mask based on rank and chunk sizes
 - [x] modify flash attention to output intermediates and figure out backwards with recompute and ring passes
 - [x] functions for splitting the sequence evenly among ranks, either within attention function, or in the external ring transformer wrapper
@@ -77,17 +85,19 @@
     - [x] handle key padding mask for forwards by translating mask to bias
     - [x] figure out how Tri handles key padding mask for backwards
     - [x] scale output of flash attention forwards on the last ring pass reduce
     - [x] verify backwards working in a100 runpod
     - [x] dk, dv needs to be float32, while kv needs to be float16. see if both can be cast to int before stacked and ring passed all in one go, then reinterpret back to float32 and float16
     - [x] prevent an unnecessary `tl.load` on the first ring pass
     - [x] cuda backwards pass must have same dq, dk, dv as naive
+- [x] fix naive flash attention backwards
+- [x] validate cuda causal and striped ring attention works
+- [x] make sure cuda striped attention works for multiple buckets, otherwise flash attention is ineffective
+- [x] for cuda striped attention, for backwards hack, pad the extra token once and index out when passing into Tri's cuda kernel
 
-- [ ] fix naive flash attention backwards
-- [ ] validate cuda causal and striped ring attention works
 - [ ] find a machine with 8 GPUs and test with a quarter million tokens first
 - [ ] think about how to craft a special `Dataset` that shards across sequence length (take into account labels for cross entropy loss) for ring transformer training
 - [ ] add ring attention to Tri's flash attention implementation. find some cuda ring reduce impl
 - [ ] `batch_isend_irecv` in the presence of key padding mask needing ring exchange, but not a big priority
 - [ ] figure out how to pytest distributed pytorch
 - [ ] use sdp context manager to validate when it is possible to use `ring_flash_attn_cuda`, otherwise assert out
```

#### html2text {}

```diff
@@ -10,69 +10,74 @@
 _P_r_o_g_r_a_m for the generous sponsorship, as well as my other sponsors, for
 affording me the independence to open source current artificial intelligence
 research ## Install ```bash $ pip install ring-attention-pytorch ``` ## Usage
 ```python import torch from ring_attention_pytorch import RingAttention attn =
 RingAttention( dim = 512, dim_head = 64, heads = 8, causal = True,
 auto_shard_seq = True, ring_attn = True, ring_seq_size = 512 ) tokens =
 torch.randn(1, 1024, 512) attended = attn(tokens) assert attended.shape ==
-tokens.shape ``` ## Test ```bash $ python assert.py ``` ## Todo - [x] make it
-work with derived causal mask based on rank and chunk sizes - [x] modify flash
-attention to output intermediates and figure out backwards with recompute and
-ring passes - [x] functions for splitting the sequence evenly among ranks,
-either within attention function, or in the external ring transformer wrapper -
-[x] basic test case with two processes and check for equivalent output and
-gradients - [x] testing - [x] make sure key padding mask works - [x] make sure
-causal mask works - [x] rotary embeddings, with proper key/value offset
-depending on ring rank - [x] striped attention - [x] add the permutating logic
-before and after transformer - [x] add causal masking logic - account for sub
-bucketing by flash attention - [x] fix issue with ring attention when flash
-buckets > 1 - [x] move flash attention back to key / value column traversal on
-outer loop and save on ring communication - [x] backwards - [x] forwards - [x]
-fix rotary positions for striped ring attention when flash buckets > 1 - [x]
-allow for variable ring passes per layer, for _l_o_c_a_l_ _-_>_ _g_l_o_b_a_l_ _a_t_t_e_n_t_i_o_n in ring
-transformer as one goes up the layers. - [x] when doing ring passes, alternate
-between designated send and receive buffers - [x] instead of max ring passes,
-able to specify lookback in terms of sequence length, and derive number of
-flash attention bucket + ring passes from that - [x] ability to have ring size
-< world size, sharding the batch and sequence, and doing ring reduce with the
-correct set of ranks - [x] add flash attention kernel version in the presence
-of cuda - [x] for forwards, use modified Triton flash attention forwards that
-outputs row sums, maxes, and exponentiated weighted sum - [x] for backwards,
-use Tri's flash attention kernels, accumulate dq, dk, dv across rings - [x]
-refactor to have naive ring+flash attention work with `(batch, seq, head, dim)`
-- [x] handle key padding mask for forwards by translating mask to bias - [x]
-figure out how Tri handles key padding mask for backwards - [x] scale output of
-flash attention forwards on the last ring pass reduce - [x] verify backwards
-working in a100 runpod - [x] dk, dv needs to be float32, while kv needs to be
-float16. see if both can be cast to int before stacked and ring passed all in
-one go, then reinterpret back to float32 and float16 - [x] prevent an
-unnecessary `tl.load` on the first ring pass - [x] cuda backwards pass must
-have same dq, dk, dv as naive - [ ] fix naive flash attention backwards - [ ]
-validate cuda causal and striped ring attention works - [ ] find a machine with
-8 GPUs and test with a quarter million tokens first - [ ] think about how to
-craft a special `Dataset` that shards across sequence length (take into account
-labels for cross entropy loss) for ring transformer training - [ ] add ring
-attention to Tri's flash attention implementation. find some cuda ring reduce
-impl - [ ] `batch_isend_irecv` in the presence of key padding mask needing ring
-exchange, but not a big priority - [ ] figure out how to pytest distributed
-pytorch - [ ] use sdp context manager to validate when it is possible to use
-`ring_flash_attn_cuda`, otherwise assert out ## Citations ```bibtex @article
-{Liu2023RingAW, title = {Ring Attention with Blockwise Transformers for Near-
-Infinite Context}, author = {Hao Liu and Matei Zaharia and Pieter Abbeel},
-journal = {ArXiv}, year = {2023}, volume = {abs/2310.01889}, url = {https://
-api.semanticscholar.org/CorpusID:263608461} } ``` ```bibtex @article
-{Brandon2023StripedAF, title = {Striped Attention: Faster Ring Attention for
-Causal Transformers}, author = {William Brandon and Aniruddha Nrusimha and
-Kevin Qian and Zachary Ankner and Tian Jin and Zhiye Song and Jonathan Ragan-
-Kelley}, journal = {ArXiv}, year = {2023}, volume = {abs/2311.09431}, url =
-{https://api.semanticscholar.org/CorpusID:265220849} } ``` ```bibtex @article
-{Dao2022FlashAttentionFA, title = {FlashAttention: Fast and Memory-Efficient
-Exact Attention with IO-Awareness}, author = {Tri Dao and Daniel Y. Fu and
-Stefano Ermon and Atri Rudra and Christopher R'e}, journal = {ArXiv}, year =
-{2022}, volume = {abs/2205.14135} } ``` ```bibtex @article
-{dao2023flashattention2, title = {Flash{A}ttention-2: Faster Attention with
-Better Parallelism and Work Partitioning, author = {Dao, Tri}, year = {2023} }
-``` ```bibtex @article{Tillet2019TritonAI, title = {Triton: an intermediate
-language and compiler for tiled neural network computations}, author =
-{Philippe Tillet and H. Kung and D. Cox}, journal = {Proceedings of the 3rd ACM
-SIGPLAN International Workshop on Machine Learning and Programming Languages},
-year = {2019} } ```
+tokens.shape ``` ## Test First install requirements ```bash $ pip install -
+r requirements.txt ``` Then say testing autoregressive striped ring attention
+on cuda would be ```bash $ python assert.py --use-cuda --causal --striped-ring-
+attn ``` ## Todo - [x] make it work with derived causal mask based on rank and
+chunk sizes - [x] modify flash attention to output intermediates and figure out
+backwards with recompute and ring passes - [x] functions for splitting the
+sequence evenly among ranks, either within attention function, or in the
+external ring transformer wrapper - [x] basic test case with two processes and
+check for equivalent output and gradients - [x] testing - [x] make sure key
+padding mask works - [x] make sure causal mask works - [x] rotary embeddings,
+with proper key/value offset depending on ring rank - [x] striped attention -
+[x] add the permutating logic before and after transformer - [x] add causal
+masking logic - account for sub bucketing by flash attention - [x] fix issue
+with ring attention when flash buckets > 1 - [x] move flash attention back to
+key / value column traversal on outer loop and save on ring communication - [x]
+backwards - [x] forwards - [x] fix rotary positions for striped ring attention
+when flash buckets > 1 - [x] allow for variable ring passes per layer, for
+_l_o_c_a_l_ _-_>_ _g_l_o_b_a_l_ _a_t_t_e_n_t_i_o_n in ring transformer as one goes up the layers. - [x]
+when doing ring passes, alternate between designated send and receive buffers -
+[x] instead of max ring passes, able to specify lookback in terms of sequence
+length, and derive number of flash attention bucket + ring passes from that -
+[x] ability to have ring size < world size, sharding the batch and sequence,
+and doing ring reduce with the correct set of ranks - [x] add flash attention
+kernel version in the presence of cuda - [x] for forwards, use modified Triton
+flash attention forwards that outputs row sums, maxes, and exponentiated
+weighted sum - [x] for backwards, use Tri's flash attention kernels, accumulate
+dq, dk, dv across rings - [x] refactor to have naive ring+flash attention work
+with `(batch, seq, head, dim)` - [x] handle key padding mask for forwards by
+translating mask to bias - [x] figure out how Tri handles key padding mask for
+backwards - [x] scale output of flash attention forwards on the last ring pass
+reduce - [x] verify backwards working in a100 runpod - [x] dk, dv needs to be
+float32, while kv needs to be float16. see if both can be cast to int before
+stacked and ring passed all in one go, then reinterpret back to float32 and
+float16 - [x] prevent an unnecessary `tl.load` on the first ring pass - [x]
+cuda backwards pass must have same dq, dk, dv as naive - [x] fix naive flash
+attention backwards - [x] validate cuda causal and striped ring attention works
+- [x] make sure cuda striped attention works for multiple buckets, otherwise
+flash attention is ineffective - [x] for cuda striped attention, for backwards
+hack, pad the extra token once and index out when passing into Tri's cuda
+kernel - [ ] find a machine with 8 GPUs and test with a quarter million tokens
+first - [ ] think about how to craft a special `Dataset` that shards across
+sequence length (take into account labels for cross entropy loss) for ring
+transformer training - [ ] add ring attention to Tri's flash attention
+implementation. find some cuda ring reduce impl - [ ] `batch_isend_irecv` in
+the presence of key padding mask needing ring exchange, but not a big priority
+- [ ] figure out how to pytest distributed pytorch - [ ] use sdp context
+manager to validate when it is possible to use `ring_flash_attn_cuda`,
+otherwise assert out ## Citations ```bibtex @article{Liu2023RingAW, title =
+{Ring Attention with Blockwise Transformers for Near-Infinite Context}, author
+= {Hao Liu and Matei Zaharia and Pieter Abbeel}, journal = {ArXiv}, year =
+{2023}, volume = {abs/2310.01889}, url = {https://api.semanticscholar.org/
+CorpusID:263608461} } ``` ```bibtex @article{Brandon2023StripedAF, title =
+{Striped Attention: Faster Ring Attention for Causal Transformers}, author =
+{William Brandon and Aniruddha Nrusimha and Kevin Qian and Zachary Ankner and
+Tian Jin and Zhiye Song and Jonathan Ragan-Kelley}, journal = {ArXiv}, year =
+{2023}, volume = {abs/2311.09431}, url = {https://api.semanticscholar.org/
+CorpusID:265220849} } ``` ```bibtex @article{Dao2022FlashAttentionFA, title =
+{FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness},
+author = {Tri Dao and Daniel Y. Fu and Stefano Ermon and Atri Rudra and
+Christopher R'e}, journal = {ArXiv}, year = {2022}, volume = {abs/2205.14135} }
+``` ```bibtex @article{dao2023flashattention2, title = {Flash{A}ttention-2:
+Faster Attention with Better Parallelism and Work Partitioning, author = {Dao,
+Tri}, year = {2023} } ``` ```bibtex @article{Tillet2019TritonAI, title =
+{Triton: an intermediate language and compiler for tiled neural network
+computations}, author = {Philippe Tillet and H. Kung and D. Cox}, journal =
+{Proceedings of the 3rd ACM SIGPLAN International Workshop on Machine Learning
+and Programming Languages}, year = {2019} } ```
```

### Comparing `ring-attention-pytorch-0.2.9/ring_attention_pytorch/distributed.py` & `ring-attention-pytorch-0.3.0/ring_attention_pytorch/distributed.py`

 * *Files identical despite different names*

### Comparing `ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring.py` & `ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,35 +90,36 @@
     send_and_receive_(x, receive_buffer, circular_rank_right(ring_size = ring_size), circular_rank_left(ring_size = ring_size))
     return receive_buffer, x
 
 one_ring_pass = partial(ring_pass, 1)
 
 # iterator for all ring passes of all tensors
 
-RingInfo = namedtuple('RingInfo', ['ring_rank', 'is_last'])
+RingInfo = namedtuple('RingInfo', ['ring_rank', 'iter_info'])
 
 def null_ring_pass(*tensors, max_iters = None, receive_buffers = None, ring_size = None):
-    yield RingInfo(0, True), (tensors, receive_buffers)
+    yield RingInfo(0, (True, True)), (tensors, receive_buffers)
 
 def all_ring_pass(*tensors, max_iters = None, receive_buffers = None, ring_size = None):
     ring_size = default(ring_size, get_world_size())
     max_iters = default(max_iters, ring_size)
 
     receive_buffers = cast_tuple(receive_buffers, len(tensors))
 
     # make sure iteration is between 1 and world size
 
     total_iters = max(1, min(ring_size, max_iters))
 
     curr_ring_pos = get_rank()
 
     for ind in range(total_iters):
+        is_first = ind == 0
         is_last = ind == (total_iters - 1)
 
-        yield RingInfo(curr_ring_pos, is_last), (tensors, receive_buffers)
+        yield RingInfo(curr_ring_pos, (is_first,  is_last)), (tensors, receive_buffers)
 
         curr_ring_pos = circular_index_left(curr_ring_pos, ring_size)
 
         if is_last:
             continue
 
         new_tensors = []
```

### Comparing `ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_attention.py` & `ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_attention.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,27 +44,28 @@
 def default_attention(
     q: Tensor,
     k: Tensor,
     v: Tensor,
     mask: Optional[Tensor] = None,
     causal: bool = False
 ):
+    device = q.device
     q = q * (q.shape[-1] ** -0.5)
 
     mask_value = -torch.finfo(q.dtype).max
 
     # similarity
 
     sim = einsum('b i h d, b j h d -> b h i j', q, k)
 
     # masking
 
     if causal:
         i, j = sim.shape[-2:]
-        causal_mask = torch.ones((i, j), dtype = torch.bool).triu(j - i + 1)
+        causal_mask = torch.ones((i, j), dtype = torch.bool, device = device).triu(j - i + 1)
         sim = torch.where(causal_mask, mask_value, sim)
 
     elif exists(mask):
         sim = einx.where('b j, b h i j, -> b h i j', mask, sim, mask_value)
 
     # attend
 
@@ -95,28 +96,31 @@
         inv_freq = theta ** -(torch.arange(0, dim, 2).float() / dim)
         self.register_buffer('inv_freq', inv_freq)
 
     @property
     def device(self):
         return self.inv_freq.device
 
+    @property
+    def is_cuda(self):
+        return self.inv_freq.is_cuda
+
     @autocast(enabled = False)
     def forward(
         self,
-        seq_len: int,
-        offset = 0
+        seq_len: int
     ):
         device = self.device
+
         pos = None
 
         if self.ring:
             if self.striped:
-                buckets = self.buckets
+                buckets = 1 if self.is_cuda else self.buckets
                 ring_stride = get_world_size() * buckets
-                ring_offset = buckets
 
                 pos = torch.arange(seq_len // buckets, device = device)
                 pos = rearrange('n -> n b', pos, b = buckets)
 
                 pos = pos * ring_stride
                 pos += torch.arange(buckets, device = device) + (get_rank() * buckets)
                 pos = rearrange('n b -> (b n)', pos)
@@ -248,33 +252,41 @@
         causal: bool = False,
         eps: float = 1e-10,
         bucket_size: int = 512,
         ring_attn: bool = False,
         ring_seq_size: int = 512,
         max_lookback_seq_len: Optional[int] = None,
         striped_ring_attn: bool = False,
-        auto_shard_seq: Optional[bool] = None,
+        auto_shard_seq: bool = False,
         prenorm: bool = True,
         force_regular_attn: bool = False,
         rotary_embed: bool = False,
         rotary_embed_theta: int = 10000,
-        use_cuda_kernel: bool = None
+        use_cuda_kernel: Optional[bool] = None
     ):
         super().__init__()
+        # whether to use flash attention cuda kernel
+
+        use_cuda_kernel = default(use_cuda_kernel, torch.cuda.is_available())
+        assert not (use_cuda_kernel and not torch.cuda.is_available())
+        self.use_cuda_kernel = use_cuda_kernel
+
         self.eps = eps
         self.heads = heads
         self.scale = dim_head ** -0.5
         self.causal = causal
 
         assert divisible_by(ring_seq_size, bucket_size)
 
         self.ring_attn = ring_attn
         self.max_lookback_seq_len = max_lookback_seq_len
         self.striped_ring_attn = striped_ring_attn
 
+        self.using_striped_ring_cuda = striped_ring_attn and use_cuda_kernel
+
         self.force_regular_attn = force_regular_attn
         self.auto_shard_seq = default(auto_shard_seq, ring_attn) # this should be done at the transformer level on the token ids for efficiency, but for testing purposes
 
         assert not (not self.ring_attn and self.auto_shard_seq)
 
         self.ring_seq_size = ring_seq_size
         self.bucket_size = bucket_size
@@ -298,19 +310,14 @@
         self.to_qkv = nn.Sequential(
             RMSNorm(dim) if prenorm else nn.Identity(),
             nn.Linear(dim, dim_inner * 3, bias = False)
         )
 
         self.to_out = nn.Linear(dim_inner, dim, bias = False)
 
-        # whether to use flash attention cuda kernel
-
-        self.use_cuda_kernel = default(use_cuda_kernel, torch.cuda.is_available())
-        assert not (use_cuda_kernel and not torch.cuda.is_available())
-
     def forward(
         self,
         x,
         mask = None,
         rotary_emb = None,
         force_ring_reduce_off = False,
         ring_size = None,
@@ -324,24 +331,27 @@
         n, i, j - sequence
         """
 
         ring_size = default(ring_size, get_world_size())
         ring_attn = self.ring_attn & is_distributed()
         auto_shard_seq = self.auto_shard_seq & is_distributed()
 
+        using_striped_ring_cuda = x.is_cuda and self.using_striped_ring_cuda
+        striped_bucket_size = self.bucket_size if not using_striped_ring_cuda else self.ring_seq_size
+
         seq_len = x.shape[-1]
 
         if auto_shard_seq:
             x, mask = maybe_pad_seq_and_mask(x, mask, self.ring_seq_size)
 
             if self.striped_ring_attn:
-                x = rearrange('b (i j) d -> b (j i) d', x, i = self.bucket_size)
+                x = rearrange('b (i j) d -> b (j i) d', x, i = striped_bucket_size)
 
                 if exists(mask):
-                    mask = rearrange('b (i j) -> b (j i)', mask, i = self.bucket_size)
+                    mask = rearrange('b (i j) -> b (j i)', mask, i = striped_bucket_size)
 
             (x, mask), batch_sizes = sharded_batch_to_sharded_seq(x, mask, self.ring_seq_size)
 
         device = x.device
 
         qkv = self.to_qkv(x)
         q, k, v = rearrange('b n (qkv h d) -> qkv b n h d', qkv, qkv = 3, h = self.heads)
@@ -391,14 +401,18 @@
         # combine heads
 
         out = rearrange('b n h d -> b n (h d)', out)
         out = self.to_out(out)
 
         if auto_shard_seq:
             out, _ = sharded_seq_to_sharded_batch(out, batch_sizes)
+
+            if self.striped_ring_attn:
+                out = rearrange('b (j i) d -> b (i j) d', out, i = striped_bucket_size)
+
             out = out[:, :seq_len]
 
         return out
 
 # simple transformer for end2end testing
 
 class RMSNorm(Module):
@@ -434,20 +448,28 @@
         bucket_size: int = 512,
         ring_attn: bool = False,
         striped_ring_attn: bool = False,
         ring_seq_size: int = 512,
         auto_shard_seq: Optional[bool] = None,
         max_lookback_seq_len: Optional[Union[Tuple[int, ...], int]] = None,
         rotary_embed_theta: int = 10000,    # will need to be changed for the million token context
-        ignore_index: int = -1
+        ignore_index: int = -1,
+        use_cuda_kernel: Optional[bool] = None
     ):
         super().__init__()
+
+        use_cuda_kernel = default(use_cuda_kernel, torch.cuda.is_available())
+        self.use_cuda_kernel = use_cuda_kernel
+        assert not (use_cuda_kernel and not torch.cuda.is_available())
+
         self.ring_attn = ring_attn
         self.striped_ring_attn = striped_ring_attn
 
+        self.using_striped_ring_cuda = use_cuda_kernel and striped_ring_attn
+
         self.ring_seq_size = ring_seq_size
         self.bucket_size = bucket_size
         assert divisible_by(ring_seq_size, bucket_size)
 
         self.auto_shard_seq = default(auto_shard_seq, ring_attn) # if ring attention is turned on, auto-shard across sequence dimension. this can also be turned off and done manually elsewhere in the data loading
 
         assert not (not self.ring_attn and self.auto_shard_seq)
@@ -478,14 +500,15 @@
                     dim_head = dim_head,
                     heads = heads,
                     bucket_size = bucket_size,
                     ring_attn = ring_attn,
                     ring_seq_size = ring_seq_size,
                     max_lookback_seq_len = layer_max_lookback_seq_len,
                     striped_ring_attn = striped_ring_attn,
+                    use_cuda_kernel = self.use_cuda_kernel,
                     auto_shard_seq = False,
                 ),
                 FeedForward(dim = dim, mult = ff_mult)
             ]))
 
         self.to_logits = nn.Sequential(
             RMSNorm(dim),
@@ -505,14 +528,17 @@
         force_ring_reduce_off = False,
         ring_size = None
     ):
         seq_len, device = x.shape[-1], x.device
 
         auto_shard_seq = not force_ring_reduce_off and self.auto_shard_seq and is_distributed()
 
+        using_striped_ring_cuda = x.is_cuda and self.using_striped_ring_cuda
+        striped_bucket_size = self.bucket_size if not using_striped_ring_cuda else self.ring_seq_size
+
         # get labels if not passed in
 
         return_loss |= exists(labels)
 
         if return_loss and not exists(labels):
             x, labels = x[:, :-1], x[:, 1:]
 
@@ -531,21 +557,21 @@
                 labels, label_mask = maybe_pad_seq_and_mask(labels, mask[:, 1:], self.ring_seq_size)
                 labels.masked_fill_(~label_mask, self.ignore_index)
 
             # account for striped attention
             # for workload balancing https://arxiv.org/abs/2311.09431 - MIT paper from Brandon et al.
 
             if self.striped_ring_attn:
-                x = rearrange('b (i j) -> b (j i)', x, i = self.bucket_size)
+                x = rearrange('b (i j) -> b (j i)', x, i = striped_bucket_size)
 
                 if exists(labels):
-                    labels = rearrange('b (i j) -> b (j i)', labels, i = self.bucket_size)
+                    labels = rearrange('b (i j) -> b (j i)', labels, i = striped_bucket_size)
 
                 if exists(mask):
-                    mask = rearrange('b (i j) -> b (j i)', mask, i = self.bucket_size)
+                    mask = rearrange('b (i j) -> b (j i)', mask, i = striped_bucket_size)
 
             # gather across batch and divide across world
 
             (x, mask), batch_sizes, num_sharded_batches = sharded_batch_to_sharded_seq(x, mask, self.ring_seq_size)
 
             if exists(labels):
                 (labels, _), *_ = sharded_batch_to_sharded_seq(labels, None, self.ring_seq_size)
@@ -593,10 +619,10 @@
 
         if not auto_shard_seq:
             return logits
 
         logits = sharded_seq_to_sharded_batch(logits, batch_sizes, num_sharded_batches)
 
         if self.striped_ring_attn:
-            logits = rearrange('b (i j) d -> b (j i) d', logits, j = self.bucket_size)
+            logits = rearrange('b (j i) d -> b (i j) d', logits, i = striped_bucket_size)
 
         return logits[:, :seq_len]
```

### Comparing `ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_flash_attention.py` & `ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_flash_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         cross_attn = q.shape[-2] != k.shape[-2]
         ring_reduce_col &= not cross_attn
         striped_ring_attn &= not cross_attn
 
         assert k.shape[-1] == v.shape[-1]
 
-        per_machine_seq_size = k.shape[-2]
+        per_machine_seq_size = k.shape[1]
 
         # calculate max ring passes
 
         max_ring_passes = None
         num_lookback_buckets = float('inf')
 
         if exists(max_lookback_seq_len):
@@ -110,24 +110,22 @@
         batch, seq, heads, _ = q.shape
 
         all_row_sums = torch.zeros((batch, heads, seq, 1), device = device)
         all_row_maxes = torch.full((batch, heads, seq, 1), max_neg_value, device = device)
 
         scale = (q.shape[-1] ** -0.5)
 
-        num_tiles = math.ceil(per_machine_seq_size / bucket_size)
-
         kv = torch.stack((k, v))
 
         # receive buffers, to be alternated with sent buffer
 
         receive_kv = None
         receive_mask = None
 
-        for (ring_rank, is_last), ((kv, mask), (receive_kv, receive_mask)) in ring_pass_fn(kv, mask, receive_buffers = (receive_kv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
+        for (ring_rank, _), ((kv, mask), (receive_kv, receive_mask)) in ring_pass_fn(kv, mask, receive_buffers = (receive_kv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
 
             k, v = kv
 
             col_splits = zip(
                 k.split(bucket_size, dim = -3),
                 v.split(bucket_size, dim = -3),
                 maybe_split(mask, bucket_size, dim = -1)
@@ -142,24 +140,24 @@
                     o.split(bucket_size, dim = -3),
                     all_row_sums.split(bucket_size, dim = -2),
                     all_row_maxes.split(bucket_size, dim = -2),
                 )
 
                 for ind, (qc, oc, row_sums, row_maxes) in enumerate(row_splits):
 
-                    qk_len_diff = kc.shape[-3] - qc.shape[-3]
-
                     row_bucket_index = row_ring_rank * per_machine_buckets + ind
 
                     attn_weights = einsum('b i h d, b j h d -> b h i j', qc, kc) * scale
 
                     if exists(col_mask):
                         attn_weights = einx.where('b j, b h i j, -> b h i j', col_mask, attn_weights, max_neg_value)
 
                     if causal:
+                        qk_len_diff = kc.shape[-3] - qc.shape[-3]
+
                         if (row_bucket_index - col_bucket_index) > num_lookback_buckets:
                             continue
 
                         if striped_ring_attn:
                             # `GetMaskStripedAttention` pseudocode at end of section 2.2.1 of https://arxiv.org/abs/2311.09431
 
                             triu_offset = int(row_bucket_index >= col_bucket_index)
@@ -232,78 +230,78 @@
             ring_size
         ) = ctx.args
 
         q, k, v, o, lse = ctx.saved_tensors
 
         row_ring_rank = (get_rank() % ring_size) if ring_reduce_col else 0
 
-        per_machine_seq_size = k.shape[-3]
+        per_machine_seq_size = k.shape[1]
         per_machine_buckets = per_machine_seq_size // bucket_size
 
         ring_pass_fn = all_ring_pass if ring_reduce_col else null_ring_pass
 
         device = q.device
 
         max_neg_value = -torch.finfo(q.dtype).max
 
         dq = torch.zeros_like(q)
         dk = torch.zeros_like(k)
         dv = torch.zeros_like(v)
 
-        row_splits = zip(
-            q.split(bucket_size, dim = -3),
-            o.split(bucket_size, dim = -3),
-            do.split(bucket_size, dim = -3),
-            lse.split(bucket_size, dim = -2),
-            dq.split(bucket_size, dim = -3)
-        )
+        # kv and dkv sent around the ring in one go
 
         kv_and_dkv = torch.stack((k, v, dk, dv))
 
         # receive buffers, to be alternated with sent buffer
 
         receive_kv_and_dkv = None
         receive_mask = None
 
-        for (ring_rank, is_last), ((kv_and_dkv, mask), (receive_kv_and_dkv, receive_mask)) in ring_pass_fn(kv_and_dkv, mask, receive_buffers = (receive_kv_and_dkv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
+        for (ring_rank, _), ((kv_and_dkv, mask), (receive_kv_and_dkv, receive_mask)) in ring_pass_fn(kv_and_dkv, mask, receive_buffers = (receive_kv_and_dkv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
+            k_ring_rank = ring_rank % ring_size
 
             k, v, dk, dv = kv_and_dkv
 
             col_splits = zip(
-                k.split(bucket_size, dim = -3),
-                v.split(bucket_size, dim = -3),
-                dk.split(bucket_size, dim = -3),
-                dv.split(bucket_size, dim = -3),
+                k.split(bucket_size, dim = 1),
+                v.split(bucket_size, dim = 1),
+                dk.split(bucket_size, dim = 1),
+                dv.split(bucket_size, dim = 1),
                 maybe_split(mask, bucket_size, dim = -1)
             )
 
             for k_ind, (kc, vc, dkc, dvc, col_mask) in enumerate(col_splits):
-                col_ring_rank = ring_rank % ring_size
-                col_bucket_index = col_ring_rank * per_machine_buckets + k_ind
+                col_bucket_index = k_ring_rank * per_machine_buckets + k_ind
+
+                row_splits = zip(
+                    q.split(bucket_size, dim = 1),
+                    o.split(bucket_size, dim = 1),
+                    do.split(bucket_size, dim = 1),
+                    lse.split(bucket_size, dim = -2),
+                    dq.split(bucket_size, dim = 1)
+                )
 
                 for ind, (qc, oc, doc, lsec, dqc) in enumerate(row_splits):
                     row_bucket_index = row_ring_rank * per_machine_buckets + ind
 
-                    qk_len_diff = kc.shape[-3] - qc.shape[-3]
-
                     attn_weights = einsum('b i h d, b j h d -> b h i j', qc, kc) * scale
 
                     if causal:
                         if (row_bucket_index - col_bucket_index) > num_lookback_buckets:
                             continue
 
                         if striped_ring_attn:
                             # `GetMaskStripedAttention` pseudocode at end of section 2.2.1 of https://arxiv.org/abs/2311.09431
 
                             triu_offset = int(row_bucket_index >= col_bucket_index)
-                            causal_mask = torch.ones((qc.shape[-3], kc.shape[-3]), dtype = torch.bool, device = device).triu(triu_offset + qk_len_diff)
+                            causal_mask = torch.ones((qc.shape[1], kc.shape[1]), dtype = torch.bool, device = device).triu(triu_offset)
                             attn_weights.masked_fill_(causal_mask, max_neg_value)
                         else:
                             if row_bucket_index == col_bucket_index:
-                                causal_mask = torch.ones((qc.shape[-3], kc.shape[-3]), dtype = torch.bool, device = device).triu(1 + qk_len_diff)
+                                causal_mask = torch.ones((qc.shape[1], kc.shape[1]), dtype = torch.bool, device = device).triu(1)
                                 attn_weights.masked_fill_(causal_mask, max_neg_value)
                             elif row_bucket_index < col_bucket_index:
                                 attn_weights.fill_(max_neg_value)
 
                     p = torch.exp(attn_weights - lsec)
 
                     if exists(col_mask):
```

### Comparing `ring-attention-pytorch-0.2.9/ring_attention_pytorch/ring_flash_attention_cuda.py` & `ring-attention-pytorch-0.3.0/ring_attention_pytorch/ring_flash_attention_cuda.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,29 +15,42 @@
     one_ring_pass,
     get_rank,
     get_world_size
 )
 
 from beartype import beartype
 
-from einops import repeat
+from einx import rearrange
 
 # helpers
 
 def exists(v):
     return v is not None
 
+def first(seq):
+    return seq[0]
+
 def pad_at_dim(t, pad: Tuple[int, int], *, dim = -1, value = 0.):
     dims_from_right = (- dim - 1) if dim < 0 else (t.ndim - dim - 1)
     zeros = ((0, 0) * dims_from_right)
     return F.pad(t, (*zeros, *pad), value = value)
 
-def is_contiguous(x):
+def is_empty(t: Tensor):
+    return t.numel() == 0
+
+def is_contiguous(x: Tensor):
     return x.stride(-1) == 1
 
+def padded_false_on_right_side(t: Tensor):
+    if t.shape[-1] <= 1:
+        return True
+
+    false_to_true = ~t[..., :-1] & t[..., 1:]
+    return not false_to_true.any()
+
 # make sure flash attention is installed for backwards
 
 import importlib
 from importlib.metadata import version
 
 assert exists(importlib.util.find_spec('flash_attn')), 'flash-attn must be installed. `pip install flash-attn --no-build-isolation` first'
 
@@ -45,14 +58,38 @@
 assert pkg_version.parse(flash_attn_version) >= pkg_version.parse('2.5.1')
 
 from flash_attn.flash_attn_interface import (
     _flash_attn_varlen_backward,
     _flash_attn_backward
 )
 
+from flash_attn.bert_padding import (
+    pad_input,
+    unpad_input
+)
+
+@beartype
+def unpad_inputs_and_return_inverse_fn(
+    tensors: Tuple[Tensor, ...],
+    mask: Tensor
+):
+    assert len(tensors) > 0
+    batch, seqlen, *_ = first(tensors).shape
+
+    outs = []
+
+    for tensor in tensors:
+        out, indices, cu_seqlens, max_seqlen = unpad_input(tensor, mask)
+        outs.append(out)
+
+    def inverse_fn(y):
+        return pad_input(y, indices, batch, seqlen)
+
+    return tuple(outs), cu_seqlens, max_seqlen, inverse_fn
+
 # make sure triton is installed for forwards
 
 assert exists(importlib.util.find_spec('triton')), 'latest triton must be installed. `pip install triton -U` first'
 
 triton_version = version('triton')
 assert pkg_version.parse(triton_version) >= pkg_version.parse('2.1')
 
@@ -345,20 +382,20 @@
     has_bias = exists(bias)
 
     if has_bias:
         assert bias.dtype in [q.dtype, torch.float]
         assert bias.is_cuda
 
         if bias.ndim == 2:
-            bias = repeat(bias, 'b j -> b h i j', h = nheads, i = seqlen_q)
+            bias = rearrange('b j -> b h i j', bias, h = nheads, i = seqlen_q)
 
         if not is_contiguous(bias):
             bias = bias.contiguous()
 
-        assert bias.shape[-2:] == (1, seqlen_k)
+        assert bias.shape[-2:] == (seqlen_q, seqlen_k)
         bias = bias.expand(batch, nheads, seqlen_q, seqlen_k)
 
     bias_strides = (bias.stride(0), bias.stride(1), bias.stride(2)) if has_bias else (0, 0, 0)
 
     seqlen_q_rounded = math.ceil(seqlen_q / 128) * 128
 
     if not exists(lse):
@@ -454,14 +491,15 @@
         bucket_size: int,
         ring_reduce_col: bool,
         striped_ring_attn: bool,
         max_lookback_seq_len: Optional[int],
         ring_size: Optional[int]
     ):
         assert all([t.is_cuda for t in (q, k, v)]), 'inputs must be all on cuda'
+        assert not exists(mask) or padded_false_on_right_side(mask), 'key padding mask must only contain True (attend) on the left hand side, and False (not attend) on the right'
 
         dtype = q.dtype
         softmax_scale = q.shape[-1] ** -0.5
 
         if q.dtype == torch.float32:
             q = q.half()
 
@@ -498,20 +536,18 @@
 
         if causal:
             mask = None
 
         bucket_size = min(per_machine_seq_size, bucket_size)
         per_machine_buckets = per_machine_seq_size // bucket_size
 
-        orig_k, orig_v, orig_mask, device = k, v, mask, q.device
+        orig_k, orig_v, orig_mask, q_seq_len, device = k, v, mask, q.shape[1], q.device
 
         ring_pass_fn = all_ring_pass if ring_reduce_col else null_ring_pass
 
-        num_tiles = math.ceil(per_machine_seq_size / bucket_size)
-
         kv = torch.stack((k, v))
 
         # accumulated values
 
         # o - output
         # m - maximum
         # lse - logsumexp
@@ -521,17 +557,15 @@
         lse = None
 
         # receive buffers, to be alternated with sent buffer
 
         receive_kv = None
         receive_mask = None
 
-        for (ring_rank, is_last), ((kv, mask), (receive_kv, receive_mask)) in ring_pass_fn(kv, mask, receive_buffers = (receive_kv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
-            is_first = ring_rank == get_rank()
-
+        for (ring_rank, (is_first, is_last)), ((kv, mask), (receive_kv, receive_mask)) in ring_pass_fn(kv, mask, receive_buffers = (receive_kv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
             k, v = kv
 
             # translate key padding mask to bias
 
             bias = None
 
             if exists(mask):
@@ -559,18 +593,24 @@
                 causal = block_causal,
                 o = o,
                 m = m,
                 lse = lse,
                 bias = bias,
                 softmax_scale = softmax_scale,
                 causal_mask_diagonal = causal_mask_diagonal,
-                return_normalized_output = is_last,
+                return_normalized_output = False,
                 load_accumulated = not is_first
             )
 
+        lse = lse[..., :q_seq_len]
+        m = m[..., :q_seq_len]
+
+        o_scale = torch.exp(m - lse)
+        o.mul_(rearrange('b h n -> b n h 1', o_scale))
+
         ctx.args = (
             causal,
             softmax_scale,
             orig_mask,
             bucket_size,
             ring_reduce_col,
             max_ring_passes,
@@ -639,59 +679,84 @@
         kv_and_dkv = torch.stack((kv, dk, dv))
 
         # receive buffers, to be alternated with sent buffer
 
         receive_kv_and_dkv = None
         receive_mask = None
 
-        for (ring_rank, is_last), ((kv_and_dkv, mask), (receive_kv_and_dkv, receive_mask)) in ring_pass_fn(kv_and_dkv, mask, receive_buffers = (receive_kv_and_dkv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
+        # hack for special causal mask for striped ring attention without having to modify cuda
+
+        if causal and striped_ring_attn:
+            # this is a hack that should also mask out the diagonal
+            # https://github.com/Dao-AILab/flash-attention?tab=readme-ov-file#21-change-behavior-of-causal-flag
+            q = pad_at_dim(q, (0, 1), dim = 1)
+            o = pad_at_dim(o, (0, 1), dim = 1)
+            do = pad_at_dim(do, (0, 1), dim = 1)
+            lse = pad_at_dim(lse, (0, 1), dim = -1)
+
+        # if not causal and has key padding mask
+        # prepare row related tensors with unpad_input
+
+        if not causal and exists(mask):
+            lse = rearrange('b h n ... -> b n h ...', lse)
+
+            (
+                (q, o, do, lse),
+                cu_seqlens_q,
+                cu_maxlen_q,
+                repad_q
+            ) = unpad_inputs_and_return_inverse_fn(
+                (q, o, do, lse),
+                mask
+            )
+
+        for (ring_rank, _), ((kv_and_dkv, mask), (receive_kv_and_dkv, receive_mask)) in ring_pass_fn(kv_and_dkv, mask, receive_buffers = (receive_kv_and_dkv, receive_mask), max_iters = max_ring_passes, ring_size = ring_size):
 
             kv, dk, dv = kv_and_dkv
 
             # reconstitute correct types for k, v, dk, dv
 
             k, v = kv.chunk(2, dim = -1)
             k, v = k.view(k_dtype), v.view(v_dtype)
 
             # determine whether to do causal mask or not
             # depends on whether it is striped attention, as well as current machine rank vs ring rank
 
+            n = row_length
+
             if causal or not exists(mask):
 
                 block_causal = False
                 need_accum = True
 
                 if causal:
                     if striped_ring_attn:
                         block_causal = True
 
                         if get_rank() < ring_rank:
-                            # this is a hack that should also mask out the diagonal
-                            # https://github.com/Dao-AILab/flash-attention?tab=readme-ov-file#21-change-behavior-of-causal-flag
-                            q = pad_at_dim(q, (0, 1), dim = -3)
-                            o = pad_at_dim(o, (0, 1), dim = -3)
+                            n += 1
                     else:
                         block_causal = get_rank() == ring_rank
 
                         if get_rank() < ring_rank:
                             need_accum = False
 
                 # use flash attention backwards kernel to calculate dq, dk, dv and accumulate
 
                 if need_accum:
                     ring_dq, ring_dk, ring_dv, *_ = _flash_attn_backward(
-                        dout = do,
-                        q = q,
+                        dout = do[:, :n],
+                        q = q[:, :n],
                         k = k,
                         v = v,
-                        out = o,
-                        softmax_lse = lse,
-                        dq = torch.zeros_like(q),
-                        dk = torch.zeros_like(k),
-                        dv = torch.zeros_like(v),
+                        out = o[:, :n],
+                        softmax_lse = lse[..., :n],
+                        dq = torch.empty_like(q[:, :n]),
+                        dk = torch.empty_like(k),
+                        dv = torch.empty_like(v),
                         dropout_p = 0.,
                         softmax_scale = softmax_scale,
                         causal = block_causal,
                         window_size = (-1, -1),
                         alibi_slopes = None,
                         deterministic = False
                     )
@@ -699,39 +764,59 @@
                     ring_dq = ring_dq[:, :row_length]
 
                 else:
                     ring_dq, ring_dk, ring_dv = 0., 0., 0.
 
                 q = q[:, :row_length]
                 o = o[:, :row_length]
+                do = do[:, :row_length]
+                lse = lse[..., :row_length]
 
             else:
-                raise NotImplementedError
 
-                ring_dq, ring_dk, ring_dv, *_ = _flash_attn_varlen_backward(
-                    dout = do,
-                    q = q,
-                    k = k,
-                    v = v,
-                    out = o,
-                    softmax_lse = lse,
-                    dq = torch.zeros_like(q),
-                    dk = torch.zeros_like(k),
-                    dv = torch.zeros_like(v),
-                    cu_seqlens_q = None,
-                    cu_seqlens_k = None,
-                    max_seqlen_q = None,
-                    max_seqlen_k = None,
-                    softmax_scale = softmax_scale,
-                    causal = False,
-                    window_size = (-1, -1),
-                    alibi_slopes = None,
-                    deterministic = False
+                (
+                    (k, v),
+                    cu_seqlens_k,
+                    cu_maxlen_k,
+                    repad_kv
+                ) = unpad_inputs_and_return_inverse_fn(
+                    (k, v),
+                    mask
                 )
 
+                if not is_empty(q) and not is_empty(k):
+                    ring_dq, ring_dk, ring_dv, *_ = _flash_attn_varlen_backward(
+                        dout = do,
+                        q = q,
+                        k = k,
+                        v = v,
+                        out = o,
+                        softmax_lse = lse,
+                        dq = torch.empty_like(q),
+                        dk = torch.empty_like(k),
+                        dv = torch.empty_like(v),
+                        cu_seqlens_q = cu_seqlens_q,
+                        cu_seqlens_k = cu_seqlens_k,
+                        max_seqlen_q = cu_maxlen_q,
+                        max_seqlen_k = cu_maxlen_k,
+                        dropout_p = 0.,
+                        softmax_scale = softmax_scale,
+                        causal = False,
+                        window_size = (-1, -1),
+                        alibi_slopes = None,
+                        deterministic = False
+                    )
+
+                    ring_dq = repad_q(ring_dq)
+                    ring_dk = repad_kv(ring_dk)
+                    ring_dv = repad_kv(ring_dv)
+
+                else:
+                    ring_dq, ring_dk, ring_dv = 0., 0., 0.
+
             dq.add_(ring_dq)
             dk.add_(ring_dk)
             dv.add_(ring_dv)
 
             if not ring_reduce_col:
                 continue
```

### Comparing `ring-attention-pytorch-0.2.9/ring_attention_pytorch.egg-info/PKG-INFO` & `ring-attention-pytorch-0.3.0/ring_attention_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ring-attention-pytorch
-Version: 0.2.9
+Version: 0.3.0
 Summary: Ring Attention - Pytorch
 Home-page: https://github.com/lucidrains/ring-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,distributed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ring-attention-pytorch-0.2.9/setup.py` & `ring-attention-pytorch-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'ring-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.9',
+  version = '0.3.0',
   license='MIT',
   description = 'Ring Attention - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/ring-attention-pytorch',
   keywords = [
```

