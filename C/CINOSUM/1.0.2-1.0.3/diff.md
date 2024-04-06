# Comparing `tmp/CINOSUM-1.0.2.tar.gz` & `tmp/CINOSUM-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CINOSUM-1.0.2.tar", last modified: Sat Apr  6 03:01:28 2024, max compression
+gzip compressed data, was "CINOSUM-1.0.3.tar", last modified: Sat Apr  6 03:28:04 2024, max compression
```

## Comparing `CINOSUM-1.0.2.tar` & `CINOSUM-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/CINOSUM/
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     4519 2024-04-04 04:13:54.000000 CINOSUM-1.0.2/CINOSUM/CINOSUM.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        0 2024-03-26 02:05:37.000000 CINOSUM-1.0.2/CINOSUM/__init__.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     4826 2024-04-04 01:47:17.000000 CINOSUM-1.0.2/CINOSUM/encoder.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)    12903 2024-04-04 03:41:49.000000 CINOSUM-1.0.2/CINOSUM/generate.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     3963 2024-03-27 01:19:12.000000 CINOSUM-1.0.2/CINOSUM/model_builder.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     8340 2024-03-26 02:05:37.000000 CINOSUM-1.0.2/CINOSUM/neural.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     9649 2024-03-26 02:05:37.000000 CINOSUM-1.0.2/CINOSUM/optimizers.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     3886 2024-04-01 13:19:09.000000 CINOSUM-1.0.2/CINOSUM/rnn.py
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/CINOSUM.egg-info/
--rw-r--r--   0 lhy       (1003) lhy       (1003)      431 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/PKG-INFO
--rw-rw-r--   0 lhy       (1003) lhy       (1003)      320 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/SOURCES.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        1 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/dependency_links.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)       28 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/requires.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        8 2024-04-06 03:01:28.000000 CINOSUM-1.0.2/CINOSUM.egg-info/top_level.txt
--rw-r--r--   0 lhy       (1003) lhy       (1003)      431 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/PKG-INFO
--rw-rw-r--   0 lhy       (1003) lhy       (1003)       38 2024-04-06 03:01:28.794221 CINOSUM-1.0.2/setup.cfg
--rw-rw-r--   0 lhy       (1003) lhy       (1003)      578 2024-04-06 03:01:26.000000 CINOSUM-1.0.2/setup.py
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:28:04.598789 CINOSUM-1.0.3/
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:28:04.598789 CINOSUM-1.0.3/CINOSUM.egg-info/
+-rw-r--r--   0 lhy       (1003) lhy       (1003)      431 2024-04-06 03:28:04.000000 CINOSUM-1.0.3/CINOSUM.egg-info/PKG-INFO
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)      312 2024-04-06 03:28:04.000000 CINOSUM-1.0.3/CINOSUM.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        1 2024-04-06 03:28:04.000000 CINOSUM-1.0.3/CINOSUM.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)       28 2024-04-06 03:28:04.000000 CINOSUM-1.0.3/CINOSUM.egg-info/requires.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        7 2024-04-06 03:28:04.000000 CINOSUM-1.0.3/CINOSUM.egg-info/top_level.txt
+-rw-r--r--   0 lhy       (1003) lhy       (1003)      431 2024-04-06 03:28:04.598789 CINOSUM-1.0.3/PKG-INFO
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:28:04.598789 CINOSUM-1.0.3/models/
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     4507 2024-04-06 03:23:37.000000 CINOSUM-1.0.3/models/CINOSUM.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:12:32.000000 CINOSUM-1.0.3/models/__init__.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     4814 2024-04-06 03:16:15.000000 CINOSUM-1.0.3/models/encoder.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)    12903 2024-04-06 03:05:07.000000 CINOSUM-1.0.3/models/generate.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     3951 2024-04-06 03:16:07.000000 CINOSUM-1.0.3/models/model_builder.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     8340 2024-03-26 02:05:37.000000 CINOSUM-1.0.3/models/neural.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     9649 2024-04-06 03:05:18.000000 CINOSUM-1.0.3/models/optimizers.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     3886 2024-04-01 13:19:09.000000 CINOSUM-1.0.3/models/rnn.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)       38 2024-04-06 03:28:04.598789 CINOSUM-1.0.3/setup.cfg
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)      578 2024-04-06 03:06:01.000000 CINOSUM-1.0.3/setup.py
```

### Comparing `CINOSUM-1.0.2/CINOSUM/CINOSUM.py` & `CINOSUM-1.0.3/models/CINOSUM.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from models.model_builder import *
-from models.generate import *
+from .model_builder import *
+from .generate import *
 import torch
 from types import SimpleNamespace
 
 args_dict = {
     "encoder": 'transformer',
     "mode": 'test',
     "bert_data_path": '/',
```

### Comparing `CINOSUM-1.0.2/CINOSUM/encoder.py` & `CINOSUM-1.0.3/models/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 
 import torch
 import torch.nn as nn
 
-from models.neural import MultiHeadedAttention, PositionwiseFeedForward
-from models.rnn import LayerNormLSTM
+from .neural import MultiHeadedAttention, PositionwiseFeedForward
+from .rnn import LayerNormLSTM
 
 
 class Classifier(nn.Module):
     def __init__(self, hidden_size):
         super(Classifier, self).__init__()
         self.linear1 = nn.Linear(hidden_size, 1)
         self.sigmoid = nn.Sigmoid()
```

### Comparing `CINOSUM-1.0.2/CINOSUM/generate.py` & `CINOSUM-1.0.3/models/generate.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.2/CINOSUM/model_builder.py` & `CINOSUM-1.0.3/models/model_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import torch
 import torch.nn as nn
 from transformers import XLMRobertaModel,XLMRobertaConfig
 from torch.nn.init import xavier_uniform_
 
-from models.encoder import TransformerInterEncoder, Classifier, RNNEncoder
-from models.optimizers import Optimizer
+from .encoder import TransformerInterEncoder, Classifier, RNNEncoder
+from .optimizers import Optimizer
 
 
 def build_optim(args, model, checkpoint):
     """ Build optimizer """
     saved_optimizer_state_dict = None
 
     if args.train_from != '':
```

### Comparing `CINOSUM-1.0.2/CINOSUM/neural.py` & `CINOSUM-1.0.3/models/neural.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.2/CINOSUM/optimizers.py` & `CINOSUM-1.0.3/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.2/CINOSUM/rnn.py` & `CINOSUM-1.0.3/models/rnn.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.2/setup.py` & `CINOSUM-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CINOSUM',
-    version='1.0.2',
+    version='1.0.3',
     description='Chinese Minority Extractive Multi-language summarization project',
     author='HaoYu Luo',
     author_email='506685820@qq.com',
     packages=find_packages(),
     install_requires=[
         'torch',
         'numpy',
```

