# Comparing `tmp/learning3d-0.0.2.tar.gz` & `tmp/learning3d-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learning3d-0.0.2.tar", last modified: Fri Apr  5 14:25:44 2024, max compression
+gzip compressed data, was "learning3d-0.0.3.tar", last modified: Sat Apr  6 14:07:05 2024, max compression
```

## Comparing `learning3d-0.0.2.tar` & `learning3d-0.0.3.tar`

### file list

```diff
@@ -1,157 +1,111 @@
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.399842 learning3d-0.0.2/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1098 2023-06-23 11:04:02.000000 learning3d-0.0.2/LICENSE
--rw-r--r--   0 vinitsarode   (501) staff       (20)      102 2024-04-05 14:14:21.000000 learning3d-0.0.2/MANIFEST.in
--rw-r--r--   0 vinitsarode   (501) staff       (20)    15802 2024-04-05 14:25:44.399520 learning3d-0.0.2/PKG-INFO
--rw-r--r--   0 vinitsarode   (501) staff       (20)    14918 2024-03-25 01:41:24.000000 learning3d-0.0.2/README.md
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.326908 learning3d-0.0.2/data/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.331103 learning3d-0.0.2/data/modelnet40_ply_hdf5_2048/
--rw-rw-r--   0 vinitsarode   (501) staff       (20)      275 2017-02-02 21:28:14.000000 learning3d-0.0.2/data/modelnet40_ply_hdf5_2048/shape_names.txt
--rw-rw-r--   0 vinitsarode   (501) staff       (20)       96 2017-02-01 22:37:48.000000 learning3d-0.0.2/data/modelnet40_ply_hdf5_2048/test_files.txt
--rw-rw-r--   0 vinitsarode   (501) staff       (20)      245 2017-02-01 22:37:41.000000 learning3d-0.0.2/data/modelnet40_ply_hdf5_2048/train_files.txt
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.327035 learning3d-0.0.2/pretrained/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.331399 learning3d-0.0.2/pretrained/exp_prnet/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      727 2023-06-23 11:04:03.000000 learning3d-0.0.2/pretrained/exp_prnet/args.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)      757 2024-04-05 14:25:31.000000 learning3d-0.0.2/pyproject.toml
--rw-r--r--   0 vinitsarode   (501) staff       (20)      172 2024-04-05 14:25:28.000000 learning3d-0.0.2/requirements.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-05 14:25:44.399888 learning3d-0.0.2/setup.cfg
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.327236 learning3d-0.0.2/src/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.331740 learning3d-0.0.2/src/learning3d/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      189 2024-04-05 14:11:13.000000 learning3d-0.0.2/src/learning3d/__init__.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.334656 learning3d-0.0.2/src/learning3d/data_utils/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      261 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/data_utils/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    14871 2024-03-25 01:41:24.000000 learning3d-0.0.2/src/learning3d/data_utils/dataloaders.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4828 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/data_utils/user_data.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.339552 learning3d-0.0.2/src/learning3d/examples/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5606 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_dcp.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5597 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_deepgmr.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4603 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_flownet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6405 2023-10-22 05:21:13.000000 learning3d-0.0.2/src/learning3d/examples/test_masknet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6859 2024-03-25 01:41:24.000000 learning3d-0.0.2/src/learning3d/examples/test_masknet2.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4342 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_pcn.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4366 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_pcrnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4456 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_pnlk.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4673 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_pointconv.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4324 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_pointnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4901 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_prnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4476 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/test_rpmnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8773 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_PointNetLK.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     9511 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_dcp.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     9397 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_deepgmr.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    10369 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_flownet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8889 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_masknet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     7542 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_pcn.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8198 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_pcrnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8939 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_pointconv.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8840 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_pointnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8373 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_prnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8530 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/examples/train_rpmnet.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.340825 learning3d-0.0.2/src/learning3d/losses/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      425 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2121 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/chamfer_distance.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      374 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/classification.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      583 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/correspondence_loss.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.327643 learning3d-0.0.2/src/learning3d/losses/cuda/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.341499 learning3d-0.0.2/src/learning3d/losses/cuda/chamfer_distance/
--rw-r--r--   0 vinitsarode   (501) staff       (20)       46 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/chamfer_distance/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6260 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5070 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cu
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1926 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.341678 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.341845 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1116 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/emd_loss_layer.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.342188 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/include/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.342348 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     9826 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/emd.cuh
--rw-r--r--   0 vinitsarode   (501) staff       (20)      469 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda_helper.h
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1215 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/include/emd.h
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.342674 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/layer/
--rw-r--r--   0 vinitsarode   (501) staff       (20)       35 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/layer/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1019 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/layer/emd_loss_layer.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.343671 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/src/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.343872 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1462 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu
--rw-r--r--   0 vinitsarode   (501) staff       (20)       17 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/src/emd.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)      574 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/setup.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      389 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/emd.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      682 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/frobenius_norm.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      453 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/losses/rmse_features.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.347219 learning3d-0.0.2/src/learning3d/models/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      642 2024-03-25 01:41:24.000000 learning3d-0.0.2/src/learning3d/models/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1205 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/classifier.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3377 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/dcp.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5298 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/deepgmr.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3057 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/dgcnn.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    17667 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/flownet3d.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2705 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/masknet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     9063 2024-03-25 01:41:24.000000 learning3d-0.0.2/src/learning3d/models/masknet2.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5346 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/pcn.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2755 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/pcrnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5151 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/pointconv.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3238 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/pointnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5805 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/pointnetlk.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      412 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/pooling.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2894 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/ppfnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    18499 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/prnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    11517 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/rpmnet.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1166 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/models/segmentation.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.348467 learning3d-0.0.2/src/learning3d/ops/
--rw-r--r--   0 vinitsarode   (501) staff       (20)        0 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/ops/__init__.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1764 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/ops/data_utils.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     4154 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/ops/invmat.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6793 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/ops/quaternion.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3957 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/ops/se3.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5228 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/ops/sinc.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5166 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/ops/so3.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    12806 2023-06-23 11:04:02.000000 learning3d-0.0.2/src/learning3d/ops/transform_functions.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.349684 learning3d-0.0.2/src/learning3d/utils/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      442 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/__init__.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.350567 learning3d-0.0.2/src/learning3d/utils/lib/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.328610 learning3d-0.0.2/src/learning3d/utils/lib/build/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.350736 learning3d-0.0.2/src/learning3d/utils/lib/build/lib.linux-x86_64-3.5/
--rwxr-xr-x   0 vinitsarode   (501) staff       (20)  7222568 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/lib.linux-x86_64-3.5/pointnet2_cuda.cpython-35m-x86_64-linux-gnu.so
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.328660 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.388816 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/
--rw-r--r--   0 vinitsarode   (501) staff       (20)  2730016 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/ball_query.o
--rw-r--r--   0 vinitsarode   (501) staff       (20)    13912 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/ball_query_gpu.o
--rw-r--r--   0 vinitsarode   (501) staff       (20)  2490896 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/group_points.o
--rw-r--r--   0 vinitsarode   (501) staff       (20)    17048 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/group_points_gpu.o
--rw-r--r--   0 vinitsarode   (501) staff       (20)  2503232 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/interpolate.o
--rw-r--r--   0 vinitsarode   (501) staff       (20)    32712 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/interpolate_gpu.o
--rw-r--r--   0 vinitsarode   (501) staff       (20)  7242784 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/pointnet2_api.o
--rw-r--r--   0 vinitsarode   (501) staff       (20)  2495440 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/sampling.o
--rw-r--r--   0 vinitsarode   (501) staff       (20)    95544 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/sampling_gpu.o
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.392163 learning3d-0.0.2/src/learning3d/utils/lib/dist/
--rw-r--r--   0 vinitsarode   (501) staff       (20)  2241340 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/dist/pointnet2-0.0.0-py3.5-linux-x86_64.egg
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.396178 learning3d-0.0.2/src/learning3d/utils/lib/pointnet2.egg-info/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      328 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/pointnet2.egg-info/SOURCES.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/pointnet2.egg-info/dependency_links.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       15 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/pointnet2.egg-info/top_level.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6339 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/pointnet2_modules.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)    10637 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/pointnet2_utils.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     6173 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/pytorch_utils.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)      679 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/setup.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.398658 learning3d-0.0.2/src/learning3d/utils/lib/src/
--rw-r--r--   0 vinitsarode   (501) staff       (20)      933 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/ball_query.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2050 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/ball_query_gpu.cu
--rw-r--r--   0 vinitsarode   (501) staff       (20)      476 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/ball_query_gpu.h
--rw-r--r--   0 vinitsarode   (501) staff       (20)      353 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/cuda_utils.h
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1171 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/group_points.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)     3307 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/group_points_gpu.cu
--rw-r--r--   0 vinitsarode   (501) staff       (20)      836 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/group_points_gpu.h
--rw-r--r--   0 vinitsarode   (501) staff       (20)     2521 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/interpolate.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)     7470 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/interpolate_gpu.cu
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1477 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/interpolate_gpu.h
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1213 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/pointnet2_api.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1549 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/sampling.cpp
--rw-r--r--   0 vinitsarode   (501) staff       (20)     7934 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/sampling_gpu.cu
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1045 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/lib/src/sampling_gpu.h
--rw-r--r--   0 vinitsarode   (501) staff       (20)    14331 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/pointconv_util.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     7989 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/ppfnet_util.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     1936 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/svd.py
--rw-r--r--   0 vinitsarode   (501) staff       (20)     8974 2023-06-23 11:04:03.000000 learning3d-0.0.2/src/learning3d/utils/transformer.py
-drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:25:44.398925 learning3d-0.0.2/src/learning3d.egg-info/
--rw-r--r--   0 vinitsarode   (501) staff       (20)    15802 2024-04-05 14:25:44.000000 learning3d-0.0.2/src/learning3d.egg-info/PKG-INFO
--rw-r--r--   0 vinitsarode   (501) staff       (20)     5333 2024-04-05 14:25:44.000000 learning3d-0.0.2/src/learning3d.egg-info/SOURCES.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-05 14:25:44.000000 learning3d-0.0.2/src/learning3d.egg-info/dependency_links.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)      173 2024-04-05 14:25:44.000000 learning3d-0.0.2/src/learning3d.egg-info/requires.txt
--rw-r--r--   0 vinitsarode   (501) staff       (20)       11 2024-04-05 14:25:44.000000 learning3d-0.0.2/src/learning3d.egg-info/top_level.txt
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.137566 learning3d-0.0.3/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1098 2023-06-23 11:04:02.000000 learning3d-0.0.3/LICENSE
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      102 2024-04-05 14:14:21.000000 learning3d-0.0.3/MANIFEST.in
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    15802 2024-04-06 14:07:05.137295 learning3d-0.0.3/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    14918 2024-03-25 01:41:24.000000 learning3d-0.0.3/README.md
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.117644 learning3d-0.0.3/data/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.120626 learning3d-0.0.3/data/modelnet40_ply_hdf5_2048/
+-rw-rw-r--   0 vinitsarode   (501) staff       (20)      275 2017-02-02 21:28:14.000000 learning3d-0.0.3/data/modelnet40_ply_hdf5_2048/shape_names.txt
+-rw-rw-r--   0 vinitsarode   (501) staff       (20)       96 2017-02-01 22:37:48.000000 learning3d-0.0.3/data/modelnet40_ply_hdf5_2048/test_files.txt
+-rw-rw-r--   0 vinitsarode   (501) staff       (20)      245 2017-02-01 22:37:41.000000 learning3d-0.0.3/data/modelnet40_ply_hdf5_2048/train_files.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      757 2024-04-06 13:57:38.000000 learning3d-0.0.3/pyproject.toml
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      172 2024-04-05 14:25:28.000000 learning3d-0.0.3/requirements.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       38 2024-04-06 14:07:05.137615 learning3d-0.0.3/setup.cfg
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.117853 learning3d-0.0.3/src/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.120911 learning3d-0.0.3/src/learning3d/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        0 2024-04-05 14:44:55.000000 learning3d-0.0.3/src/learning3d/__init__.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.122238 learning3d-0.0.3/src/learning3d/data_utils/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      261 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/data_utils/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    14871 2024-03-25 01:41:24.000000 learning3d-0.0.3/src/learning3d/data_utils/dataloaders.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4828 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/data_utils/user_data.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.126816 learning3d-0.0.3/src/learning3d/examples/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5606 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_dcp.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5597 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_deepgmr.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     6405 2023-10-22 05:21:13.000000 learning3d-0.0.3/src/learning3d/examples/test_masknet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     6859 2024-03-25 01:41:24.000000 learning3d-0.0.3/src/learning3d/examples/test_masknet2.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4342 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_pcn.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4366 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_pcrnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4456 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_pnlk.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4673 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_pointconv.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4324 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_pointnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4901 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_prnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4476 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/test_rpmnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8773 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_PointNetLK.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     9511 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_dcp.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     9397 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_deepgmr.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8889 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_masknet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     7542 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_pcn.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8198 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_pcrnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8939 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_pointconv.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8840 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_pointnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8373 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_prnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8530 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/examples/train_rpmnet.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.128198 learning3d-0.0.3/src/learning3d/losses/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      425 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     2121 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/chamfer_distance.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      374 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/classification.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      583 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/correspondence_loss.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.118263 learning3d-0.0.3/src/learning3d/losses/cuda/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.128975 learning3d-0.0.3/src/learning3d/losses/cuda/chamfer_distance/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       46 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/chamfer_distance/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     6260 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cpp
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5070 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cu
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1926 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.129168 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.129343 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1116 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/emd_loss_layer.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.129685 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/include/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.129844 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     9826 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/emd.cuh
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      469 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda_helper.h
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1215 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/include/emd.h
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.130225 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/layer/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       35 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/layer/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1019 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/layer/emd_loss_layer.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.130416 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/src/
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.130590 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1462 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       17 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/src/emd.cpp
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      574 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/setup.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      389 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/emd.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      682 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/frobenius_norm.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      453 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/losses/rmse_features.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.134152 learning3d-0.0.3/src/learning3d/models/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      473 2024-04-06 14:05:14.000000 learning3d-0.0.3/src/learning3d/models/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1205 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/classifier.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3377 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/dcp.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5298 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/deepgmr.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3057 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/dgcnn.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     2705 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/masknet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     9063 2024-03-25 01:41:24.000000 learning3d-0.0.3/src/learning3d/models/masknet2.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5346 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/pcn.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     2755 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/pcrnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5151 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/pointconv.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3238 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/pointnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5805 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/pointnetlk.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      412 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/pooling.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     2894 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/ppfnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    18499 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/prnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    11517 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/rpmnet.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1166 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/models/segmentation.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.135635 learning3d-0.0.3/src/learning3d/ops/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        0 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/ops/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1764 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/ops/data_utils.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     4154 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/ops/invmat.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     6793 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/ops/quaternion.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3957 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/ops/se3.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5228 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/ops/sinc.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     5166 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/ops/so3.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    12806 2023-06-23 11:04:02.000000 learning3d-0.0.3/src/learning3d/ops/transform_functions.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.136789 learning3d-0.0.3/src/learning3d/utils/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      286 2024-04-06 14:03:38.000000 learning3d-0.0.3/src/learning3d/utils/__init__.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    14331 2023-06-23 11:04:03.000000 learning3d-0.0.3/src/learning3d/utils/pointconv_util.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     7989 2023-06-23 11:04:03.000000 learning3d-0.0.3/src/learning3d/utils/ppfnet_util.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     1936 2023-06-23 11:04:03.000000 learning3d-0.0.3/src/learning3d/utils/svd.py
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     8974 2023-06-23 11:04:03.000000 learning3d-0.0.3/src/learning3d/utils/transformer.py
+drwxr-xr-x   0 vinitsarode   (501) staff       (20)        0 2024-04-06 14:07:05.137013 learning3d-0.0.3/src/learning3d.egg-info/
+-rw-r--r--   0 vinitsarode   (501) staff       (20)    15802 2024-04-06 14:07:05.000000 learning3d-0.0.3/src/learning3d.egg-info/PKG-INFO
+-rw-r--r--   0 vinitsarode   (501) staff       (20)     3383 2024-04-06 14:07:05.000000 learning3d-0.0.3/src/learning3d.egg-info/SOURCES.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)        1 2024-04-06 14:07:05.000000 learning3d-0.0.3/src/learning3d.egg-info/dependency_links.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)      173 2024-04-06 14:07:05.000000 learning3d-0.0.3/src/learning3d.egg-info/requires.txt
+-rw-r--r--   0 vinitsarode   (501) staff       (20)       11 2024-04-06 14:07:05.000000 learning3d-0.0.3/src/learning3d.egg-info/top_level.txt
```

### Comparing `learning3d-0.0.2/LICENSE` & `learning3d-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/PKG-INFO` & `learning3d-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learning3d
-Version: 0.0.2
+Version: 0.0.3
 Summary: Learning3D: A Modern Library for Deep Learning on 3D Point Clouds Data
 Author-email: Vinit Sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/vinits5/learning3d
 Project-URL: Issues, https://github.com/vinits5/learning3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `learning3d-0.0.2/README.md` & `learning3d-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/pyproject.toml` & `learning3d-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "learning3d"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Vinit Sarode", email="vinitsarode5@gmail.com"},
 ]
 description = "Learning3D: A Modern Library for Deep Learning on 3D Point Clouds Data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `learning3d-0.0.2/src/learning3d/data_utils/dataloaders.py` & `learning3d-0.0.3/src/learning3d/data_utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/data_utils/user_data.py` & `learning3d-0.0.3/src/learning3d/data_utils/user_data.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_dcp.py` & `learning3d-0.0.3/src/learning3d/examples/test_dcp.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_deepgmr.py` & `learning3d-0.0.3/src/learning3d/examples/test_deepgmr.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_masknet.py` & `learning3d-0.0.3/src/learning3d/examples/test_masknet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_masknet2.py` & `learning3d-0.0.3/src/learning3d/examples/test_masknet2.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_pcn.py` & `learning3d-0.0.3/src/learning3d/examples/test_pcn.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_pcrnet.py` & `learning3d-0.0.3/src/learning3d/examples/test_pcrnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_pnlk.py` & `learning3d-0.0.3/src/learning3d/examples/test_pnlk.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_pointconv.py` & `learning3d-0.0.3/src/learning3d/examples/test_pointconv.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_pointnet.py` & `learning3d-0.0.3/src/learning3d/examples/test_pointnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_prnet.py` & `learning3d-0.0.3/src/learning3d/examples/test_prnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/test_rpmnet.py` & `learning3d-0.0.3/src/learning3d/examples/test_rpmnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_PointNetLK.py` & `learning3d-0.0.3/src/learning3d/examples/train_PointNetLK.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_dcp.py` & `learning3d-0.0.3/src/learning3d/examples/train_dcp.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_deepgmr.py` & `learning3d-0.0.3/src/learning3d/examples/train_deepgmr.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_masknet.py` & `learning3d-0.0.3/src/learning3d/examples/train_masknet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_pcn.py` & `learning3d-0.0.3/src/learning3d/examples/train_pcn.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_pcrnet.py` & `learning3d-0.0.3/src/learning3d/examples/train_pcrnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_pointconv.py` & `learning3d-0.0.3/src/learning3d/examples/train_pointconv.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_pointnet.py` & `learning3d-0.0.3/src/learning3d/examples/train_pointnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_prnet.py` & `learning3d-0.0.3/src/learning3d/examples/train_prnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/examples/train_rpmnet.py` & `learning3d-0.0.3/src/learning3d/examples/train_rpmnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/chamfer_distance.py` & `learning3d-0.0.3/src/learning3d/losses/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/correspondence_loss.py` & `learning3d-0.0.3/src/learning3d/losses/correspondence_loss.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cpp` & `learning3d-0.0.3/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cpp`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cu` & `learning3d-0.0.3/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.cu`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.py` & `learning3d-0.0.3/src/learning3d/losses/cuda/chamfer_distance/chamfer_distance.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/emd_loss_layer.py` & `learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/emd_loss_layer.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/emd.cuh` & `learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/include/cuda/emd.cuh`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/include/emd.h` & `learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/include/emd.h`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/layer/emd_loss_layer.py` & `learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/layer/emd_loss_layer.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu` & `learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/cuda/emd_torch/setup.py` & `learning3d-0.0.3/src/learning3d/losses/cuda/emd_torch/setup.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/losses/frobenius_norm.py` & `learning3d-0.0.3/src/learning3d/losses/frobenius_norm.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/classifier.py` & `learning3d-0.0.3/src/learning3d/models/classifier.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/dcp.py` & `learning3d-0.0.3/src/learning3d/models/dcp.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/deepgmr.py` & `learning3d-0.0.3/src/learning3d/models/deepgmr.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/dgcnn.py` & `learning3d-0.0.3/src/learning3d/models/dgcnn.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/masknet.py` & `learning3d-0.0.3/src/learning3d/models/masknet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/masknet2.py` & `learning3d-0.0.3/src/learning3d/models/masknet2.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/pcn.py` & `learning3d-0.0.3/src/learning3d/models/pcn.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/pcrnet.py` & `learning3d-0.0.3/src/learning3d/models/pcrnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/pointconv.py` & `learning3d-0.0.3/src/learning3d/models/pointconv.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/pointnet.py` & `learning3d-0.0.3/src/learning3d/models/pointnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/pointnetlk.py` & `learning3d-0.0.3/src/learning3d/models/pointnetlk.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/ppfnet.py` & `learning3d-0.0.3/src/learning3d/models/ppfnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/prnet.py` & `learning3d-0.0.3/src/learning3d/models/prnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/rpmnet.py` & `learning3d-0.0.3/src/learning3d/models/rpmnet.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/models/segmentation.py` & `learning3d-0.0.3/src/learning3d/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/ops/data_utils.py` & `learning3d-0.0.3/src/learning3d/ops/data_utils.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/ops/invmat.py` & `learning3d-0.0.3/src/learning3d/ops/invmat.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/ops/quaternion.py` & `learning3d-0.0.3/src/learning3d/ops/quaternion.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/ops/se3.py` & `learning3d-0.0.3/src/learning3d/ops/se3.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/ops/sinc.py` & `learning3d-0.0.3/src/learning3d/ops/sinc.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/ops/so3.py` & `learning3d-0.0.3/src/learning3d/ops/so3.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/ops/transform_functions.py` & `learning3d-0.0.3/src/learning3d/ops/transform_functions.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/utils/pointconv_util.py` & `learning3d-0.0.3/src/learning3d/utils/pointconv_util.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/utils/ppfnet_util.py` & `learning3d-0.0.3/src/learning3d/utils/ppfnet_util.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/utils/svd.py` & `learning3d-0.0.3/src/learning3d/utils/svd.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d/utils/transformer.py` & `learning3d-0.0.3/src/learning3d/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `learning3d-0.0.2/src/learning3d.egg-info/PKG-INFO` & `learning3d-0.0.3/src/learning3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: learning3d
-Version: 0.0.2
+Version: 0.0.3
 Summary: Learning3D: A Modern Library for Deep Learning on 3D Point Clouds Data
 Author-email: Vinit Sarode <vinitsarode5@gmail.com>
 Project-URL: Homepage, https://github.com/vinits5/learning3d
 Project-URL: Issues, https://github.com/vinits5/learning3d/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `learning3d-0.0.2/src/learning3d.egg-info/SOURCES.txt` & `learning3d-0.0.3/src/learning3d.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -2,40 +2,37 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 data/modelnet40_ply_hdf5_2048/shape_names.txt
 data/modelnet40_ply_hdf5_2048/test_files.txt
 data/modelnet40_ply_hdf5_2048/train_files.txt
-pretrained/exp_prnet/args.txt
 src/learning3d/__init__.py
 src/learning3d.egg-info/PKG-INFO
 src/learning3d.egg-info/SOURCES.txt
 src/learning3d.egg-info/dependency_links.txt
 src/learning3d.egg-info/requires.txt
 src/learning3d.egg-info/top_level.txt
 src/learning3d/data_utils/__init__.py
 src/learning3d/data_utils/dataloaders.py
 src/learning3d/data_utils/user_data.py
 src/learning3d/examples/test_dcp.py
 src/learning3d/examples/test_deepgmr.py
-src/learning3d/examples/test_flownet.py
 src/learning3d/examples/test_masknet.py
 src/learning3d/examples/test_masknet2.py
 src/learning3d/examples/test_pcn.py
 src/learning3d/examples/test_pcrnet.py
 src/learning3d/examples/test_pnlk.py
 src/learning3d/examples/test_pointconv.py
 src/learning3d/examples/test_pointnet.py
 src/learning3d/examples/test_prnet.py
 src/learning3d/examples/test_rpmnet.py
 src/learning3d/examples/train_PointNetLK.py
 src/learning3d/examples/train_dcp.py
 src/learning3d/examples/train_deepgmr.py
-src/learning3d/examples/train_flownet.py
 src/learning3d/examples/train_masknet.py
 src/learning3d/examples/train_pcn.py
 src/learning3d/examples/train_pcrnet.py
 src/learning3d/examples/train_pointconv.py
 src/learning3d/examples/train_pointnet.py
 src/learning3d/examples/train_prnet.py
 src/learning3d/examples/train_rpmnet.py
@@ -60,15 +57,14 @@
 src/learning3d/losses/cuda/emd_torch/pkg/src/emd.cpp
 src/learning3d/losses/cuda/emd_torch/pkg/src/cuda/emd.cu
 src/learning3d/models/__init__.py
 src/learning3d/models/classifier.py
 src/learning3d/models/dcp.py
 src/learning3d/models/deepgmr.py
 src/learning3d/models/dgcnn.py
-src/learning3d/models/flownet3d.py
 src/learning3d/models/masknet.py
 src/learning3d/models/masknet2.py
 src/learning3d/models/pcn.py
 src/learning3d/models/pcrnet.py
 src/learning3d/models/pointconv.py
 src/learning3d/models/pointnet.py
 src/learning3d/models/pointnetlk.py
@@ -85,40 +81,8 @@
 src/learning3d/ops/sinc.py
 src/learning3d/ops/so3.py
 src/learning3d/ops/transform_functions.py
 src/learning3d/utils/__init__.py
 src/learning3d/utils/pointconv_util.py
 src/learning3d/utils/ppfnet_util.py
 src/learning3d/utils/svd.py
-src/learning3d/utils/transformer.py
-src/learning3d/utils/lib/pointnet2_modules.py
-src/learning3d/utils/lib/pointnet2_utils.py
-src/learning3d/utils/lib/pytorch_utils.py
-src/learning3d/utils/lib/setup.py
-src/learning3d/utils/lib/build/lib.linux-x86_64-3.5/pointnet2_cuda.cpython-35m-x86_64-linux-gnu.so
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/ball_query.o
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/ball_query_gpu.o
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/group_points.o
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/group_points_gpu.o
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/interpolate.o
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/interpolate_gpu.o
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/pointnet2_api.o
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/sampling.o
-src/learning3d/utils/lib/build/temp.linux-x86_64-3.5/src/sampling_gpu.o
-src/learning3d/utils/lib/dist/pointnet2-0.0.0-py3.5-linux-x86_64.egg
-src/learning3d/utils/lib/pointnet2.egg-info/SOURCES.txt
-src/learning3d/utils/lib/pointnet2.egg-info/dependency_links.txt
-src/learning3d/utils/lib/pointnet2.egg-info/top_level.txt
-src/learning3d/utils/lib/src/ball_query.cpp
-src/learning3d/utils/lib/src/ball_query_gpu.cu
-src/learning3d/utils/lib/src/ball_query_gpu.h
-src/learning3d/utils/lib/src/cuda_utils.h
-src/learning3d/utils/lib/src/group_points.cpp
-src/learning3d/utils/lib/src/group_points_gpu.cu
-src/learning3d/utils/lib/src/group_points_gpu.h
-src/learning3d/utils/lib/src/interpolate.cpp
-src/learning3d/utils/lib/src/interpolate_gpu.cu
-src/learning3d/utils/lib/src/interpolate_gpu.h
-src/learning3d/utils/lib/src/pointnet2_api.cpp
-src/learning3d/utils/lib/src/sampling.cpp
-src/learning3d/utils/lib/src/sampling_gpu.cu
-src/learning3d/utils/lib/src/sampling_gpu.h
+src/learning3d/utils/transformer.py
```

