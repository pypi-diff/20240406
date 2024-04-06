# Comparing `tmp/learning3d-0.0.6.tar.gz` & `tmp/learning3d-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning3d-0.0.6.tar", last modified: Sat Apr  6 18:36:01 2024, max compression
+gzip compressed data, was "learning3d-0.0.7.tar", last modified: Sat Apr  6 19:04:47 2024, max compression
```

## Comparing `learning3d-0.0.6.tar` & `learning3d-0.0.7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.803932 learning3d-0.0.6/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1098 2023-06-23 11:04:02.000000 learning3d-0.0.6/LICENSE
--rw-r--r--   0 vinitsarode   (501) staff       (20)      102 2024-04-06 17:33:11.000000 learning3d-0.0.6/MANIFEST.in
--rw-r--r--   0 vinitsarode   (501) staff       (20)    15802 2024-04-06 18:36:01.803643 learning3d-0.0.6/PKG-INFO
--rw-r--r--   0 vinitsarode   (501) staff       (20)    14918 2024-03-25 01:41:24.000000 learning3d-0.0.6/README.md
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.784354 learning3d-0.0.6/data/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.787691 learning3d-0.0.6/data/modelnet40_ply_hdf5_2048/
--rw-rw-r--   0 vinitsarode   (501) staff       (20)      275 2017-02-02 21:28:14.000000 learning3d-0.0.6/data/modelnet40_ply_hdf5_2048/shape_names.txt
--rw-rw-r--   0 vinitsarode   (501) staff       (20)       96 2017-02-01 22:37:48.000000 learning3d-0.0.6/data/modelnet40_ply_hdf5_2048/test_files.txt
--rw-rw-r--   0 vinitsarode   (501) staff       (20)      245 2017-02-01 22:37:41.000000 learning3d-0.0.6/data/modelnet40_ply_hdf5_2048/train_files.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)      757 2024-04-06 18:35:46.000000 learning3d-0.0.6/pyproject.toml
--rw-r--r--   0 vinitsarode   (501) staff       (20)      172 2024-04-06 17:33:11.000000 learning3d-0.0.6/requirements.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-06 18:36:01.803988 learning3d-0.0.6/setup.cfg
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.784573 learning3d-0.0.6/src/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.787971 learning3d-0.0.6/src/learning3d/
--rw-r--r--   0 vinitsarode   (501) staff       (20)        0 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/__init__.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.789450 learning3d-0.0.6/src/learning3d/data_utils/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      261 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/data_utils/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    14813 2024-04-06 18:34:07.000000 learning3d-0.0.6/src/learning3d/data_utils/dataloaders.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4828 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/data_utils/user_data.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.793765 learning3d-0.0.6/src/learning3d/examples/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5606 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_dcp.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5597 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_deepgmr.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6405 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_masknet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6859 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_masknet2.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4342 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_pcn.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4366 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_pcrnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4456 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_pnlk.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4673 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_pointconv.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4324 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_pointnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4901 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_prnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4476 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/test_rpmnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8773 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_PointNetLK.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     9511 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_dcp.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     9397 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_deepgmr.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8889 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_masknet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     7542 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_pcn.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8198 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_pcrnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8939 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_pointconv.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8840 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_pointnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8373 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_prnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8530 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/examples/train_rpmnet.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.795102 learning3d-0.0.6/src/learning3d/losses/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      425 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2121 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/chamfer_distance.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      374 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/classification.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      583 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/correspondence_loss.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.784993 learning3d-0.0.6/src/learning3d/losses/cuda/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.795857 learning3d-0.0.6/src/learning3d/losses/cuda/chamfer_distance/
--rw-r--r--   0 vinitsarode   (501) staff       (20)       46 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/chamfer_distance/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6260 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5070 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cu
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1926 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.796049 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.796217 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1116 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/emd_loss_layer.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.796540 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/include/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.796722 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     9826 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/emd.cuh
--rw-r--r--   0 vinitsarode   (501) staff       (20)      469 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda_helper.h
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1215 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/include/emd.h
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.797045 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/layer/
--rw-r--r--   0 vinitsarode   (501) staff       (20)       35 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/layer/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1019 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/layer/emd_loss_layer.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.797193 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/src/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.797350 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1462 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu
--rw-r--r--   0 vinitsarode   (501) staff       (20)       17 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/src/emd.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)      574 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/setup.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      389 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/emd.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      682 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/frobenius_norm.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      453 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/losses/rmse_features.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.800415 learning3d-0.0.6/src/learning3d/models/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      473 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1205 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/classifier.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3377 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/dcp.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5298 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/deepgmr.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3057 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/dgcnn.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2705 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/masknet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     9063 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/masknet2.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5346 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/pcn.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2755 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/pcrnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5151 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/pointconv.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3238 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/pointnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5805 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/pointnetlk.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      412 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/pooling.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2894 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/ppfnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    18499 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/prnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    11517 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/rpmnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1166 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/models/segmentation.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.801961 learning3d-0.0.6/src/learning3d/ops/
--rw-r--r--   0 vinitsarode   (501) staff       (20)        0 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/ops/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1764 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/ops/data_utils.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4154 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/ops/invmat.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6793 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/ops/quaternion.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3957 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/ops/se3.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5228 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/ops/sinc.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5166 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/ops/so3.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    12806 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/ops/transform_functions.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.803046 learning3d-0.0.6/src/learning3d/utils/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      286 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/utils/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    14331 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/utils/pointconv_util.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     7989 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/utils/ppfnet_util.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1936 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/utils/svd.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8974 2024-04-06 17:33:11.000000 learning3d-0.0.6/src/learning3d/utils/transformer.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 18:36:01.803309 learning3d-0.0.6/src/learning3d.egg-info/
--rw-r--r--   0 vinitsarode   (501) staff       (20)    15802 2024-04-06 18:36:01.000000 learning3d-0.0.6/src/learning3d.egg-info/PKG-INFO
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3383 2024-04-06 18:36:01.000000 learning3d-0.0.6/src/learning3d.egg-info/SOURCES.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-06 18:36:01.000000 learning3d-0.0.6/src/learning3d.egg-info/dependency_links.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)      173 2024-04-06 18:36:01.000000 learning3d-0.0.6/src/learning3d.egg-info/requires.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       11 2024-04-06 18:36:01.000000 learning3d-0.0.6/src/learning3d.egg-info/top_level.txt
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.108907 learning3d-0.0.7/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1098 2023-06-23 11:04:02.000000 learning3d-0.0.7/LICENSE
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      102 2024-04-06 17:33:11.000000 learning3d-0.0.7/MANIFEST.in
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    15802 2024-04-06 19:04:47.108643 learning3d-0.0.7/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    14918 2024-03-25 01:41:24.000000 learning3d-0.0.7/README.md
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.084686 learning3d-0.0.7/data/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.088375 learning3d-0.0.7/data/modelnet40_ply_hdf5_2048/
+-rw-rw-r--   0 vinitsarode   (501) staff       (20)      275 2017-02-02 21:28:14.000000 learning3d-0.0.7/data/modelnet40_ply_hdf5_2048/shape_names.txt
+-rw-rw-r--   0 vinitsarode   (501) staff       (20)       96 2017-02-01 22:37:48.000000 learning3d-0.0.7/data/modelnet40_ply_hdf5_2048/test_files.txt
+-rw-rw-r--   0 vinitsarode   (501) staff       (20)      245 2017-02-01 22:37:41.000000 learning3d-0.0.7/data/modelnet40_ply_hdf5_2048/train_files.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      757 2024-04-06 19:04:30.000000 learning3d-0.0.7/pyproject.toml
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      172 2024-04-06 17:33:11.000000 learning3d-0.0.7/requirements.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-06 19:04:47.108958 learning3d-0.0.7/setup.cfg
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.084897 learning3d-0.0.7/src/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.088665 learning3d-0.0.7/src/learning3d/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        0 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/__init__.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.089996 learning3d-0.0.7/src/learning3d/data_utils/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      261 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/data_utils/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    14675 2024-04-06 19:04:05.000000 learning3d-0.0.7/src/learning3d/data_utils/dataloaders.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4828 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/data_utils/user_data.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.095564 learning3d-0.0.7/src/learning3d/examples/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5606 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_dcp.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5597 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_deepgmr.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     6405 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_masknet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     6859 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_masknet2.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4342 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_pcn.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4366 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_pcrnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4456 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_pnlk.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4673 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_pointconv.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4324 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_pointnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4901 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_prnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4476 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/test_rpmnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8773 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_PointNetLK.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     9511 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_dcp.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     9397 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_deepgmr.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8889 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_masknet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     7542 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_pcn.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8198 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_pcrnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8939 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_pointconv.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8840 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_pointnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8373 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_prnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8530 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/examples/train_rpmnet.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.097187 learning3d-0.0.7/src/learning3d/losses/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      425 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     2121 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/chamfer_distance.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      374 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/classification.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      583 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/correspondence_loss.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.085315 learning3d-0.0.7/src/learning3d/losses/cuda/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.098214 learning3d-0.0.7/src/learning3d/losses/cuda/chamfer_distance/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       46 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/chamfer_distance/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     6260 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cpp
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5070 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cu
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1926 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.098475 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.098757 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1116 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/emd_loss_layer.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.099231 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/include/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.099429 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     9826 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/emd.cuh
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      469 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda_helper.h
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1215 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/include/emd.h
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.099848 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/layer/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       35 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/layer/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1019 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/layer/emd_loss_layer.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.100110 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/src/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.100329 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1462 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       17 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/src/emd.cpp
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      574 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/setup.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      389 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/emd.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      682 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/frobenius_norm.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      453 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/losses/rmse_features.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.104790 learning3d-0.0.7/src/learning3d/models/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      473 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1205 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/classifier.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3377 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/dcp.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5298 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/deepgmr.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3057 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/dgcnn.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     2705 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/masknet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     9063 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/masknet2.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5346 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/pcn.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     2755 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/pcrnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5151 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/pointconv.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3238 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/pointnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5805 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/pointnetlk.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      412 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/pooling.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     2894 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/ppfnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    18499 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/prnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    11517 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/rpmnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1166 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/models/segmentation.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.106746 learning3d-0.0.7/src/learning3d/ops/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        0 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/ops/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1764 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/ops/data_utils.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4154 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/ops/invmat.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     6793 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/ops/quaternion.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3957 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/ops/se3.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5228 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/ops/sinc.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5166 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/ops/so3.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    12806 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/ops/transform_functions.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.107969 learning3d-0.0.7/src/learning3d/utils/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      286 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/utils/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    14331 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/utils/pointconv_util.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     7989 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/utils/ppfnet_util.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1936 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/utils/svd.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8974 2024-04-06 17:33:11.000000 learning3d-0.0.7/src/learning3d/utils/transformer.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 19:04:47.108325 learning3d-0.0.7/src/learning3d.egg-info/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    15802 2024-04-06 19:04:47.000000 learning3d-0.0.7/src/learning3d.egg-info/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3383 2024-04-06 19:04:47.000000 learning3d-0.0.7/src/learning3d.egg-info/SOURCES.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-06 19:04:47.000000 learning3d-0.0.7/src/learning3d.egg-info/dependency_links.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      173 2024-04-06 19:04:47.000000 learning3d-0.0.7/src/learning3d.egg-info/requires.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       11 2024-04-06 19:04:47.000000 learning3d-0.0.7/src/learning3d.egg-info/top_level.txt
```

### Comparing `learning3d-0.0.6/LICENSE` & `learning3d-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/PKG-INFO` & `learning3d-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learning3d
-Version: 0.0.6
+Version: 0.0.7
 Summary: Learning3D: A Modern Library for Deep Learning on 3D Point Clouds Data
 Author-email: Vinit Sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/vinits5/learning3d
 Project-URL: Issues, https://github.com/vinits5/learning3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `learning3d-0.0.6/README.md` & `learning3d-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/pyproject.toml` & `learning3d-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "learning3d"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name="Vinit Sarode", email="vinitsarode5@gmail.com"},
 ]
 description = "Learning3D: A Modern Library for Deep Learning on 3D Point Clouds Data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `learning3d-0.0.6/src/learning3d/data_utils/dataloaders.py` & `learning3d-0.0.7/src/learning3d/data_utils/dataloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,42 +222,42 @@
 		file = open(os.path.join(DATA_DIR, 'modelnet40_ply_hdf5_2048', 'shape_names.txt'), 'r')
 		shape_names = file.read()
 		shape_names = np.array(shape_names.split('\n')[:-1])
 		return shape_names
 
 
 class ClassificationData(Dataset):
-	def __init__(self, data_class=ModelNet40Data, root_dir='./'):
+	def __init__(self, data_class):
 		super(ClassificationData, self).__init__()
-		self.set_class(data_class, root_dir)
+		self.set_class(data_class)
 
 	def __len__(self):
 		return len(self.data_class)
 
-	def set_class(self, data_class, root_dir):
-		self.data_class = data_class(root_dir=root_dir)
+	def set_class(self, data_class):
+		self.data_class = data_class
 
 	def get_shape(self, label):
 		try:
 			return self.data_class.get_shape(label)
 		except:
 			return -1
 
 	def __getitem__(self, index):
 		return self.data_class[index]
 
 
 class RegistrationData(Dataset):
-	def __init__(self, algorithm, root_dir='./', data_class=ModelNet40Data, partial_source=False, partial_template=False, noise=False, additional_params={}):
+	def __init__(self, algorithm, data_class, partial_source=False, partial_template=False, noise=False, additional_params={}):
 		super(RegistrationData, self).__init__()
 		available_algorithms = ['PCRNet', 'PointNetLK', 'DCP', 'PRNet', 'iPCRNet', 'RPMNet', 'DeepGMR']
 		if algorithm in available_algorithms: self.algorithm = algorithm
 		else: raise Exception("Algorithm not available for registration.")
 		
-		self.set_class(data_class, root_dir)
+		self.set_class(data_class)
 		self.partial_template = partial_template
 		self.partial_source = partial_source
 		self.noise = noise
 		self.additional_params = additional_params
 		self.use_rri = False
 
 		if self.algorithm == 'PCRNet' or self.algorithm == 'iPCRNet':
@@ -279,16 +279,16 @@
 			if 'nearest_neighbors' in self.additional_params.keys() and self.additional_params['nearest_neighbors'] > 0:
 				self.use_rri = True
 				self.nearest_neighbors = self.additional_params['nearest_neighbors']
 
 	def __len__(self):
 		return len(self.data_class)
 
-	def set_class(self, data_class, root_dir):
-		self.data_class = data_class(root_dir=root_dir)
+	def set_class(self, data_class):
+		self.data_class = data_class
 
 	def __getitem__(self, index):
 		template, label = self.data_class[index]
 		self.transforms.index = index				# for fixed transformations in PCRNet.
 		source = self.transforms(template)
 
 		# Check for Partial Data.
```

### Comparing `learning3d-0.0.6/src/learning3d/data_utils/user_data.py` & `learning3d-0.0.7/src/learning3d/data_utils/user_data.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_dcp.py` & `learning3d-0.0.7/src/learning3d/examples/test_dcp.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_deepgmr.py` & `learning3d-0.0.7/src/learning3d/examples/test_deepgmr.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_masknet.py` & `learning3d-0.0.7/src/learning3d/examples/test_masknet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_masknet2.py` & `learning3d-0.0.7/src/learning3d/examples/test_masknet2.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_pcn.py` & `learning3d-0.0.7/src/learning3d/examples/test_pcn.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_pcrnet.py` & `learning3d-0.0.7/src/learning3d/examples/test_pcrnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_pnlk.py` & `learning3d-0.0.7/src/learning3d/examples/test_pnlk.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_pointconv.py` & `learning3d-0.0.7/src/learning3d/examples/test_pointconv.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_pointnet.py` & `learning3d-0.0.7/src/learning3d/examples/test_pointnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_prnet.py` & `learning3d-0.0.7/src/learning3d/examples/test_prnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/test_rpmnet.py` & `learning3d-0.0.7/src/learning3d/examples/test_rpmnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_PointNetLK.py` & `learning3d-0.0.7/src/learning3d/examples/train_PointNetLK.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_dcp.py` & `learning3d-0.0.7/src/learning3d/examples/train_dcp.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_deepgmr.py` & `learning3d-0.0.7/src/learning3d/examples/train_deepgmr.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_masknet.py` & `learning3d-0.0.7/src/learning3d/examples/train_masknet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_pcn.py` & `learning3d-0.0.7/src/learning3d/examples/train_pcn.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_pcrnet.py` & `learning3d-0.0.7/src/learning3d/examples/train_pcrnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_pointconv.py` & `learning3d-0.0.7/src/learning3d/examples/train_pointconv.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_pointnet.py` & `learning3d-0.0.7/src/learning3d/examples/train_pointnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_prnet.py` & `learning3d-0.0.7/src/learning3d/examples/train_prnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/examples/train_rpmnet.py` & `learning3d-0.0.7/src/learning3d/examples/train_rpmnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/chamfer_distance.py` & `learning3d-0.0.7/src/learning3d/losses/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/correspondence_loss.py` & `learning3d-0.0.7/src/learning3d/losses/correspondence_loss.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cpp` & `learning3d-0.0.7/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cpp`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cu` & `learning3d-0.0.7/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cu`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.py` & `learning3d-0.0.7/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/emd_loss_layer.py` & `learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/emd_loss_layer.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/emd.cuh` & `learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/emd.cuh`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/include/emd.h` & `learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/include/emd.h`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/layer/emd_loss_layer.py` & `learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/layer/emd_loss_layer.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu` & `learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/cuda/emd_torch/setup.py` & `learning3d-0.0.7/src/learning3d/losses/cuda/emd_torch/setup.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/losses/frobenius_norm.py` & `learning3d-0.0.7/src/learning3d/losses/frobenius_norm.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/classifier.py` & `learning3d-0.0.7/src/learning3d/models/classifier.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/dcp.py` & `learning3d-0.0.7/src/learning3d/models/dcp.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/deepgmr.py` & `learning3d-0.0.7/src/learning3d/models/deepgmr.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/dgcnn.py` & `learning3d-0.0.7/src/learning3d/models/dgcnn.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/masknet.py` & `learning3d-0.0.7/src/learning3d/models/masknet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/masknet2.py` & `learning3d-0.0.7/src/learning3d/models/masknet2.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/pcn.py` & `learning3d-0.0.7/src/learning3d/models/pcn.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/pcrnet.py` & `learning3d-0.0.7/src/learning3d/models/pcrnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/pointconv.py` & `learning3d-0.0.7/src/learning3d/models/pointconv.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/pointnet.py` & `learning3d-0.0.7/src/learning3d/models/pointnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/pointnetlk.py` & `learning3d-0.0.7/src/learning3d/models/pointnetlk.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/ppfnet.py` & `learning3d-0.0.7/src/learning3d/models/ppfnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/prnet.py` & `learning3d-0.0.7/src/learning3d/models/prnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/rpmnet.py` & `learning3d-0.0.7/src/learning3d/models/rpmnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/models/segmentation.py` & `learning3d-0.0.7/src/learning3d/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/ops/data_utils.py` & `learning3d-0.0.7/src/learning3d/ops/data_utils.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/ops/invmat.py` & `learning3d-0.0.7/src/learning3d/ops/invmat.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/ops/quaternion.py` & `learning3d-0.0.7/src/learning3d/ops/quaternion.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/ops/se3.py` & `learning3d-0.0.7/src/learning3d/ops/se3.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/ops/sinc.py` & `learning3d-0.0.7/src/learning3d/ops/sinc.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/ops/so3.py` & `learning3d-0.0.7/src/learning3d/ops/so3.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/ops/transform_functions.py` & `learning3d-0.0.7/src/learning3d/ops/transform_functions.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/utils/pointconv_util.py` & `learning3d-0.0.7/src/learning3d/utils/pointconv_util.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/utils/ppfnet_util.py` & `learning3d-0.0.7/src/learning3d/utils/ppfnet_util.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/utils/svd.py` & `learning3d-0.0.7/src/learning3d/utils/svd.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d/utils/transformer.py` & `learning3d-0.0.7/src/learning3d/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.6/src/learning3d.egg-info/PKG-INFO` & `learning3d-0.0.7/src/learning3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learning3d
-Version: 0.0.6
+Version: 0.0.7
 Summary: Learning3D: A Modern Library for Deep Learning on 3D Point Clouds Data
 Author-email: Vinit Sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/vinits5/learning3d
 Project-URL: Issues, https://github.com/vinits5/learning3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `learning3d-0.0.6/src/learning3d.egg-info/SOURCES.txt` & `learning3d-0.0.7/src/learning3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

