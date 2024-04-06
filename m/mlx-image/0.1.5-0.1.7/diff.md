# Comparing `tmp/mlx_image-0.1.5.tar.gz` & `tmp/mlx_image-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlx_image-0.1.5.tar", max compression
+gzip compressed data, was "mlx_image-0.1.7.tar", max compression
```

## Comparing `mlx_image-0.1.5.tar` & `mlx_image-0.1.7.tar`

### file list

```diff
@@ -1,60 +1,54 @@
--rw-r--r--   0        0        0     1073 2024-02-07 20:33:19.109304 mlx_image-0.1.5/LICENSE
--rw-r--r--   0        0        0     4417 2024-03-21 20:52:29.243960 mlx_image-0.1.5/README.md
--rw-r--r--   0        0        0     5192 2024-03-21 20:58:35.851180 mlx_image-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-21 20:58:35.851819 mlx_image-0.1.5/src/mlxim/__init__.py
--rw-r--r--   0        0        0       40 2024-03-01 11:32:18.990445 mlx_image-0.1.5/src/mlxim/callbacks/__init__.py
--rw-r--r--   0        0        0     5939 2024-03-05 20:00:19.720966 mlx_image-0.1.5/src/mlxim/callbacks/checkpoint.py
--rw-r--r--   0        0        0       85 2024-03-04 16:59:00.611241 mlx_image-0.1.5/src/mlxim/data/__init__.py
--rw-r--r--   0        0        0      368 2024-03-04 20:16:42.712955 mlx_image-0.1.5/src/mlxim/data/_base.py
--rw-r--r--   0        0        0      610 2024-03-04 20:17:51.396246 mlx_image-0.1.5/src/mlxim/data/_utils.py
--rw-r--r--   0        0        0     6560 2024-03-05 18:57:59.461170 mlx_image-0.1.5/src/mlxim/data/folder.py
--rw-r--r--   0        0        0     3133 2024-03-04 20:28:24.954317 mlx_image-0.1.5/src/mlxim/data/loader.py
--rw-r--r--   0        0        0       84 2024-03-05 18:56:25.827318 mlx_image-0.1.5/src/mlxim/io/__init__.py
--rw-r--r--   0        0        0      646 2024-03-05 16:57:06.613445 mlx_image-0.1.5/src/mlxim/io/config.py
--rw-r--r--   0        0        0     2004 2024-03-04 20:21:54.387790 mlx_image-0.1.5/src/mlxim/io/image.py
--rw-r--r--   0        0        0        0 2024-03-01 15:49:29.969302 mlx_image-0.1.5/src/mlxim/metrics/__init__.py
--rw-r--r--   0        0        0     2350 2024-03-05 18:58:08.153363 mlx_image-0.1.5/src/mlxim/metrics/classification.py
--rw-r--r--   0        0        0      106 2024-03-05 20:48:48.888933 mlx_image-0.1.5/src/mlxim/model/__init__.py
--rw-r--r--   0        0        0      549 2024-03-19 20:23:47.603070 mlx_image-0.1.5/src/mlxim/model/_config.py
--rw-r--r--   0        0        0     2785 2024-03-21 20:52:29.246756 mlx_image-0.1.5/src/mlxim/model/_factory.py
--rw-r--r--   0        0        0      498 2024-03-21 20:52:29.247487 mlx_image-0.1.5/src/mlxim/model/_registry.py
--rw-r--r--   0        0        0     4510 2024-03-21 20:52:29.248162 mlx_image-0.1.5/src/mlxim/model/_utils.py
--rw-r--r--   0        0        0       71 2024-03-18 18:37:11.338405 mlx_image-0.1.5/src/mlxim/model/layers/__init__.py
--rw-r--r--   0        0        0     1940 2024-03-21 20:52:29.249088 mlx_image-0.1.5/src/mlxim/model/layers/_ops.py
--rw-r--r--   0        0        0     1716 2024-03-21 20:52:29.249433 mlx_image-0.1.5/src/mlxim/model/layers/functional.py
--rw-r--r--   0        0        0     8001 2024-03-21 20:52:29.250137 mlx_image-0.1.5/src/mlxim/model/layers/misc.py
--rw-r--r--   0        0        0     1896 2024-03-21 20:52:29.250816 mlx_image-0.1.5/src/mlxim/model/layers/mlp.py
--rw-r--r--   0        0        0      894 2024-03-01 17:17:52.576711 mlx_image-0.1.5/src/mlxim/model/layers/pool.py
--rw-r--r--   0        0        0     1147 2024-03-06 16:39:57.689715 mlx_image-0.1.5/src/mlxim/model/layers/utils.py
--rw-r--r--   0        0        0        0 2024-03-21 20:52:29.250870 mlx_image-0.1.5/src/mlxim/model/layers/weight_init.py
--rw-r--r--   0        0        0        0 2024-03-08 08:09:20.930514 mlx_image-0.1.5/src/mlxim/model/mobilenet/__init__.py
--rw-r--r--   0        0        0     1072 2024-03-19 20:56:26.565437 mlx_image-0.1.5/src/mlxim/model/mobilenet/_factory.py
--rw-r--r--   0        0        0    10063 2024-03-19 20:56:35.937548 mlx_image-0.1.5/src/mlxim/model/mobilenet/mobilenet.py
--rw-r--r--   0        0        0       52 2024-03-06 20:55:50.203503 mlx_image-0.1.5/src/mlxim/model/regnet/__init__.py
--rw-r--r--   0        0        0     1903 2024-03-19 20:56:41.458717 mlx_image-0.1.5/src/mlxim/model/regnet/_factory.py
--rw-r--r--   0        0        0    13624 2024-03-19 20:56:05.719439 mlx_image-0.1.5/src/mlxim/model/regnet/regnet.py
--rw-r--r--   0        0        0      826 2024-03-21 20:52:29.251713 mlx_image-0.1.5/src/mlxim/model/resnet/__init__.py
--rw-r--r--   0        0        0     4614 2024-03-21 20:52:29.252469 mlx_image-0.1.5/src/mlxim/model/resnet/_factory.py
--rw-r--r--   0        0        0    11613 2024-03-21 20:52:29.253183 mlx_image-0.1.5/src/mlxim/model/resnet/resnet.py
--rw-r--r--   0        0        0     1290 2024-03-21 20:52:29.253570 mlx_image-0.1.5/src/mlxim/model/swin_transformer/__init__.py
--rw-r--r--   0        0        0     4558 2024-03-21 20:52:29.254054 mlx_image-0.1.5/src/mlxim/model/swin_transformer/_factory.py
--rw-r--r--   0        0        0    25997 2024-03-21 20:52:29.254390 mlx_image-0.1.5/src/mlxim/model/swin_transformer/swin_transformer.py
--rw-r--r--   0        0        0     1328 2024-03-21 20:52:29.255362 mlx_image-0.1.5/src/mlxim/model/vit/__init__.py
--rw-r--r--   0        0        0     5763 2024-03-21 20:52:29.256041 mlx_image-0.1.5/src/mlxim/model/vit/_factory.py
--rw-r--r--   0        0        0     8350 2024-03-21 20:52:29.256780 mlx_image-0.1.5/src/mlxim/model/vit/vit.py
--rw-r--r--   0        0        0        0 2024-02-22 17:59:10.648259 mlx_image-0.1.5/src/mlxim/torch/__init__.py
--rw-r--r--   0        0        0     2062 2024-03-19 20:30:30.501834 mlx_image-0.1.5/src/mlxim/torch/mobilenet_v3.py
--rw-r--r--   0        0        0     1589 2024-03-08 14:53:32.529203 mlx_image-0.1.5/src/mlxim/torch/resnet.py
--rw-r--r--   0        0        0     2504 2024-03-21 20:52:29.257105 mlx_image-0.1.5/src/mlxim/torch/swin_transformers.py
--rw-r--r--   0        0        0      883 2024-03-21 20:52:29.257944 mlx_image-0.1.5/src/mlxim/torch/utils.py
--rw-r--r--   0        0        0     3830 2024-03-06 21:54:54.994830 mlx_image-0.1.5/src/mlxim/torch/vit.py
--rw-r--r--   0        0        0        0 2024-03-01 07:59:15.402821 mlx_image-0.1.5/src/mlxim/trainer/__init__.py
--rw-r--r--   0        0        0     8009 2024-03-05 21:12:03.152220 mlx_image-0.1.5/src/mlxim/trainer/trainer.py
--rw-r--r--   0        0        0       40 2024-02-29 18:00:42.924881 mlx_image-0.1.5/src/mlxim/transform/__init__.py
--rw-r--r--   0        0        0      379 2024-03-18 19:38:42.451357 mlx_image-0.1.5/src/mlxim/transform/_utils.py
--rw-r--r--   0        0        0     8111 2024-03-18 21:14:38.973719 mlx_image-0.1.5/src/mlxim/transform/imagenet.py
--rw-r--r--   0        0        0        0 2024-03-05 18:59:57.740115 mlx_image-0.1.5/src/mlxim/utils/__init__.py
--rw-r--r--   0        0        0    46361 2024-03-08 06:39:04.824940 mlx_image-0.1.5/src/mlxim/utils/imagenet.py
--rw-r--r--   0        0        0      287 2024-03-01 16:40:27.649485 mlx_image-0.1.5/src/mlxim/utils/time.py
--rw-r--r--   0        0        0     2078 2024-03-21 20:52:29.258624 mlx_image-0.1.5/src/mlxim/utils/validation.py
--rw-r--r--   0        0        0     5789 1970-01-01 00:00:00.000000 mlx_image-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-07 20:33:19.109304 mlx_image-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5337 2024-04-06 09:42:33.396341 mlx_image-0.1.7/README.md
+-rw-r--r--   0        0        0     5278 2024-04-06 09:42:33.419412 mlx_image-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-06 09:42:33.421717 mlx_image-0.1.7/src/mlxim/__init__.py
+-rw-r--r--   0        0        0       40 2024-03-01 11:32:18.990445 mlx_image-0.1.7/src/mlxim/callbacks/__init__.py
+-rw-r--r--   0        0        0     5939 2024-04-02 16:48:09.515905 mlx_image-0.1.7/src/mlxim/callbacks/checkpoint.py
+-rw-r--r--   0        0        0       85 2024-03-04 16:59:00.611241 mlx_image-0.1.7/src/mlxim/data/__init__.py
+-rw-r--r--   0        0        0      368 2024-03-04 20:16:42.712955 mlx_image-0.1.7/src/mlxim/data/_base.py
+-rw-r--r--   0        0        0      610 2024-03-04 20:17:51.396246 mlx_image-0.1.7/src/mlxim/data/_utils.py
+-rw-r--r--   0        0        0     6560 2024-03-05 18:57:59.461170 mlx_image-0.1.7/src/mlxim/data/folder.py
+-rw-r--r--   0        0        0     3133 2024-04-02 19:11:58.066297 mlx_image-0.1.7/src/mlxim/data/loader.py
+-rw-r--r--   0        0        0       84 2024-03-05 18:56:25.827318 mlx_image-0.1.7/src/mlxim/io/__init__.py
+-rw-r--r--   0        0        0      646 2024-03-05 16:57:06.613445 mlx_image-0.1.7/src/mlxim/io/config.py
+-rw-r--r--   0        0        0     2004 2024-03-04 20:21:54.387790 mlx_image-0.1.7/src/mlxim/io/image.py
+-rw-r--r--   0        0        0        0 2024-03-01 15:49:29.969302 mlx_image-0.1.7/src/mlxim/metrics/__init__.py
+-rw-r--r--   0        0        0     2350 2024-03-22 14:27:55.500832 mlx_image-0.1.7/src/mlxim/metrics/classification.py
+-rw-r--r--   0        0        0      120 2024-04-06 09:42:33.426761 mlx_image-0.1.7/src/mlxim/model/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-06 09:42:33.427620 mlx_image-0.1.7/src/mlxim/model/_config.py
+-rw-r--r--   0        0        0     2787 2024-04-05 16:27:31.379964 mlx_image-0.1.7/src/mlxim/model/_factory.py
+-rw-r--r--   0        0        0      498 2024-03-22 06:47:00.408439 mlx_image-0.1.7/src/mlxim/model/_registry.py
+-rw-r--r--   0        0        0     4510 2024-04-05 16:54:34.571010 mlx_image-0.1.7/src/mlxim/model/_utils.py
+-rw-r--r--   0        0        0       71 2024-03-22 07:58:15.886292 mlx_image-0.1.7/src/mlxim/model/layers/__init__.py
+-rw-r--r--   0        0        0     1940 2024-03-22 08:30:37.353908 mlx_image-0.1.7/src/mlxim/model/layers/_ops.py
+-rw-r--r--   0        0        0     1716 2024-03-21 20:52:29.249433 mlx_image-0.1.7/src/mlxim/model/layers/functional.py
+-rw-r--r--   0        0        0     8001 2024-04-06 09:42:28.080802 mlx_image-0.1.7/src/mlxim/model/layers/misc.py
+-rw-r--r--   0        0        0     1896 2024-04-06 08:24:17.507964 mlx_image-0.1.7/src/mlxim/model/layers/mlp.py
+-rw-r--r--   0        0        0      894 2024-03-01 17:17:52.576711 mlx_image-0.1.7/src/mlxim/model/layers/pool.py
+-rw-r--r--   0        0        0     1147 2024-03-06 16:39:57.689715 mlx_image-0.1.7/src/mlxim/model/layers/utils.py
+-rw-r--r--   0        0        0        0 2024-03-21 20:52:29.250870 mlx_image-0.1.7/src/mlxim/model/layers/weight_init.py
+-rw-r--r--   0        0        0        0 2024-03-08 08:09:20.930514 mlx_image-0.1.7/src/mlxim/model/mobilenet/__init__.py
+-rw-r--r--   0        0        0     1072 2024-03-19 20:56:26.565437 mlx_image-0.1.7/src/mlxim/model/mobilenet/_factory.py
+-rw-r--r--   0        0        0    10063 2024-03-19 20:56:35.937548 mlx_image-0.1.7/src/mlxim/model/mobilenet/mobilenet.py
+-rw-r--r--   0        0        0       52 2024-03-06 20:55:50.203503 mlx_image-0.1.7/src/mlxim/model/regnet/__init__.py
+-rw-r--r--   0        0        0     1902 2024-04-06 08:20:31.970232 mlx_image-0.1.7/src/mlxim/model/regnet/_factory.py
+-rw-r--r--   0        0        0    13624 2024-03-19 20:56:05.719439 mlx_image-0.1.7/src/mlxim/model/regnet/regnet.py
+-rw-r--r--   0        0        0      826 2024-03-21 20:52:29.251713 mlx_image-0.1.7/src/mlxim/model/resnet/__init__.py
+-rw-r--r--   0        0        0     4614 2024-03-21 20:52:29.252469 mlx_image-0.1.7/src/mlxim/model/resnet/_factory.py
+-rw-r--r--   0        0        0    11613 2024-03-21 20:52:29.253183 mlx_image-0.1.7/src/mlxim/model/resnet/resnet.py
+-rw-r--r--   0        0        0     1290 2024-03-21 20:52:29.253570 mlx_image-0.1.7/src/mlxim/model/swin_transformer/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-06 09:42:33.428429 mlx_image-0.1.7/src/mlxim/model/swin_transformer/_factory.py
+-rw-r--r--   0        0        0    25997 2024-04-02 19:56:06.711210 mlx_image-0.1.7/src/mlxim/model/swin_transformer/swin_transformer.py
+-rw-r--r--   0        0        0     2316 2024-04-06 09:42:33.429481 mlx_image-0.1.7/src/mlxim/model/vit/__init__.py
+-rw-r--r--   0        0        0    10251 2024-04-06 09:42:33.430295 mlx_image-0.1.7/src/mlxim/model/vit/_factory.py
+-rw-r--r--   0        0        0    17481 2024-04-06 09:42:33.430890 mlx_image-0.1.7/src/mlxim/model/vit/vit.py
+-rw-r--r--   0        0        0        0 2024-03-01 07:59:15.402821 mlx_image-0.1.7/src/mlxim/trainer/__init__.py
+-rw-r--r--   0        0        0     8010 2024-04-06 09:42:33.431546 mlx_image-0.1.7/src/mlxim/trainer/trainer.py
+-rw-r--r--   0        0        0       40 2024-02-29 18:00:42.924881 mlx_image-0.1.7/src/mlxim/transform/__init__.py
+-rw-r--r--   0        0        0      379 2024-03-18 19:38:42.451357 mlx_image-0.1.7/src/mlxim/transform/_utils.py
+-rw-r--r--   0        0        0     8111 2024-03-18 21:14:38.973719 mlx_image-0.1.7/src/mlxim/transform/imagenet.py
+-rw-r--r--   0        0        0        0 2024-03-05 18:59:57.740115 mlx_image-0.1.7/src/mlxim/utils/__init__.py
+-rw-r--r--   0        0        0    46361 2024-03-08 06:39:04.824940 mlx_image-0.1.7/src/mlxim/utils/imagenet.py
+-rw-r--r--   0        0        0      287 2024-03-01 16:40:27.649485 mlx_image-0.1.7/src/mlxim/utils/time.py
+-rw-r--r--   0        0        0     2078 2024-03-21 20:52:29.258624 mlx_image-0.1.7/src/mlxim/utils/validation.py
+-rw-r--r--   0        0        0     6733 1970-01-01 00:00:00.000000 mlx_image-0.1.7/PKG-INFO
```

### Comparing `mlx_image-0.1.5/LICENSE` & `mlx_image-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/README.md` & `mlx_image-0.1.7/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -35,14 +35,27 @@
 ```python
 from mlxim.model import list_models
 list_models()
 ```
 > [!WARNING]
 > As of today (2024-03-08) mlx does not support `group` param for nn.Conv2d. Therefore, architectures such as `resnext`, `regnet` or `efficientnet` are not yet supported in `mlx-image`.
 
+### Supported models
+
+List of all models available in `mlx-image`:
+
+* **ResNet**: resnet18, resnet34, resnet50, resnet101, resnet152, wide_resnet50_2, wide_resnet101_2
+* **ViT**:
+    * **supervised**: vit_base_patch16_224, vit_base_patch16_224.swag_lin, vit_base_patch16_384.swag_e2e, vit_base_patch32_224, vit_large_patch16_224, vit_large_patch16_224, vit_large_patch16_224.swag_lin, vit_large_patch16_512.swag_e2e, vit_huge_patch14_224.swag_lin, vit_huge_patch14_518.swag_e2e
+    
+    * **DINO v1**: vit_base_patch16_224.dino, vit_small_patch16_224.dino, vit_small_patch8_224.dino, vit_base_patch8_224.dino
+
+    * **DINO v2**: vit_small_patch14_518.dinov2, vit_base_patch14_518.dinov2, vit_large_patch14_518.dinov2
+* **Swin**: swin_tiny_patch4_window7_224, swin_small_patch4_window7_224, swin_base_patch4_window7_224, swin_v2_tiny_patch4_window8_256, swin_v2_small_patch4_window8_256, swin_v2_base_patch4_window8_256
+
 ## ImageNet-1K Results
 
 Go to [results-imagenet-1k.csv](https://github.com/riccardomusmeci/mlx-image/blob/main/results/results-imagenet-1k.csv) to check every model converted to `mlx-image` and its performance on ImageNet-1K with different settings.
 
 > **TL;DR** performance is comparable to the original models from PyTorch implementations.
```

### Comparing `mlx_image-0.1.5/pyproject.toml` & `mlx_image-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 [tool.poetry]
 name = "mlx-image"
-version = "0.1.5"
+version = "0.1.7"
 description = "Apple MLX image models library"
 authors = ["Riccardo Musmeci <riccardomusmeci92@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "mlxim", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python="^3.10"
-mlx = "0.6.0"
-torch = "*"
-torchvision = "*"
+mlx = "*"
 numpy = "1.26.2"
 tqdm = "*"
 safetensors = "*"
 opencv-python = "*"
 Pillow = "*"
 pandas = "*"
 matplotlib = "*"
@@ -27,14 +25,16 @@
 # dev dependencies
 black = { version = "23.3.0", optional = true, extras = ["jupyter"] }
 ruff = { version = "0.0.264", optional = true }
 mypy = { version = "1.2.0", optional = true }
 pre-commit = { version = "3.3.1", optional = true }
 docstr-coverage = { version = "2.2.0", optional = true }
 twine = { version = ">=4.0.0,<5", optional = true }
+torch = { version = "*", optional = true }
+torchvision = { version = "*", optional = true }
 
 # test dependencies
 pytest = { version = "7.3.1", optional = true }
 pytest-cov = { version = "4.0.0", optional = true }
 # beautify pytest output
 pytest-sugar = { version = "0.9.7", optional = true }
 # parallel test execution
@@ -45,14 +45,16 @@
 dev = [
   "black",
   "ruff",
   "mypy",
   "pre-commit",
   "docstr-coverage",
   "twine",
+  "torch",
+  "torchvision",
 ]
 test = ["pytest", "pytest-cov", "pytest-sugar", "pytest-xdist"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mlx_image-0.1.5/src/mlxim/callbacks/checkpoint.py` & `mlx_image-0.1.7/src/mlxim/callbacks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/data/_utils.py` & `mlx_image-0.1.7/src/mlxim/data/_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/data/folder.py` & `mlx_image-0.1.7/src/mlxim/data/folder.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/data/loader.py` & `mlx_image-0.1.7/src/mlxim/data/loader.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/io/config.py` & `mlx_image-0.1.7/src/mlxim/io/config.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/io/image.py` & `mlx_image-0.1.7/src/mlxim/io/image.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/metrics/classification.py` & `mlx_image-0.1.7/src/mlxim/metrics/classification.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/_config.py` & `mlx_image-0.1.7/src/mlxim/model/_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 from typing import Dict, Optional, Tuple
 
 
 @dataclass
 class Metrics:
     dataset: str
-    accuracy_at_1: float
-    accuracy_at_5: float
+    accuracy_at_1: Optional[float] = None
+    accuracy_at_5: Optional[float] = None
 
 
 @dataclass
 class HFWeights:
     repo_id: str
     filename: str
```

### Comparing `mlx_image-0.1.5/src/mlxim/model/_factory.py` & `mlx_image-0.1.7/src/mlxim/model/_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """Create an image model.
 
     Example:
 
     ```
     >>> from mlxim.model import create_model
 
-    >>> # Create a Phi2 model with no pretrained weights.
+    >>> # Create a resnet model with no pretrained weights.
     >>> model = create_model('resnet18')
 
     >>> # Create a resnet18 model with pretrained weights from HF.
     >>> model = create_model('resnet18', weights=True)
 
     >>> # Create a resnet18 model with custom weights.
     >>> model = create_model('resnet18', weights="path/to/weights.npz")
```

### Comparing `mlx_image-0.1.5/src/mlxim/model/_utils.py` & `mlx_image-0.1.7/src/mlxim/model/_utils.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/layers/_ops.py` & `mlx_image-0.1.7/src/mlxim/model/layers/_ops.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/layers/functional.py` & `mlx_image-0.1.7/src/mlxim/model/layers/functional.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/layers/misc.py` & `mlx_image-0.1.7/src/mlxim/model/layers/misc.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/layers/mlp.py` & `mlx_image-0.1.7/src/mlxim/model/layers/mlp.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/layers/pool.py` & `mlx_image-0.1.7/src/mlxim/model/layers/pool.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/layers/utils.py` & `mlx_image-0.1.7/src/mlxim/model/layers/utils.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/mobilenet/_factory.py` & `mlx_image-0.1.7/src/mlxim/model/mobilenet/_factory.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/mobilenet/mobilenet.py` & `mlx_image-0.1.7/src/mlxim/model/mobilenet/mobilenet.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/regnet/_factory.py` & `mlx_image-0.1.7/src/mlxim/model/regnet/_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         transform=Transform(crop=224, resize=232),
         weights=HFWeights(repo_id="mlx-vision/regnet_x_400mf-mlxim", filename=None),
     )
 }
 
 
 def regnet_y_400mf(num_classes: int = 1000, **kwargs) -> RegNet:  # type: ignore
-
     block_params = BlockParams.from_init_params(
         depth=16, w_0=48, w_a=27.89, w_m=2.09, group_width=8, se_ratio=0.25, **kwargs
     )
     return RegNet(
         block_params=block_params, norm_layer=partial(nn.BatchNorm, eps=1e-05, momentum=0.1), num_classes=num_classes
     )
```

### Comparing `mlx_image-0.1.5/src/mlxim/model/regnet/regnet.py` & `mlx_image-0.1.7/src/mlxim/model/regnet/regnet.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/resnet/__init__.py` & `mlx_image-0.1.7/src/mlxim/model/resnet/__init__.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/resnet/_factory.py` & `mlx_image-0.1.7/src/mlxim/model/resnet/_factory.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/resnet/resnet.py` & `mlx_image-0.1.7/src/mlxim/model/resnet/resnet.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/swin_transformer/__init__.py` & `mlx_image-0.1.7/src/mlxim/model/swin_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/model/swin_transformer/_factory.py` & `mlx_image-0.1.7/src/mlxim/model/swin_transformer/_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from functools import partial
 
 import mlx.nn as nn
-from torchvision.models import swin_transformer
 
 from .._config import HFWeights, Metrics, ModelConfig, Transform
 from .swin_transformer import PatchMergingV2, SwinTransformer, SwinTransformerBlockV2
 
 swin_configs = {
     "swin_tiny_patch4_window7_224": ModelConfig(
         metrics=Metrics(dataset="ImageNet-1K", accuracy_at_1=0.80266, accuracy_at_5=0.94962),
```

### Comparing `mlx_image-0.1.5/src/mlxim/model/swin_transformer/swin_transformer.py` & `mlx_image-0.1.7/src/mlxim/model/swin_transformer/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/trainer/trainer.py` & `mlx_image-0.1.7/src/mlxim/trainer/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,29 +105,30 @@
         epoch_loss = []
         throughput = []
         for batch_idx, batch in enumerate(self.train_loader):
             x, target = batch
 
             tic = time.perf_counter()
             train_step_fn = nn.value_and_grad(self.model, self._train_step)
+
             loss, grads = train_step_fn(x, target)
             self.optimizer.update(self.model, grads)
             mx.eval(self.state)
             toc = time.perf_counter()
 
             epoch_loss.append(loss.item())
             throughput.append(x.shape[0] / (toc - tic))
 
             if batch_idx % self.log_every == 0:
                 print(
                     " | ".join(
                         [
                             f"> iter=[{batch_idx}/{len(self.train_loader)}]",
-                            f"train_loss={np.mean(epoch_loss[-1]):.3f}",
-                            f"train_throughput={np.mean(throughput[-1]):.2f} images/second",
+                            f"train_loss={np.mean(epoch_loss):.3f}",
+                            f"train_throughput={np.mean(throughput):.2f} images/second",
                             f"lr={self.optimizer.state['learning_rate'].item():.5f}",
                         ]
                     )
                 )
 
         epoch_acc = self.train_acc.compute()
         self.train_acc.reset()
@@ -167,26 +168,26 @@
                 "> "
                 + " | ".join(
                     [
                         f"epoch_time={toc-tic:.2f}s",
                         f"train_loss={train_loss:.3f}",
                         f"train_throughput={train_throughput:.2f} images/second",
                     ]
-                    + [f"train_acc@{k}={train_acc[f'acc@{k}']}" for k in self.top_k]
+                    + [f"train_acc@{k}={train_acc[f'acc@{k}']:.3f}" for k in self.top_k]
                 )
             )
 
             if self.val_loader is not None:
                 print("running validation...")
                 val_loss, val_acc, val_throughput = self.val_epoch()
                 print(
                     "> "
                     + " | ".join(
                         [f"val_loss={val_loss:.3f}", f"val_throughput={val_throughput:.2f} images/second"]
-                        + [f"val_acc@{k}={val_acc[f'acc@{k}']}" for k in self.top_k]
+                        + [f"val_acc@{k}={val_acc[f'acc@{k}']:.3f}" for k in self.top_k]
                     )
                 )
 
                 if self.model_checkpoint:
                     val_metrics = {"val_loss": val_loss} | {f"val_acc@{k}": val_acc[f"acc@{k}"] for k in self.top_k}
                     self.model_checkpoint.step(
                         epoch=epoch,
```

### Comparing `mlx_image-0.1.5/src/mlxim/transform/imagenet.py` & `mlx_image-0.1.7/src/mlxim/transform/imagenet.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/utils/imagenet.py` & `mlx_image-0.1.7/src/mlxim/utils/imagenet.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/src/mlxim/utils/validation.py` & `mlx_image-0.1.7/src/mlxim/utils/validation.py`

 * *Files identical despite different names*

### Comparing `mlx_image-0.1.5/PKG-INFO` & `mlx_image-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlx-image
-Version: 0.1.5
+Version: 0.1.7
 Summary: Apple MLX image models library
 Author: Riccardo Musmeci
 Author-email: riccardomusmeci92@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,28 +13,28 @@
 Provides-Extra: test
 Requires-Dist: Pillow
 Requires-Dist: albumentations
 Requires-Dist: black[jupyter] (==23.3.0) ; extra == "dev"
 Requires-Dist: docstr-coverage (==2.2.0) ; extra == "dev"
 Requires-Dist: huggingface_hub
 Requires-Dist: matplotlib
-Requires-Dist: mlx (==0.6.0)
+Requires-Dist: mlx
 Requires-Dist: mypy (==1.2.0) ; extra == "dev"
 Requires-Dist: numpy (==1.26.2)
 Requires-Dist: opencv-python
 Requires-Dist: pandas
 Requires-Dist: pre-commit (==3.3.1) ; extra == "dev"
 Requires-Dist: pytest (==7.3.1) ; extra == "test"
 Requires-Dist: pytest-cov (==4.0.0) ; extra == "test"
 Requires-Dist: pytest-sugar (==0.9.7) ; extra == "test"
 Requires-Dist: pytest-xdist (==3.2.1) ; extra == "test"
 Requires-Dist: ruff (==0.0.264) ; extra == "dev"
 Requires-Dist: safetensors
-Requires-Dist: torch
-Requires-Dist: torchvision
+Requires-Dist: torch ; extra == "dev"
+Requires-Dist: torchvision ; extra == "dev"
 Requires-Dist: tqdm
 Requires-Dist: twine (>=4.0.0,<5) ; extra == "dev"
 Requires-Dist: types-pyyaml (>=6.0.12.12,<7.0.0.0)
 Description-Content-Type: text/markdown
 
 # **mlx-image**
 Image models based on [Apple MLX framework](https://github.com/ml-explore/mlx) for Apple Silicon machines.
@@ -73,14 +73,27 @@
 ```python
 from mlxim.model import list_models
 list_models()
 ```
 > [!WARNING]
 > As of today (2024-03-08) mlx does not support `group` param for nn.Conv2d. Therefore, architectures such as `resnext`, `regnet` or `efficientnet` are not yet supported in `mlx-image`.
 
+### Supported models
+
+List of all models available in `mlx-image`:
+
+* **ResNet**: resnet18, resnet34, resnet50, resnet101, resnet152, wide_resnet50_2, wide_resnet101_2
+* **ViT**:
+    * **supervised**: vit_base_patch16_224, vit_base_patch16_224.swag_lin, vit_base_patch16_384.swag_e2e, vit_base_patch32_224, vit_large_patch16_224, vit_large_patch16_224, vit_large_patch16_224.swag_lin, vit_large_patch16_512.swag_e2e, vit_huge_patch14_224.swag_lin, vit_huge_patch14_518.swag_e2e
+    
+    * **DINO v1**: vit_base_patch16_224.dino, vit_small_patch16_224.dino, vit_small_patch8_224.dino, vit_base_patch8_224.dino
+
+    * **DINO v2**: vit_small_patch14_518.dinov2, vit_base_patch14_518.dinov2, vit_large_patch14_518.dinov2
+* **Swin**: swin_tiny_patch4_window7_224, swin_small_patch4_window7_224, swin_base_patch4_window7_224, swin_v2_tiny_patch4_window8_256, swin_v2_small_patch4_window8_256, swin_v2_base_patch4_window8_256
+
 ## ImageNet-1K Results
 
 Go to [results-imagenet-1k.csv](https://github.com/riccardomusmeci/mlx-image/blob/main/results/results-imagenet-1k.csv) to check every model converted to `mlx-image` and its performance on ImageNet-1K with different settings.
 
 > **TL;DR** performance is comparable to the original models from PyTorch implementations.
```

