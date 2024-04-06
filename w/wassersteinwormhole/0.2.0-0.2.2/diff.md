# Comparing `tmp/wassersteinwormhole-0.2.0.tar.gz` & `tmp/wassersteinwormhole-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wassersteinwormhole-0.2.0.tar", max compression
+gzip compressed data, was "wassersteinwormhole-0.2.2.tar", max compression
```

## Comparing `wassersteinwormhole-0.2.0.tar` & `wassersteinwormhole-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      876 2024-01-25 17:38:53.637955 wassersteinwormhole-0.2.0/README.md
--rw-r--r--   0        0        0      383 2024-03-21 15:14:14.238623 wassersteinwormhole-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    15335 2024-01-25 17:22:48.198091 wassersteinwormhole-0.2.0/wassersteinwormhole/Wormhole.py
--rw-r--r--   0        0        0       30 2024-01-22 22:16:06.499619 wassersteinwormhole-0.2.0/wassersteinwormhole/__init__.py
--rw-r--r--   0        0        0     6997 2024-01-22 22:03:46.527178 wassersteinwormhole-0.2.0/wassersteinwormhole/utils_OT.py
--rw-r--r--   0        0        0     8168 2024-03-21 15:11:34.371864 wassersteinwormhole-0.2.0/wassersteinwormhole/utils_Transformer.py
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 wassersteinwormhole-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      884 2024-04-06 20:42:04.006829 wassersteinwormhole-0.2.2/README.md
+-rw-r--r--   0        0        0      382 2024-04-06 20:42:16.956757 wassersteinwormhole-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    15335 2024-04-06 20:41:25.158630 wassersteinwormhole-0.2.2/wassersteinwormhole/Wormhole.py
+-rw-r--r--   0        0        0       30 2024-04-06 20:41:25.929478 wassersteinwormhole-0.2.2/wassersteinwormhole/__init__.py
+-rw-r--r--   0        0        0     6997 2024-04-06 20:41:24.569044 wassersteinwormhole-0.2.2/wassersteinwormhole/utils_OT.py
+-rw-r--r--   0        0        0     8357 2024-04-06 20:41:24.875511 wassersteinwormhole-0.2.2/wassersteinwormhole/utils_Transformer.py
+-rw-r--r--   0        0        0     1540 1970-01-01 00:00:00.000000 wassersteinwormhole-0.2.2/PKG-INFO
```

### Comparing `wassersteinwormhole-0.2.0/README.md` & `wassersteinwormhole-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Embedding point-clouds by presering Wasserstein distancse with the Wormhole.
 
 This implementation is written in Python3 and relies on FLAX, JAX, & JAX-OTT.
 
 
 To install JAX, simply run the command:
 
-    pip install --upgrade "jax[cuda11_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+    pip install --upgrade "jax[cuda11_pip]==0.4.23" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 
 And to install WassersteinWormhole along with the rest of the requirements: 
 
     pip install wassersteinwormhole
 
 And running the Womrhole on your own set of point-clouds is as simple as:
```

### Comparing `wassersteinwormhole-0.2.0/wassersteinwormhole/Wormhole.py` & `wassersteinwormhole-0.2.2/wassersteinwormhole/Wormhole.py`

 * *Files identical despite different names*

### Comparing `wassersteinwormhole-0.2.0/wassersteinwormhole/utils_OT.py` & `wassersteinwormhole-0.2.2/wassersteinwormhole/utils_OT.py`

 * *Files identical despite different names*

### Comparing `wassersteinwormhole-0.2.0/wassersteinwormhole/utils_Transformer.py` & `wassersteinwormhole-0.2.2/wassersteinwormhole/utils_Transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,26 +146,30 @@
 
     config: TransformerConfig
 
     @nn.compact
     def __call__(self, inputs, masks, deterministic):
         config = self.config
 
+        # Attention block.
+        # x = nn.LayerNorm(dtype=config.dtype)(inputs)
         x = nn.MultiHeadDotProductAttention(
             num_heads=config.num_heads,
             dtype=config.dtype,
             qkv_features=config.qkv_dim,
             kernel_init=config.kernel_init,
             bias_init=config.bias_init,
             use_bias=False,
             broadcast_dropout=False,
             dropout_rate=config.attention_dropout_rate,
             deterministic=deterministic,
         )(inputs, mask = masks[:, None, None, :]) + inputs
-        
+
+        #x = nn.Dropout(rate=config.attention_dropout_rate)(x, deterministic=deterministic)
+        x = x + inputs
         x = nn.LayerNorm(dtype=config.dtype)(x)
         output = FeedForward(config=config)(x)
         return output
 
 class DecoderBlock(nn.Module):
     """Transformer decoder layer.
```

### Comparing `wassersteinwormhole-0.2.0/PKG-INFO` & `wassersteinwormhole-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wassersteinwormhole
-Version: 0.2.0
+Version: 0.2.2
 Summary: Transformer based embeddings for Wasserstein Distances
 License: MIT
 Author: Anon
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -23,15 +23,15 @@
 Embedding point-clouds by presering Wasserstein distancse with the Wormhole.
 
 This implementation is written in Python3 and relies on FLAX, JAX, & JAX-OTT.
 
 
 To install JAX, simply run the command:
 
-    pip install --upgrade "jax[cuda11_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+    pip install --upgrade "jax[cuda11_pip]==0.4.23" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 
 And to install WassersteinWormhole along with the rest of the requirements: 
 
     pip install wassersteinwormhole
 
 And running the Womrhole on your own set of point-clouds is as simple as:
```

