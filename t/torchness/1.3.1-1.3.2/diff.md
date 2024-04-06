# Comparing `tmp/torchness-1.3.1.tar.gz` & `tmp/torchness-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchness-1.3.1.tar", last modified: Mon Feb 12 22:55:57 2024, max compression
+gzip compressed data, was "torchness-1.3.2.tar", last modified: Sat Apr  6 18:51:43 2024, max compression
```

## Comparing `torchness-1.3.1.tar` & `torchness-1.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-02-12 22:55:57.680268 torchness-1.3.1/
--rw-r--r--   0 pniewinski  (1000) pniewinski  (1000)      421 2024-02-12 22:55:57.676268 torchness-1.3.1/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      299 2023-10-10 21:57:36.000000 torchness-1.3.1/README.md
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2024-02-12 22:55:57.680268 torchness-1.3.1/setup.cfg
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      493 2024-02-12 22:55:24.000000 torchness-1.3.1/setup.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-02-12 22:55:57.676268 torchness-1.3.1/tests/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3608 2023-11-30 16:54:32.000000 torchness-1.3.1/tests/test_base_elements.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3917 2023-11-02 14:45:27.000000 torchness-1.3.1/tests/test_devices.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    16224 2023-11-28 20:08:11.000000 torchness-1.3.1/tests/test_encoders.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1852 2023-10-29 14:27:23.000000 torchness-1.3.1/tests/test_grad_clipping.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2355 2023-05-30 13:23:32.000000 torchness-1.3.1/tests/test_layers.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    19763 2023-11-14 10:01:29.000000 torchness-1.3.1/tests/test_motorch.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      715 2023-02-27 22:31:45.000000 torchness-1.3.1/tests/test_tbwr.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-02-12 22:55:57.676268 torchness-1.3.1/torchness/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2022-11-21 13:13:23.000000 torchness-1.3.1/torchness/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4726 2023-12-23 17:11:07.000000 torchness-1.3.1/torchness/base_elements.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-02-12 22:55:57.676268 torchness-1.3.1/torchness/comoneural/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2022-04-29 09:41:51.000000 torchness-1.3.1/torchness/comoneural/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      501 2023-03-11 13:46:24.000000 torchness-1.3.1/torchness/comoneural/avg_probs.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     6458 2024-02-12 22:49:24.000000 torchness-1.3.1/torchness/comoneural/batcher.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2285 2023-11-02 15:02:35.000000 torchness-1.3.1/torchness/comoneural/zeroes_processor.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     7157 2023-12-23 21:00:57.000000 torchness-1.3.1/torchness/devices.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    29472 2023-11-28 20:05:44.000000 torchness-1.3.1/torchness/encoders.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3140 2023-11-19 16:01:21.000000 torchness-1.3.1/torchness/grad_clipping.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     7468 2023-11-28 20:05:44.000000 torchness-1.3.1/torchness/layers.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-02-12 22:55:57.676268 torchness-1.3.1/torchness/models/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-01-15 19:48:10.000000 torchness-1.3.1/torchness/models/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2877 2023-10-30 14:43:57.000000 torchness-1.3.1/torchness/models/simple_feats_classifier.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     4488 2023-11-02 21:48:33.000000 torchness-1.3.1/torchness/models/simple_text_classifier.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2836 2023-10-30 14:43:57.000000 torchness-1.3.1/torchness/models/text_embbeder.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)    41618 2024-02-12 22:49:24.000000 torchness-1.3.1/torchness/motorch.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2194 2024-02-03 12:55:24.000000 torchness-1.3.1/torchness/scaled_LR.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2090 2023-12-10 20:31:20.000000 torchness-1.3.1/torchness/tbwr.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      502 2024-02-11 21:34:40.000000 torchness-1.3.1/torchness/types.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2024-02-12 22:55:57.676268 torchness-1.3.1/torchness.egg-info/
--rw-r--r--   0 pniewinski  (1000) pniewinski  (1000)      421 2024-02-12 22:55:57.000000 torchness-1.3.1/torchness.egg-info/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      855 2024-02-12 22:55:57.000000 torchness-1.3.1/torchness.egg-info/SOURCES.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2024-02-12 22:55:57.000000 torchness-1.3.1/torchness.egg-info/dependency_links.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       84 2024-02-12 22:55:57.000000 torchness-1.3.1/torchness.egg-info/requires.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       10 2024-02-12 22:55:57.000000 torchness-1.3.1/torchness.egg-info/top_level.txt
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.329340 torchness-1.3.2/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      421 2024-04-06 18:51:43.329340 torchness-1.3.2/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      308 2024-04-06 18:17:30.000000 torchness-1.3.2/README.md
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       38 2024-04-06 18:51:43.329340 torchness-1.3.2/setup.cfg
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      493 2024-04-06 18:51:41.000000 torchness-1.3.2/setup.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.325340 torchness-1.3.2/tests/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3608 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_base_elements.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3917 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_devices.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)    16816 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_encoders.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     1852 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_grad_clipping.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2355 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_layers.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)    19732 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_motorch.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      715 2024-04-06 18:17:30.000000 torchness-1.3.2/tests/test_tbwr.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.325340 torchness-1.3.2/torchness/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     4726 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/base_elements.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.329340 torchness-1.3.2/torchness/comoneural/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/comoneural/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      501 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/comoneural/avg_probs.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     6458 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/comoneural/batcher.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2761 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/comoneural/zeroes_processor.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     7157 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/devices.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)    27977 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/encoders.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3140 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/grad_clipping.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     7236 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/layers.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.329340 torchness-1.3.2/torchness/models/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/models/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3173 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/models/simple_feats_classifier.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     4372 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/models/simple_text_classifier.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2825 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/models/text_embbeder.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)    41563 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/motorch.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2194 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/scaled_LR.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2090 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/tbwr.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      502 2024-04-06 18:17:30.000000 torchness-1.3.2/torchness/types.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:51:43.329340 torchness-1.3.2/torchness.egg-info/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      421 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      855 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/SOURCES.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        1 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/dependency_links.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       84 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/requires.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       10 2024-04-06 18:51:43.000000 torchness-1.3.2/torchness.egg-info/top_level.txt
```

### Comparing `torchness-1.3.1/tests/test_base_elements.py` & `torchness-1.3.2/tests/test_base_elements.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/tests/test_devices.py` & `torchness-1.3.2/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/tests/test_encoders.py` & `torchness-1.3.2/tests/test_encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 
 from torchness.base_elements import TorchnessException
 from torchness.encoders import LayBlockDRT, EncDRT, LayBlockCNN, EncCNN, LayBlockTNS, EncTNS
 
 
 class TestEncoders(unittest.TestCase):
 
+    def test_LayBlockDRT_init(self):
+        lay_drt = LayBlockDRT(10, in_lay_norm=False)
+        print(lay_drt)
+
+    def test_LayBlockDRT_init_more(self):
+        lay_drt = LayBlockDRT(
+            in_width=           10,
+            do_scaled_dns=      True,
+            interlay_dropout=   0.1,
+            lay_dropout=        0.1,
+            res_dropout=        0.1)
+        print(lay_drt)
+
     def test_LayBlockDRT_base(self):
 
         in_width = 10
         inp = torch.rand(in_width) - 0.5
         print(inp, inp.dtype)
 
         lay_drt = LayBlockDRT(in_width)
@@ -22,19 +35,20 @@
 
     def test_LayBlockDRT_kwargs(self):
 
         in_width = 10
         inp = torch.rand(in_width) - 0.5
 
         lay_drt = LayBlockDRT(
-            in_width=       in_width,
-            do_scaled_dns=  True,
-            dns_scale=      4,
-            lay_dropout=    0.1,
-            res_dropout=    0.1)
+            in_width=           in_width,
+            do_scaled_dns=      True,
+            dns_scale=          4,
+            interlay_dropout=   0.1,
+            lay_dropout=        0.1,
+            res_dropout=        0.1)
         print(lay_drt)
         out = lay_drt(inp)
         print(out)
         self.assertTrue(out['out'].shape[-1] == in_width)
         self.assertTrue(out['zeroes'].shape[-1] == in_width * 4)
 
     def test_LayBlockDRT_device(self):
@@ -59,22 +73,36 @@
         in_width = 10
         inp = torch.rand(in_width) - 0.5
 
         lay_drt = LayBlockDRT(
             in_width=       in_width,
             do_scaled_dns=  True,
             lay_dropout=    0.1,
-            res_dropout=    0.1,
-            dtype=          torch.double)
+            res_dropout=    0.1)
         print(lay_drt)
-        inp = inp.to(torch.double)
         out = lay_drt(inp)
         print(out['out'].dtype)
         print(out)
 
+    def test_EncDRT_init(self):
+        enc_drt = EncDRT(
+            in_width=           10,
+            in_dropout=         0.1,
+            n_layers=           2,
+            lay_width=          12,
+            dns_scale=          4,
+            interlay_dropout=   0.1,
+            lay_dropout=        0.1,
+            res_dropout=        0.1)
+        print(enc_drt)
+
+    def test_EncDRT_init_shared(self):
+        enc_drt = EncDRT(10, n_layers=6, shared_lays=True, dns_scale=4)
+        print(enc_drt)
+
     def test_EncDRT(self):
 
         in_width = 10
         inp = torch.rand(in_width) - 0.5
         print(inp, inp.dtype)
 
         enc_drt = EncDRT(in_width, n_layers=6, shared_lays=True, dns_scale=4)
@@ -95,26 +123,21 @@
             in_width=       in_width,
             in_dropout=     0.1,
             n_layers=       4,
             lay_width=      16,
             do_scaled_dns=  True,
             dns_scale=      3,
             lay_dropout=    0.3,
-            res_dropout=    0.3,
-            dtype=          torch.double)
+            res_dropout=    0.3)
         print(enc_drt)
         self.assertTrue(len(list(enc_drt.children())) == 7) # in_drop, projection, ln_in, 4 * LayDRT
-        inp = inp.to(torch.double)
         out = enc_drt(inp)
         print(out)
         self.assertTrue(out['zeroes'].shape[0] == 4*16*3)
 
-        enc_drt.to(torch.float)
-        self.assertRaises(RuntimeError, enc_drt, inp) # expected scalar type Double but found Float
-
     def test_LayBlockCNN_base_init_call(self):
 
         n_filters = 6
         lay_cnn = LayBlockCNN(n_filters, do_zeroes=False)
         print(lay_cnn)
 
         inp = torch.rand(4, n_filters)
@@ -383,29 +406,27 @@
 
     def test_EncCNN_kwargs(self):
 
         n_filters = 48
         in_features = 32
         inp = torch.rand(18,96,in_features)
         print(inp.shape)
-        inp = inp.to(torch.double)
 
         enc = EncCNN(
             in_features=        in_features,
             time_drop=          0.1,
             feat_drop=          0.2,
             n_layers=           5,
             kernel_size=        7,
             n_filters=          n_filters,
             lay_dropout=        0.15,
             res_dropout=        0.25,
             do_ldrt=            True,
             ldrt_drop=          0.05,
-            ldrt_res_dropout=   0.07,
-            dtype=              torch.double)
+            ldrt_res_dropout=   0.07)
         print(enc)
         enc_out = enc(inp)
 
         print(enc_out['out'].shape)
         in_sh = list(inp.shape)
         in_sh[-1] = n_filters
         self.assertTrue(list(enc_out['out'].shape) == in_sh)
```

### Comparing `torchness-1.3.1/tests/test_grad_clipping.py` & `torchness-1.3.2/tests/test_grad_clipping.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/tests/test_layers.py` & `torchness-1.3.2/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/tests/test_motorch.py` & `torchness-1.3.2/tests/test_motorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     def __init__(
             self,
             in_drop: float,
             in_shape=   784,
             out_shape=  10,
             loss_func=  torch.nn.functional.cross_entropy,
             device=     None,
-            dtype=      None,
             seed=       121,
             **kwargs,
     ):
 
         Module.__init__(self, **kwargs)
 
         self.in_drop_lay = torch.nn.Dropout(p=in_drop) if in_drop>0 else None
@@ -66,15 +65,14 @@
     def test_base_init(self):
         model = MOTorch(
             module_type=    LinModel,
             in_drop=        0.0,
             logger=         get_child(logger, change_level=-10),
         )
         print(model)
-
         self.assertTrue(model.size == 7850)
         self.assertFalse(model.module.training)
         self.assertTrue(type(model.module) is LinModel)
         self.assertTrue(model.dtype == torch.float32)
 
     def test_init_raises(self):
         self.assertRaises(Exception, MOTorch)
```

### Comparing `torchness-1.3.1/tests/test_tbwr.py` & `torchness-1.3.2/tests/test_tbwr.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/torchness/base_elements.py` & `torchness-1.3.2/torchness/base_elements.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/torchness/comoneural/batcher.py` & `torchness-1.3.2/torchness/comoneural/batcher.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/torchness/comoneural/zeroes_processor.py` & `torchness-1.3.2/torchness/comoneural/zeroes_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,55 @@
 import torch
 from typing import Optional, Dict, List, Union
 
 from torchness.types import TNS, NUM
 
 
 class ZeroesProcessor:
-    """ processes zeroes arrays accumulated in intervals """
+    """ ZeroesProcessor
+    processes (analyzes) zeroes arrays
+    usually accumulated by NN in intervals of FWD/BWD """
 
     def __init__(
             self,
             intervals: tuple=   (50,500,5000),
             tag_pfx=            'nane',     # prefix of tag in TB, (Not Activated NEurons)
             tbwr: Optional=     None):      # if given will put summaries to TB with intervals frequencies
         self.intervals = intervals
         self.zsDL: Dict[int,List[TNS]] = {k: [] for k in self.intervals}
         self.single: List[TNS] = []
         self.tag_pfx = tag_pfx
         self.tbwr = tbwr
         self.step = 0
 
+    @staticmethod
+    def _extract_TNS_from(l:List) -> List[TNS]:
+        """ extract TNS from a (nested) list of TNS """
+        tL = []
+        for e in l:
+            if type(e) is list: tL += ZeroesProcessor._extract_TNS_from(e)
+            else:               tL.append(e)
+        return tL
+
     def process(
             self,
-            zeroes: Union[TNS,List[TNS]],
-            step: Optional[int]=    None
+            zeroes: Union[TNS,List],
+            step: Optional[int]=None
     ) -> Dict[int,NUM]:
         """ processes next zeroes
-        returned dict may be empty if no interval passed """
+        returned dict may be empty if no interval passed
+        zeroes may be given as Tensor or (nested) list of Tensor """
 
         iv_nane = {}
 
         if step is None:
             step = self.step
 
         if type(zeroes) is list:
+            zeroes = ZeroesProcessor._extract_TNS_from(zeroes)
             if not zeroes:
                 return iv_nane
             zeroes = torch.cat(zeroes)
 
         with torch.no_grad():
 
             self.single.append(torch.mean(zeroes, dtype=torch.float32))
```

### Comparing `torchness-1.3.1/torchness/devices.py` & `torchness-1.3.2/torchness/devices.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/torchness/encoders.py` & `torchness-1.3.2/torchness/encoders.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,85 +4,83 @@
 from torchness.types import ACT, INI, TNS, DTNS
 from torchness.base_elements import bert_initializer, my_initializer, TorchnessException
 from torchness.layers import LayDense, TF_Dropout, LayConv1D, LayRES, zeroes
 
 
 class LayBlockDRT(torch.nn.Module):
     """ Block (Layer) of EncDRT
-    LN > Dense or two_with_drop_in_between > drop > RES with drop """
+    LN > Dense or two with drop in between > drop > RES with drop """
 
     def __init__(
             self,
             in_width: int,
+            in_lay_norm=                True,           # input layer norm
             do_scaled_dns: bool=        False,          # two denses (True) or single dense (False)
-            dns_scale: int=             4,              # up-scale for first dense of two
+            dns_scale: int=             4,              # first dense up-scale
             activation: ACT=            torch.nn.ReLU,
             interlay_dropout: float=    0.0,            # dropout in between two denses
             lay_dropout: float=         0.0,            # dropout after dense/s
             residual: bool=             True,           # residual yes/no
             res_dropout: float=         0.0,            # dropout on residual connection
             do_zeroes: bool=            True,
-            device=                     None,
-            dtype=                      None,
             initializer: INI=           None):
 
         super().__init__()
 
         self.do_zeroes = do_zeroes
 
-        if initializer is None: initializer = my_initializer
+        if initializer is None:
+            initializer = my_initializer
 
-        self.ln_in = torch.nn.LayerNorm(
-            normalized_shape=   in_width,
-            device=             device,
-            dtype=              dtype)
+        self.ln_in = torch.nn.LayerNorm(normalized_shape=in_width) if in_lay_norm else None
 
         self.denses = []
+        self.drop_interlay = None
         if do_scaled_dns:
             # dense (scale up) with activation
             self.denses.append(LayDense(
                 in_features=    in_width,
                 out_features=   in_width * dns_scale,
                 activation=     activation,
                 bias=           True,
-                device=         device,
-                dtype=          dtype,
                 initializer=    initializer))
+            self.add_module(f'dense0', self.denses[-1])
+
+            if interlay_dropout:
+                self.drop_interlay = torch.nn.Dropout(p=interlay_dropout)
+
             # dense (scale down) without activation
             self.denses.append(LayDense(
                 in_features=    in_width * dns_scale,
                 out_features=   in_width,
                 activation=     None,
                 bias=           True,
-                device=         device,
-                dtype=          dtype,
                 initializer=    initializer))
+            self.add_module(f'dense1', self.denses[-1])
         else:
             # just single dense, with activation
             self.denses.append(LayDense(
                 in_features=    in_width,
                 out_features=   in_width,
                 activation=     activation,
                 bias=           True,
-                device=         device,
-                dtype=          dtype,
                 initializer=    initializer))
-        for dix, l in enumerate(self.denses): self.add_module(f'dense{dix}', l)
-
-        self.drop_interlay = torch.nn.Dropout(p=interlay_dropout) if interlay_dropout and do_scaled_dns else None
+            self.add_module(f'dense0', self.denses[-1])
 
         self.drop_lay = torch.nn.Dropout(p=lay_dropout) if lay_dropout else None
 
         self.res = LayRES(in_features=in_width, dropout=res_dropout) if residual else None
 
     def forward(self, inp:TNS) -> DTNS:
 
         zs = None
 
-        out = self.ln_in(inp)
+        out = inp
+        if self.ln_in:
+            out = self.ln_in(out)
 
         out = self.denses[0](out)
         if self.do_zeroes:
             zs = zeroes(out).detach()
 
         if len(self.denses) > 1: # there is second one, without activation
 
@@ -104,88 +102,93 @@
 
 class EncDRT(torch.nn.Module):
     """ Deep Residual encoder based on stacked LayBlockDRT """
 
     def __init__(
             self,
             in_width: int,
+            in_lay_norm: bool=          True,           # input LN
             in_dropout: float=          0.0,            # dropout on input
-            n_layers: int=              6,
+            n_layers: int=              6,              # number of blocks
             shared_lays: bool=          False,          # shared variables in enc_layers
             lay_width: Optional[int]=   None,           # for None matches input width
             do_scaled_dns: bool=        True,
-            dns_scale: int=             4,              # scale(*) of first dense
-            activation: ACT=            torch.nn.ReLU,  # gelu is really worth a try
-            lay_dropout: float=         0.0,            # dropout after two denses
-            residual: bool=             True,           # residual yes/no
-            res_dropout: float=         0.0,            # dropout on residual connection
-            device=                     None,
-            dtype=                      None,
+            dns_scale: int=             4,
+            activation: ACT=            torch.nn.ReLU,
+            interlay_dropout=           0.0,
+            lay_dropout: float=         0.0,
+            residual: bool=             True,
+            res_dropout: float=         0.0,
+            lay_norm=                   True,           # LN in each LayBlockDRT (input)
+            do_zeroes: bool=            True,
             initializer: INI=           None):
 
-        super(EncDRT, self).__init__()
+        super().__init__()
+
+        self.do_zeroes = do_zeroes
+
+        if initializer is None:
+            initializer = my_initializer
 
-        if initializer is None: initializer = my_initializer
+        self.ln_in = torch.nn.LayerNorm(normalized_shape=in_width) if in_lay_norm else None
 
         self.in_drop_lay = torch.nn.Dropout(p=in_dropout) if in_dropout else None
 
         self.in_width = in_width
         self.lay_width = lay_width or self.in_width
         self.projection_lay = LayDense(
             in_features=    self.in_width,
             out_features=   self.lay_width,
             activation=     None,
             bias=           False,
-            device=         device,
-            dtype=          dtype,
             initializer=    initializer) if self.lay_width != self.in_width else None
 
-        self.ln_in = torch.nn.LayerNorm(
-            normalized_shape=   self.lay_width,
-            device=             device,
-            dtype=              dtype)
-
         num_layers_to_build = 1 if shared_lays else n_layers
         self.drt_lays = [LayBlockDRT(
-            in_width=       self.lay_width,
-            do_scaled_dns=  do_scaled_dns,
-            dns_scale=      dns_scale,
-            activation=     activation,
-            lay_dropout=    lay_dropout,
-            residual=       residual,
-            res_dropout=    res_dropout,
-            device=         device,
-            dtype=          dtype,
-            initializer=    initializer
+            in_width=           self.lay_width,
+            in_lay_norm=        lay_norm,
+            do_scaled_dns=      do_scaled_dns,
+            dns_scale=          dns_scale,
+            activation=         activation,
+            interlay_dropout=   interlay_dropout,
+            lay_dropout=        lay_dropout,
+            residual=           residual,
+            res_dropout=        res_dropout,
+            do_zeroes=          self.do_zeroes,
+            initializer=        initializer
         ) for _ in range(num_layers_to_build)]
-        for lix,lay in enumerate(self.drt_lays): self.add_module(f'lay_drt_{lix}',lay)
-        if shared_lays and n_layers > 1: self.drt_lays *= n_layers
+        for lix,lay in enumerate(self.drt_lays):
+            self.add_module(f'lay_drt_{lix}',lay)
+        if shared_lays and n_layers > 1:
+            self.drt_lays *= n_layers
 
     def forward(self, inp:TNS) -> DTNS:
 
         zsL = []
 
         out = inp
 
+        if self.ln_in:
+            out = self.ln_in(out)
+
         if self.in_drop_lay: # input dropout
             out = self.in_drop_lay(out)
 
         if self.projection_lay: # input projection, no activation <- do not catch zeroes
             out = self.projection_lay(out)
 
-        out = self.ln_in(out)
-
         for drt_lay in self.drt_lays:
             lay_out = drt_lay(out)
             out = lay_out['out']
-            zsL.append(lay_out['zeroes'])
+            if self.do_zeroes:
+                zsL.append(lay_out['zeroes'])
 
         return {
             'out':      out,
-            'zeroes':   torch.cat(zsL).detach()}
+            'zeroes':   torch.cat(zsL).detach() if self.do_zeroes else None}
 
 
 class LayBlockCNN(torch.nn.Module):
     """ Block (Layer) of EncCNN
     LN > CNN > act > drop > RES > LayBlockDRT
 
     in general input for LayBlockCNN has a shape of:
@@ -218,38 +221,31 @@
             ldrt_dns_scale: int=        4,
             ldrt_drop: float or None=   0.0,
             ldrt_residual: bool=        True,
             ldrt_res_dropout: float=    0.0,
             # other
             do_zeroes: bool=            True,
             detach_history: bool=       True,           # by default state (history) will be detached on output
-            device=                     None,
-            dtype=                      None,
             initializer: INI=           None):
 
         super().__init__()
 
         self.n_filters = n_filters
         self.padded = padded
         if kernel_size % 2 == 0: raise TorchnessException('LayBlockCNN kernel_size cannot be even number')
         self.kernel_size = kernel_size
         self.do_zeroes = do_zeroes
 
-        self.lay_ln = torch.nn.LayerNorm(
-            normalized_shape=   self.n_filters,
-            device=             device,
-            dtype=              dtype)
+        self.lay_ln = torch.nn.LayerNorm(normalized_shape=self.n_filters)
 
         self.lay_conv1D = LayConv1D(
             in_features=    self.n_filters,
             n_filters=      self.n_filters,
             kernel_size=    self.kernel_size,
             padding=        'valid',
-            device=         device,
-            dtype=          dtype,
             activation=     None,
             initializer=    initializer)
 
         self.activation = activation() if activation else None
 
         self.lay_drop = torch.nn.Dropout(p=lay_dropout) if lay_dropout else None
 
@@ -262,16 +258,14 @@
             do_scaled_dns=  ldrt_do_scaled_dns,
             dns_scale=      ldrt_dns_scale,
             activation=     activation,
             lay_dropout=    ldrt_drop,
             residual=       ldrt_residual,
             res_dropout=    ldrt_res_dropout,
             do_zeroes=      self.do_zeroes,
-            device=         device,
-            dtype=          dtype,
             initializer=    initializer) if do_ldrt else None
 
         self.detach_history = detach_history
 
     def get_zero_history(self) -> TNS:
         """ prepares initial history for casual mode
         zero_history shape: [kernel_size-1, n_filters] """
@@ -287,15 +281,15 @@
 
         # expand single token
         if len(inp_orig_shape) == 1:
             inp = inp.expand([1, inp_orig_shape[0]])
 
         inp_shape = inp.shape
 
-        zsL = [] if self.do_zeroes else None
+        zsL = []
         out = self.lay_ln(inp)
 
         state = None
 
         # concatenate with history on the left -> casual block
         if history is not None:
 
@@ -347,21 +341,18 @@
 
         if len(inp_orig_shape) == 1:
             out = torch.squeeze(out, dim=0)
 
         if state is not None and self.detach_history:
             state = state.detach()
 
-        if zsL:
-            zsL = torch.cat(zsL).detach()
-
         return {
             'out':      out,
             'state':    state,
-            'zeroes':   zsL}
+            'zeroes':   torch.cat(zsL).detach() if self.do_zeroes else None}
 
 
 class EncCNN(torch.nn.Module):
     """ CNN 1D Encoder (for sequences)
     encoder built of stacked layers of LayBlockCNN
 
     EncCNN - number of parameters: projection + n_layers*LayBlockCNN """
@@ -386,16 +377,14 @@
             ldrt_dns_scale: int=        4,
             ldrt_drop: float or None=   0.0,
             ldrt_residual: bool=        True,
             ldrt_res_dropout: float=    0.0,
             # other
             do_zeroes: bool=            True,
             detach_history: bool=       True,           # by default state (history) will be detached in output
-            device=                     None,
-            dtype=                      None,
             initializer: INI=           None):
 
         super(EncCNN, self).__init__()
 
         self.in_features = in_features
         self.n_layers = n_layers
         self.kernel_size = kernel_size
@@ -407,16 +396,14 @@
             feat_drop=  feat_drop) if time_drop or feat_drop else None
 
         self.projection_lay = LayDense(
             in_features=    self.in_features,
             out_features=   self.n_filters,
             activation=     None,
             bias=           False,
-            device=         device,
-            dtype=          dtype,
             initializer=    initializer) if self.in_features != self.n_filters else None
 
         num_blocks_to_build = 1 if shared_lays else self.n_layers
 
         self.blocks = [LayBlockCNN(
             n_filters=          self.n_filters,
             padded=             padded,
@@ -428,26 +415,21 @@
             ldrt_do_scaled_dns= ldrt_do_scaled_dns,
             ldrt_dns_scale=     ldrt_dns_scale,
             ldrt_drop=          ldrt_drop,
             ldrt_residual=      ldrt_residual,
             ldrt_res_dropout=   ldrt_res_dropout,
             do_zeroes=          self.do_zeroes,
             detach_history=     detach_history,
-            device=             device,
-            dtype=              dtype,
             initializer=        initializer) for _ in range(num_blocks_to_build)]
 
         for bix,block in enumerate(self.blocks): self.add_module(f'block_{bix}',block)
 
         if shared_lays and self.n_layers > 1: self.blocks *= self.n_layers
 
-        self.out_ln = torch.nn.LayerNorm(
-            normalized_shape=   self.n_filters,
-            device=             device,
-            dtype=              dtype)
+        self.out_ln = torch.nn.LayerNorm(normalized_shape=self.n_filters)
 
     def get_zero_history(self) -> TNS:
         """ prepares initial history for casual mode
         zero_history shape: [n_layers, kernel_size-1, n_filters] """
         block_zero_history = self.blocks[0].get_zero_history()
         return block_zero_history.expand([self.n_layers] + list(block_zero_history.shape))
 
@@ -536,37 +518,30 @@
             d_model: int=       512,
             nhead: int=         8,
             dns_scale: int=     4,              # up-scale for first dense of two
             dropout: float=     0.1,
             dropout_att: float= 0.0,            # in original (torch.nn..) implementation dropout_att == dropout
             activation: ACT=    torch.nn.ReLU,
             dropout_res: float= 0.0,            # dropout on residual bypass
-            do_zeroes: bool=    True,
-            device=             None,
-            dtype=              None):
+            do_zeroes: bool=    True):
 
         super().__init__()
 
-        self.norm1 = torch.nn.LayerNorm(
-            normalized_shape=   d_model,
-            device=             device,
-            dtype=              dtype)
+        self.norm1 = torch.nn.LayerNorm(normalized_shape=d_model)
 
         self.self_attn = MyMHA(
             embed_dim=      d_model,
             num_heads=      nhead,
             dropout=        dropout_att,
             bias=           True,
             add_bias_kv=    False,
             add_zero_attn=  False,
             kdim=           None,
             vdim=           None,
-            batch_first=    True,
-            device=         device,
-            dtype=          dtype)
+            batch_first=    True)
 
         self.dropout1 = torch.nn.Dropout(p=dropout) if dropout else None
 
         self.res1 = LayRES(in_features=d_model, dropout=dropout_res)
 
         # (LN > Dense or two_with_drop_in_between > drop > RES with drop)
         self.lay_drt = LayBlockDRT(
@@ -575,16 +550,14 @@
             dns_scale=          dns_scale,
             activation=         activation,
             interlay_dropout=   dropout, # INFO: TF implementation has not this dropout
             lay_dropout=        dropout,
             residual=           True,
             res_dropout=        dropout_res,
             do_zeroes=          do_zeroes,
-            device=             device,
-            dtype=              dtype,
             initializer=        bert_initializer)
 
     def forward(
             self,
             inp: TNS,
             task_query: Optional[TNS]=              None,           # forces task-attention mode (TAT)
             inp_mask: Optional[TNS]=                None,
@@ -630,36 +603,31 @@
             nhead: int=                             8,
             dns_scale: int=                         4,
             dropout: float=                         0.1,
             dropout_att: float=                     0.0,
             activation: ACT=                        torch.nn.ReLU,
             dropout_res: float=                     0.0,
             do_zeroes: bool=                        True,
-            device=                                 None,
-            dtype=                                  None):
+    ):
 
         super().__init__()
 
         self.d_model = d_model
         self.do_zeroes = do_zeroes
 
         # positional embeddings (trainable)
         self.pos_emb = None
         if max_seq_len:
-            self.pos_emb = torch.nn.Parameter(
-                data=   torch.empty(
-                    size=   (max_seq_len, self.d_model),
-                    device= device,
-                    dtype=  dtype))
+            self.pos_emb = torch.nn.Parameter(data=torch.empty(size=(max_seq_len, self.d_model)))
             bert_initializer(self.pos_emb)
 
         self.initial_task_query = None
         if not initial_TAT_avg:
             self.initial_task_query = torch.nn.Parameter(
-                data=           torch.empty(self.d_model, device=device, dtype=dtype),
+                data=           torch.empty(self.d_model),
                 requires_grad=  False) # TODO: check with experiments
             bert_initializer(self.initial_task_query)
 
         # manage layers number
         num_layers_to_build = num_layers + num_layers_TAT
         if shared_lays is not None:
 
@@ -673,32 +641,27 @@
             nhead=          nhead,
             dns_scale=      dns_scale,
             dropout=        dropout,
             dropout_att=    dropout_att,
             activation=     activation,
             dropout_res=    dropout_res,
             do_zeroes=      self.do_zeroes,
-            device=         device,
-            dtype=          dtype,
         ) for _ in range(num_layers_to_build)]
         for lix,lay in enumerate(layers): self.add_module(f'lay_{lix}',lay)
 
         if shared_lays is not None:
             exp_layers = []
             for lay,mul in zip(layers,shared_lays):
                 exp_layers += [lay]*mul
             layers = exp_layers
 
         self.layers = layers[:num_layers]
         self.layers_TAT = layers[num_layers:]
 
-        self.norm = torch.nn.LayerNorm(
-            normalized_shape=   self.d_model,
-            device=             device,
-            dtype=              dtype)
+        self.norm = torch.nn.LayerNorm(normalized_shape=self.d_model)
 
     def _encode(self, inp:TNS, mask:Optional[TNS]=None) -> DTNS:
         """ base Transformer encoding """
 
         output = inp
 
         # it is possible to receive higher than 3-dim input [batch,seq,feats]
```

### Comparing `torchness-1.3.1/torchness/grad_clipping.py` & `torchness-1.3.2/torchness/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/torchness/layers.py` & `torchness-1.3.2/torchness/layers.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,25 +13,22 @@
 
     def __init__(
             self,
             in_features: int,
             out_features: int,
             activation: ACT=    torch.nn.ReLU,
             bias: bool=         True,
-            device=             None,
-            dtype=              None,
-            initializer: INI=   None):
+            initializer: INI=   None,
+            **kwargs):
         self.initializer = initializer or my_initializer
-        torch.nn.Linear.__init__(
-            self,
+        super().__init__(
             in_features=    in_features,
             out_features=   out_features,
             bias=           bias,
-            device=         device,
-            dtype=          dtype)
+            **kwargs)
         self.activation = activation() if activation else None
 
     def reset_parameters(self) -> None:
 
         self.initializer(self.weight)
         if self.bias is not None:
             torch.nn.init.zeros_(self.bias)
@@ -105,31 +102,29 @@
             kernel_size: int=   3,
             stride=             1,              # single number or a one-element tuple
             padding=            'same',
             dilation=           1,
             groups=             1,
             bias=               True,
             padding_mode=       'zeros',
-            device=             None,
-            dtype=              None,
             activation: ACT=    torch.nn.ReLU,
-            initializer: INI=   None):
+            initializer: INI=   None,
+            **kwargs):
 
         super(LayConv1D, self).__init__(
             in_channels=    in_features,
             out_channels=   n_filters,
             kernel_size=    kernel_size,
             stride=         stride,
             padding=        padding,
             dilation=       dilation,
             groups=         groups,
             bias=           bias,
             padding_mode=   padding_mode,
-            device=         device,
-            dtype=          dtype)
+            **kwargs)
 
         self.activation = activation() if activation else None
 
         if not initializer: initializer = my_initializer
         initializer(self.weight)
         if self.bias is not None:
             # original Conv1D (with uniform) reset for bias
```

### Comparing `torchness-1.3.1/torchness/models/simple_feats_classifier.py` & `torchness-1.3.2/torchness/models/simple_feats_classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,78 @@
 import torch
 from typing import Tuple, Optional
 
 from torchness.motorch import Module
 from torchness.types import TNS, DTNS, INI
 from torchness.base_elements import my_initializer
 from torchness.layers import LayDense
+from torchness.encoders import EncDRT
 
 
 class SFeatsCSF(Module):
     """ Simple Feats Classification Module """
 
     def __init__(
             self,
-            feats_width: int,
-            in_drop: float=                         0.0,
-            mid_width: Optional[int]=               30,
-            mid_drop: float=                        0.0,
-            num_classes: int=                       2,
+            feats_width: int,                               # input
+            in_lay_norm: bool=                      True,
+            in_dropout: float=                      0.0,
+            n_hidden: int=                          2,
+            hidden_width: int=                      12,
+            hidden_drop: float=                     0.0,
+            num_classes: int=                       2,      # output
+            lay_norm=                               True,
+            do_zeroes: bool=                        True,
             class_weights: Optional[Tuple[float]]=  None,
             initializer: INI=                       None,
-            dtype=                                  None,
             **kwargs):
 
-        Module.__init__(self, **kwargs)
+        super().__init__(**kwargs)
 
         self.logger.info(f'*** SFeatsCSF (Module) *** inits for feats of width {feats_width}')
 
         if initializer is None:
             initializer = my_initializer
 
-        self.drop = torch.nn.Dropout(p=in_drop) if in_drop else None
-
-        self.mid = LayDense(
-            in_features=    feats_width,
-            out_features=   mid_width,
-            activation=     torch.nn.ReLU,
-            bias=           True,
-            initializer=    initializer,
-            dtype=          dtype) if mid_width else None
-
-        self.mid_drop = torch.nn.Dropout(p=mid_drop) if self.mid and mid_drop else None
+        self.enc_drt = EncDRT(
+            in_width=           feats_width,
+            in_lay_norm=        in_lay_norm,
+            in_dropout=         in_dropout,
+            n_layers=           n_hidden,
+            lay_width=          hidden_width,
+            do_scaled_dns=      False,
+            activation=         torch.nn.ReLU,
+            interlay_dropout=   0.0,
+            lay_dropout=        hidden_drop,
+            res_dropout=        0.0,
+            lay_norm=           lay_norm,
+            do_zeroes=          do_zeroes,
+            initializer=        initializer)
 
         self.logits = LayDense(
-            in_features=    mid_width if self.mid else feats_width,
+            in_features=    hidden_width,
             out_features=   num_classes,
             activation=     None,
             bias=           False,
-            initializer=    initializer,
-            dtype=          dtype)
+            initializer=    initializer)
 
         if class_weights:
             class_weights = torch.nn.Parameter(torch.tensor(class_weights), requires_grad=False)
         self.class_weights = class_weights
 
     def forward(self, feats:TNS) -> DTNS:
-
-        out = feats
-
-        if self.drop:
-            out = self.drop(out)
-
-        if self.mid:
-            out = self.mid(out)
-            if self.mid_drop:
-                out = self.mid_drop(out)
-
-        logits = self.logits(out)
-
+        enc_out = self.enc_drt(feats)
+        logits = self.logits(enc_out['out'])
+        dist = torch.distributions.Categorical(logits=logits)
         return {
             'logits':   logits,
-            'probs':    torch.nn.functional.softmax(logits, dim=-1),
-            'preds':    torch.argmax(logits, dim=-1)}
+            'entropy':  dist.entropy(),
+            'probs':    dist.probs,
+            'preds':    torch.argmax(logits, dim=-1),
+            'zeroes':   enc_out['zeroes']}
 
     def loss(self, feats:TNS, labels:TNS) -> DTNS:
 
         out = self.forward(feats)
         logits = out['logits']
 
         loss = torch.nn.functional.cross_entropy(
```

### Comparing `torchness-1.3.1/torchness/models/simple_text_classifier.py` & `torchness-1.3.2/torchness/models/simple_text_classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,32 +18,30 @@
             enc_batch_size=                         256,
             in_drop: float=                         0.0,
             mid_width: int=                         30,
             mid_drop: float=                        0.0,
             num_classes: int=                       2,
             class_weights: Optional[List[float]]=   None,
             initializer: INI=                       None,
-            dtype=                                  None,
             **kwargs):
 
-        Module.__init__(self, **kwargs)
+        super().__init__(**kwargs)
 
         self.te_module = TextEMB(
             st_name=        st_name,
             enc_batch_size= enc_batch_size)
 
         self.csf = SFeatsCSF(
             feats_width=    self.te_module.width,
             in_drop=        in_drop,
             mid_width=      mid_width,
             mid_drop=       mid_drop,
             num_classes=    num_classes,
             class_weights=  class_weights,
             initializer=    initializer,
-            dtype=          dtype,
             logger=         self.logger)
 
     def encode(
             self,
             texts: Union[str, List[str]],
             show_progress_bar=  'auto',
             device=             None,
@@ -69,16 +67,15 @@
     def __init__(
             self,
             module_type: Optional[type(STextCSF)]=  STextCSF,
             enc_batch_size=                         128,    # number of lines in batch for embeddings
             fwd_batch_size=                         256,    # number of embeddings in batch for probs
             **kwargs):
 
-        MOTorch.__init__(
-            self,
+        super().__init__(
             module_type=    module_type,
             enc_batch_size= enc_batch_size,
             fwd_batch_size= fwd_batch_size,
             **kwargs)
 
     def get_embeddings(
             self,
```

### Comparing `torchness-1.3.1/torchness/models/text_embbeder.py` & `torchness-1.3.2/torchness/models/text_embbeder.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     prepares embedding for given text (str) """
 
     def __init__(
             self,
             st_name: str=   'all-MiniLM-L6-v2',
             enc_batch_size= 256,
             **kwargs):
-        Module.__init__(self, **kwargs)
+        super().__init__(**kwargs)
         self.st_name = st_name
         self.st_model = SentenceTransformer(model_name_or_path=st_name)
         self.enc_batch_size = enc_batch_size
         self.logger.info(f'*** TextEMB : {self.st_name} *** initialized, feats width:{self.width} seq length:{self.length}')
 
     def tokenize(self, texts:Union[str,List[str]]) -> Union[List[str], List[List[str]]]:
         tokenizer = self.st_model.tokenizer
@@ -49,15 +49,15 @@
         return self.st_model.get_max_seq_length()
 
 
 # is MOTorch for given st_name (SentenceTransformer) based on TextEMB module
 class TextEMB_MOTorch(MOTorch):
 
     def __init__(self, module_type:type(TextEMB)=TextEMB, **kwargs):
-        MOTorch.__init__(self, module_type=module_type, **kwargs)
+        super().__init__(module_type=module_type, **kwargs)
 
     def get_tokens(self, lines:Union[str, List[str]]) -> Union[List[str], List[List[str]]]:
         self.logger.info(f'{self.name} prepares tokens for {len(lines)} lines..')
         return self.module.tokenize(lines)
 
     def get_embeddings(
             self,
```

### Comparing `torchness-1.3.1/torchness/motorch.py` & `torchness-1.3.2/torchness/motorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class Module(torch.nn.Module):
     """ Module type supported by MOTorch
     defines computation graph of forward (FWD) and loss
     accuracy() and f1() are metrics used by MOTorch while training """
 
     def __init__(self, logger=None, loglevel=20):
-        torch.nn.Module.__init__(self)
+        super().__init__()
         if not logger:
             logger = get_pylogger(name=f'{self.__class__.__name__}_logger', level=loglevel)
         self.logger = logger
 
 
     def forward(self, **kwargs) -> DTNS:
         """ forward pass (FWD) function
@@ -131,15 +131,15 @@
     it would not be possible to distinguish between sources 1 and 4.
 
     @DynamicAttrs <-- disables warning for unresolved attributes references """
 
     MOTORCH_DEFAULTS = {
         'seed':             123,                # seed for torch and numpy
         'device':           -1,                 # :DevicesTorchness (check torchness.devices)
-        'dtype':            torch.float32,      # dtype of floats in MOTorch (16/32/64 etc)
+        'dtype':            torch.float32,
         'bypass_data_conv': False,              # to bypass input data conversion with when calling: __call__, loss, backward
             # training
         'batch_size':       64,                 # training batch size
         'n_batches':        1000,               # default length of training
         'opt_class':        torch.optim.Adam,   # default optimizer
         'train_step':       0,                  # default (starting) train step, updated with backward()
             # LR management (check torchness.base_elements.ScaledLR)
@@ -214,16 +214,15 @@
                 flat_child= flat_child)
         self._log = logger
 
         self._log.info(f'*** MOTorch : {name} *** initializes..')
         self._log.info(f'> {name} save_topdir: {save_topdir}{" <- read only mode!" if _read_only else ""}')
 
         # init as a ParaSave
-        ParaSave.__init__(
-            self,
+        super().__init__(
             name=           name,
             save_topdir=    save_topdir,
             save_fn_pfx=    save_fn_pfx,
             logger=         get_child(self._log, 'ParaSave_logger'),
             **kwargs)
         point_saved = self.get_point()
 
@@ -244,34 +243,36 @@
         module_type = module_type_saved or module_type
         self._log.info(f'> {self.name} module_type: {module_type.__name__}')
 
         ### manage params from self.module_type.__init__
 
         _module_init_def = get_class_init_params(module_type)['with_defaults'] # defaults of self.module_type.__init__
 
+        """
         # special case of params: [device, dtype] <- those will be set with values prepared by MOTorch below, BUT...
         _override_in_module_for_none = {
             'device':   self.MOTORCH_DEFAULTS['device'],
             'dtype':    self.MOTORCH_DEFAULTS['dtype']}
 
         # ..EXCEPT a case when are set in self.module_type.__init__ to other value than None
         remove_from_override = []
         for param in _override_in_module_for_none:
             if param in _module_init_def and _module_init_def[param] is not None:
                 remove_from_override.append(param)
         for param in remove_from_override:
             _override_in_module_for_none.pop(param)
+        """
 
         ### update in proper order
 
         self._point = {}
         self._point.update(ParaSave.PARASAVE_DEFAULTS)
         self._point.update(self.MOTORCH_DEFAULTS)
         self._point.update(_module_init_def)
-        self._point.update(_override_in_module_for_none)
+        #self._point.update(_override_in_module_for_none)
         self._point.update(point_saved)
         self._point.update(kwargs)
         self._point["module_type"] = module_type
 
         # remove logger (may come from Module init defaults)
         if 'logger' in self._point:
             self._point.pop('logger')
```

### Comparing `torchness-1.3.1/torchness/scaled_LR.py` & `torchness-1.3.2/torchness/scaled_LR.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/torchness/tbwr.py` & `torchness-1.3.2/torchness/tbwr.py`

 * *Files identical despite different names*

### Comparing `torchness-1.3.1/torchness.egg-info/SOURCES.txt` & `torchness-1.3.2/torchness.egg-info/SOURCES.txt`

 * *Files identical despite different names*

