# Comparing `tmp/DeepTorchBlocks-0.0.1.tar.gz` & `tmp/DeepTorchBlocks-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepTorchBlocks-0.0.1.tar", last modified: Wed Apr  3 16:27:46 2024, max compression
+gzip compressed data, was "DeepTorchBlocks-0.0.1a0.tar", last modified: Sat Apr  6 09:45:38 2024, max compression
```

## Comparing `DeepTorchBlocks-0.0.1.tar` & `DeepTorchBlocks-0.0.1a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 stefanogiacomelli   (501) staff       (20)        0 2024-04-03 16:27:46.109156 DeepTorchBlocks-0.0.1/
-drwxr-xr-x   0 stefanogiacomelli   (501) staff       (20)        0 2024-04-03 16:27:46.099281 DeepTorchBlocks-0.0.1/DeepTorchBlocks.egg-info/
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)      664 2024-04-03 16:27:46.000000 DeepTorchBlocks-0.0.1/DeepTorchBlocks.egg-info/PKG-INFO
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)      384 2024-04-03 16:27:46.000000 DeepTorchBlocks-0.0.1/DeepTorchBlocks.egg-info/SOURCES.txt
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)        1 2024-04-03 16:27:46.000000 DeepTorchBlocks-0.0.1/DeepTorchBlocks.egg-info/dependency_links.txt
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)       12 2024-04-03 16:27:46.000000 DeepTorchBlocks-0.0.1/DeepTorchBlocks.egg-info/requires.txt
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)       11 2024-04-03 16:27:46.000000 DeepTorchBlocks-0.0.1/DeepTorchBlocks.egg-info/top_level.txt
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     1076 2024-04-03 16:05:03.000000 DeepTorchBlocks-0.0.1/LICENSE
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)      664 2024-04-03 16:27:46.108134 DeepTorchBlocks-0.0.1/PKG-INFO
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)       24 2024-04-03 16:04:14.000000 DeepTorchBlocks-0.0.1/README.md
-drwxr-xr-x   0 stefanogiacomelli   (501) staff       (20)        0 2024-04-03 16:27:46.107044 DeepTorchBlocks-0.0.1/nn_modules/
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     7251 2024-04-03 10:59:41.000000 DeepTorchBlocks-0.0.1/nn_modules/Autoencoders.py
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     8479 2024-04-02 10:30:57.000000 DeepTorchBlocks-0.0.1/nn_modules/Dense.py
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    36501 2024-04-02 10:30:57.000000 DeepTorchBlocks-0.0.1/nn_modules/Inception.py
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    26601 2024-04-02 10:30:57.000000 DeepTorchBlocks-0.0.1/nn_modules/Recurrent.py
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    32035 2024-04-03 16:09:23.000000 DeepTorchBlocks-0.0.1/nn_modules/Residual.py
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    25124 2024-04-03 10:44:15.000000 DeepTorchBlocks-0.0.1/nn_modules/Standard.py
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)      538 2024-04-03 16:10:52.000000 DeepTorchBlocks-0.0.1/nn_modules/__init__.py
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)       38 2024-04-03 16:27:46.109375 DeepTorchBlocks-0.0.1/setup.cfg
--rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     1284 2024-04-03 16:21:43.000000 DeepTorchBlocks-0.0.1/setup.py
+drwxr-xr-x   0 stefanogiacomelli   (501) staff       (20)        0 2024-04-06 09:45:38.079742 DeepTorchBlocks-0.0.1a0/
+drwxr-xr-x   0 stefanogiacomelli   (501) staff       (20)        0 2024-04-06 09:45:38.071165 DeepTorchBlocks-0.0.1a0/DeepTorchBlocks.egg-info/
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    10031 2024-04-06 09:45:38.000000 DeepTorchBlocks-0.0.1a0/DeepTorchBlocks.egg-info/PKG-INFO
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)      384 2024-04-06 09:45:38.000000 DeepTorchBlocks-0.0.1a0/DeepTorchBlocks.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)        1 2024-04-06 09:45:38.000000 DeepTorchBlocks-0.0.1a0/DeepTorchBlocks.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)       12 2024-04-06 09:45:38.000000 DeepTorchBlocks-0.0.1a0/DeepTorchBlocks.egg-info/requires.txt
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)       11 2024-04-06 09:45:38.000000 DeepTorchBlocks-0.0.1a0/DeepTorchBlocks.egg-info/top_level.txt
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     1076 2024-04-03 16:05:03.000000 DeepTorchBlocks-0.0.1a0/LICENSE
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    10031 2024-04-06 09:45:38.079011 DeepTorchBlocks-0.0.1a0/PKG-INFO
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     9389 2024-04-06 09:38:18.000000 DeepTorchBlocks-0.0.1a0/README.md
+drwxr-xr-x   0 stefanogiacomelli   (501) staff       (20)        0 2024-04-06 09:45:38.077935 DeepTorchBlocks-0.0.1a0/nn_modules/
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     7340 2024-04-05 17:34:17.000000 DeepTorchBlocks-0.0.1a0/nn_modules/Autoencoders.py
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     8479 2024-04-02 10:30:57.000000 DeepTorchBlocks-0.0.1a0/nn_modules/Dense.py
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    36501 2024-04-02 10:30:57.000000 DeepTorchBlocks-0.0.1a0/nn_modules/Inception.py
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    36092 2024-04-05 17:34:17.000000 DeepTorchBlocks-0.0.1a0/nn_modules/Recurrent.py
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    32035 2024-04-03 16:09:23.000000 DeepTorchBlocks-0.0.1a0/nn_modules/Residual.py
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)    25312 2024-04-05 17:34:17.000000 DeepTorchBlocks-0.0.1a0/nn_modules/Standard.py
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)      563 2024-04-05 17:34:17.000000 DeepTorchBlocks-0.0.1a0/nn_modules/__init__.py
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)       38 2024-04-06 09:45:38.079977 DeepTorchBlocks-0.0.1a0/setup.cfg
+-rw-r--r--   0 stefanogiacomelli   (501) staff       (20)     1285 2024-04-06 09:42:51.000000 DeepTorchBlocks-0.0.1a0/setup.py
```

### Comparing `DeepTorchBlocks-0.0.1/LICENSE` & `DeepTorchBlocks-0.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepTorchBlocks-0.0.1/nn_modules/Autoencoders.py` & `DeepTorchBlocks-0.0.1a0/nn_modules/Autoencoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,19 @@
                                                                 device=device)
 
     def forward(self, x, skip):
         """Forward method
 
         :param x    : Input Tensor (batch_size, in_channels, height, width)
         :type x     : torch.Tensor
+        :param skip : Intermediate encoding tensors
+        :type       : torch.Tensor
         :return x   : Output Tensor (batch_size, channels[-1], input_height, input_width)
         :rtype x    : torch.Tensor
         """
         for stage in range(self.stages):
             x = self.layers[f'{stage + 1}_UpConv_Block'](x)
-            x = torch.cat(x, skip[::-1][1:], axis=1)
+            x = torch.cat((x, skip[::-1][1:]), axis=1)
             x = self.layers[f'{stage + 1}_ConvBlock_1'](x)
             x = self.layers[f'{stage + 1}_ConvBlock_2'](x)
 
             return x
```

### Comparing `DeepTorchBlocks-0.0.1/nn_modules/Dense.py` & `DeepTorchBlocks-0.0.1a0/nn_modules/Dense.py`

 * *Files identical despite different names*

### Comparing `DeepTorchBlocks-0.0.1/nn_modules/Inception.py` & `DeepTorchBlocks-0.0.1a0/nn_modules/Inception.py`

 * *Files identical despite different names*

### Comparing `DeepTorchBlocks-0.0.1/nn_modules/Recurrent.py` & `DeepTorchBlocks-0.0.1a0/nn_modules/Recurrent.py`

 * *Files 14% similar despite different names*

```diff
@@ -586,7 +586,213 @@
 
         out = self.layers['out_fc'](out)
 
         return out
 
 
 # ------------------------------------- Convolutional Recurrent Networks (CRNN) ----------------------------------------
+class ConvLSTMCell(nn.Module):
+    def __init__(self, in_shape, in_channels, hidden_channels, kernel_size, padding, peephole=False, device=device):
+        """Creates a Pytorch module consisting of a Convolutional LSTM cell.
+        (see Xingjian Shi et al. - "Convolutional LSTM Network: A Machine Learning Approach for Precipitation Nowcasting",
+        https://arxiv.org/pdf/1506.04214.pdf)
+
+        :param in_shape         : Input features map tensor shape
+        :type in_shape          : tuple
+        :param in_channels      : Input features map tensor channels
+        :type in_channels       : int
+        :param hidden_channels  : LSTM Hidden channels
+        :type hidden_channels   : int
+        :param kernel_size      : Convolutional kernel (filter) dimensions
+        :type kernel_size       : int or tuple
+        :param padding          : Input tensor padding quantity and/or mode
+        :type padding           : str or int or tuple
+        :param peephole         : Peephole connections condition
+        :type peephole          : bool
+        :param device           : Host device ('cpu' or 'cuda:X')
+        :type device            : str
+        """
+        super(ConvLSTMCell, self).__init__()
+        self.height, self.width = in_shape
+        self.in_channels = in_channels
+        self.hidden_channels = hidden_channels
+        self.kernel_size = kernel_size
+        if isinstance(padding, str):
+            self.padding = padding
+        elif isinstance(padding, int):
+            self.padding = kernel_size // 2, kernel_size // 2
+        else:
+            self.padding = kernel_size[0] // 2, kernel_size[1] // 2
+        self.peephole = peephole
+        self.device = device
+        self.act_fun_i = nn.Sigmoid().to(device)
+        self.act_fun_f = nn.Sigmoid().to(device)
+        self.act_fun_o = nn.Sigmoid().to(device)
+        self.act_fun_g = nn.Tanh().to(device)
+        self.layers = nn.ModuleDict()
+
+        # Peephole weights layer initialization
+        if peephole:
+            self.Wci = nn.Parameter(torch.FloatTensor(self.hidden_channels, self.height, self.width)).to(device)
+            self.Wcf = nn.Parameter(torch.FloatTensor(self.hidden_channels, self.height, self.width)).to(device)
+            self.Wco = nn.Parameter(torch.FloatTensor(self.hidden_channels, self.height, self.width)).to(device)
+
+        # Features mapping layer initialization
+        self.layers['Feature_Extraction'] = nn.Conv2d(in_channels=self.in_channels + self.hidden_channels,
+                                                      out_channels=4 * self.hidden_channels,
+                                                      kernel_size=self.kernel_size,
+                                                      padding=self.padding,
+                                                      stride=1,
+                                                      bias=True).to(device)
+
+        # Parameters initialization
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        """Parameters initialization method
+
+        Convolutional layer --> Xavier uniform
+        Peephole weights --> U[-std, std]
+        """
+        # Convolutional layer init (Weights & Bias)
+        nn.init.xavier_uniform_(self.layers['Feature_Extraction'].weight, gain=nn.init.calculate_gain('tanh'))
+        self.layers['Feature_Extraction'].bias.data.zero_()
+
+        # LSTM Peephole parameters init
+        if self.peephole:
+            std = 1. / np.sqrt(self.hidden_dim)
+
+            self.Wci.data.uniform_(-std, std)
+            self.Wcf.data.uniform_(-std, std)
+            self.Wco.data.uniform_(-std, std)
+
+    def forward(self, x, prev_state=None):
+        """Forward method
+
+        :param x            : Input Tensor (batch_size, in_channels, in_size[0], in_size[1])
+        :type x             : torch.Tensor
+        :param prev_state   : Previous Hidden state Tensor (batch_size, hidden_channels, in_size[0], in_size[1])
+        :type prev_state    : torch.Tensor
+        :return h_cur       : Hidden state Tensor (batch_size, hidden_channels, ..., ...)
+        :rtype h_cur        : torch.Tensor
+        :return c_cur       : Cell state Tensor (batch_size, hidden_channels, ..., ...)
+        :rtype c_cur        : torch.Tensor
+        """
+        if prev_state is None:
+            prev_state = (torch.zeros(x.shape[0], self.hidden_channels, self.height, self.width, device=self.device),
+                          torch.zeros(x.shape[0], self.hidden_channels, self.height, self.width, device=self.device))
+
+        h_prev, c_prev = prev_state
+
+        combined = torch.cat((x, h_prev), dim=1)
+        combined_conv = self.layers['Feature_Extraction'](combined)
+
+        cc_i, cc_f, cc_o, cc_g = torch.split(combined_conv, self.hidden_channels, dim=1)
+
+        if self.peephole:
+            input_gate = self.act_fun_i(cc_i + self.Wci * c_prev)
+            forget_gate = self.act_fun_f(cc_f + self.Wcf * c_prev)
+        else:
+            input_gate = self.act_fun_i(cc_i)
+            forget_gate = self.act_fun_f(cc_f)
+
+        g = self.act_fun_g(cc_g)
+        c_cur = forget_gate * c_prev + input_gate * g
+
+        if self.peephole:
+            out = self.act_fun_o(cc_o + self.Wco * c_cur)
+        else:
+            out = self.act_fun_o(cc_o)
+
+        h_cur = out * self.act_fun_g(c_cur)
+
+        return h_cur, c_cur
+
+
+class ConvGRUCell(nn.Module):
+    def __init__(self, in_shape, in_channels, hidden_channels, kernel_size, padding, device=device):
+        """Creates a Pytorch module consisting of a Convolutional GRU cell. (see N. Ballas et al. -
+        "Delving Deeper into Convolutional Networks for Learning Video Representations", https://arxiv.org/pdf/1511.06432v4.pdf)
+
+        :param in_shape         : Input features map tensor shape
+        :type in_shape          : tuple
+        :param in_channels      : Input features map tensor channels
+        :type in_channels       : int
+        :param hidden_channels  : LSTM Hidden channels
+        :type hidden_channels   : int
+        :param kernel_size      : Convolutional kernel (filter) dimensions
+        :type kernel_size       : int or tuple
+        :param padding          : Input tensor padding quantity and/or mode
+        :type padding           : str or int or tuple
+        :param device           : Host device ('cpu' or 'cuda:X')
+        :type device            : str
+        """
+        super(ConvGRUCell, self).__init__()
+        self.height, self.width = in_shape
+        self.in_channels = in_channels
+        self.hidden_channels = hidden_channels
+        self.kernel_size = kernel_size
+        if isinstance(padding, str):
+            self.padding = padding
+        elif isinstance(padding, int):
+            self.padding = kernel_size // 2, kernel_size // 2
+        else:
+            self.padding = kernel_size[0] // 2, kernel_size[1] // 2
+        self.device = device
+        self.layers = nn.ModuleDict()
+
+        # Layers initialization
+        self.layers['Conv_ZR'] = nn.Conv2d(in_channels=self.in_channels + self.hidden_channels,
+                                           out_channels=2 * self.hidden_channels,
+                                           kernel_size=self.kernel_size,
+                                           padding=self.padding,
+                                           bias=True).to(device)
+
+        self.layers['Conv_H1'] = nn.Conv2d(in_channels=self.in_channels,
+                                           out_channels=self.hidden_channels,
+                                           kernel_size=self.kernel_size,
+                                           padding=self.padding,
+                                           bias=True).to(device)
+
+        self.layers['Conv_H2'] = nn.Conv2d(in_channels=self.hidden_channels,
+                                           out_channels=self.hidden_channels,
+                                           kernel_size=self.kernel_size,
+                                           padding=self.padding,
+                                           bias=True).to(device)
+
+        # Activation functions
+        self.act_fun = nn.Sigmoid()
+        self.out_act = nn.Tanh()
+
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        """Parameters initialization method
+
+        Convolutional layers --> Xavier uniform
+        """
+        for layer in self.layers.keys():
+            nn.init.xavier_uniform_(self.layers[layer].weight, gain=nn.init.calculate_gain('tanh'))
+            self.layers[layer].bias.data.zero_()
+
+    def forward(self, x, prev_state=None):
+        """Forward method
+
+        :param x            : Input Tensor (batch_size, in_channels, in_size[0], in_size[1])
+        :type x             : torch.Tensor
+        :param prev_state   : Previous Hidden state Tensor (batch_size, hidden_channels, in_size[0], in_size[1])
+        :type prev_state    : torch.Tensor
+        :return out         : Hidden Tensor (batch_size, hidden_channels, ..., ...)
+        :rtype out          : torch.Tensor
+        """
+        if prev_state is None:
+            prev_state = torch.zeros(x.shape[0], self.hidden_dim, self.height, self.width, device=self.device)
+
+        combined = torch.cat((x, prev_state), dim=1)
+        combined_conv = self.act_fun(self.layers['Conv_ZR'](combined))
+
+        z, r = torch.split(combined_conv, self.hidden_dim, dim=1)
+        h_ = self.out_act(self.layers['Conv_H1'](x) + r * self.layers['Conv_H2'](prev_state))
+
+        out = (1 - z) * h_ + z * prev_state
+
+        return out
```

### Comparing `DeepTorchBlocks-0.0.1/nn_modules/Residual.py` & `DeepTorchBlocks-0.0.1a0/nn_modules/Residual.py`

 * *Files identical despite different names*

### Comparing `DeepTorchBlocks-0.0.1/nn_modules/Standard.py` & `DeepTorchBlocks-0.0.1a0/nn_modules/Standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 device = 'cuda' if torch.cuda.is_available() else 'cpu'
 
 
 # ------------------------------------------- Multi-Layer Perceptrons (MLP) --------------------------------------------
 class MLPBin(nn.Module):
     def __init__(self, in_features, hidden_units, activation, rate_in, rate_hidden, device=device):
         """Creates a Pytorch module consisting of a Multi-Layer Perceptron (MLP) w. a unique normalized probability (logit).
+        It is also referred to as a Binary classifier (or Binary logistic regressor).
         (see I. Goodfellow et al. - "The Deep Learning Book, Deep Feedforward Networks Ch.6",
         https://www.deeplearningbook.org/contents/mlp.html)
 
         :param in_features  : Input tensor features
         :type in_features   : int
         :param hidden_units : Hidden units' quantity (per layer)
         :type hidden_units  : int or list
@@ -99,35 +100,36 @@
         # Output Layer pass (Sigmoidal activation)
         x = self.layers['OUT_layer'](x)
         x = nn.Sigmoid(x)
 
         return x
 
 
-class MLPSoftmax(nn.Module):
-    def __init__(self, in_features, hidden_units, n_classes, activation, rate_in, rate_hidden, device=device):
-        """Creates a Pytorch module consisting of a Multi-Layer Perceptron (MLP) w. a unique normalized probability (logit).
+class MLPMulti(nn.Module):
+    def __init__(self, in_features, hidden_units, n_outs, activation, rate_in, rate_hidden, device=device):
+        """Creates a Pytorch module consisting of a Multi-Layer Perceptron (MLP) w. a vector of non-normalized outputs.
+        It is also referred to as Multinomial logistic regressor or Universal approximator.
         (see I. Goodfellow et al. - "The Deep Learning Book, Deep Feedforward Networks Ch.6",
         https://www.deeplearningbook.org/contents/mlp.html)
 
         :param in_features  : Input tensor features
         :type in_features   : int
         :param hidden_units : Hidden units' quantity (per layer)
         :type hidden_units  : int or list
-        :param n_classes    : Output classification classes (non normalized probabilities)
-        :type n_classes     : int
+        :param n_outs       : Output classification classes (non normalized probabilities) or regression output values
+        :type n_outs        : int
         :param activation   : Output activation function (w. attributes), defaults to nn.ReLU()
         :param rate_in      : Dropout rate (for input nodes)
         :type rate_in       : float
         :param rate_hidden  : Dropout rate (for hidden layers nodes)
         :type rate_hidden   : float
         :param device       : Host device ('cpu' or 'cuda:X')
         :type device        : str
         """
-        super(MLPSoftmax, self).__init__()
+        super(MLPMulti, self).__init__()
         self.dr_in = rate_in
         self.dr_hidden = rate_hidden
         self.act_fun = activation.to(device)
         if type(hidden_units) == list:
             self.nLayers = len(hidden_units)
         else:
             self.nLayers = 1
@@ -148,17 +150,17 @@
                 self.layers[f'BatchNorm_{i + 1}'] = nn.BatchNorm1d(hidden_units[i]).to(device)
         else:
             self.layers[f'Hidden_layer'] = nn.Linear(in_features=hidden_units, out_features=hidden_units, device=device)
             self.layers[f'BatchNorm'] = nn.BatchNorm1d(hidden_units).to(device)
 
         # Output Layer initialization
         if self.nLayers > 1:
-            self.layers['OUT_layer'] = nn.Linear(in_features=hidden_units[self.nLayers - 1], out_features=n_classes, device=device)
+            self.layers['OUT_layer'] = nn.Linear(in_features=hidden_units[self.nLayers - 1], out_features=n_outs, device=device)
         else:
-            self.layers['OUT_layer'] = nn.Linear(in_features=hidden_units, out_features=n_classes, device=device)
+            self.layers['OUT_layer'] = nn.Linear(in_features=hidden_units, out_features=n_outs, device=device)
 
         # Parameters initialization
         for layer in self.layers.keys():
             try:
                 nn.init.kaiming_normal_(self.layers[layer].weight, mode='fan_in')                                       # Kaiming-He (Normal) init
             except:
                 pass                                                                                                    # Batch Layers could not be init!
```

### Comparing `DeepTorchBlocks-0.0.1/nn_modules/__init__.py` & `DeepTorchBlocks-0.0.1a0/nn_modules/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from Standard import MLPBin, MLPSoftmax, ConvBlock, DWConv, PWConv, DWSepBlock, HardSigmoid, HardSwish, SquExBlock
+from Standard import MLPBin, MLPMulti, ConvBlock, DWConv, PWConv, DWSepBlock, HardSigmoid, HardSwish, SquExBlock
 
 from Residual import ResidualBlock, BottleneckBlock, ResNextBlock, BottleNextBlock, InvResBlock, InvBottleNextBlock, \
     ConvNextStage, InvResSEBlock
 
-from Recurrent import RNNCell, LSTMCell, GRUCell, DeepRNN, DeepLSTM, DeepGRU, BRNN
+from Recurrent import RNNCell, LSTMCell, GRUCell, DeepRNN, DeepLSTM, DeepGRU, BRNN, ConvLSTMCell, ConvGRUCell
 
 from Inception import V1Block, V25Block, V26Block, V27Block, V210Block
 
 from Dense import DenseConvBlock, DenseLayer, TransitionLayer
 
 from Autoencoders import UNetEncoder, UNetDecoder
```

### Comparing `DeepTorchBlocks-0.0.1/setup.py` & `DeepTorchBlocks-0.0.1a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.1a'
 DESCRIPTION = 'Personal repository for SoA Deep Learning building blocks (in PyTorch)'
 LONG_DESCRIPTION = 'This package contains "all" the SoA NNs architecture building blocks (inheriting nn.Module) from PyTorch framework'
 
 # Setting up
 setup(name="DeepTorchBlocks",
       version=VERSION,
       author="Stefano Giacomelli (Ph.D. student UnivAQ)",
```

