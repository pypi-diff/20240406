# Comparing `tmp/fedscale-0.5.tar.gz` & `tmp/fedscale-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fedscale-0.5.tar", last modified: Mon Jul 18 20:53:34 2022, max compression
+gzip compressed data, was "dist/fedscale-1.0.tar", last modified: Sat Apr  6 00:11:33 2024, max compression
```

## Comparing `fedscale-0.5.tar` & `fedscale-1.0.tar`

### file list

```diff
@@ -1,248 +1,271 @@
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/
--rw-r--r--   0 yinweidai   (501) staff       (20)      306 2022-07-18 20:53:34.000000 fedscale-0.5/PKG-INFO
--rw-r--r--   0 yinweidai   (501) staff       (20)     4953 2022-07-18 20:36:42.000000 fedscale-0.5/README.md
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/__init__.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/core/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/__init__.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/core/aggregation/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/aggregation/__init__.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)    37538 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/aggregation/aggregator.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     3543 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/aggregation/optimizers.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/core/channels/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/channels/__init__.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     1141 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/channels/channel_context.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     3624 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/channels/job_api_pb2.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     6218 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/channels/job_api_pb2_grpc.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9728 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/client_manager.py
--rw-r--r--   0 yinweidai   (501) staff       (20)      440 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/commons.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11446 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/config_parser.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/core/execution/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/execution/__init__.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9129 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/execution/client.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     1337 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/execution/data_processor.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)    16071 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/execution/executor.py
--rw-r--r--   0 yinweidai   (501) staff       (20)      371 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/execution/optimizers.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     4795 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/execution/rlclient.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    17751 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/fllibs.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/core/internal/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/internal/__init__.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     1858 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/internal/client.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/core/logger/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/logger/__init__.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     3032 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/logger/aggragation.py
--rw-r--r--   0 yinweidai   (501) staff       (20)      730 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/logger/execution.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     1697 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/resource_manager.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/core/storage/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/core/storage/__init__.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/dataloaders/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/__init__.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     2368 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/amazon.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8201 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/decoder.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)     4670 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/divide_data.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     3472 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/dqn.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)     3729 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/femnist.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     4341 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/inaturalist.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)     8660 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/nlp.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)     3808 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/openimage.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/dataloaders/rcnn/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/rcnn/__init__.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)      314 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/rcnn/_init_paths.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     6020 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/reddit.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16404 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/sparse_image_warp.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     4878 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/spec_augment.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     5118 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/speech.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)     8695 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/stackoverflow.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     4183 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/transforms_stft.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     5080 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/transforms_wav.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)     6954 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/utils_data.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14958 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/voice_data_loader.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     2929 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/word2vec.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     2247 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/dataloaders/yelp.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/utils/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/__init__.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)    13035 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/model_test_module.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/utils/models/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/__init__.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/utils/models/cv_models/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/__init__.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12582 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/airnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11590 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/airnext.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9267 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/alexnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     6320 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/alphapose_coco.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10926 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/bagnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13346 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/bamresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13294 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/bisenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16366 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/bninception.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12957 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/cbamresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16660 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/centernet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13678 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/cgnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    18535 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/channelnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    74592 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/common.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14785 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/condensenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13009 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/contextnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16430 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/dabnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12844 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/danet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8562 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/darknet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     6728 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/darknet53.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    20340 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/darts.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    22340 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/deeplabv3.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9989 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/densenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    29502 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/densenet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    21252 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/diapreresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    20638 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/diapreresnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    24182 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/diaresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    19980 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/diaresnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    23582 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/dicenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8477 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/diracnetv2.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    19938 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/dla.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    19045 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/dpn.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    18898 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/drn.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10224 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/edanet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    37903 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/efficientnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14975 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/efficientnetedge.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    18765 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/enet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9380 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/erfnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10934 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/esnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12178 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/espcnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    17316 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/espnetv2.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15389 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/fastscnn.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9392 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/fastseresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10093 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/fbnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16419 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/fcn8sd.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     4809 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/fdmobilenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    19419 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/fishnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12677 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/fpenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16094 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/fractalnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12972 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/ghostnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    22073 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/hardnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    22444 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/hrnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12034 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/ibnbresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12706 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/ibndensenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12605 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/ibnresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10795 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/ibnresnext.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    17538 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/ibppose_coco.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12455 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/icnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9938 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/igcv3.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    17054 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/inceptionresnetv1.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9659 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/inceptionresnetv2.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    21545 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/inceptionv3.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    17935 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/inceptionv4.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15288 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/irevnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16156 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/isqrtcovresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    35455 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/jasper.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     2982 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/jasperdr.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13701 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/lednet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10640 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/lffd.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9630 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/linknet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    21250 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/lwopenpose_cmupan.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15952 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/menet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    20912 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/mixnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14295 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/mnasnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8541 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/mobilenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     7269 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/mobilenet_cub.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     3805 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/mobilenetb.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12809 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/mobilenetv2.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    19142 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/mobilenetv3.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    94881 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/model_store.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    19667 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/msdnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10281 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/msdnet_cifar10.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    38698 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/nasnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8092 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/nin_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14346 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/ntsnet_cub.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8850 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/nvpattexp.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    28161 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/octresnet.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/utils/models/cv_models/others/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/others/__init__.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8319 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/others/_espnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15402 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/others/_inceptionresnetv1_.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15819 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/others/oth_espnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9310 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/others/oth_inception_resnet_v1.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11244 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/others/oth_quartznet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9517 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/others/oth_vit.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10848 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/peleenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     5334 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/pfpcnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    18286 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/pnasnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    28421 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/polynet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    26565 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/preresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    24645 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/preresnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13979 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/prnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14875 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/proxylessnas.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     4166 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/proxylessnas_cub.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    18688 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/pspnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11118 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/pyramidnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    23887 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/pyramidnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13827 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/quartznet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    24400 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/regnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    20131 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resattnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9985 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resdropresnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    17635 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resnesta.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    25396 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    25200 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14148 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resnet_cub.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14467 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resneta.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9720 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resnetd.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14892 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resnext.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    23103 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/resnext_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15694 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/revnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10732 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/rir_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16743 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/ror_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15002 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/scnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     7112 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/segnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12484 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/selecsls.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13142 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/senet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    18506 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/sepreresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    24684 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/sepreresnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    18258 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/seresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    24057 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/seresnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14391 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/seresnet_cub.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8766 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/seresnext.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10860 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/shakedropresnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14480 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/shakeshakeresnet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    19891 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/sharesnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15801 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/shufflenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11778 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/shufflenetv2.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12487 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/shufflenetv2b.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12837 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/simplepose_coco.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12842 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/simpleposemobile_coco.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    34001 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/sinet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10944 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/sknet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11717 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/sparsenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10495 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/spnasnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11668 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/sqnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12197 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/squeezenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12271 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/squeezenext.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11524 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/superpointnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    15705 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/tresnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9445 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/unet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    13562 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/vgg.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     8409 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/visemenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     6704 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/voca.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    10298 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/vovnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11437 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/wrn.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    24953 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/wrn1bit_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11378 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/wrn_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    11597 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/xception.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    16317 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/xdensenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    12847 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/xdensenet_cifar.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     3677 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/cv_models/zfnet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    47567 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/model_provider.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/utils/models/simple/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/simple/__init__.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)    23606 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/simple/models.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/utils/models/specialized/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/specialized/__init__.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)    16113 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/specialized/inception.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     6658 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/specialized/mobilenet.py
--rw-r--r--   0 yinweidai   (501) staff       (20)    14584 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/specialized/resnet_speech.py
--rw-r--r--   0 yinweidai   (501) staff       (20)     9726 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/models/specialized/voice_model.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale/utils/optimizer/
--rw-r--r--   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/optimizer/__init__.py
--rwxr-xr-x   0 yinweidai   (501) staff       (20)     1244 2022-07-18 20:36:42.000000 fedscale-0.5/fedscale/utils/optimizer/yogi.py
-drwxr-xr-x   0 yinweidai   (501) staff       (20)        0 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale.egg-info/
--rw-r--r--   0 yinweidai   (501) staff       (20)      306 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale.egg-info/PKG-INFO
--rw-r--r--   0 yinweidai   (501) staff       (20)     9642 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale.egg-info/SOURCES.txt
--rw-r--r--   0 yinweidai   (501) staff       (20)        1 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale.egg-info/dependency_links.txt
--rw-r--r--   0 yinweidai   (501) staff       (20)        9 2022-07-18 20:53:34.000000 fedscale-0.5/fedscale.egg-info/top_level.txt
--rw-r--r--   0 yinweidai   (501) staff       (20)       79 2022-07-18 20:53:34.000000 fedscale-0.5/setup.cfg
--rw-r--r--   0 yinweidai   (501) staff       (20)      346 2022-07-18 20:36:42.000000 fedscale-0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.090557 fedscale-1.0/
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-06 00:11:33.090557 fedscale-1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5571 2024-04-06 00:03:29.000000 fedscale-1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.063557 fedscale-1.0/fedscale/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.064557 fedscale-1.0/fedscale/cloud/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.065557 fedscale-1.0/fedscale/cloud/aggregation/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/aggregation/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    39605 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/aggregation/aggregator.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/aggregation/aggregator_mnn.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/aggregation/aggregator_tflite.py
+-rwxr-xr-x   0 root         (0) root         (0)     6469 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/aggregation/async_aggregator.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/aggregation/optimizers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.065557 fedscale-1.0/fedscale/cloud/channels/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/channels/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/channels/channel_context.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/channels/job_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6224 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/channels/job_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9690 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/client_manager.py
+-rw-r--r--   0 root         (0) root         (0)      464 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/commons.py
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/config_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.066557 fedscale-1.0/fedscale/cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/execution/client_base.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/execution/data_processor.py
+-rwxr-xr-x   0 root         (0) root         (0)    16662 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/execution/executor.py
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/execution/optimizers.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/execution/rl_client.py
+-rw-r--r--   0 root         (0) root         (0)     3733 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/execution/tensorflow_client.py
+-rw-r--r--   0 root         (0) root         (0)    11266 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/execution/torch_client.py
+-rw-r--r--   0 root         (0) root         (0)    19487 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/fllibs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.067557 fedscale-1.0/fedscale/cloud/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/internal/client_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/internal/model_adapter_base.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/internal/tensorflow_model_adapter.py
+-rw-r--r--   0 root         (0) root         (0)      584 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/internal/tflite_model_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     2222 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/internal/torch_model_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.067557 fedscale-1.0/fedscale/cloud/logger/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/logger/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/logger/aggregator_logging.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/logger/dummy_logger.py
+-rw-r--r--   0 root         (0) root         (0)      741 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/logger/executor_logging.py
+-rw-r--r--   0 root         (0) root         (0)     2056 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/resource_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.067557 fedscale-1.0/fedscale/cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/cloud/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.069557 fedscale-1.0/fedscale/dataloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/amazon.py
+-rw-r--r--   0 root         (0) root         (0)     8201 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/decoder.py
+-rwxr-xr-x   0 root         (0) root         (0)     4726 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/divide_data.py
+-rw-r--r--   0 root         (0) root         (0)     3472 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/dqn.py
+-rwxr-xr-x   0 root         (0) root         (0)     3729 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/femnist.py
+-rw-r--r--   0 root         (0) root         (0)     4341 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/inaturalist.py
+-rwxr-xr-x   0 root         (0) root         (0)     8660 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/nlp.py
+-rwxr-xr-x   0 root         (0) root         (0)     3808 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/openimage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.069557 fedscale-1.0/fedscale/dataloaders/rcnn/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/rcnn/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      314 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/rcnn/_init_paths.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/reddit.py
+-rw-r--r--   0 root         (0) root         (0)    16404 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/sparse_image_warp.py
+-rw-r--r--   0 root         (0) root         (0)     4878 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/spec_augment.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/speech.py
+-rwxr-xr-x   0 root         (0) root         (0)     8700 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/stackoverflow.py
+-rw-r--r--   0 root         (0) root         (0)     4183 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/transforms_stft.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/transforms_wav.py
+-rwxr-xr-x   0 root         (0) root         (0)     6951 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/utils_data.py
+-rw-r--r--   0 root         (0) root         (0)    14958 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/voice_data_loader.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/word2vec.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/dataloaders/yelp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.070557 fedscale-1.0/fedscale/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    13270 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/model_test_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.070557 fedscale-1.0/fedscale/utils/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.088557 fedscale-1.0/fedscale/utils/models/cv_models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12582 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/airnet.py
+-rw-r--r--   0 root         (0) root         (0)    11590 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/airnext.py
+-rw-r--r--   0 root         (0) root         (0)     9267 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/alexnet.py
+-rw-r--r--   0 root         (0) root         (0)     6320 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/alphapose_coco.py
+-rw-r--r--   0 root         (0) root         (0)    10926 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/bagnet.py
+-rw-r--r--   0 root         (0) root         (0)    13346 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/bamresnet.py
+-rw-r--r--   0 root         (0) root         (0)    13294 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/bisenet.py
+-rw-r--r--   0 root         (0) root         (0)    16366 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/bninception.py
+-rw-r--r--   0 root         (0) root         (0)    12957 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/cbamresnet.py
+-rw-r--r--   0 root         (0) root         (0)    16660 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/centernet.py
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/cgnet.py
+-rw-r--r--   0 root         (0) root         (0)    18535 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/channelnet.py
+-rw-r--r--   0 root         (0) root         (0)    74592 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/common.py
+-rw-r--r--   0 root         (0) root         (0)    14785 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/condensenet.py
+-rw-r--r--   0 root         (0) root         (0)    13009 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/contextnet.py
+-rw-r--r--   0 root         (0) root         (0)    16430 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/dabnet.py
+-rw-r--r--   0 root         (0) root         (0)    12844 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/danet.py
+-rw-r--r--   0 root         (0) root         (0)     8562 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/darknet.py
+-rw-r--r--   0 root         (0) root         (0)     6728 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/darknet53.py
+-rw-r--r--   0 root         (0) root         (0)    20340 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/darts.py
+-rw-r--r--   0 root         (0) root         (0)    22340 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/deeplabv3.py
+-rw-r--r--   0 root         (0) root         (0)     9989 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/densenet.py
+-rw-r--r--   0 root         (0) root         (0)    29502 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/densenet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    21252 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/diapreresnet.py
+-rw-r--r--   0 root         (0) root         (0)    20638 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/diapreresnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    24182 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/diaresnet.py
+-rw-r--r--   0 root         (0) root         (0)    19980 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/diaresnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    23582 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/dicenet.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/diracnetv2.py
+-rw-r--r--   0 root         (0) root         (0)    19938 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/dla.py
+-rw-r--r--   0 root         (0) root         (0)    19045 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/dpn.py
+-rw-r--r--   0 root         (0) root         (0)    18898 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/drn.py
+-rw-r--r--   0 root         (0) root         (0)    10224 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/edanet.py
+-rw-r--r--   0 root         (0) root         (0)    37903 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/efficientnet.py
+-rw-r--r--   0 root         (0) root         (0)    14975 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/efficientnetedge.py
+-rw-r--r--   0 root         (0) root         (0)    18765 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/enet.py
+-rw-r--r--   0 root         (0) root         (0)     9380 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/erfnet.py
+-rw-r--r--   0 root         (0) root         (0)    10934 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/esnet.py
+-rw-r--r--   0 root         (0) root         (0)    12178 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/espcnet.py
+-rw-r--r--   0 root         (0) root         (0)    17316 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/espnetv2.py
+-rw-r--r--   0 root         (0) root         (0)    15389 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/fastscnn.py
+-rw-r--r--   0 root         (0) root         (0)     9392 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/fastseresnet.py
+-rw-r--r--   0 root         (0) root         (0)    10093 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/fbnet.py
+-rw-r--r--   0 root         (0) root         (0)    16419 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/fcn8sd.py
+-rw-r--r--   0 root         (0) root         (0)     4809 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/fdmobilenet.py
+-rw-r--r--   0 root         (0) root         (0)    19419 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/fishnet.py
+-rw-r--r--   0 root         (0) root         (0)    12677 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/fpenet.py
+-rw-r--r--   0 root         (0) root         (0)    16094 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/fractalnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    12972 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/ghostnet.py
+-rw-r--r--   0 root         (0) root         (0)    22073 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/hardnet.py
+-rw-r--r--   0 root         (0) root         (0)    22444 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/hrnet.py
+-rw-r--r--   0 root         (0) root         (0)    12034 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/ibnbresnet.py
+-rw-r--r--   0 root         (0) root         (0)    12706 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/ibndensenet.py
+-rw-r--r--   0 root         (0) root         (0)    12605 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/ibnresnet.py
+-rw-r--r--   0 root         (0) root         (0)    10795 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/ibnresnext.py
+-rw-r--r--   0 root         (0) root         (0)    17538 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/ibppose_coco.py
+-rw-r--r--   0 root         (0) root         (0)    12455 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/icnet.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/igcv3.py
+-rw-r--r--   0 root         (0) root         (0)    17054 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/inceptionresnetv1.py
+-rw-r--r--   0 root         (0) root         (0)     9659 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/inceptionresnetv2.py
+-rw-r--r--   0 root         (0) root         (0)    21545 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/inceptionv3.py
+-rw-r--r--   0 root         (0) root         (0)    17935 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/inceptionv4.py
+-rw-r--r--   0 root         (0) root         (0)    15288 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/irevnet.py
+-rw-r--r--   0 root         (0) root         (0)    16156 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/isqrtcovresnet.py
+-rw-r--r--   0 root         (0) root         (0)    35455 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/jasper.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/jasperdr.py
+-rw-r--r--   0 root         (0) root         (0)    13701 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/lednet.py
+-rw-r--r--   0 root         (0) root         (0)    10640 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/lffd.py
+-rw-r--r--   0 root         (0) root         (0)     9630 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/linknet.py
+-rw-r--r--   0 root         (0) root         (0)    21250 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/lwopenpose_cmupan.py
+-rw-r--r--   0 root         (0) root         (0)    15952 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/menet.py
+-rw-r--r--   0 root         (0) root         (0)    20912 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/mixnet.py
+-rw-r--r--   0 root         (0) root         (0)    14295 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/mnasnet.py
+-rw-r--r--   0 root         (0) root         (0)     8541 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/mobilenet.py
+-rw-r--r--   0 root         (0) root         (0)     7269 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/mobilenet_cub.py
+-rw-r--r--   0 root         (0) root         (0)     3805 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/mobilenetb.py
+-rw-r--r--   0 root         (0) root         (0)    12809 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/mobilenetv2.py
+-rw-r--r--   0 root         (0) root         (0)    19142 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/mobilenetv3.py
+-rw-r--r--   0 root         (0) root         (0)    94881 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/model_store.py
+-rw-r--r--   0 root         (0) root         (0)    19667 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/msdnet.py
+-rw-r--r--   0 root         (0) root         (0)    10281 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/msdnet_cifar10.py
+-rw-r--r--   0 root         (0) root         (0)    38698 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/nasnet.py
+-rw-r--r--   0 root         (0) root         (0)     8092 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/nin_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    14346 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/ntsnet_cub.py
+-rw-r--r--   0 root         (0) root         (0)     8850 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/nvpattexp.py
+-rw-r--r--   0 root         (0) root         (0)    28161 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/octresnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.088557 fedscale-1.0/fedscale/utils/models/cv_models/others/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8319 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/others/_espnet.py
+-rw-r--r--   0 root         (0) root         (0)    15402 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/others/_inceptionresnetv1_.py
+-rw-r--r--   0 root         (0) root         (0)    15819 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/others/oth_espnet.py
+-rw-r--r--   0 root         (0) root         (0)     9310 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/others/oth_inception_resnet_v1.py
+-rw-r--r--   0 root         (0) root         (0)    11244 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/others/oth_quartznet.py
+-rw-r--r--   0 root         (0) root         (0)     9517 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/others/oth_vit.py
+-rw-r--r--   0 root         (0) root         (0)    10848 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/peleenet.py
+-rw-r--r--   0 root         (0) root         (0)     5334 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/pfpcnet.py
+-rw-r--r--   0 root         (0) root         (0)    18286 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/pnasnet.py
+-rw-r--r--   0 root         (0) root         (0)    28421 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/polynet.py
+-rw-r--r--   0 root         (0) root         (0)    26565 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/preresnet.py
+-rw-r--r--   0 root         (0) root         (0)    24645 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/preresnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    13979 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/prnet.py
+-rw-r--r--   0 root         (0) root         (0)    14875 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/proxylessnas.py
+-rw-r--r--   0 root         (0) root         (0)     4166 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/proxylessnas_cub.py
+-rw-r--r--   0 root         (0) root         (0)    18688 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/pspnet.py
+-rw-r--r--   0 root         (0) root         (0)    11118 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/pyramidnet.py
+-rw-r--r--   0 root         (0) root         (0)    23887 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/pyramidnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    13827 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/quartznet.py
+-rw-r--r--   0 root         (0) root         (0)    24400 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/regnet.py
+-rw-r--r--   0 root         (0) root         (0)    20131 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resattnet.py
+-rw-r--r--   0 root         (0) root         (0)     9985 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resdropresnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    17635 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resnesta.py
+-rw-r--r--   0 root         (0) root         (0)    25396 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resnet.py
+-rw-r--r--   0 root         (0) root         (0)    25200 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    14148 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resnet_cub.py
+-rw-r--r--   0 root         (0) root         (0)    14467 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resneta.py
+-rw-r--r--   0 root         (0) root         (0)     9720 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resnetd.py
+-rw-r--r--   0 root         (0) root         (0)    14892 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resnext.py
+-rw-r--r--   0 root         (0) root         (0)    23103 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/resnext_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    15694 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/revnet.py
+-rw-r--r--   0 root         (0) root         (0)    10732 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/rir_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    16743 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/ror_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    15002 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/scnet.py
+-rw-r--r--   0 root         (0) root         (0)     7112 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/segnet.py
+-rw-r--r--   0 root         (0) root         (0)    12484 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/selecsls.py
+-rw-r--r--   0 root         (0) root         (0)    13142 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/senet.py
+-rw-r--r--   0 root         (0) root         (0)    18506 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/sepreresnet.py
+-rw-r--r--   0 root         (0) root         (0)    24684 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/sepreresnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    18258 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/seresnet.py
+-rw-r--r--   0 root         (0) root         (0)    24057 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/seresnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    14391 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/seresnet_cub.py
+-rw-r--r--   0 root         (0) root         (0)     8766 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/seresnext.py
+-rw-r--r--   0 root         (0) root         (0)    10860 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/shakedropresnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    14480 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/shakeshakeresnet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    19891 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/sharesnet.py
+-rw-r--r--   0 root         (0) root         (0)    15801 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/shufflenet.py
+-rw-r--r--   0 root         (0) root         (0)    11778 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/shufflenetv2.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/shufflenetv2b.py
+-rw-r--r--   0 root         (0) root         (0)    12837 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/simplepose_coco.py
+-rw-r--r--   0 root         (0) root         (0)    12842 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/simpleposemobile_coco.py
+-rw-r--r--   0 root         (0) root         (0)    34001 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/sinet.py
+-rw-r--r--   0 root         (0) root         (0)    10944 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/sknet.py
+-rw-r--r--   0 root         (0) root         (0)    11717 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/sparsenet.py
+-rw-r--r--   0 root         (0) root         (0)    10495 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/spnasnet.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/sqnet.py
+-rw-r--r--   0 root         (0) root         (0)    12197 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/squeezenet.py
+-rw-r--r--   0 root         (0) root         (0)    12271 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/squeezenext.py
+-rw-r--r--   0 root         (0) root         (0)    11524 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/superpointnet.py
+-rw-r--r--   0 root         (0) root         (0)    15705 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/tresnet.py
+-rw-r--r--   0 root         (0) root         (0)     9445 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/unet.py
+-rw-r--r--   0 root         (0) root         (0)    13562 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/vgg.py
+-rw-r--r--   0 root         (0) root         (0)     8409 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/visemenet.py
+-rw-r--r--   0 root         (0) root         (0)     6704 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/voca.py
+-rw-r--r--   0 root         (0) root         (0)    10298 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/vovnet.py
+-rw-r--r--   0 root         (0) root         (0)    11437 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/wrn.py
+-rw-r--r--   0 root         (0) root         (0)    24953 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/wrn1bit_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    11378 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/wrn_cifar.py
+-rw-r--r--   0 root         (0) root         (0)    11597 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/xception.py
+-rw-r--r--   0 root         (0) root         (0)    16317 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/xdensenet.py
+-rw-r--r--   0 root         (0) root         (0)    12847 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/xdensenet_cifar.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/cv_models/zfnet.py
+-rw-r--r--   0 root         (0) root         (0)     6673 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/mnn_model_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.089557 fedscale-1.0/fedscale/utils/models/simple/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/simple/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    23606 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/simple/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.089557 fedscale-1.0/fedscale/utils/models/specialized/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/specialized/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    16113 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/specialized/inception.py
+-rw-r--r--   0 root         (0) root         (0)     6658 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/specialized/mobilenet.py
+-rw-r--r--   0 root         (0) root         (0)    14584 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/specialized/resnet_speech.py
+-rw-r--r--   0 root         (0) root         (0)     9726 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/specialized/voice_model.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/tensorflow_model_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12908 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/tflite_model_provider.py
+-rw-r--r--   0 root         (0) root         (0)    47559 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/models/torch_model_provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.089557 fedscale-1.0/fedscale/utils/optimizer/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/optimizer/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1093 2024-04-06 00:03:29.000000 fedscale-1.0/fedscale/utils/optimizer/yogi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.064557 fedscale-1.0/fedscale.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      306 2024-04-06 00:11:33.000000 fedscale-1.0/fedscale.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10508 2024-04-06 00:11:33.000000 fedscale-1.0/fedscale.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 00:11:33.000000 fedscale-1.0/fedscale.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-04-06 00:11:33.000000 fedscale-1.0/fedscale.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-06 00:11:33.090557 fedscale-1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      347 2024-04-06 00:11:23.000000 fedscale-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.089557 fedscale-1.0/thirdparty/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 00:03:29.000000 fedscale-1.0/thirdparty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.090557 fedscale-1.0/thirdparty/oort/
+-rw-r--r--   0 root         (0) root         (0)       68 2024-04-06 00:03:29.000000 fedscale-1.0/thirdparty/oort/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18064 2024-04-06 00:03:29.000000 fedscale-1.0/thirdparty/oort/oort.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 00:11:33.090557 fedscale-1.0/thirdparty/oort/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 00:03:29.000000 fedscale-1.0/thirdparty/oort/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2024-04-06 00:03:29.000000 fedscale-1.0/thirdparty/oort/utils/lp.py
+-rw-r--r--   0 root         (0) root         (0)     3648 2024-04-06 00:03:29.000000 fedscale-1.0/thirdparty/oort/utils/lp_cplex.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2024-04-06 00:03:29.000000 fedscale-1.0/thirdparty/oort/utils/lp_gurobi.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fedscale-0.5/README.md` & `fedscale-1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <p align="center">
-<img src="./docs/imgs/FedScale-logo.png" width="340" height="63"/>
+<img src="./docs/imgs/FedScale-logo.png" width="300" height="55"/>
 </p>
 
-[![](https://img.shields.io/badge/FedScale-Homepage-orange)](https://fedscale.github.io/)
-[![](https://img.shields.io/badge/Benchmark-Submit%20Results-brightgreen)](https://fedscale.github.io/docs/leader_overview)
+[![](https://img.shields.io/badge/FedScale-Homepage-orange)](https://fedscale.ai/)
+[![](https://img.shields.io/badge/Benchmark-Submit%20Results-brightgreen)](https://fedscale.ai/docs/leader_overview)
 [![](https://img.shields.io/badge/FedScale-Join%20Slack-blue)](https://join.slack.com/t/fedscale/shared_invite/zt-uzouv5wh-ON8ONCGIzwjXwMYDC2fiKw)
 
 **FedScale is a scalable and extensible open-source federated learning (FL) engine and benchmark**. 
 
-FedScale ([fedscale.ai](https://fedscale.github.io/)) provides high-level APIs to implement FL algorithms, deploy and evaluate them at scale across diverse hardware and software backends. 
+FedScale ([fedscale.ai](https://fedscale.ai/)) provides high-level APIs to implement FL algorithms, deploy and evaluate them at scale across diverse hardware and software backends. 
 FedScale also includes the largest FL benchmark that contains FL tasks ranging from image classification and object detection to language modeling and speech recognition. 
 Moreover, it provides datasets to faithfully emulate FL training environments where FL will realistically be deployed.
 
 
 ## Getting Started
 
 ### Quick Installation (Linux)
@@ -50,44 +50,47 @@
 ### Tutorials
 
 Now that you have FedScale installed, you can start exploring FedScale following one of these introductory tutorials.
 
 1. [Explore FedScale datasets](./docs/Femnist_stats.md)
 2. [Deploy your FL experiment](./docs/tutorial.md)
 3. [Implement an FL algorithm](./examples/README.md)
-
+4. [Deploy FL on smartphones](./fedscale/edge/android/README.md)
 
 ## FedScale Datasets
 
 ***We are adding more datasets! Please contribute!***
 
-FedScale consists of 20+ large-scale, heterogeneous FL datasets covering computer vision (CV), natural language processing (NLP), and miscellaneous tasks. 
+FedScale consists of 20+ large-scale, heterogeneous FL datasets and 70+ various [models](./fedscale/utils/models/cv_models/README.md), covering computer vision (CV), natural language processing (NLP), and miscellaneous tasks. 
 Each one is associated with its training, validation, and testing datasets. 
-Please go to the `./benchmark/dataset` directory and follow the dataset [README](./benchmark/dataset/README.md) for more details.
+We acknowledge the contributors of these raw datasets. Please go to the `./benchmark/dataset` directory and follow the dataset [README](./benchmark/dataset/README.md) for more details.
 
 ## FedScale Runtime
 FedScale Runtime is an scalable and extensible deployment as well as evaluation platform to simplify and standardize FL experimental setup and model evaluation. 
 It evolved from our prior system, [Oort](https://github.com/SymbioticLab/Oort), which has been shown to scale well and can emulate FL training of thousands of clients in each round.
 
-Please go to `./fedscale/core` directory and follow the [README](./fedscale/core/README.md) to set up FL training scripts.
+Please go to `./fedscale/cloud` directory and follow the [README](./fedscale/cloud/README.md) to set up FL training scripts and the [README](./fedscale/edge/android/README.md) for practical on-device deployment.
 
 
 ## Repo Structure
 
 ```
 Repo Root
 |---- fedscale          # FedScale source code
-  |---- core            # Core of FedScale service
+  |---- cloud           # Core of FedScale service
   |---- utils           # Auxiliaries (e.g, model zoo and FL optimizer)
-  |---- deploy          # Deployment backends (e.g., mobile)
+  |---- edge            # Backends for practical deployments (e.g., mobile)
   |---- dataloaders     # Data loaders of benchmarking dataset
 
+|---- docker            # FedScale docker and container deployment (e.g., Kubernetes)
 |---- benchmark         # FedScale datasets and configs
   |---- dataset         # Benchmarking datasets
+  |---- configs         # Example configurations
 
+|---- scripts           # Scripts for installing dependencies
 |---- examples          # Examples of implementing new FL designs
 |---- docs              # FedScale tutorials and APIs
 ```
 
 ## References
 Please read and/or cite as appropriate to use FedScale code or data or learn more about FedScale.
 
@@ -110,9 +113,11 @@
   year={2021}
 }
 ```
 
 ## Contributions and Communication
 Please submit [issues](https://github.com/SymbioticLab/FedScale/issues) or [pull requests](https://github.com/SymbioticLab/FedScale/pulls) as you find bugs or improve FedScale.
 
+For each submission, please add unit tests to the corresponding changes and make sure that all unit tests pass by running `pytest fedscale/tests`.
+
 If you have any questions or comments, please join our [Slack](https://join.slack.com/t/fedscale/shared_invite/zt-uzouv5wh-ON8ONCGIzwjXwMYDC2fiKw) channel, or email us ([fedscale@googlegroups.com](mailto:fedscale@googlegroups.com)).
```

### Comparing `fedscale-0.5/fedscale/core/aggregation/aggregator.py` & `fedscale-1.0/fedscale/cloud/aggregation/aggregator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,112 +1,152 @@
 # -*- coding: utf-8 -*-
-
+import collections
+import copy
+import math
+import os
 import pickle
+import random
 import threading
+import time
 from concurrent import futures
 
 import grpc
+import numpy as np
 import torch
+import wandb
 from torch.utils.tensorboard import SummaryWriter
 
-import fedscale.core.channels.job_api_pb2_grpc as job_api_pb2_grpc
-from fedscale.core import commons
-from fedscale.core.channels import job_api_pb2
-from fedscale.core.logger.aggragation import *
-from fedscale.core.resource_manager import ResourceManager
+import fedscale.cloud.channels.job_api_pb2_grpc as job_api_pb2_grpc
+import fedscale.cloud.logger.aggregator_logging as logger
+from fedscale.cloud.aggregation.optimizers import TorchServerOptimizer
+from fedscale.cloud.channels import job_api_pb2
+from fedscale.cloud.client_manager import ClientManager
+from fedscale.cloud.internal.tensorflow_model_adapter import TensorflowModelAdapter
+from fedscale.cloud.internal.torch_model_adapter import TorchModelAdapter
+from fedscale.cloud.resource_manager import ResourceManager
+from fedscale.cloud.fllibs import *
+from torch.utils.tensorboard import SummaryWriter
 
-MAX_MESSAGE_LENGTH = 1*1024*1024*1024  # 1GB
+MAX_MESSAGE_LENGTH = 1 * 1024 * 1024 * 1024  # 1GB
 
 
 class Aggregator(job_api_pb2_grpc.JobServiceServicer):
     """This centralized aggregator collects training/testing feedbacks from executors
-    
+
     Args:
         args (dictionary): Variable arguments for fedscale runtime config. defaults to the setup in arg_parser.py
 
     """
+
     def __init__(self, args):
-        logging.info(f"Job args {args}")
+        # init aggregator loger
+        logger.initiate_aggregator_setting()
 
+        logging.info(f"Job args {args}")
         self.args = args
         self.experiment_mode = args.experiment_mode
-        self.device = args.cuda_device if args.use_cuda else torch.device(
-            'cpu')
+        self.device = args.cuda_device if args.use_cuda else torch.device("cpu")
 
         # ======== env information ========
         self.this_rank = 0
-        self.global_virtual_clock = 0.
-        self.round_duration = 0.
+        self.global_virtual_clock = 0.0
+        self.round_duration = 0.0
         self.resource_manager = ResourceManager(self.experiment_mode)
         self.client_manager = self.init_client_manager(args=args)
 
         # ======== model and data ========
-        self.model = None
+        self.model_wrapper = None
         self.model_in_update = 0
         self.update_lock = threading.Lock()
         # all weights including bias/#_batch_tracked (e.g., state_dict)
-        self.model_weights = collections.OrderedDict()
-        self.last_gradient_weights = []  # only gradient variables
-        self.model_state_dict = None
-        # NOTE: if <param_name, param_tensor> (e.g., model.parameters() in PyTorch), then False
-        # True, if <param_name, list_param_tensors> (e.g., layer.get_weights() in Tensorflow)
-        self.using_group_params = self.args.engine == commons.TENSORFLOW
+        self.model_weights = None
+        self.temp_model_path = os.path.join(
+            logger.logDir, "model_" + str(args.this_rank) + ".npy"
+        )
+        self.last_saved_round = 0
 
         # ======== channels ========
         self.connection_timeout = self.args.connection_timeout
         self.executors = None
         self.grpc_server = None
 
         # ======== Event Queue =======
-        self.individual_client_events = {}    # Unicast
-        self.sever_events_queue = collections.deque()
+        self.individual_client_events = {}  # Unicast
+        self.server_events_queue = collections.deque()
         self.broadcast_events_queue = collections.deque()  # Broadcast
 
         # ======== runtime information ========
         self.tasks_round = 0
         self.num_of_clients = 0
 
         # NOTE: sampled_participants = sampled_executors in deployment,
         # because every participant is an executor. However, in simulation mode,
         # executors is the physical machines (VMs), thus:
         # |sampled_executors| << |sampled_participants| as an VM may run multiple participants
         self.sampled_participants = []
         self.sampled_executors = []
 
         self.round_stragglers = []
-        self.model_update_size = 0.
+        self.model_update_size = 0.0
 
         self.collate_fn = None
-        self.task = args.task
         self.round = 0
 
         self.start_run_time = time.time()
         self.client_conf = {}
 
         self.stats_util_accumulator = []
         self.loss_accumulator = []
         self.client_training_results = []
 
         # number of registered executors
         self.registered_executor_info = set()
         self.test_result_accumulator = []
-        self.testing_history = {'data_set': args.data_set, 'model': args.model, 'sample_mode': args.sample_mode,
-                                'gradient_policy': args.gradient_policy, 'task': args.task, 'perf': collections.OrderedDict()}
-
-        self.log_writer = SummaryWriter(log_dir=logDir)
+        self.testing_history = {
+            "data_set": args.data_set,
+            "model": args.model,
+            "sample_mode": args.sample_mode,
+            "gradient_policy": args.gradient_policy,
+            "task": args.task,
+            "perf": collections.OrderedDict(),
+        }
+        self.log_writer = SummaryWriter(log_dir=logger.logDir)
+        if args.wandb_token != "":
+            os.environ["WANDB_API_KEY"] = args.wandb_token
+            self.wandb = wandb
+            if self.wandb.run is None:
+                self.wandb.init(
+                    project=f"fedscale-{args.job_name}",
+                    name=f"aggregator{args.this_rank}-{args.time_stamp}",
+                    group=f"{args.time_stamp}",
+                )
+                self.wandb.config.update(
+                    {
+                        "num_participants": args.num_participants,
+                        "data_set": args.data_set,
+                        "model": args.model,
+                        "gradient_policy": args.gradient_policy,
+                        "eval_interval": args.eval_interval,
+                        "rounds": args.rounds,
+                        "batch_size": args.batch_size,
+                        "use_cuda": args.use_cuda,
+                    }
+                )
+            else:
+                logging.error("Warning: wandb has already been initialized")
+            # self.wandb.run.name = f'{args.job_name}-{args.time_stamp}'
+        else:
+            self.wandb = None
 
         # ======== Task specific ============
         self.init_task_context()
 
     def setup_env(self):
-        """Set up experiments environment and server optimizer
-        """
+        """Set up experiments environment and server optimizer"""
         self.setup_seed(seed=1)
-        self.optimizer = ServerOptimizer(
-            self.args.gradient_policy, self.args, self.device)
 
     def setup_seed(self, seed=1):
         """Set global random seed for better reproducibility
 
         Args:
             seed (int): random seed
 
@@ -121,86 +161,91 @@
         """Create communication channel between coordinator and executor.
         This channel serves control messages.
         """
         logging.info(f"Initiating control plane communication ...")
         if self.experiment_mode == commons.SIMULATION_MODE:
             num_of_executors = 0
             for ip_numgpu in self.args.executor_configs.split("="):
-                ip, numgpu = ip_numgpu.split(':')
-                for numexe in numgpu.strip()[1:-1].split(','):
+                ip, numgpu = ip_numgpu.split(":")
+                for numexe in numgpu.strip()[1:-1].split(","):
                     for _ in range(int(numexe.strip())):
                         num_of_executors += 1
             self.executors = list(range(num_of_executors))
         else:
             self.executors = list(range(self.args.num_participants))
 
         # initiate a server process
         self.grpc_server = grpc.server(
             futures.ThreadPoolExecutor(max_workers=20),
             options=[
-                ('grpc.max_send_message_length', MAX_MESSAGE_LENGTH),
-                ('grpc.max_receive_message_length', MAX_MESSAGE_LENGTH),
+                ("grpc.max_send_message_length", MAX_MESSAGE_LENGTH),
+                ("grpc.max_receive_message_length", MAX_MESSAGE_LENGTH),
             ],
         )
-        job_api_pb2_grpc.add_JobServiceServicer_to_server(
-            self, self.grpc_server)
-        port = '[::]:{}'.format(self.args.ps_port)
+        job_api_pb2_grpc.add_JobServiceServicer_to_server(self, self.grpc_server)
+        port = "[::]:{}".format(self.args.ps_port)
 
-        logging.info(f'%%%%%%%%%% Opening aggregator sever using port {port} %%%%%%%%%%')
+        logging.info(
+            f"%%%%%%%%%% Opening aggregator server using port {port} %%%%%%%%%%"
+        )
 
         self.grpc_server.add_insecure_port(port)
         self.grpc_server.start()
 
     def init_data_communication(self):
-        """For jumbo traffics (e.g., training results).
-        """
+        """For jumbo traffics (e.g., training results)."""
         pass
 
     def init_model(self):
-        """Load the model architecture
-        """
-        assert self.args.engine == commons.PYTORCH, "Please define model for non-PyTorch models"
-
-        self.model = init_model()
-
-        # Initiate model parameters dictionary <param_name, param>
-        self.model_weights = self.model.state_dict()
+        """Initialize the model"""
+        if self.args.engine == commons.TENSORFLOW:
+            self.model_wrapper = TensorflowModelAdapter(init_model())
+        elif self.args.engine == commons.PYTORCH:
+            self.model_wrapper = TorchModelAdapter(
+                init_model(),
+                optimizer=TorchServerOptimizer(
+                    self.args.gradient_policy, self.args, self.device
+                ),
+            )
+        else:
+            raise ValueError(f"{self.args.engine} is not a supported engine.")
+        self.model_weights = self.model_wrapper.get_weights()
 
     def init_task_context(self):
-        """Initiate execution context for specific tasks
-        """
+        """Initiate execution context for specific tasks"""
         if self.args.task == "detection":
             cfg_from_file(self.args.cfg_file)
             np.random.seed(self.cfg.RNG_SEED)
             self.imdb, _, _, _ = combined_roidb(
-                "voc_2007_test", ['DATA_DIR', self.args.data_dir], server=True)
+                "voc_2007_test", ["DATA_DIR", self.args.data_dir], server=True
+            )
 
     def init_client_manager(self, args):
-        """ Initialize client sampler
+        """Initialize client sampler
 
         Args:
             args (dictionary): Variable arguments for fedscale runtime config. defaults to the setup in arg_parser.py
-        
+
         Returns:
-            clientManager: The client manager class
+            ClientManager: The client manager class
 
         Currently we implement two client managers:
 
-        1. Random client sampler - it selects participants randomly in each round 
+        1. Random client sampler - it selects participants randomly in each round
         [Ref]: https://arxiv.org/abs/1902.01046
 
         2. Oort sampler
         Oort prioritizes the use of those clients who have both data that offers the greatest utility
         in improving model accuracy and the capability to run training quickly.
         [Ref]: https://www.usenix.org/conference/osdi21/presentation/lai
 
         """
 
         # sample_mode: random or oort
-        client_manager = clientManager(args.sample_mode, args=args)
+        client_manager = ClientManager(args.sample_mode, args=args)
 
         return client_manager
 
     def load_client_profile(self, file_path):
         """For Simulation Mode: load client profiles/traces
 
         Args:
@@ -208,548 +253,599 @@
 
         Returns:
             dictionary: Return the client profiles/traces
 
         """
         global_client_profile = {}
         if os.path.exists(file_path):
-            with open(file_path, 'rb') as fin:
-                # {clientId: [computer, bandwidth]}
+            with open(file_path, "rb") as fin:
+                # {client_id: [computer, bandwidth]}
                 global_client_profile = pickle.load(fin)
 
         return global_client_profile
 
     def client_register_handler(self, executorId, info):
         """Triggered once receive new executor registration.
-        
+
         Args:
             executorId (int): Executor Id
             info (dictionary): Executor information
 
         """
         logging.info(f"Loading {len(info['size'])} client traces ...")
-        for _size in info['size']:
+        for _size in info["size"]:
             # since the worker rankId starts from 1, we also configure the initial dataId as 1
-            mapped_id = (self.num_of_clients+1) % len(
-                self.client_profiles) if len(self.client_profiles) > 0 else 1
+            mapped_id = (
+                (self.num_of_clients + 1) % len(self.client_profiles)
+                if len(self.client_profiles) > 0
+                else 1
+            )
             systemProfile = self.client_profiles.get(
-                mapped_id, {'computation': 1.0, 'communication': 1.0})
+                mapped_id, {"computation": 1.0, "communication": 1.0}
+            )
 
-            clientId = (
-                self.num_of_clients+1) if self.experiment_mode == commons.SIMULATION_MODE else executorId
+            client_id = (
+                (self.num_of_clients + 1)
+                if self.experiment_mode == commons.SIMULATION_MODE
+                else executorId
+            )
             self.client_manager.register_client(
-                executorId, clientId, size=_size, speed=systemProfile)
-            self.client_manager.registerDuration(clientId, batch_size=self.args.batch_size,
-                                                 upload_step=self.args.local_steps, upload_size=self.model_update_size, download_size=self.model_update_size)
+                executorId, client_id, size=_size, speed=systemProfile
+            )
+            self.client_manager.registerDuration(
+                client_id,
+                batch_size=self.args.batch_size,
+                local_steps=self.args.local_steps,
+                upload_size=self.model_update_size,
+                download_size=self.model_update_size,
+            )
             self.num_of_clients += 1
 
-        logging.info("Info of all feasible clients {}".format(
-            self.client_manager.getDataInfo()))
+        logging.info(
+            "Info of all feasible clients {}".format(self.client_manager.getDataInfo())
+        )
 
     def executor_info_handler(self, executorId, info):
         """Handler for register executor info and it will start the round after number of
         executor reaches requirement.
-        
+
         Args:
             executorId (int): Executor Id
             info (dictionary): Executor information
 
         """
         self.registered_executor_info.add(executorId)
-        logging.info(f"Received executor {executorId} information, {len(self.registered_executor_info)}/{len(self.executors)}")
+        logging.info(
+            f"Received executor {executorId} information, {len(self.registered_executor_info)}/{len(self.executors)}"
+        )
 
         # In this simulation, we run data split on each worker, so collecting info from one executor is enough
         # Waiting for data information from executors, or timeout
         if self.experiment_mode == commons.SIMULATION_MODE:
-
             if len(self.registered_executor_info) == len(self.executors):
                 self.client_register_handler(executorId, info)
                 # start to sample clients
                 self.round_completion_handler()
         else:
             # In real deployments, we need to register for each client
             self.client_register_handler(executorId, info)
             if len(self.registered_executor_info) == len(self.executors):
                 self.round_completion_handler()
 
     def tictak_client_tasks(self, sampled_clients, num_clients_to_collect):
         """Record sampled client execution information in last round. In the SIMULATION_MODE,
         further filter the sampled_client and pick the top num_clients_to_collect clients.
-        
+
         Args:
             sampled_clients (list of int): Sampled clients from client manager
             num_clients_to_collect (int): The number of clients actually needed for next round.
 
         Returns:
-            tuple: Return the sampled clients and client execution information in the last round.
+            Tuple: (the List of clients to run, the List of stragglers in the round, a Dict of the virtual clock of each
+            client, the duration of the aggregation round, and the durations of each client's task).
 
         """
         if self.experiment_mode == commons.SIMULATION_MODE:
             # NOTE: We try to remove dummy events as much as possible in simulations,
             # by removing the stragglers/offline clients in overcommitment"""
             sampledClientsReal = []
             completionTimes = []
             completed_client_clock = {}
             # 1. remove dummy clients that are not available to the end of training
             for client_to_run in sampled_clients:
                 client_cfg = self.client_conf.get(client_to_run, self.args)
 
-                exe_cost = self.client_manager.getCompletionTime(client_to_run,
-                                                                 batch_size=client_cfg.batch_size, upload_step=client_cfg.local_steps,
-                                                                 upload_size=self.model_update_size, download_size=self.model_update_size)
+                exe_cost = self.client_manager.get_completion_time(
+                    client_to_run,
+                    batch_size=client_cfg.batch_size,
+                    local_steps=client_cfg.local_steps,
+                    upload_size=self.model_update_size,
+                    download_size=self.model_update_size,
+                )
 
-                roundDuration = exe_cost['computation'] + \
-                    exe_cost['communication']
+                roundDuration = exe_cost["computation"] + exe_cost["communication"]
                 # if the client is not active by the time of collection, we consider it is lost in this round
-                if self.client_manager.isClientActive(client_to_run, roundDuration + self.global_virtual_clock):
+                if self.client_manager.isClientActive(
+                    client_to_run, roundDuration + self.global_virtual_clock
+                ):
                     sampledClientsReal.append(client_to_run)
                     completionTimes.append(roundDuration)
                     completed_client_clock[client_to_run] = exe_cost
 
-            num_clients_to_collect = min(
-                num_clients_to_collect, len(completionTimes))
+            num_clients_to_collect = min(num_clients_to_collect, len(completionTimes))
             # 2. get the top-k completions to remove stragglers
-            sortedWorkersByCompletion = sorted(
-                range(len(completionTimes)), key=lambda k: completionTimes[k])
-            top_k_index = sortedWorkersByCompletion[:num_clients_to_collect]
+            workers_sorted_by_completion_time = sorted(
+                range(len(completionTimes)), key=lambda k: completionTimes[k]
+            )
+            top_k_index = workers_sorted_by_completion_time[:num_clients_to_collect]
             clients_to_run = [sampledClientsReal[k] for k in top_k_index]
 
-            dummy_clients = [sampledClientsReal[k]
-                             for k in sortedWorkersByCompletion[num_clients_to_collect:]]
+            stragglers = [
+                sampledClientsReal[k]
+                for k in workers_sorted_by_completion_time[num_clients_to_collect:]
+            ]
             round_duration = completionTimes[top_k_index[-1]]
             completionTimes.sort()
 
-            return (clients_to_run, dummy_clients,
-                    completed_client_clock, round_duration,
-                    completionTimes[:num_clients_to_collect])
+            return (
+                clients_to_run,
+                stragglers,
+                completed_client_clock,
+                round_duration,
+                completionTimes[:num_clients_to_collect],
+            )
         else:
             completed_client_clock = {
-                client: {'computation': 1, 'communication': 1} for client in sampled_clients}
+                client: {"computation": 1, "communication": 1}
+                for client in sampled_clients
+            }
             completionTimes = [1 for c in sampled_clients]
-            return (sampled_clients, sampled_clients, completed_client_clock,
-                    1, completionTimes)
+            return (
+                sampled_clients,
+                sampled_clients,
+                completed_client_clock,
+                1,
+                completionTimes,
+            )
 
     def run(self):
-        """Start running the aggregator server by setting up execution 
+        """Start running the aggregator server by setting up execution
         and communication environment, and monitoring the grpc message.
         """
         self.setup_env()
+        self.client_profiles = self.load_client_profile(
+            file_path=self.args.device_conf_file
+        )
+
         self.init_control_communication()
         self.init_data_communication()
 
         self.init_model()
-        self.save_last_param()
-        self.model_update_size = sys.getsizeof(
-            pickle.dumps(self.model))/1024.0*8.  # kbits
-        self.client_profiles = self.load_client_profile(
-            file_path=self.args.device_conf_file)
+        self.model_update_size = (
+            sys.getsizeof(pickle.dumps(self.model_wrapper)) / 1024.0 * 8.0
+        )  # kbits
 
         self.event_monitor()
+        self.stop()
+
+    def _is_first_result_in_round(self):
+        return self.model_in_update == 1
+
+    def _is_last_result_in_round(self):
+        return self.model_in_update == self.tasks_round
 
     def select_participants(self, select_num_participants, overcommitment=1.3):
         """Select clients for next round.
 
-        Args: 
+        Args:
             select_num_participants (int): Number of clients to select.
             overcommitment (float): Overcommit ration for next round.
 
         Returns:
             list of int: The list of sampled clients id.
 
         """
-        return sorted(self.client_manager.select_participants(
-            int(select_num_participants*overcommitment),
-            cur_time=self.global_virtual_clock),
+        return sorted(
+            self.client_manager.select_participants(
+                int(select_num_participants * overcommitment),
+                cur_time=self.global_virtual_clock,
+            ),
         )
 
     def client_completion_handler(self, results):
-        """We may need to keep all updates from clients, 
+        """We may need to keep all updates from clients,
         if so, we need to append results to the cache
-        
+
         Args:
             results (dictionary): client's training result
-        
+
         """
         # Format:
-        #       -results = {'clientId':clientId, 'update_weight': model_param, 'moving_loss': round_train_loss,
+        #       -results = {'client_id':client_id, 'update_weight': model_param, 'moving_loss': round_train_loss,
         #       'trained_size': count, 'wall_duration': time_cost, 'success': is_success 'utility': utility}
 
-        if self.args.gradient_policy in ['q-fedavg']:
+        if self.args.gradient_policy in ["q-fedavg"]:
             self.client_training_results.append(results)
         # Feed metrics to client sampler
-        self.stats_util_accumulator.append(results['utility'])
-        self.loss_accumulator.append(results['moving_loss'])
+        self.stats_util_accumulator.append(results["utility"])
+        self.loss_accumulator.append(results["moving_loss"])
 
-        self.client_manager.register_feedback(results['clientId'], results['utility'],
-                                          auxi=math.sqrt(
-                                              results['moving_loss']),
-                                          time_stamp=self.round,
-                                          duration=self.virtual_client_clock[results['clientId']]['computation'] +
-                                          self.virtual_client_clock[results['clientId']
-                                                                    ]['communication']
-                                          )
+        self.client_manager.register_feedback(
+            results["client_id"],
+            results["utility"],
+            auxi=math.sqrt(results["moving_loss"]),
+            time_stamp=self.round,
+            duration=self.virtual_client_clock[results["client_id"]]["computation"]
+            + self.virtual_client_clock[results["client_id"]]["communication"],
+        )
 
         # ================== Aggregate weights ======================
         self.update_lock.acquire()
 
         self.model_in_update += 1
-        if self.using_group_params == True:
-            self.aggregate_client_group_weights(results)
-        else:
-            self.aggregate_client_weights(results)
+        self.update_weight_aggregation(results)
 
         self.update_lock.release()
 
-    def aggregate_client_weights(self, results):
-        """May aggregate client updates on the fly
-        
-        Args:
-            results (dictionary): client's training result
-        
-        [FedAvg] "Communication-Efficient Learning of Deep Networks from Decentralized Data".
-        H. Brendan McMahan, Eider Moore, Daniel Ramage, Seth Hampson, Blaise Aguera y Arcas. AISTATS, 2017
-        """
-        # Start to take the average of updates, and we do not keep updates to save memory
-        # Importance of each update is 1/#_of_participants
-        # importance = 1./self.tasks_round
-
-        for p in results['update_weight']:
-            param_weight = results['update_weight'][p]
-            if isinstance(param_weight, list):
-                param_weight = np.asarray(param_weight, dtype=np.float32)
-            param_weight = torch.from_numpy(
-                param_weight).to(device=self.device)
-
-            if self.model_in_update == 1:
-                self.model_weights[p].data = param_weight
-            else:
-                self.model_weights[p].data += param_weight
-
-        if self.model_in_update == self.tasks_round:
-            for p in self.model_weights:
-                d_type = self.model_weights[p].data.dtype
-
-                self.model_weights[p].data = (
-                    self.model_weights[p]/float(self.tasks_round)).to(dtype=d_type)
-
-    def aggregate_client_group_weights(self, results):
-        """Streaming weight aggregation. Similar to aggregate_client_weights, 
-        but each key corresponds to a group of weights (e.g., for Tensorflow)
-        
-        Args:
-            results (dictionary): Client's training result
-        
-        """
-        for p_g in results['update_weight']:
-            param_weights = results['update_weight'][p_g]
-            for idx, param_weight in enumerate(param_weights):
-                if isinstance(param_weight, list):
-                    param_weight = np.asarray(param_weight, dtype=np.float32)
-                param_weight = torch.from_numpy(
-                    param_weight).to(device=self.device)
-
-                if self.model_in_update == 1:
-                    self.model_weights[p_g][idx].data = param_weight
-                else:
-                    self.model_weights[p_g][idx].data += param_weight
+    def update_weight_aggregation(self, results):
+        """Updates the aggregation with the new results.
 
-        if self.model_in_update == self.tasks_round:
-            for p in self.model_weights:
-                for idx in range(len(self.model_weights[p])):
-                    d_type = self.model_weights[p][idx].data.dtype
-
-                    self.model_weights[p][idx].data = (
-                        self.model_weights[p][idx].data/float(self.tasks_round)
-                    ).to(dtype=d_type)
-
-    def save_last_param(self):
-        """ Save the last model parameters
+        :param results: the results collected from the client.
         """
-        if self.args.engine == commons.TENSORFLOW:
-            self.last_gradient_weights = [
-                layer.get_weights() for layer in self.model.layers]
+        update_weights = results["update_weight"]
+        if type(update_weights) is dict:
+            update_weights = [x for x in update_weights.values()]
+        if self._is_first_result_in_round():
+            self.model_weights = update_weights
         else:
-            self.last_gradient_weights = [
-                p.data.clone() for p in self.model.parameters()]
+            self.model_weights = [
+                weight + update_weights[i]
+                for i, weight in enumerate(self.model_weights)
+            ]
+        if self._is_last_result_in_round():
+            self.model_weights = [
+                np.divide(weight, self.tasks_round) for weight in self.model_weights
+            ]
+            self.model_wrapper.set_weights(
+                copy.deepcopy(self.model_weights),
+                client_training_results=self.client_training_results,
+            )
 
-    def round_weight_handler(self, last_model):
-        """Update model when the round completes
-        
-        Args:
-            last_model (list): A list of global model weight in last round.
-        
-        """
-        if self.round > 1:
-            if self.args.engine == commons.TENSORFLOW:
-                for layer in self.model.layers:
-                    layer.set_weights([p.cpu().detach().numpy()
-                                      for p in self.model_weights[layer.name]])
+    def aggregate_test_result(self):
+        accumulator = self.test_result_accumulator[0]
+        for i in range(1, len(self.test_result_accumulator)):
+            if self.args.task == "detection":
+                for key in accumulator:
+                    if key == "boxes":
+                        for j in range(596):
+                            accumulator[key][j] = (
+                                accumulator[key][j]
+                                + self.test_result_accumulator[i][key][j]
+                            )
+                    else:
+                        accumulator[key] += self.test_result_accumulator[i][key]
             else:
-                self.model.load_state_dict(self.model_weights)
-                current_grad_weights = [param.data.clone()
-                                        for param in self.model.parameters()]
-                self.optimizer.update_round_gradient(
-                    last_model, current_grad_weights, self.model)
+                for key in accumulator:
+                    accumulator[key] += self.test_result_accumulator[i][key]
+        self.testing_history["perf"][self.round] = {
+            "round": self.round,
+            "clock": self.global_virtual_clock,
+        }
+        for metric_name in accumulator.keys():
+            if metric_name == "test_loss":
+                self.testing_history["perf"][self.round]["loss"] = (
+                    accumulator["test_loss"]
+                    if self.args.task == "detection"
+                    else accumulator["test_loss"] / accumulator["test_len"]
+                )
+            elif metric_name not in ["test_len"]:
+                self.testing_history["perf"][self.round][metric_name] = (
+                    accumulator[metric_name] / accumulator["test_len"]
+                )
+
+        round_perf = self.testing_history["perf"][self.round]
+        logging.info(
+            "FL Testing in round: {}, virtual_clock: {}, results: {}".format(
+                self.round, self.global_virtual_clock, round_perf
+            )
+        )
+
+    def update_default_task_config(self):
+        """Update the default task configuration after each round"""
+        if self.round % self.args.decay_round == 0:
+            self.args.learning_rate = max(
+                self.args.learning_rate * self.args.decay_factor,
+                self.args.min_learning_rate,
+            )
 
     def round_completion_handler(self):
         """Triggered upon the round completion, it registers the last round execution info,
         broadcast new tasks for executors and select clients for next round.
         """
         self.global_virtual_clock += self.round_duration
         self.round += 1
-
-        if self.round % self.args.decay_round == 0:
-            self.args.learning_rate = max(
-                self.args.learning_rate*self.args.decay_factor, self.args.min_learning_rate)
-
-        # handle the global update w/ current and last
-        self.round_weight_handler(self.last_gradient_weights)
-
-        avgUtilLastround = sum(self.stats_util_accumulator) / \
-            max(1, len(self.stats_util_accumulator))
+        last_round_avg_util = sum(self.stats_util_accumulator) / max(
+            1, len(self.stats_util_accumulator)
+        )
         # assign avg reward to explored, but not ran workers
-        for clientId in self.round_stragglers:
-            self.client_manager.register_feedback(clientId, avgUtilLastround,
-                                              time_stamp=self.round,
-                                              duration=self.virtual_client_clock[clientId]['computation'] +
-                                              self.virtual_client_clock[clientId]['communication'],
-                                              success=False)
-
-        avg_loss = sum(self.loss_accumulator) / \
-            max(1, len(self.loss_accumulator))
-        logging.info(f"Wall clock: {round(self.global_virtual_clock)} s, round: {self.round}, Planned participants: " +
-                     f"{len(self.sampled_participants)}, Succeed participants: {len(self.stats_util_accumulator)}, Training loss: {avg_loss}")
+        for client_id in self.round_stragglers:
+            self.client_manager.register_feedback(
+                client_id,
+                last_round_avg_util,
+                time_stamp=self.round,
+                duration=self.virtual_client_clock[client_id]["computation"]
+                + self.virtual_client_clock[client_id]["communication"],
+                success=False,
+            )
+
+        avg_loss = sum(self.loss_accumulator) / max(1, len(self.loss_accumulator))
+        logging.info(
+            f"Wall clock: {round(self.global_virtual_clock)} s, round: {self.round}, Planned participants: "
+            + f"{len(self.sampled_participants)}, Succeed participants: {len(self.stats_util_accumulator)}, Training loss: {avg_loss}"
+        )
 
         # dump round completion information to tensorboard
         if len(self.loss_accumulator):
             self.log_train_result(avg_loss)
 
         # update select participants
         self.sampled_participants = self.select_participants(
-            select_num_participants=self.args.num_participants, overcommitment=self.args.overcommitment)
-        (clientsToRun, round_stragglers, virtual_client_clock, round_duration, flatten_client_duration) = self.tictak_client_tasks(
-            self.sampled_participants, self.args.num_participants)
+            select_num_participants=self.args.num_participants,
+            overcommitment=self.args.overcommitment,
+        )
+        (
+            clients_to_run,
+            round_stragglers,
+            virtual_client_clock,
+            round_duration,
+            flatten_client_duration,
+        ) = self.tictak_client_tasks(
+            self.sampled_participants, self.args.num_participants
+        )
 
-        logging.info(f"Selected participants to run: {clientsToRun}")
+        logging.info(f"Selected participants to run: {clients_to_run}")
 
         # Issue requests to the resource manager; Tasks ordered by the completion time
-        self.resource_manager.register_tasks(clientsToRun)
-        self.tasks_round = len(clientsToRun)
+        self.resource_manager.register_tasks(clients_to_run)
+        self.tasks_round = len(clients_to_run)
 
         # Update executors and participants
         if self.experiment_mode == commons.SIMULATION_MODE:
-            self.sampled_executors = list(
-                self.individual_client_events.keys())
+            self.sampled_executors = list(self.individual_client_events.keys())
         else:
-            self.sampled_executors = [str(c_id)
-                                      for c_id in self.sampled_participants]
-
-        self.save_last_param()
+            self.sampled_executors = [str(c_id) for c_id in self.sampled_participants]
         self.round_stragglers = round_stragglers
         self.virtual_client_clock = virtual_client_clock
-        self.flatten_client_duration = numpy.array(flatten_client_duration)
+        self.flatten_client_duration = np.array(flatten_client_duration)
         self.round_duration = round_duration
         self.model_in_update = 0
         self.test_result_accumulator = []
         self.stats_util_accumulator = []
         self.client_training_results = []
+        self.loss_accumulator = []
+        self.update_default_task_config()
 
         if self.round >= self.args.rounds:
             self.broadcast_aggregator_events(commons.SHUT_DOWN)
-        elif self.round % self.args.eval_interval == 0:
+        elif self.round % self.args.eval_interval == 0 or self.round == 1:
             self.broadcast_aggregator_events(commons.UPDATE_MODEL)
             self.broadcast_aggregator_events(commons.MODEL_TEST)
         else:
             self.broadcast_aggregator_events(commons.UPDATE_MODEL)
             self.broadcast_aggregator_events(commons.START_ROUND)
 
     def log_train_result(self, avg_loss):
-        """Log training result on TensorBoard
-        """
-        self.log_writer.add_scalar('Train/round_to_loss', avg_loss, self.round)
+        """Log training result on TensorBoard and optionally WanDB"""
+        self.log_writer.add_scalar("Train/round_to_loss", avg_loss, self.round)
         self.log_writer.add_scalar(
-            'FAR/time_to_train_loss (min)', avg_loss, self.global_virtual_clock/60.)
+            "Train/time_to_train_loss (min)", avg_loss, self.global_virtual_clock / 60.0
+        )
         self.log_writer.add_scalar(
-            'FAR/round_duration (min)', self.round_duration/60., self.round)
+            "Train/round_duration (min)", self.round_duration / 60.0, self.round
+        )
         self.log_writer.add_histogram(
-            'FAR/client_duration (min)', self.flatten_client_duration, self.round)
+            "Train/client_duration (min)", self.flatten_client_duration, self.round
+        )
+
+        if self.wandb != None:
+            self.wandb.log(
+                {
+                    "Train/round_to_loss": avg_loss,
+                    "Train/round_duration (min)": self.round_duration / 60.0,
+                    "Train/client_duration (min)": self.flatten_client_duration,
+                    "Train/time_to_round (min)": self.global_virtual_clock / 60.0,
+                },
+                step=self.round,
+            )
 
     def log_test_result(self):
-        """Log testing result on TensorBoard
-        """
+        """Log testing result on TensorBoard and optionally WanDB"""
         self.log_writer.add_scalar(
-            'Test/round_to_loss', self.testing_history['perf'][self.round]['loss'], self.round)
+            "Test/round_to_loss",
+            self.testing_history["perf"][self.round]["loss"],
+            self.round,
+        )
         self.log_writer.add_scalar(
-            'Test/round_to_accuracy', self.testing_history['perf'][self.round]['top_1'], self.round)
-        self.log_writer.add_scalar('FAR/time_to_test_loss (min)', self.testing_history['perf'][self.round]['loss'],
-                                   self.global_virtual_clock/60.)
-        self.log_writer.add_scalar('FAR/time_to_test_accuracy (min)', self.testing_history['perf'][self.round]['top_1'],
-                                   self.global_virtual_clock/60.)
+            "Test/round_to_accuracy",
+            self.testing_history["perf"][self.round]["top_1"],
+            self.round,
+        )
+        self.log_writer.add_scalar(
+            "Test/time_to_test_loss (min)",
+            self.testing_history["perf"][self.round]["loss"],
+            self.global_virtual_clock / 60.0,
+        )
+        self.log_writer.add_scalar(
+            "Test/time_to_test_accuracy (min)",
+            self.testing_history["perf"][self.round]["top_1"],
+            self.global_virtual_clock / 60.0,
+        )
+
+    def save_model(self):
+        """Save model to the wandb server if enabled"""
+        if parser.args.save_checkpoint and self.last_saved_round < self.round:
+            self.last_saved_round = self.round
+            np.save(self.temp_model_path, self.model_weights)
+            if self.wandb != None:
+                artifact = self.wandb.Artifact(
+                    name="model_" + str(self.this_rank), type="model"
+                )
+                artifact.add_file(local_path=self.temp_model_path)
+                self.wandb.log_artifact(artifact)
 
     def deserialize_response(self, responses):
         """Deserialize the response from executor
-        
+
         Args:
             responses (byte stream): Serialized response from executor.
 
         Returns:
             string, bool, or bytes: The deserialized response object from executor.
         """
         return pickle.loads(responses)
 
     def serialize_response(self, responses):
-        """ Serialize the response to send to server upon assigned job completion
+        """Serialize the response to send to server upon assigned job completion
 
         Args:
             responses (ServerResponse): Serialized response from server.
 
         Returns:
             bytes: The serialized response object to server.
 
         """
         return pickle.dumps(responses)
 
     def testing_completion_handler(self, client_id, results):
         """Each executor will handle a subset of testing dataset
-        
+
         Args:
             client_id (int): The client id.
             results (dictionary): The client test results.
 
         """
 
-        results = results['results']
+        results = results["results"]
 
         # List append is thread-safe
         self.test_result_accumulator.append(results)
 
         # Have collected all testing results
 
         if len(self.test_result_accumulator) == len(self.executors):
-            
-            aggregate_test_result(
-                self.test_result_accumulator, self.args.task, \
-                self.round, self.global_virtual_clock, self.testing_history)
+            self.aggregate_test_result()
             # Dump the testing result
-            with open(os.path.join(logDir, 'testing_perf'), 'wb') as fout:
+            with open(os.path.join(logger.logDir, "testing_perf"), "wb") as fout:
                 pickle.dump(self.testing_history, fout)
 
+            self.save_model()
+
             if len(self.loss_accumulator):
+                logging.info("logging test result")
                 self.log_test_result()
 
             self.broadcast_events_queue.append(commons.START_ROUND)
 
     def broadcast_aggregator_events(self, event):
         """Issue tasks (events) to aggregator worker processes by adding grpc request event
         (e.g. MODEL_TEST, MODEL_TRAIN) to event_queue.
 
         Args:
             event (string): grpc event (e.g. MODEL_TEST, MODEL_TRAIN) to event_queue.
-        
+
         """
         self.broadcast_events_queue.append(event)
 
     def dispatch_client_events(self, event, clients=None):
         """Issue tasks (events) to clients
-        
+
         Args:
             event (string): grpc event (e.g. MODEL_TEST, MODEL_TRAIN) to event_queue.
             clients (list of int): target client ids for event.
-        
+
         """
         if clients is None:
             clients = self.sampled_executors
 
         for client_id in clients:
             self.individual_client_events[client_id].append(event)
 
-    def get_client_conf(self, clientId):
+    def get_client_conf(self, client_id):
         """Training configurations that will be applied on clients,
         developers can further define personalized client config here.
 
         Args:
-            clientId (int): The client id.
+            client_id (int): The client id.
 
         Returns:
-            dictionary: Client training config.
+            dictionary: TorchClient training config.
 
         """
         conf = {
-            'learning_rate': self.args.learning_rate,
-            'model': None  # none indicates we are using the global model
+            "learning_rate": self.args.learning_rate,
         }
         return conf
 
-    def create_client_task(self, executorId):
+    def create_client_task(self, executor_id):
         """Issue a new client training task to specific executor
-        
+
         Args:
             executorId (int): Executor Id.
-        
+
         Returns:
             tuple: Training config for new task. (dictionary, PyTorch or TensorFlow module)
 
         """
-        next_clientId = self.resource_manager.get_next_task(executorId)
+        next_client_id = self.resource_manager.get_next_task(executor_id)
         train_config = None
         # NOTE: model = None then the executor will load the global model broadcasted in UPDATE_MODEL
-        model = None
-        if next_clientId != None:
-            config = self.get_client_conf(next_clientId)
-            train_config = {'client_id': next_clientId, 'task_config': config}
-        return train_config, model
+        if next_client_id is not None:
+            config = self.get_client_conf(next_client_id)
+            train_config = {"client_id": next_client_id, "task_config": config}
+        return train_config, self.model_wrapper.get_weights()
 
     def get_test_config(self, client_id):
         """FL model testing on clients, developers can further define personalized client config here.
-        
+
         Args:
             client_id (int): The client id.
-        
-        Returns:
-            dictionary: The testing config for new task.
-        
-        """
-        return {'client_id': client_id}
-
-    def get_global_model(self):
-        """Get global model that would be used by all FL clients (in default FL)
 
         Returns:
-            PyTorch or TensorFlow module: Based on the executor's machine learning framework, initialize and return the model for training.
+            dictionary: The testing config for new task.
 
         """
-        return self.model
+        return {"client_id": client_id}, self.model_wrapper.get_weights()
 
     def get_shutdown_config(self, client_id):
         """Shutdown config for client, developers can further define personalized client config here.
 
         Args:
-            client_id (int): Client id.
-        
+            client_id (int): TorchClient id.
+
         Returns:
             dictionary: Shutdown config for new task.
 
         """
-        return {'client_id': client_id}
+        return {"client_id": client_id}
 
     def add_event_handler(self, client_id, event, meta, data):
-        """ Due to the large volume of requests, we will put all events into a queue first.
+        """Due to the large volume of requests, we will put all events into a queue first.
 
         Args:
             client_id (int): The client id.
             event (string): grpc event MODEL_TEST or UPLOAD_MODEL.
             meta (dictionary or string): Meta message for grpc communication, could be event.
             data (dictionary): Data transferred in grpc communication, could be model parameters, test result.
 
         """
-        self.sever_events_queue.append((client_id, event, meta, data))
+        self.server_events_queue.append((client_id, event, meta, data))
 
     def CLIENT_REGISTER(self, request, context):
-        """FL Client register to the aggregator
-        
+        """FL TorchClient register to the aggregator
+
         Args:
             request (RegisterRequest): Registeration request info from executor.
 
         Returns:
             ServerResponse: Server response to registeration request
 
         """
@@ -764,20 +860,21 @@
         else:
             logging.info(f"Previous client: {executor_id} resumes connecting")
 
         # We can customize whether to admit the clients here
         self.executor_info_handler(executor_id, executor_info)
         dummy_data = self.serialize_response(commons.DUMMY_RESPONSE)
 
-        return job_api_pb2.ServerResponse(event=commons.DUMMY_EVENT,
-                                          meta=dummy_data, data=dummy_data)
+        return job_api_pb2.ServerResponse(
+            event=commons.DUMMY_EVENT, meta=dummy_data, data=dummy_data
+        )
 
     def CLIENT_PING(self, request, context):
         """Handle client ping requests
-        
+
         Args:
             request (PingRequest): Ping request info from executor.
 
         Returns:
             ServerResponse: Server response to ping request
 
         """
@@ -787,75 +884,90 @@
         response_data = response_msg = commons.DUMMY_RESPONSE
 
         if len(self.individual_client_events[executor_id]) == 0:
             # send dummy response
             current_event = commons.DUMMY_EVENT
             response_data = response_msg = commons.DUMMY_RESPONSE
         else:
-            current_event = self.individual_client_events[executor_id].popleft(
-            )
+            current_event = self.individual_client_events[executor_id].popleft()
             if current_event == commons.CLIENT_TRAIN:
-                response_msg, response_data = self.create_client_task(
-                    client_id)
+                response_msg, response_data = self.create_client_task(executor_id)
                 if response_msg is None:
                     current_event = commons.DUMMY_EVENT
                     if self.experiment_mode != commons.SIMULATION_MODE:
-                        self.individual_client_events[executor_id].appendleft(
-                            commons.CLIENT_TRAIN)
+                        self.individual_client_events[executor_id].append(
+                            commons.CLIENT_TRAIN
+                        )
             elif current_event == commons.MODEL_TEST:
-                response_msg = self.get_test_config(client_id)
+                response_msg, response_data = self.get_test_config(client_id)
             elif current_event == commons.UPDATE_MODEL:
-                response_data = self.get_global_model()
+                response_data = self.model_wrapper.get_weights()
             elif current_event == commons.SHUT_DOWN:
                 response_msg = self.get_shutdown_config(executor_id)
 
-        if current_event != commons.DUMMY_EVENT:
-            logging.info(f"Issue EVENT ({current_event}) to EXECUTOR ({executor_id})")
         response_msg, response_data = self.serialize_response(
-            response_msg), self.serialize_response(response_data)
+            response_msg
+        ), self.serialize_response(response_data)
         # NOTE: in simulation mode, response data is pickle for faster (de)serialization
-        return job_api_pb2.ServerResponse(event=current_event,
-                                          meta=response_msg, data=response_data)
+        response = job_api_pb2.ServerResponse(
+            event=current_event, meta=response_msg, data=response_data
+        )
+        if current_event != commons.DUMMY_EVENT:
+            logging.info(f"Issue EVENT ({current_event}) to EXECUTOR ({executor_id})")
+
+        return response
 
     def CLIENT_EXECUTE_COMPLETION(self, request, context):
         """FL clients complete the execution task.
-        
+
         Args:
             request (CompleteRequest): Complete request info from executor.
 
         Returns:
             ServerResponse: Server response to job completion request
 
         """
 
-        executor_id, client_id, event = request.executor_id, request.client_id, request.event
+        executor_id, client_id, event = (
+            request.executor_id,
+            request.client_id,
+            request.event,
+        )
         execution_status, execution_msg = request.status, request.msg
         meta_result, data_result = request.meta_result, request.data_result
 
         if event == commons.CLIENT_TRAIN:
             # Training results may be uploaded in CLIENT_EXECUTE_RESULT request later,
             # so we need to specify whether to ask client to do so (in case of straggler/timeout in real FL).
             if execution_status is False:
-                logging.error(f"Executor {executor_id} fails to run client {client_id}, due to {execution_msg}")
+                logging.error(
+                    f"Executor {executor_id} fails to run client {client_id}, due to {execution_msg}"
+                )
+
+            # TODO: whether we should schedule tasks when client_ping or client_complete
             if self.resource_manager.has_next_task(executor_id):
                 # NOTE: we do not pop the train immediately in simulation mode,
                 # since the executor may run multiple clients
-                self.individual_client_events[executor_id].appendleft(
-                    commons.CLIENT_TRAIN)
+                if (
+                    commons.CLIENT_TRAIN
+                    not in self.individual_client_events[executor_id]
+                ):
+                    self.individual_client_events[executor_id].append(
+                        commons.CLIENT_TRAIN
+                    )
 
         elif event in (commons.MODEL_TEST, commons.UPLOAD_MODEL):
-            self.add_event_handler(
-                executor_id, event, meta_result, data_result)
+            self.add_event_handler(executor_id, event, meta_result, data_result)
         else:
             logging.error(f"Received undefined event {event} from client {client_id}")
+
         return self.CLIENT_PING(request, context)
 
     def event_monitor(self):
-        """Activate event handler according to the received new message
-        """
+        """Activate event handler according to the received new message"""
         logging.info("Start monitoring events ...")
 
         while True:
             # Broadcast events to clients
             if len(self.broadcast_events_queue) > 0:
                 current_event = self.broadcast_events_queue.popleft()
 
@@ -866,37 +978,43 @@
                     self.dispatch_client_events(commons.CLIENT_TRAIN)
 
                 elif current_event == commons.SHUT_DOWN:
                     self.dispatch_client_events(commons.SHUT_DOWN)
                     break
 
             # Handle events queued on the aggregator
-            elif len(self.sever_events_queue) > 0:
-                client_id, current_event, meta, data = self.sever_events_queue.popleft()
+            elif len(self.server_events_queue) > 0:
+                (
+                    client_id,
+                    current_event,
+                    meta,
+                    data,
+                ) = self.server_events_queue.popleft()
 
                 if current_event == commons.UPLOAD_MODEL:
-                    self.client_completion_handler(
-                        self.deserialize_response(data))
+                    self.client_completion_handler(self.deserialize_response(data))
                     if len(self.stats_util_accumulator) == self.tasks_round:
                         self.round_completion_handler()
 
                 elif current_event == commons.MODEL_TEST:
                     self.testing_completion_handler(
-                        client_id, self.deserialize_response(data))
+                        client_id, self.deserialize_response(data)
+                    )
 
                 else:
                     logging.error(f"Event {current_event} is not defined")
 
             else:
                 # execute every 100 ms
                 time.sleep(0.1)
 
     def stop(self):
-        """Stop the aggregator
-        """
+        """Stop the aggregator"""
         logging.info(f"Terminating the aggregator ...")
+        if self.wandb != None:
+            self.wandb.finish()
         time.sleep(5)
 
 
 if __name__ == "__main__":
-    aggregator = Aggregator(args)
+    aggregator = Aggregator(parser.args)
     aggregator.run()
```

### Comparing `fedscale-0.5/fedscale/core/aggregation/optimizers.py` & `fedscale-1.0/fedscale/cloud/aggregation/optimizers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,78 +1,108 @@
-class ServerOptimizer(object):
+import numpy as np
+import torch
+
+
+class TorchServerOptimizer(object):
     """This is a abstract server optimizer class
-    
+
     Args:
         mode (string): mode of gradient aggregation policy
         args (distionary): Variable arguments for fedscale runtime config. defaults to the setup in arg_parser.py
         device (string): Runtime device type
         sample_seed (int): Random seed
 
     """
-    def __init__(self, mode, args, device, sample_seed=233):
 
+    def __init__(self, mode, args, device, sample_seed=233):
         self.mode = mode
         self.args = args
         self.device = device
 
-        if mode == 'fed-yogi':
+        if mode == "fed-yogi":
             from fedscale.utils.optimizer.yogi import YoGi
+
             self.gradient_controller = YoGi(
-                eta=args.yogi_eta, tau=args.yogi_tau, beta=args.yogi_beta, beta2=args.yogi_beta2)
+                eta=args.yogi_eta,
+                tau=args.yogi_tau,
+                beta=args.yogi_beta,
+                beta2=args.yogi_beta2,
+            )
+
+    def update_round_gradient(
+        self, last_model, current_model, target_model, client_training_results=None
+    ):
+        """update global model based on different policy
 
-    def update_round_gradient(self, last_model, current_model, target_model):
-        """ update global model based on different policy
-        
         Args:
             last_model (list of tensor weight): A list of global model weight in last round.
             current_model (list of tensor weight): A list of global model weight in this round.
             target_model (PyTorch or TensorFlow nn module): Aggregated model.
-        
+            client_training_results list of gradients from every clients, for q-fedavg
+
         """
-        if self.mode == 'fed-yogi':
+        if self.mode == "fed-yogi":
             """
-            "Adaptive Federated Optimizations", 
+            "Adaptive Federated Optimizations",
             Sashank J. Reddi, Zachary Charles, Manzil Zaheer, Zachary Garrett, Keith Rush, Jakub Konecný, Sanjiv Kumar, H. Brendan McMahan,
             ICLR 2021.
             """
             last_model = [x.to(device=self.device) for x in last_model]
             current_model = [x.to(device=self.device) for x in current_model]
 
             diff_weight = self.gradient_controller.update(
-                [pb-pa for pa, pb in zip(last_model, current_model)])
+                [pb - pa for pa, pb in zip(last_model, current_model)]
+            )
+
+            new_state_dict = {
+                name: torch.from_numpy(
+                    np.array(last_model[idx] + diff_weight[idx], dtype=np.float32)
+                )
+                for idx, name in enumerate(target_model.state_dict().keys())
+            }
 
-            for idx, param in enumerate(target_model.parameters()):
-                param.data = last_model[idx] + diff_weight[idx]
+            target_model.load_state_dict(new_state_dict)
 
-        elif self.mode == 'q-fedavg':
+        elif self.mode == "q-fedavg":
             """
             "Fair Resource Allocation in Federated Learning", Tian Li, Maziar Sanjabi, Ahmad Beirami, Virginia Smith, ICLR 2020.
             """
             learning_rate, qfedq = self.args.learning_rate, self.args.qfed_q
-            Deltas, hs = None, 0.
+            Deltas, hs = None, 0.0
             last_model = [x.to(device=self.device) for x in last_model]
 
-            for result in self.client_training_results:
+            for result in client_training_results:
                 # plug in the weight updates into the gradient
-                grads = [(u - torch.from_numpy(v).to(device=self.device)) * 1.0 /
-                         learning_rate for u, v in zip(last_model, result['update_weight'])]
-                loss = result['moving_loss']
+                update_weights = result["update_weight"]
+                if type(update_weights) is dict:
+                    update_weights = [x for x in update_weights.values()]
+
+                weights = [
+                    torch.tensor(x).to(device=self.device) for x in update_weights
+                ]
+                grads = [
+                    (u - v) * 1.0 / learning_rate for u, v in zip(last_model, weights)
+                ]
+                loss = result["moving_loss"]
 
                 if Deltas is None:
-                    Deltas = [np.float_power(
-                        loss+1e-10, qfedq) * grad for grad in grads]
+                    Deltas = [
+                        np.float_power(loss + 1e-10, qfedq) * grad for grad in grads
+                    ]
                 else:
                     for idx in range(len(Deltas)):
-                        Deltas[idx] += np.float_power(loss +
-                                                      1e-10, qfedq) * grads[idx]
+                        Deltas[idx] += np.float_power(loss + 1e-10, qfedq) * grads[idx]
 
                 # estimation of the local Lipchitz constant
-                hs += (qfedq * np.float_power(loss+1e-10, (qfedq-1)) * torch.sum(torch.stack([torch.square(
-                    grad).sum() for grad in grads])) + (1.0/learning_rate) * np.float_power(loss+1e-10, qfedq))
+                hs += qfedq * np.float_power(loss + 1e-10, (qfedq - 1)) * torch.sum(
+                    torch.stack([torch.square(grad).sum() for grad in grads])
+                ) + (1.0 / learning_rate) * np.float_power(loss + 1e-10, qfedq)
 
             # update global model
-            for idx, param in enumerate(target_model.parameters()):
-                param.data = last_model[idx] - Deltas[idx]/(hs+1e-10)
+            new_state_dict = {
+                name: last_model[idx] - Deltas[idx] / (hs + 1e-10) for idx, name in enumerate(target_model.state_dict().keys())
+            }
+            target_model.load_state_dict(new_state_dict)
 
         else:
             # The default optimizer, FedAvg, has been applied in aggregator.py on the fly
             pass
```

### Comparing `fedscale-0.5/fedscale/core/channels/channel_context.py` & `fedscale-1.0/fedscale/cloud/channels/channel_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 
 import grpc
 
-import fedscale.core.channels.job_api_pb2_grpc as job_api_pb2_grpc
+import fedscale.cloud.channels.job_api_pb2_grpc as job_api_pb2_grpc
 
 MAX_MESSAGE_LENGTH = 1*1024*1024*1024  # 1GB
 
 
 class ClientConnections(object):
     """"Clients build connections to the cloud aggregator."""
```

### Comparing `fedscale-0.5/fedscale/core/channels/job_api_pb2.py` & `fedscale-1.0/fedscale/cloud/channels/job_api_pb2.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/core/channels/job_api_pb2_grpc.py` & `fedscale-1.0/fedscale/cloud/channels/job_api_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
-"""Client and server classes corresponding to protobuf-defined services."""
+"""TorchClient and server classes corresponding to protobuf-defined services."""
 import grpc
 
-import fedscale.core.channels.job_api_pb2 as job__api__pb2
+import fedscale.cloud.channels.job_api_pb2 as job__api__pb2
 
 
 class JobServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `fedscale-0.5/fedscale/core/client_manager.py` & `fedscale-1.0/fedscale/cloud/client_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,257 +1,250 @@
 import logging
 import math
 import pickle
 from random import Random
 from typing import Dict, List
 
-from fedscale.core.internal.client import Client
+from fedscale.cloud.internal.client_metadata import ClientMetadata
 
 
-class clientManager(object):
+class ClientManager:
 
     def __init__(self, mode, args, sample_seed=233):
-        self.Clients = {}
-        self.clientOnHosts = {}
+        self.client_metadata = {}
+        self.client_on_hosts = {}
         self.mode = mode
         self.filter_less = args.filter_less
         self.filter_more = args.filter_more
 
-        self.ucbSampler = None
+        self.ucb_sampler = None
 
         if self.mode == 'oort':
-            import os
-            import sys
-            current = os.path.dirname(os.path.realpath(__file__))
-            parent = os.path.dirname(current)
-            sys.path.append(parent)
             from thirdparty.oort.oort import create_training_selector
+            self.ucb_sampler = create_training_selector(args=args)
 
-            # sys.path.append(current)
-            self.ucbSampler = create_training_selector(args=args)
         self.feasibleClients = []
         self.rng = Random()
         self.rng.seed(sample_seed)
         self.count = 0
         self.feasible_samples = 0
         self.user_trace = None
         self.args = args
 
         if args.device_avail_file is not None:
             with open(args.device_avail_file, 'rb') as fin:
                 self.user_trace = pickle.load(fin)
             self.user_trace_keys = list(self.user_trace.keys())
 
-    def registerClient(self, hostId, clientId, size, speed, duration=1):
-        self.register_client(hostId, clientId, size, speed, duration)
-
-    def register_client(self, hostId: int, clientId: int, size: int, speed: Dict[str, float], duration: float=1) -> None:
+    def register_client(self, host_id: int, client_id: int, size: int, speed: Dict[str, float],
+                        duration: float = 1) -> None:
         """Register client information to the client manager.
 
-        Args: 
-            hostId (int): executor Id.
-            clientId (int): client Id.
+        Args:
+            host_id (int): executor Id.
+            client_id (int): client Id.
             size (int): number of samples on this client.
             speed (Dict[str, float]): device speed (e.g., compuutation and communication).
             duration (float): execution latency.
 
         """
-        uniqueId = self.getUniqueId(hostId, clientId)
+        uniqueId = self.getUniqueId(host_id, client_id)
         user_trace = None if self.user_trace is None else self.user_trace[self.user_trace_keys[int(
-            clientId) % len(self.user_trace)]]
+            client_id) % len(self.user_trace)]]
 
-        self.Clients[uniqueId] = Client(hostId, clientId, speed, user_trace)
+        self.client_metadata[uniqueId] = ClientMetadata(host_id, client_id, speed, user_trace)
 
         # remove clients
         if size >= self.filter_less and size <= self.filter_more:
-            self.feasibleClients.append(clientId)
+            self.feasibleClients.append(client_id)
             self.feasible_samples += size
 
             if self.mode == "oort":
-                feedbacks = {'reward': min(size, self.args.local_steps*self.args.batch_size),
+                feedbacks = {'reward': min(size, self.args.local_steps * self.args.batch_size),
                              'duration': duration,
                              }
-                self.ucbSampler.register_client(clientId, feedbacks=feedbacks)
+                self.ucb_sampler.register_client(client_id, feedbacks=feedbacks)
         else:
-            del self.Clients[uniqueId]
-            
+            del self.client_metadata[uniqueId]
+
     def getAllClients(self):
         return self.feasibleClients
 
     def getAllClientsLength(self):
         return len(self.feasibleClients)
 
-    def getClient(self, clientId):
-        return self.Clients[self.getUniqueId(0, clientId)]
+    def getClient(self, client_id):
+        return self.client_metadata[self.getUniqueId(0, client_id)]
 
-    def registerDuration(self, clientId, batch_size, upload_step, upload_size, download_size):
-        if self.mode == "oort" and self.getUniqueId(0, clientId) in self.Clients:
-            exe_cost = self.Clients[self.getUniqueId(0, clientId)].getCompletionTime(
-                batch_size=batch_size, upload_step=upload_step,
+    def registerDuration(self, client_id, batch_size, local_steps, upload_size, download_size):
+        if self.mode == "oort" and self.getUniqueId(0, client_id) in self.client_metadata:
+            exe_cost = self.client_metadata[self.getUniqueId(0, client_id)].get_completion_time(
+                batch_size=batch_size, local_steps=local_steps,
                 upload_size=upload_size, download_size=download_size
             )
-            self.ucbSampler.update_duration(
-                clientId, exe_cost['computation']+exe_cost['communication'])
+            self.ucb_sampler.update_duration(
+                client_id, exe_cost['computation'] + exe_cost['communication'])
 
-    def getCompletionTime(self, clientId, batch_size, upload_step, upload_size, download_size):
-        return self.Clients[self.getUniqueId(0, clientId)].getCompletionTime(
-            batch_size=batch_size, upload_step=upload_step,
+    def get_completion_time(self, client_id, batch_size, local_steps, upload_size, download_size):
+        return self.client_metadata[self.getUniqueId(0, client_id)].get_completion_time(
+            batch_size=batch_size, local_steps=local_steps,
             upload_size=upload_size, download_size=download_size
         )
 
-    def registerSpeed(self, hostId, clientId, speed):
-        uniqueId = self.getUniqueId(hostId, clientId)
-        self.Clients[uniqueId].speed = speed
+    def registerSpeed(self, host_id, client_id, speed):
+        uniqueId = self.getUniqueId(host_id, client_id)
+        self.client_metadata[uniqueId].speed = speed
 
-    def registerScore(self, clientId, reward, auxi=1.0, time_stamp=0, duration=1., success=True):
-        self.register_feedback(clientId, reward, auxi=auxi, time_stamp=time_stamp, duration=duration, success=success)
+    def registerScore(self, client_id, reward, auxi=1.0, time_stamp=0, duration=1., success=True):
+        self.register_feedback(client_id, reward, auxi=auxi, time_stamp=time_stamp, duration=duration, success=success)
 
-    def register_feedback(self, clientId: int, reward: float, auxi: float=1.0, time_stamp: float=0, duration: float=1., success: bool=True) -> None:
+    def register_feedback(self, client_id: int, reward: float, auxi: float = 1.0, time_stamp: float = 0,
+                          duration: float = 1., success: bool = True) -> None:
         """Collect client execution feedbacks of last round.
 
-        Args: 
-            clientId (int): client Id.
+        Args:
+            client_id (int): client Id.
             reward (float): execution utilities (processed feedbacks).
             auxi (float): unprocessed feedbacks.
             time_stamp (float): current wall clock time.
             duration (float): system execution duration.
-            success (bool): whether this client runs successfully. 
+            success (bool): whether this client runs successfully.
 
         """
         # currently, we only use distance as reward
         if self.mode == "oort":
             feedbacks = {
                 'reward': reward,
                 'duration': duration,
                 'status': True,
                 'time_stamp': time_stamp
             }
 
-            self.ucbSampler.update_client_util(clientId, feedbacks=feedbacks)
+            self.ucb_sampler.update_client_util(client_id, feedbacks=feedbacks)
 
-    def registerClientScore(self, clientId, reward):
-        self.Clients[self.getUniqueId(0, clientId)].registerReward(reward)
+    def registerClientScore(self, client_id, reward):
+        self.client_metadata[self.getUniqueId(0, client_id)].register_reward(reward)
 
-    def getScore(self, hostId, clientId):
-        uniqueId = self.getUniqueId(hostId, clientId)
-        return self.Clients[uniqueId].getScore()
+    def get_score(self, host_id, client_id):
+        uniqueId = self.getUniqueId(host_id, client_id)
+        return self.client_metadata[uniqueId].get_score()
 
     def getClientsInfo(self):
         clientInfo = {}
-        for i, clientId in enumerate(self.Clients.keys()):
-            client = self.Clients[clientId]
-            clientInfo[client.clientId] = client.distance
+        for i, client_id in enumerate(self.client_metadata.keys()):
+            client = self.client_metadata[client_id]
+            clientInfo[client.client_id] = client.distance
         return clientInfo
 
-    def nextClientIdToRun(self, hostId):
-        init_id = hostId - 1
+    def next_client_id_to_run(self, host_id):
+        init_id = host_id - 1
         lenPossible = len(self.feasibleClients)
 
         while True:
-            clientId = str(self.feasibleClients[init_id])
-            csize = self.Clients[clientId].size
+            client_id = str(self.feasibleClients[init_id])
+            csize = self.client_metadata[client_id].size
             if csize >= self.filter_less and csize <= self.filter_more:
-                return int(clientId)
+                return int(client_id)
 
             init_id = max(
                 0, min(int(math.floor(self.rng.random() * lenPossible)), lenPossible - 1))
 
-    def getUniqueId(self, hostId, clientId):
-        return str(clientId)
-        # return (str(hostId) + '_' + str(clientId))
+    def getUniqueId(self, host_id, client_id):
+        return str(client_id)
+        # return (str(host_id) + '_' + str(client_id))
 
-    def clientSampler(self, clientId):
-        return self.Clients[self.getUniqueId(0, clientId)].size
+    def clientSampler(self, client_id):
+        return self.client_metadata[self.getUniqueId(0, client_id)].size
 
-    def clientOnHost(self, clientIds, hostId):
-        self.clientOnHosts[hostId] = clientIds
+    def clientOnHost(self, client_ids, host_id):
+        self.client_on_hosts[host_id] = client_ids
 
-    def getCurrentClientIds(self, hostId):
-        return self.clientOnHosts[hostId]
+    def getCurrentclient_ids(self, host_id):
+        return self.client_on_hosts[host_id]
 
-    def getClientLenOnHost(self, hostId):
-        return len(self.clientOnHosts[hostId])
+    def getClientLenOnHost(self, host_id):
+        return len(self.client_on_hosts[host_id])
 
-    def getClientSize(self, clientId):
-        return self.Clients[self.getUniqueId(0, clientId)].size
+    def getClientSize(self, client_id):
+        return self.client_metadata[self.getUniqueId(0, client_id)].size
 
-    def getSampleRatio(self, clientId, hostId, even=False):
+    def getSampleRatio(self, client_id, host_id, even=False):
         totalSampleInTraining = 0.
 
         if not even:
-            for key in self.clientOnHosts.keys():
-                for client in self.clientOnHosts[key]:
+            for key in self.client_on_hosts.keys():
+                for client in self.client_on_hosts[key]:
                     uniqueId = self.getUniqueId(key, client)
-                    totalSampleInTraining += self.Clients[uniqueId].size
+                    totalSampleInTraining += self.client_metadata[uniqueId].size
 
-            # 1./len(self.clientOnHosts.keys())
-            return float(self.Clients[self.getUniqueId(hostId, clientId)].size)/float(totalSampleInTraining)
+            # 1./len(self.client_on_hosts.keys())
+            return float(self.client_metadata[self.getUniqueId(host_id, client_id)].size) / float(totalSampleInTraining)
         else:
-            for key in self.clientOnHosts.keys():
-                totalSampleInTraining += len(self.clientOnHosts[key])
+            for key in self.client_on_hosts.keys():
+                totalSampleInTraining += len(self.client_on_hosts[key])
 
-            return 1./totalSampleInTraining
+            return 1. / totalSampleInTraining
 
     def getFeasibleClients(self, cur_time):
         if self.user_trace is None:
             clients_online = self.feasibleClients
         else:
-            clients_online = [clientId for clientId in self.feasibleClients if self.Clients[self.getUniqueId(
-                0, clientId)].isActive(cur_time)]
+            clients_online = [client_id for client_id in self.feasibleClients if self.client_metadata[self.getUniqueId(
+                0, client_id)].is_active(cur_time)]
 
         logging.info(f"Wall clock time: {round(cur_time)}, {len(clients_online)} clients online, " +
-                     f"{len(self.feasibleClients)-len(clients_online)} clients offline")
+                     f"{len(self.feasibleClients) - len(clients_online)} clients offline")
 
         return clients_online
 
-    def isClientActive(self, clientId, cur_time):
-        return self.Clients[self.getUniqueId(0, clientId)].isActive(cur_time)
+    def isClientActive(self, client_id, cur_time):
+        return self.client_metadata[self.getUniqueId(0, client_id)].is_active(cur_time)
 
-    def select_participants(self, num_of_clients: int, cur_time: float=0) -> List[int]:
+    def select_participants(self, num_of_clients: int, cur_time: float = 0) -> List[int]:
         """Select participating clients for current execution task.
 
-        Args: 
+        Args:
             num_of_clients (int): number of participants to select.
-            cur_time (float): current wall clock time. 
+            cur_time (float): current wall clock time.
 
         Returns:
             List[int]: indices of selected clients.
-    
+
         """
         self.count += 1
 
         clients_online = self.getFeasibleClients(cur_time)
 
         if len(clients_online) <= num_of_clients:
             return clients_online
 
         pickled_clients = None
         clients_online_set = set(clients_online)
 
         if self.mode == "oort" and self.count > 1:
-            pickled_clients = self.ucbSampler.select_participant(
+            pickled_clients = self.ucb_sampler.select_participant(
                 num_of_clients, feasible_clients=clients_online_set)
         else:
             self.rng.shuffle(clients_online)
             client_len = min(num_of_clients, len(clients_online) - 1)
             pickled_clients = clients_online[:client_len]
 
         return pickled_clients
 
-    def resampleClients(self, numOfClients, cur_time=0):
-        return self.select_participants(numOfClients, cur_time)
+    def resampleClients(self, num_of_clients, cur_time=0):
+        return self.select_participants(num_of_clients, cur_time)
 
     def getAllMetrics(self):
         if self.mode == "oort":
-            return self.ucbSampler.getAllMetrics()
+            return self.ucb_sampler.getAllMetrics()
         return {}
 
     def getDataInfo(self):
         return {'total_feasible_clients': len(self.feasibleClients), 'total_num_samples': self.feasible_samples}
 
-    def getClientReward(self, clientId):
-        return self.ucbSampler.get_client_reward(clientId)
+    def getClientReward(self, client_id):
+        return self.ucb_sampler.get_client_reward(client_id)
 
     def get_median_reward(self):
         if self.mode == 'oort':
-            return self.ucbSampler.get_median_reward()
+            return self.ucb_sampler.get_median_reward()
         return 0.
```

### Comparing `fedscale-0.5/fedscale/core/config_parser.py` & `fedscale-1.0/fedscale/cloud/config_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,238 +1,317 @@
 import argparse
 
-from fedscale.core import commons
+from fedscale.cloud import commons
 
 parser = argparse.ArgumentParser()
-parser.add_argument('--job_name', type=str, default='demo_job')
-parser.add_argument('--log_path', type=str, default='./',
-                    help="default path is ../log")
+parser.add_argument("--job_name", type=str, default="demo_job")
+parser.add_argument("--log_path", type=str, default="./", help="default path is ../log")
+parser.add_argument(
+    "--wandb_token", type=str, default="", help="API key for wandb as login credentials"
+)
 
 # The basic configuration of the cluster
-parser.add_argument('--ps_ip', type=str, default='127.0.0.1')
-parser.add_argument('--ps_port', type=str, default='29501')
-parser.add_argument('--this_rank', type=int, default=1)
-parser.add_argument('--connection_timeout', type=int, default=60)
-parser.add_argument('--experiment_mode', type=str,
-                    default=commons.SIMULATION_MODE)
-parser.add_argument('--engine', type=str, default=commons.PYTORCH,
-                    help="Tensorflow or Pytorch for cloud aggregation")
-parser.add_argument('--num_executors', type=int, default=1)
-parser.add_argument('--executor_configs', type=str,
-                    default="127.0.0.1:[1]")  # seperated by ;
-parser.add_argument('--num_participants', type=int, default=4)
-parser.add_argument('--data_map_file', type=str, default=None)
-parser.add_argument('--use_cuda', type=str, default='True')
-parser.add_argument('--cuda_device', type=str, default=None)
-parser.add_argument('--time_stamp', type=str, default='logs')
-parser.add_argument('--task', type=str, default='cv')
-parser.add_argument('--device_avail_file', type=str, default=None)
-parser.add_argument('--clock_factor', type=float, default=1.0,
-                    help="Refactor the clock time given the profile")
+parser.add_argument("--ps_ip", type=str, default="127.0.0.1")
+parser.add_argument("--ps_port", type=str, default="29500")
+parser.add_argument("--this_rank", type=int, default=1)
+parser.add_argument("--connection_timeout", type=int, default=60)
+parser.add_argument("--experiment_mode", type=str, default=commons.SIMULATION_MODE)
+parser.add_argument(
+    "--engine",
+    type=str,
+    default=commons.PYTORCH,
+    help="Tensorflow or Pytorch for cloud aggregation",
+)
+parser.add_argument("--num_executors", type=int, default=1)
+parser.add_argument(
+    "--executor_configs", type=str, default="127.0.0.1:[1]"
+)  # seperated by ;
+# Note: In async mode, the num_participants param is treated as the async buffer size. In sync, this is the number
+# of clients that are selected each round.
+parser.add_argument("--num_participants", type=int, default=4)
+parser.add_argument("--data_map_file", type=str, default=None)
+parser.add_argument("--use_cuda", type=str, default="True")
+parser.add_argument("--cuda_device", type=str, default=None)
+parser.add_argument("--time_stamp", type=str, default="logs")
+parser.add_argument("--task", type=str, default="cv")
+parser.add_argument("--device_avail_file", type=str, default=None)
+parser.add_argument(
+    "--clock_factor",
+    type=float,
+    default=1.0,
+    help="Refactor the clock time given the profile",
+)
 
 # The configuration of model and dataset
-parser.add_argument('--model_zoo', type=str, default='torchcv',
-                    help="model zoo to load the models from", choices=["torchcv", "fedscale-zoo"])
-parser.add_argument('--data_dir', type=str, default='~/cifar10/')
-parser.add_argument('--device_conf_file', type=str, default='/tmp/client.cfg')
-parser.add_argument('--model', type=str, default='shufflenet_v2_x2_0')
-parser.add_argument('--data_set', type=str, default='cifar10')
-parser.add_argument('--sample_mode', type=str, default='random')
-parser.add_argument('--filter_less', type=int, default=32)
-parser.add_argument('--filter_more', type=int, default=1e15)
-parser.add_argument('--train_uniform', type=bool, default=False)
-parser.add_argument('--conf_path', type=str, default='~/dataset/')
-parser.add_argument('--overcommitment', type=float, default=1.3)
-parser.add_argument('--model_size', type=float, default=65536)
-parser.add_argument('--round_threshold', type=float, default=30)
-parser.add_argument('--round_penalty', type=float, default=2.0)
-parser.add_argument('--clip_bound', type=float, default=0.9)
-parser.add_argument('--blacklist_rounds', type=int, default=-1)
-parser.add_argument('--blacklist_max_len', type=float, default=0.3)
-parser.add_argument('--embedding_file', type=str,
-                    default='glove.840B.300d.txt')
+parser.add_argument(
+    "--model_zoo",
+    type=str,
+    default="torchcv",
+    help="model zoo to load the models from",
+    choices=["torchcv", "fedscale-torch-zoo", "fedscale-tensorflow-zoo"],
+)
+parser.add_argument("--data_dir", type=str, default="~/cifar10/")
+parser.add_argument("--device_conf_file", type=str, default="/tmp/client.cfg")
+parser.add_argument("--model", type=str, default="shufflenet_v2_x2_0")
+parser.add_argument("--data_set", type=str, default="cifar10")
+parser.add_argument("--sample_mode", type=str, default="random")
+parser.add_argument("--filter_less", type=int, default=32)
+parser.add_argument("--filter_more", type=int, default=1e15)
+parser.add_argument("--train_uniform", type=bool, default=False)
+parser.add_argument("--conf_path", type=str, default="~/dataset/")
+parser.add_argument("--overcommitment", type=float, default=1.3)
+parser.add_argument("--model_size", type=float, default=65536)
+parser.add_argument("--round_threshold", type=float, default=30)
+parser.add_argument("--round_penalty", type=float, default=2.0)
+parser.add_argument("--clip_bound", type=float, default=0.9)
+parser.add_argument("--blacklist_rounds", type=int, default=-1)
+parser.add_argument("--blacklist_max_len", type=float, default=0.3)
+parser.add_argument("--embedding_file", type=str, default="glove.840B.300d.txt")
+parser.add_argument("--input_shape", type=int, nargs="+", default=[1, 3, 28, 28])
+parser.add_argument("--save_checkpoint", type=bool, default=False)
 
 
 # The configuration of different hyper-parameters for training
-parser.add_argument('--rounds', type=int, default=50)
-parser.add_argument('--local_steps', type=int, default=20)
-parser.add_argument('--batch_size', type=int, default=30)
-parser.add_argument('--test_bsz', type=int, default=128)
-parser.add_argument('--backend', type=str, default="gloo")
-parser.add_argument('--upload_step', type=int, default=20)
-parser.add_argument('--learning_rate', type=float, default=5e-2)
-parser.add_argument('--min_learning_rate', type=float, default=5e-5)
-parser.add_argument('--input_dim', type=int, default=0)
-parser.add_argument('--output_dim', type=int, default=0)
-parser.add_argument('--dump_epoch', type=int, default=1e10)
-parser.add_argument('--decay_factor', type=float, default=0.98)
-parser.add_argument('--decay_round', type=float, default=10)
-parser.add_argument('--num_loaders', type=int, default=2)
-parser.add_argument('--eval_interval', type=int, default=5)
-parser.add_argument('--sample_seed', type=int, default=233)  # 123 #233
-parser.add_argument('--test_ratio', type=float, default=1.0)
-parser.add_argument('--loss_decay', type=float, default=0.2)
-parser.add_argument('--exploration_min', type=float, default=0.3)
-parser.add_argument('--cut_off_util', type=float,
-                    default=0.05)  # 95 percentile
+parser.add_argument("--rounds", type=int, default=50)
+parser.add_argument("--local_steps", type=int, default=20)
+parser.add_argument("--batch_size", type=int, default=30)
+parser.add_argument("--test_bsz", type=int, default=128)
+parser.add_argument("--backend", type=str, default="gloo")
+parser.add_argument("--learning_rate", type=float, default=5e-2)
+parser.add_argument("--min_learning_rate", type=float, default=5e-5)
+parser.add_argument("--input_dim", type=int, default=0)
+parser.add_argument("--output_dim", type=int, default=0)
+parser.add_argument("--dump_epoch", type=int, default=1e10)
+parser.add_argument("--decay_factor", type=float, default=0.98)
+parser.add_argument("--decay_round", type=float, default=10)
+parser.add_argument("--num_loaders", type=int, default=2)
+parser.add_argument("--eval_interval", type=int, default=5)
+parser.add_argument("--sample_seed", type=int, default=233)  # 123 #233
+parser.add_argument("--test_ratio", type=float, default=1.0)
+parser.add_argument("--loss_decay", type=float, default=0.2)
+parser.add_argument("--exploration_min", type=float, default=0.3)
+parser.add_argument("--cut_off_util", type=float, default=0.05)  # 95 percentile
 
-parser.add_argument('--gradient_policy', type=str, default=None)
+parser.add_argument("--gradient_policy", type=str, default=None)
 
 # for yogi
-parser.add_argument('--yogi_eta', type=float, default=3e-3)
-parser.add_argument('--yogi_tau', type=float, default=1e-8)
-parser.add_argument('--yogi_beta', type=float, default=0.9)
-parser.add_argument('--yogi_beta2', type=float, default=0.99)
+parser.add_argument("--yogi_eta", type=float, default=3e-3)
+parser.add_argument("--yogi_tau", type=float, default=1e-8)
+parser.add_argument("--yogi_beta", type=float, default=0.9)
+parser.add_argument("--yogi_beta2", type=float, default=0.99)
+
+# for q-fedavg
+parser.add_argument("--qfed_q", type=float, default=1.0)
 
 
 # for prox
-parser.add_argument('--proxy_mu', type=float, default=0.1)
+parser.add_argument("--proxy_mu", type=float, default=0.1)
 
 # for detection
-parser.add_argument('--cfg_file', type=str,
-                    default='./utils/rcnn/cfgs/res101.yml')
-parser.add_argument('--test_output_dir', type=str, default='./logs/server')
-parser.add_argument('--train_size_file', type=str, default='')
-parser.add_argument('--test_size_file', type=str, default='')
-parser.add_argument('--data_cache', type=str, default='')
-parser.add_argument('--backbone', type=str, default='./resnet50.pth')
+parser.add_argument("--cfg_file", type=str, default="./utils/rcnn/cfgs/res101.yml")
+parser.add_argument("--test_output_dir", type=str, default="./logs/server")
+parser.add_argument("--train_size_file", type=str, default="")
+parser.add_argument("--test_size_file", type=str, default="")
+parser.add_argument("--data_cache", type=str, default="")
+parser.add_argument("--backbone", type=str, default="./resnet50.pth")
 
 
 # for malicious
-parser.add_argument('--malicious_factor', type=int, default=1e15)
-
-# for asynchronous FL buffer size
-parser.add_argument('--async_buffer', type=int, default=10)
-parser.add_argument(
-    '--checkin_period', type=int, default=50, help='number of rounds to sample async clients'
-)
-parser.add_argument('--arrival_interval', type=int, default=3)
-parser.add_argument(
-    "--async_mode", type=bool, default=False, help="use async FL aggregation"
-)
+parser.add_argument("--malicious_factor", type=int, default=1e15)
 
+# for asynchronous FL
+parser.add_argument("--max_concurrency", type=int, default=10)
+parser.add_argument("--max_staleness", type=int, default=5)
 
 # for differential privacy
-parser.add_argument('--noise_factor', type=float, default=0.1)
-parser.add_argument('--clip_threshold', type=float, default=3.0)
-parser.add_argument('--target_delta', type=float, default=0.0001)
+parser.add_argument("--noise_factor", type=float, default=0.1)
+parser.add_argument("--clip_threshold", type=float, default=3.0)
+parser.add_argument("--target_delta", type=float, default=0.0001)
 
 # for Oort
-parser.add_argument('--pacer_delta', type=float, default=5)
-parser.add_argument('--pacer_step', type=int, default=20)
-parser.add_argument('--exploration_alpha', type=float, default=0.3)
-parser.add_argument('--exploration_factor', type=float, default=0.9)
-parser.add_argument('--exploration_decay', type=float, default=0.98)
-parser.add_argument('--sample_window', type=float, default=5.0)
+parser.add_argument("--pacer_delta", type=float, default=5)
+parser.add_argument("--pacer_step", type=int, default=20)
+parser.add_argument("--exploration_alpha", type=float, default=0.3)
+parser.add_argument("--exploration_factor", type=float, default=0.9)
+parser.add_argument("--exploration_decay", type=float, default=0.98)
+parser.add_argument("--sample_window", type=float, default=5.0)
 
 # for albert
 parser.add_argument(
     "--line_by_line",
     action="store_true",
     help="Whether distinct lines of text in the dataset are to be handled as distinct sequences.",
 )
-parser.add_argument('--clf_block_size', type=int, default=32)
+parser.add_argument("--clf_block_size", type=int, default=32)
 
 
 parser.add_argument(
-    "--mlm", type=bool, default=False, help="Train with masked-language modeling loss instead of language modeling."
+    "--mlm",
+    type=bool,
+    default=False,
+    help="Train with masked-language modeling loss instead of language modeling.",
 )
 parser.add_argument(
-    "--mlm_probability", type=float, default=0.15, help="Ratio of tokens to mask for masked language modeling loss"
+    "--mlm_probability",
+    type=float,
+    default=0.15,
+    help="Ratio of tokens to mask for masked language modeling loss",
 )
 parser.add_argument(
-    "--overwrite_cache", type=bool, default=False, help="Overwrite the cached training and evaluation sets"
+    "--overwrite_cache",
+    type=bool,
+    default=False,
+    help="Overwrite the cached training and evaluation sets",
 )
 parser.add_argument(
     "--block_size",
     default=64,
     type=int,
     help="Optional input sequence length after tokenization."
     "The training dataset will be truncated in block of this size for training."
     "Default to the model max input length for single sentence inputs (take into account special tokens).",
 )
 
 
-parser.add_argument("--weight_decay", default=0, type=float,
-                    help="Weight decay if we apply some.")
-parser.add_argument("--adam_epsilon", default=1e-8,
-                    type=float, help="Epsilon for Adam optimizer.")
+parser.add_argument(
+    "--weight_decay", default=0, type=float, help="Weight decay if we apply some."
+)
+parser.add_argument(
+    "--adam_epsilon", default=1e-8, type=float, help="Epsilon for Adam optimizer."
+)
 
 # for tag prediction
-parser.add_argument("--vocab_token_size", type=int,
-                    default=10000, help="For vocab token size")
-parser.add_argument("--vocab_tag_size", type=int,
-                    default=500, help="For vocab tag size")
+parser.add_argument(
+    "--vocab_token_size", type=int, default=10000, help="For vocab token size"
+)
+parser.add_argument(
+    "--vocab_tag_size", type=int, default=500, help="For vocab tag size"
+)
 
 # for rl example
 parser.add_argument("--epsilon", type=float, default=0.9, help="greedy policy")
 parser.add_argument("--gamma", type=float, default=0.9, help="reward discount")
-parser.add_argument("--memory_capacity", type=int,
-                    default=2000, help="memory capacity")
-parser.add_argument("--target_replace_iter", type=int,
-                    default=15, help="update frequency")
+parser.add_argument("--memory_capacity", type=int, default=2000, help="memory capacity")
+parser.add_argument(
+    "--target_replace_iter", type=int, default=15, help="update frequency"
+)
 parser.add_argument("--n_actions", type=int, default=2, help="action number")
 parser.add_argument("--n_states", type=int, default=4, help="state number")
 
 
-# for speech
-parser.add_argument("--num_classes", type=int, default=35,
-                    help="For number of classes in speech")
+parser.add_argument(
+    "--num_classes", type=int, default=35, help="For number of classes of the dataset"
+)
 
 
 # for voice
-parser.add_argument('--train-manifest', metavar='DIR',
-                    help='path to train manifest csv', default='data/train_manifest.csv')
-parser.add_argument('--test-manifest', metavar='DIR',
-                    help='path to test manifest csv', default='data/test_manifest.csv')
-parser.add_argument('--sample-rate', default=16000,
-                    type=int, help='Sample rate')
-parser.add_argument('--labels-path', default='labels.json',
-                    help='Contains all characters for transcription')
-parser.add_argument('--window-size', default=.02, type=float,
-                    help='Window size for spectrogram in seconds')
-parser.add_argument('--window-stride', default=.01, type=float,
-                    help='Window stride for spectrogram in seconds')
-parser.add_argument('--window', default='hamming',
-                    help='Window type for spectrogram generation')
-parser.add_argument('--hidden-size', default=256,
-                    type=int, help='Hidden size of RNNs')
-parser.add_argument('--hidden-layers', default=7,
-                    type=int, help='Number of RNN layers')
-parser.add_argument('--rnn-type', default='lstm',
-                    help='Type of the RNN. rnn|gru|lstm are supported')
-parser.add_argument('--finetune', dest='finetune', action='store_true',
-                    help='Finetune the model from checkpoint "continue_from"')
-parser.add_argument('--speed-volume-perturb', dest='speed_volume_perturb', action='store_true',
-                    help='Use random tempo and gain perturbations.')
-parser.add_argument('--spec-augment', dest='spec_augment', action='store_true',
-                    help='Use simple spectral augmentation on mel spectograms.')
-parser.add_argument('--noise-dir', default=None,
-                    help='Directory to inject noise into audio. If default, noise Inject not added')
-parser.add_argument('--noise-prob', default=0.4,
-                    help='Probability of noise being added per sample')
-parser.add_argument('--noise-min', default=0.0,
-                    help='Minimum noise level to sample from. (1.0 means all noise, not original signal)', type=float)
-parser.add_argument('--noise-max', default=0.5,
-                    help='Maximum noise levels to sample from. Maximum 1.0', type=float)
-parser.add_argument('--no-bidirectional', dest='bidirectional', action='store_false', default=True,
-                    help='Turn off bi-directional RNNs, introduces lookahead convolution')
+parser.add_argument(
+    "--train-manifest",
+    metavar="DIR",
+    help="path to train manifest csv",
+    default="data/train_manifest.csv",
+)
+parser.add_argument(
+    "--test-manifest",
+    metavar="DIR",
+    help="path to test manifest csv",
+    default="data/test_manifest.csv",
+)
+parser.add_argument("--sample-rate", default=16000, type=int, help="Sample rate")
+parser.add_argument(
+    "--labels-path",
+    default="labels.json",
+    help="Contains all characters for transcription",
+)
+parser.add_argument(
+    "--window-size",
+    default=0.02,
+    type=float,
+    help="Window size for spectrogram in seconds",
+)
+parser.add_argument(
+    "--window-stride",
+    default=0.01,
+    type=float,
+    help="Window stride for spectrogram in seconds",
+)
+parser.add_argument(
+    "--window", default="hamming", help="Window type for spectrogram generation"
+)
+parser.add_argument("--hidden-size", default=256, type=int, help="Hidden size of RNNs")
+parser.add_argument("--hidden-layers", default=7, type=int, help="Number of RNN layers")
+parser.add_argument(
+    "--rnn-type", default="lstm", help="Type of the RNN. rnn|gru|lstm are supported"
+)
+parser.add_argument(
+    "--finetune",
+    dest="finetune",
+    action="store_true",
+    help='Finetune the model from checkpoint "continue_from"',
+)
+parser.add_argument(
+    "--speed-volume-perturb",
+    dest="speed_volume_perturb",
+    action="store_true",
+    help="Use random tempo and gain perturbations.",
+)
+parser.add_argument(
+    "--spec-augment",
+    dest="spec_augment",
+    action="store_true",
+    help="Use simple spectral augmentation on mel spectograms.",
+)
+parser.add_argument(
+    "--noise-dir",
+    default=None,
+    help="Directory to inject noise into audio. If default, noise Inject not added",
+)
+parser.add_argument(
+    "--noise-prob", default=0.4, help="Probability of noise being added per sample"
+)
+parser.add_argument(
+    "--noise-min",
+    default=0.0,
+    help="Minimum noise level to sample from. (1.0 means all noise, not original signal)",
+    type=float,
+)
+parser.add_argument(
+    "--noise-max",
+    default=0.5,
+    help="Maximum noise levels to sample from. Maximum 1.0",
+    type=float,
+)
+parser.add_argument(
+    "--no-bidirectional",
+    dest="bidirectional",
+    action="store_false",
+    default=True,
+    help="Turn off bi-directional RNNs, introduces lookahead convolution",
+)
 
 args, unknown = parser.parse_known_args()
 args.use_cuda = eval(args.use_cuda)
 
 
-datasetCategories = {'Mnist': 10, 'cifar10': 10, "imagenet": 1000, 'emnist': 47,
-                     'openImg': 596, 'google_speech': 35, 'femnist': 62, 'yelp': 5
-                     }
+datasetCategories = {
+    "Mnist": 10,
+    "cifar10": 10,
+    "imagenet": 1000,
+    "emnist": 47,
+    "openImg": 596,
+    "google_speech": 35,
+    "femnist": 62,
+    "yelp": 5,
+}
 
 # Profiled relative speech w.r.t. Mobilenet
-model_factor = {'shufflenet': 0.0644/0.0554,
-                'albert': 0.335/0.0554,
-                'resnet': 0.135/0.0554,
-                }
+model_factor = {
+    "shufflenet": 0.0644 / 0.0554,
+    "albert": 0.335 / 0.0554,
+    "resnet": 0.135 / 0.0554,
+}
 
-args.num_class = datasetCategories.get(args.data_set, 10)
+args.num_class = datasetCategories.get(args.data_set, args.num_classes)
 for model_name in model_factor:
     if model_name in args.model:
         args.clock_factor = args.clock_factor * model_factor[model_name]
         break
```

### Comparing `fedscale-0.5/fedscale/core/execution/client.py` & `fedscale-1.0/fedscale/cloud/execution/torch_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,113 @@
 import logging
 import math
+import time
 
 import torch
 from torch.autograd import Variable
+from overrides import overrides
+from torch.nn import CTCLoss
 
-from fedscale.core.execution.optimizers import ClientOptimizer
+from fedscale.cloud.execution.client_base import ClientBase
+from fedscale.cloud.execution.optimizers import ClientOptimizer
+from fedscale.cloud.internal.torch_model_adapter import TorchModelAdapter
 from fedscale.dataloaders.nlp import mask_tokens
+from fedscale.utils.model_test_module import test_pytorch_model
 
 
-class Client(object):
-    """Basic client component in Federated Learning"""
+class TorchClient(ClientBase):
+    """Implements a PyTorch-based client for training and evaluation."""
 
-    def __init__(self, conf):
+    def __init__(self, args):
+        """
+        Initializes a torch client.
+        :param args: Job args
+        """
+        self.args = args
         self.optimizer = ClientOptimizer()
-        self.init_task(conf)
-    
-    def init_task(self, conf):
-        if conf.task == "detection":
+        self.device = args.cuda_device if args.use_cuda else torch.device(
+            'cpu')
+        if args.task == "detection":
             self.im_data = Variable(torch.FloatTensor(1).cuda())
             self.im_info = Variable(torch.FloatTensor(1).cuda())
             self.num_boxes = Variable(torch.LongTensor(1).cuda())
             self.gt_boxes = Variable(torch.FloatTensor(1).cuda())
 
         self.epoch_train_loss = 1e-4
         self.completed_steps = 0
-        self.loss_squre = 0
+        self.loss_squared = 0
 
+    @overrides
     def train(self, client_data, model, conf):
+        """
+        Perform a training task.
+        :param client_data: client training dataset
+        :param model: the framework-specific model
+        :param conf: job config
+        :return: training results
+        """
+        client_id = conf.client_id
+        logging.info(f"Start to train (CLIENT: {client_id}) ...")
+        tokenizer = conf.tokenizer
 
-        clientId = conf.clientId
-        logging.info(f"Start to train (CLIENT: {clientId}) ...")
-        tokenizer, device = conf.tokenizer, conf.device
-
-        model = model.to(device=device)
+        model = model.to(device=self.device)
         model.train()
 
         trained_unique_samples = min(
             len(client_data.dataset), conf.local_steps * conf.batch_size)
         self.global_model = None
 
         if conf.gradient_policy == 'fed-prox':
             # could be move to optimizer
             self.global_model = [param.data.clone() for param in model.parameters()]
 
         optimizer = self.get_optimizer(model, conf)
         criterion = self.get_criterion(conf)
         error_type = None
 
-        # TODO: One may hope to run fixed number of epochs, instead of iterations
+        # NOTE: If one may hope to run fixed number of epochs, instead of iterations,
+        # use `while self.completed_steps < conf.local_steps * len(client_data)` instead
         while self.completed_steps < conf.local_steps:
-
             try:
                 self.train_step(client_data, conf, model, optimizer, criterion)
             except Exception as ex:
                 error_type = ex
                 break
 
         state_dicts = model.state_dict()
         model_param = {p: state_dicts[p].data.cpu().numpy()
                        for p in state_dicts}
-        results = {'clientId': clientId, 'moving_loss': self.epoch_train_loss,
-                   'trained_size': self.completed_steps*conf.batch_size, 'success': self.completed_steps > 0}
-        results['utility'] = math.sqrt(
-            self.loss_squre)*float(trained_unique_samples)
+        results = {'client_id': client_id, 'moving_loss': self.epoch_train_loss,
+                   'trained_size': self.completed_steps * conf.batch_size,
+                   'success': self.completed_steps == conf.local_steps}
 
         if error_type is None:
-            logging.info(f"Training of (CLIENT: {clientId}) completes, {results}")
+            logging.info(f"Training of (CLIENT: {client_id}) completes, {results}")
         else:
-            logging.info(f"Training of (CLIENT: {clientId}) failed as {error_type}")
+            logging.info(f"Training of (CLIENT: {client_id}) failed as {error_type}")
 
+        results['utility'] = math.sqrt(
+            self.loss_squared) * float(trained_unique_samples)
         results['update_weight'] = model_param
         results['wall_duration'] = 0
 
         return results
 
     def get_optimizer(self, model, conf):
         optimizer = None
         if conf.task == "detection":
             lr = conf.learning_rate
             params = []
             for key, value in dict(model.named_parameters()).items():
                 if value.requires_grad:
                     if 'bias' in key:
-                        params += [{'params': [value], 'lr':lr*(cfg.TRAIN.DOUBLE_BIAS + 1),
+                        params += [{'params': [value], 'lr': lr * (cfg.TRAIN.DOUBLE_BIAS + 1),
                                     'weight_decay': cfg.TRAIN.BIAS_DECAY and cfg.TRAIN.WEIGHT_DECAY or 0}]
                     else:
-                        params += [{'params': [value], 'lr':lr,
+                        params += [{'params': [value], 'lr': lr,
                                     'weight_decay': cfg.TRAIN.WEIGHT_DECAY}]
             optimizer = torch.optim.SGD(params, momentum=cfg.TRAIN.MOMENTUM)
 
         elif conf.task == 'nlp':
 
             no_decay = ["bias", "LayerNorm.weight"]
             optimizer_grouped_parameters = [
@@ -111,30 +129,30 @@
         return optimizer
 
     def get_criterion(self, conf):
 
         criterion = None
         if conf.task == 'voice':
             from torch_baidu_ctc import CTCLoss
-            criterion = CTCLoss(reduction='none').to(device=conf.device)
+            criterion = CTCLoss(reduction='none').to(device=self.device)
         else:
             criterion = torch.nn.CrossEntropyLoss(
-                reduction='none').to(device=conf.device)
+                reduction='none').to(device=self.device)
         return criterion
 
     def train_step(self, client_data, conf, model, optimizer, criterion):
 
         for data_pair in client_data:
             if conf.task == 'nlp':
                 (data, _) = data_pair
                 data, target = mask_tokens(
-                    data, tokenizer, conf, device=conf.device)
+                    data, tokenizer, conf, device=self.device)
             elif conf.task == 'voice':
                 (data, target, input_percentages,
-                    target_sizes), _ = data_pair
+                 target_sizes), _ = data_pair
                 input_sizes = input_percentages.mul_(
                     int(data.size(3))).int()
             elif conf.task == 'detection':
                 temp_data = data_pair
                 target = temp_data[4]
                 data = temp_data[0:4]
             else:
@@ -142,24 +160,24 @@
 
             if conf.task == "detection":
                 self.im_data.resize_(data[0].size()).copy_(data[0])
                 self.im_info.resize_(data[1].size()).copy_(data[1])
                 self.gt_boxes.resize_(data[2].size()).copy_(data[2])
                 self.num_boxes.resize_(data[3].size()).copy_(data[3])
             elif conf.task == 'speech':
-                data = torch.unsqueeze(data, 1).to(device=conf.device)
+                data = torch.unsqueeze(data, 1).to(device=self.device)
             elif conf.task == 'text_clf' and conf.model == 'albert-base-v2':
                 (data, masks) = data
                 data, masks = Variable(data).to(
-                    device=conf.device), Variable(masks).to(device=conf.device)
+                    device=self.device), Variable(masks).to(device=self.device)
 
             else:
-                data = Variable(data).to(device=conf.device)
+                data = Variable(data).to(device=self.device)
 
-            target = Variable(target).to(device=conf.device)
+            target = Variable(target).to(device=self.device)
 
             if conf.task == 'nlp':
                 outputs = model(data, labels=target)
                 loss = outputs[0]
             elif conf.task == 'voice':
                 outputs, output_sizes = model(data, input_sizes)
                 outputs = outputs.transpose(0, 1).float()  # TxNxH
@@ -168,27 +186,27 @@
             elif conf.task == 'text_clf' and conf.model == 'albert-base-v2':
                 outputs = model(
                     data, attention_mask=masks, labels=target)
                 loss = outputs.loss
                 output = outputs.logits
             elif conf.task == "detection":
                 rois, cls_prob, bbox_pred, \
-                    rpn_loss_cls, rpn_loss_box, \
-                    RCNN_loss_cls, RCNN_loss_bbox, \
-                    rois_label = model(
-                        self.im_data, self.im_info, self.gt_boxes, self.num_boxes)
+                rpn_loss_cls, rpn_loss_box, \
+                RCNN_loss_cls, RCNN_loss_bbox, \
+                rois_label = model(
+                    self.im_data, self.im_info, self.gt_boxes, self.num_boxes)
 
                 loss = rpn_loss_cls + rpn_loss_box \
-                    + RCNN_loss_cls + RCNN_loss_bbox
+                       + RCNN_loss_cls + RCNN_loss_bbox
 
                 loss_rpn_cls = rpn_loss_cls.item()
                 loss_rpn_box = rpn_loss_box.item()
                 loss_rcnn_cls = RCNN_loss_cls.item()
                 loss_rcnn_box = RCNN_loss_bbox.item()
-                
+
             else:
                 output = model(data)
                 loss = criterion(output, target)
 
             # ======== collect training feedback for other decision components [e.g., oort selector] ======
 
             if conf.task == 'nlp' or (conf.task == 'text_clf' and conf.model == 'albert-base-v2'):
@@ -197,24 +215,24 @@
             elif conf.task == "detection":
                 loss_list = [loss.tolist()]
                 loss = loss.mean()
             else:
                 loss_list = loss.tolist()
                 loss = loss.mean()
 
-            temp_loss = sum(loss_list)/float(len(loss_list))
-            self.loss_squre = sum([l**2 for l in loss_list]
-                                )/float(len(loss_list))
+            temp_loss = sum(loss_list) / float(len(loss_list))
+            self.loss_squared = sum([l ** 2 for l in loss_list]
+                                    ) / float(len(loss_list))
             # only measure the loss of the first epoch
             if self.completed_steps < len(client_data):
                 if self.epoch_train_loss == 1e-4:
                     self.epoch_train_loss = temp_loss
                 else:
                     self.epoch_train_loss = (
-                        1. - conf.loss_decay) * self.epoch_train_loss + conf.loss_decay * temp_loss
+                                                    1. - conf.loss_decay) * self.epoch_train_loss + conf.loss_decay * temp_loss
 
             # ========= Define the backward loss ==============
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
             # ========= Weight handler ========================
@@ -222,10 +240,38 @@
                 conf, model, self.global_model if self.global_model is not None else None)
 
             self.completed_steps += 1
 
             if self.completed_steps == conf.local_steps:
                 break
 
-
-    def test(self, conf):
-        pass
+    @overrides
+    def test(self, client_data, model, conf):
+        """
+        Perform a testing task.
+        :param client_data: client evaluation dataset
+        :param model: the framework-specific model
+        :param conf: job config
+        :return: testing results
+        """
+        evalStart = time.time()
+        if self.args.task == 'voice':
+            criterion = CTCLoss(reduction='mean').to(device=self.device)
+        else:
+            criterion = torch.nn.CrossEntropyLoss().to(device=self.device)
+        test_loss, acc, acc_5, test_results = test_pytorch_model(conf.rank, model, client_data,
+                                                                 device=self.device, criterion=criterion,
+                                                                 tokenizer=conf.tokenizer)
+        logging.info(
+            "Test results: Eval_time {}, test_loss {}, test_accuracy {:.2f}%, "
+            "test_5_accuracy {:.2f}% \n"
+                .format(round(time.time() - evalStart, 4), test_loss, acc * 100., acc_5 * 100.))
+        return test_results
+
+    @overrides
+    def get_model_adapter(self, model) -> TorchModelAdapter:
+        """
+        Return framework-specific model adapter.
+        :param model: the model
+        :return: a model adapter containing the model
+        """
+        return TorchModelAdapter(model)
```

### Comparing `fedscale-0.5/fedscale/core/execution/data_processor.py` & `fedscale-1.0/fedscale/cloud/execution/data_processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-import os
-
+import torch
 from torch.nn.utils.rnn import pad_sequence
 
-from fedscale.core.fllibs import *
+from fedscale.cloud.fllibs import *
 
 
 def collate(examples):
     if tokenizer._pad_token is None:
         return (pad_sequence(examples, batch_first=True), None)
     return (pad_sequence(examples, batch_first=True, padding_value=tokenizer.pad_token_id), None)
 
 
 def voice_collate_fn(batch):
     def func(p):
         return p[0].size(1)
-
-    start_time = time.time()
-
     batch = sorted(batch, key=lambda sample: sample[0].size(1), reverse=True)
     longest_sample = max(batch, key=func)[0]
     freq_size = longest_sample.size(0)
     minibatch_size = len(batch)
     max_seqlength = longest_sample.size(1)
     inputs = torch.zeros(minibatch_size, 1, freq_size, max_seqlength)
     input_percentages = torch.FloatTensor(minibatch_size)
@@ -32,11 +28,8 @@
         target = sample[1]
         seq_length = tensor.size(1)
         inputs[x][0].narrow(1, 0, seq_length).copy_(tensor)
         input_percentages[x] = seq_length / float(max_seqlength)
         target_sizes[x] = len(target)
         targets.extend(target)
     targets = torch.IntTensor(targets)
-
-    end_time = time.time()
-
     return (inputs, targets, input_percentages, target_sizes), None
```

### Comparing `fedscale-0.5/fedscale/core/execution/executor.py` & `fedscale-1.0/fedscale/cloud/execution/executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,284 +1,279 @@
 # -*- coding: utf-8 -*-
 import collections
 import gc
 import pickle
+import random
+import time
 from argparse import Namespace
 
+import numpy as np
 import torch
+import wandb
 
-import fedscale.core.channels.job_api_pb2 as job_api_pb2
-from fedscale.core import commons
-from fedscale.core.channels.channel_context import ClientConnections
-from fedscale.core.execution.client import Client
-from fedscale.core.execution.data_processor import collate, voice_collate_fn
-from fedscale.core.execution.rlclient import RLClient
-from fedscale.core.logger.execution import *
+import fedscale.cloud.channels.job_api_pb2 as job_api_pb2
+import fedscale.cloud.logger.executor_logging as logger
+from fedscale.cloud.channels.channel_context import ClientConnections
+from fedscale.cloud.execution.tensorflow_client import TensorflowClient
+from fedscale.cloud.execution.torch_client import TorchClient
+from fedscale.cloud.execution.data_processor import collate, voice_collate_fn
+from fedscale.cloud.execution.rl_client import RLClient
+from fedscale.cloud.fllibs import *
+from fedscale.dataloaders.divide_data import DataPartitioner, select_dataset
 
 
 class Executor(object):
     """Abstract class for FedScale executor.
 
     Args:
         args (dictionary): Variable arguments for fedscale runtime config. defaults to the setup in arg_parser.py
 
     """
+
     def __init__(self, args):
+        # initiate the executor log path, and executor ips
+        logger.initiate_client_setting()
+
+        self.model_adapter = self.get_client_trainer(args).get_model_adapter(
+            init_model()
+        )
 
         self.args = args
-        self.device = args.cuda_device if args.use_cuda else torch.device(
-            'cpu')
         self.num_executors = args.num_executors
         # ======== env information ========
         self.this_rank = args.this_rank
         self.executor_id = str(self.this_rank)
 
         # ======== model and data ========
-        self.model = self.training_sets = self.test_dataset = None
-        self.temp_model_path = os.path.join(
-            logDir, 'model_'+str(args.this_rank)+'.pth.tar')
+        self.training_sets = self.test_dataset = None
 
         # ======== channels ========
-        self.aggregator_communicator = ClientConnections(
-            args.ps_ip, args.ps_port)
+        self.aggregator_communicator = ClientConnections(args.ps_ip, args.ps_port)
 
         # ======== runtime information ========
         self.collate_fn = None
-        self.task = args.task
         self.round = 0
         self.start_run_time = time.time()
         self.received_stop_request = False
         self.event_queue = collections.deque()
 
+        if args.wandb_token != "":
+            os.environ["WANDB_API_KEY"] = args.wandb_token
+            self.wandb = wandb
+            if self.wandb.run is None:
+                self.wandb.init(
+                    project=f"fedscale-{args.job_name}",
+                    name=f"executor{args.this_rank}-{args.time_stamp}",
+                    group=f"{args.time_stamp}",
+                )
+            else:
+                logging.error("Warning: wandb has already been initialized")
+
+        else:
+            self.wandb = None
         super(Executor, self).__init__()
 
     def setup_env(self):
-        """Set up experiments environment
-        """
+        """Set up experiments environment"""
         logging.info(f"(EXECUTOR:{self.this_rank}) is setting up environ ...")
         self.setup_seed(seed=1)
 
     def setup_communication(self):
-        """Set up grpc connection
-        """
+        """Set up grpc connection"""
         self.init_control_communication()
         self.init_data_communication()
 
     def setup_seed(self, seed=1):
         """Set random seed for reproducibility
 
         Args:
             seed (int): random seed
 
         """
         torch.manual_seed(seed)
+        torch.backends.cudnn.deterministic = True
         torch.cuda.manual_seed_all(seed)
         np.random.seed(seed)
         random.seed(seed)
-        torch.backends.cudnn.deterministic = True
 
     def init_control_communication(self):
         """Create communication channel between coordinator and executor.
         This channel serves control messages.
         """
         self.aggregator_communicator.connect_to_server()
 
     def init_data_communication(self):
-        """In charge of jumbo data traffics (e.g., fetch training result)
-        """
+        """In charge of jumbo data traffics (e.g., fetch training result)"""
         pass
 
-    def init_model(self):
-        """Get the model architecture used in training
-
-        Returns: 
-            PyTorch or TensorFlow module: Based on the executor's machine learning framework, initialize and return the model for training
-        
-        """
-        assert self.args.engine == commons.PYTORCH, "Please override this function to define non-PyTorch models"
-        model = init_model()
-        model = model.to(device=self.device)
-        return model
-
     def init_data(self):
         """Return the training and testing dataset
 
         Returns:
             Tuple of DataPartitioner class: The partioned dataset class for training and testing
 
         """
         train_dataset, test_dataset = init_dataset()
-        if self.task == "rl":
+        if self.args.task == "rl":
             return train_dataset, test_dataset
-        # load data partitioner (entire_train_data)
+        if self.args.task == "nlp":
+            self.collate_fn = collate
+        elif self.args.task == "voice":
+            self.collate_fn = voice_collate_fn
+        # load data partitionxr (entire_train_data)
         logging.info("Data partitioner starts ...")
 
         training_sets = DataPartitioner(
-            data=train_dataset, args=self.args, numOfClass=self.args.num_class)
+            data=train_dataset, args=self.args, numOfClass=self.args.num_class
+        )
         training_sets.partition_data_helper(
-            num_clients=self.args.num_participants, data_map_file=self.args.data_map_file)
+            num_clients=self.args.num_participants,
+            data_map_file=self.args.data_map_file,
+        )
 
         testing_sets = DataPartitioner(
-            data=test_dataset, args=self.args, numOfClass=self.args.num_class, isTest=True)
+            data=test_dataset,
+            args=self.args,
+            numOfClass=self.args.num_class,
+            isTest=True,
+        )
         testing_sets.partition_data_helper(num_clients=self.num_executors)
 
         logging.info("Data partitioner completes ...")
 
-        if self.task == 'nlp':
-            self.collate_fn = collate
-        elif self.task == 'voice':
-            self.collate_fn = voice_collate_fn
-
         return training_sets, testing_sets
 
     def run(self):
-        """Start running the executor by setting up execution and communication environment, and monitoring the grpc message.
-        """
+        """Start running the executor by setting up execution and communication environment, and monitoring the grpc message."""
         self.setup_env()
-        self.model = self.init_model()
         self.training_sets, self.testing_sets = self.init_data()
         self.setup_communication()
         self.event_monitor()
 
     def dispatch_worker_events(self, request):
         """Add new events to worker queues
-        
+
         Args:
             request (string): Add grpc request from server (e.g. MODEL_TEST, MODEL_TRAIN) to event_queue.
-        
+
         """
         self.event_queue.append(request)
 
     def deserialize_response(self, responses):
         """Deserialize the response from server
 
         Args:
             responses (byte stream): Serialized response from server.
 
         Returns:
             ServerResponse defined at job_api.proto: The deserialized response object from server.
-        
+
         """
         return pickle.loads(responses)
 
     def serialize_response(self, responses):
         """Serialize the response to send to server upon assigned job completion
 
         Args:
-            responses (string, bool, or bytes): Client responses after job completion.
+            responses (string, bool, or bytes): TorchClient responses after job completion.
 
         Returns:
             bytes stream: The serialized response object to server.
-        
+
         """
         return pickle.dumps(responses)
 
-    def UpdateModel(self, config):
+    def UpdateModel(self, model_weights):
         """Receive the broadcasted global model for current round
 
         Args:
             config (PyTorch or TensorFlow model): The broadcasted global model config
-        
+
         """
-        self.update_model_handler(model=config)
+        self.round += 1
+        self.model_adapter.set_weights(model_weights, is_aggregator=False)
 
     def Train(self, config):
         """Load train config and data to start training on that client
 
         Args:
             config (dictionary): The client training config.
 
-        Returns:     
+        Returns:
             tuple (int, dictionary): The client id and train result
 
         """
-        client_id, train_config = config['client_id'], config['task_config']
-
-        model = None
-        if 'model' in train_config and train_config['model'] is not None:
-            model = train_config['model']
+        client_id, train_config = config["client_id"], config["task_config"]
 
+        if "model" not in config or not config["model"]:
+            raise "The 'model' object must be a non-null value in the training config."
         client_conf = self.override_conf(train_config)
         train_res = self.training_handler(
-            clientId=client_id, conf=client_conf, model=model)
+            client_id=client_id, conf=client_conf, model=config["model"]
+        )
 
         # Report execution completion meta information
         response = self.aggregator_communicator.stub.CLIENT_EXECUTE_COMPLETION(
             job_api_pb2.CompleteRequest(
-                client_id=str(client_id), executor_id=self.executor_id,
-                event=commons.CLIENT_TRAIN, status=True, msg=None,
-                meta_result=None, data_result=None
+                client_id=str(client_id),
+                executor_id=self.executor_id,
+                event=commons.CLIENT_TRAIN,
+                status=True,
+                msg=None,
+                meta_result=None,
+                data_result=None,
             )
         )
         self.dispatch_worker_events(response)
 
         return client_id, train_res
 
     def Test(self, config):
         """Model Testing. By default, we test the accuracy on all data of clients in the test group
-        
+
         Args:
             config (dictionary): The client testing config.
-        
+
         """
-        test_res = self.testing_handler(args=self.args)
-        test_res = {'executorId': self.this_rank, 'results': test_res}
+        test_res = self.testing_handler(model=config["model"])
+        test_res = {"executorId": self.this_rank, "results": test_res}
 
         # Report execution completion information
         response = self.aggregator_communicator.stub.CLIENT_EXECUTE_COMPLETION(
             job_api_pb2.CompleteRequest(
-                client_id=self.executor_id, executor_id=self.executor_id,
-                event=commons.MODEL_TEST, status=True, msg=None,
-                meta_result=None, data_result=self.serialize_response(test_res)
+                client_id=self.executor_id,
+                executor_id=self.executor_id,
+                event=commons.MODEL_TEST,
+                status=True,
+                msg=None,
+                meta_result=None,
+                data_result=self.serialize_response(test_res),
             )
         )
         self.dispatch_worker_events(response)
 
     def Stop(self):
-        """Stop the current executor
-        """
+        """Stop the current executor"""
+        logging.info(f"Terminating the executor ...")
         self.aggregator_communicator.close_sever_connection()
         self.received_stop_request = True
+        if self.wandb != None:
+            self.wandb.finish()
 
     def report_executor_info_handler(self):
         """Return the statistics of training dataset
 
         Returns:
             int: Return the statistics of training dataset, in simulation return the number of clients
 
         """
         return self.training_sets.getSize()
 
-    def update_model_handler(self, model):
-        """Update the model copy on this executor
-
-        Args:
-            config (PyTorch or TensorFlow model): The broadcasted global model
-
-        """
-        self.model = model
-        self.round += 1
-
-        # Dump latest model to disk
-        with open(self.temp_model_path, 'wb') as model_out:
-            pickle.dump(self.model, model_out)
-
-    def load_global_model(self):
-        """ Load last global model
-
-        Returns:
-            PyTorch or TensorFlow model: The lastest global model
-
-        """
-        with open(self.temp_model_path, 'rb') as model_in:
-            model = pickle.load(model_in)
-        return model
-
     def override_conf(self, config):
-        """ Override the variable arguments for different client
+        """Override the variable arguments for different client
 
         Args:
             config (dictionary): The client runtime config.
 
         Returns:
             dictionary: Variable arguments for client runtime config.
 
@@ -287,167 +282,200 @@
 
         for key in config:
             default_conf[key] = config[key]
 
         return Namespace(**default_conf)
 
     def get_client_trainer(self, conf):
-        """A abstract base class for client with training handler, developer can redefine to this function to customize the client training:
-
-        Args:
-            config (dictionary): The client runtime config.
-
-        Returns:
-            Client: A abstract base client class with runtime config conf.
-
         """
-        return Client(conf)
+        Returns a framework-specific client that handles training and evaluation.
+        :param conf: job config
+        :return: framework-specific client instance
+        """
+        if conf.engine == commons.TENSORFLOW:
+            return TensorflowClient(conf)
+        elif conf.engine == commons.PYTORCH:
+            if conf.task == "rl":
+                return RLClient(conf)
+            else:
+                return TorchClient(conf)
+        raise "Currently, FedScale supports tensorflow and pytorch."
 
-    def training_handler(self, clientId, conf, model=None):
+    def training_handler(self, client_id, conf, model):
         """Train model given client id
-        
+
         Args:
-            clientId (int): The client id.
+            client_id (int): The client id.
             conf (dictionary): The client runtime config.
 
         Returns:
             dictionary: The train result
-        
-        """
-        # load last global model
-        client_model = self.load_global_model() if model is None else model
 
-        conf.clientId, conf.device = clientId, self.device
+        """
+        self.model_adapter.set_weights(model, is_aggregator=False)
+        conf.client_id = client_id
         conf.tokenizer = tokenizer
-        if self.args.task == "rl":
-            client_data = self.training_sets
-            client = RLClient(conf)
-            train_res = client.train(
-                client_data=client_data, model=client_model, conf=conf)
-        else:
-            client_data = select_dataset(clientId, self.training_sets,
-                                         batch_size=conf.batch_size, args=self.args,
-                                         collate_fn=self.collate_fn
-                                         )
-
-            client = self.get_client_trainer(conf)
-            train_res = client.train(
-                client_data=client_data, model=client_model, conf=conf)
+        client_data = (
+            self.training_sets
+            if self.args.task == "rl"
+            else select_dataset(
+                client_id,
+                self.training_sets,
+                batch_size=conf.batch_size,
+                args=self.args,
+                collate_fn=self.collate_fn,
+            )
+        )
+        client = self.get_client_trainer(self.args)
+        train_res = client.train(
+            client_data=client_data, model=self.model_adapter.get_model(), conf=conf
+        )
 
         return train_res
 
-    def testing_handler(self, args):
+    def testing_handler(self, model):
         """Test model
-        
+
         Args:
             args (dictionary): Variable arguments for fedscale runtime config. defaults to the setup in arg_parser.py
-
+            config (dictionary): Variable arguments from coordinator.
         Returns:
             dictionary: The test result
 
         """
-        evalStart = time.time()
-        device = self.device
-        model = self.load_global_model()
-        if self.task == 'rl':
-            client = RLClient(args)
-            test_res = client.test(args, self.this_rank, model, device=device)
-            _, _, _, testResults = test_res
-        else:
-            data_loader = select_dataset(self.this_rank, self.testing_sets,
-                                         batch_size=args.test_bsz, args=args,
-                                         isTest=True, collate_fn=self.collate_fn
-                                         )
-
-            if self.task == 'voice':
-                criterion = CTCLoss(reduction='mean').to(device=device)
-            else:
-                criterion = torch.nn.CrossEntropyLoss().to(device=device)
-
-            if self.args.engine == commons.PYTORCH:
-                test_res = test_model(self.this_rank, model, data_loader,
-                                      device=device, criterion=criterion, tokenizer=tokenizer)
-            else:
-                raise Exception(f"Need customized implementation for model testing in {self.args.engine} engine")
-
-            test_loss, acc, acc_5, testResults = test_res
-            logging.info("After aggregation round {}, CumulTime {}, eval_time {}, test_loss {}, test_accuracy {:.2f}%, test_5_accuracy {:.2f}% \n"
-                         .format(self.round, round(time.time() - self.start_run_time, 4), round(time.time() - evalStart, 4), test_loss, acc*100., acc_5*100.))
+        self.model_adapter.set_weights(model, is_aggregator=False)
+        test_config = self.override_conf(
+            {
+                "rank": self.this_rank,
+                "memory_capacity": self.args.memory_capacity,
+                "tokenizer": tokenizer,
+            }
+        )
+        client = self.get_client_trainer(test_config)
+        data_loader = select_dataset(
+            self.this_rank,
+            self.testing_sets,
+            batch_size=self.args.test_bsz,
+            args=self.args,
+            isTest=True,
+            collate_fn=self.collate_fn,
+        )
 
+        test_results = client.test(
+            data_loader, model=self.model_adapter.get_model(), conf=test_config
+        )
+        self.log_test_result(test_results)
         gc.collect()
 
-        return testResults
+        return test_results
 
     def client_register(self):
-        """Register the executor information to the aggregator
-        """
+        """Register the executor information to the aggregator"""
         start_time = time.time()
         while time.time() - start_time < 180:
             try:
                 response = self.aggregator_communicator.stub.CLIENT_REGISTER(
                     job_api_pb2.RegisterRequest(
                         client_id=self.executor_id,
                         executor_id=self.executor_id,
                         executor_info=self.serialize_response(
-                            self.report_executor_info_handler())
+                            self.report_executor_info_handler()
+                        ),
                     )
                 )
                 self.dispatch_worker_events(response)
                 break
             except Exception as e:
-                logging.warning(f"Failed to connect to aggregator {e}. Will retry in 5 sec.")
+                logging.warning(
+                    f"Failed to connect to aggregator {e}. Will retry in 5 sec."
+                )
                 time.sleep(5)
 
     def client_ping(self):
-        """Ping the aggregator for new task
-        """
-        response = self.aggregator_communicator.stub.CLIENT_PING(job_api_pb2.PingRequest(
-            client_id=self.executor_id,
-            executor_id=self.executor_id
-        ))
+        """Ping the aggregator for new task"""
+        response = self.aggregator_communicator.stub.CLIENT_PING(
+            job_api_pb2.PingRequest(
+                client_id=self.executor_id, executor_id=self.executor_id
+            )
+        )
         self.dispatch_worker_events(response)
 
     def event_monitor(self):
-        """Activate event handler once receiving new message
-        """
+        """Activate event handler once receiving new message"""
         logging.info("Start monitoring events ...")
         self.client_register()
 
-        while self.received_stop_request == False:
+        while not self.received_stop_request:
             if len(self.event_queue) > 0:
                 request = self.event_queue.popleft()
                 current_event = request.event
 
                 if current_event == commons.CLIENT_TRAIN:
                     train_config = self.deserialize_response(request.meta)
                     train_model = self.deserialize_response(request.data)
-                    train_config['model'] = train_model
-                    train_config['client_id'] = int(train_config['client_id'])
+                    train_config["model"] = train_model
+                    train_config["client_id"] = int(train_config["client_id"])
                     client_id, train_res = self.Train(train_config)
 
                     # Upload model updates
-                    _ = self.aggregator_communicator.stub.CLIENT_EXECUTE_COMPLETION.future(
-                        job_api_pb2.CompleteRequest(client_id=str(client_id), executor_id=self.executor_id,
-                                                    event=commons.UPLOAD_MODEL, status=True, msg=None,
-                                                    meta_result=None, data_result=self.serialize_response(train_res)
-                                                    ))
+                    future_call = self.aggregator_communicator.stub.CLIENT_EXECUTE_COMPLETION.future(
+                        job_api_pb2.CompleteRequest(
+                            client_id=str(client_id),
+                            executor_id=self.executor_id,
+                            event=commons.UPLOAD_MODEL,
+                            status=True,
+                            msg=None,
+                            meta_result=None,
+                            data_result=self.serialize_response(train_res),
+                        )
+                    )
+                    future_call.add_done_callback(
+                        lambda _response: self.dispatch_worker_events(
+                            _response.result()
+                        )
+                    )
 
                 elif current_event == commons.MODEL_TEST:
-                    self.Test(self.deserialize_response(request.meta))
+                    test_config = self.deserialize_response(request.meta)
+                    test_model = self.deserialize_response(request.data)
+                    test_config["model"] = test_model
+                    test_config["client_id"] = int(test_config["client_id"])
+                    self.Test(test_config)
 
                 elif current_event == commons.UPDATE_MODEL:
-                    broadcast_config = self.deserialize_response(request.data)
-                    self.UpdateModel(broadcast_config)
+                    model_weights = self.deserialize_response(request.data)
+                    self.UpdateModel(model_weights)
 
                 elif current_event == commons.SHUT_DOWN:
                     self.Stop()
 
                 elif current_event == commons.DUMMY_EVENT:
                     pass
             else:
                 time.sleep(1)
-                self.client_ping()
+                try:
+                    self.client_ping()
+                except Exception as e:
+                    logging.info(
+                        f"Caught exception {e} from aggregator, terminating executor {self.this_rank} ..."
+                    )
+                    self.Stop()
+
+    def log_test_result(self, test_res):
+        """Log test results to wandb server if enabled"""
+        acc = round(test_res["top_1"] / test_res["test_len"], 4)
+        acc_5 = round(test_res["top_5"] / test_res["test_len"], 4)
+        test_loss = test_res["test_loss"] / test_res["test_len"]
+        if self.wandb != None:
+            self.wandb.log(
+                {
+                    "Test/round_to_top1_accuracy": acc,
+                    "Test/round_to_top5_accuracy": acc_5,
+                    "Test/round_to_loss": test_loss,
+                },
+                step=self.round,
+            )
 
 
 if __name__ == "__main__":
-    executor = Executor(args)
+    executor = Executor(parser.args)
     executor.run()
```

### Comparing `fedscale-0.5/fedscale/core/execution/rlclient.py` & `fedscale-1.0/fedscale/cloud/execution/rl_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import logging
 import math
 
-from fedscale.core.execution.client import Client
-from fedscale.core.execution.optimizers import ClientOptimizer
-from fedscale.dataloaders.dqn import *
+from fedscale.cloud.execution.torch_client import TorchClient
+from fedscale.cloud.execution.optimizers import ClientOptimizer
 
+import fedscale.cloud.config_parser as parser
+if parser.args.task == 'rl':
+    from fedscale.dataloaders.dqn import *
 
-class RLClient(Client):
+
+class RLClient(TorchClient):
     """Basic client component in Federated Learning"""
 
     def __init__(self, conf):
         self.optimizer = ClientOptimizer()
         self.dqn = DQN(conf)
         pass
 
     def train(self, client_data, model, conf):
 
-        clientId = conf.clientId
-        logging.info(f"Start to train (CLIENT: {clientId}) ...")
-        device = conf.device
+        client_id = conf.client_id
+        logging.info(f"Start to train (CLIENT: {client_id}) ...")
+        device = self.device
         model = model.to(device=device)
         # self.dqn.eval_net = self.dqn.eval_net.to(device=device)
         # self.dqn.target_net = self.dqn.target_net.to(device=device)
         global_model = None
 
         if conf.gradient_policy == 'prox':
             # could be move to optimizer
@@ -71,31 +74,31 @@
             except Exception as ex:
                 error_type = ex
                 break
 
         model.load_state_dict(self.dqn.target_net.state_dict())
         model_param = [param.data.cpu().numpy()
                        for param in model.parameters()]
-        results = {'clientId': clientId, 'moving_loss': epoch_train_loss,
+        results = {'client_id': client_id, 'moving_loss': epoch_train_loss,
                    'trained_size': completed_steps*conf.batch_size, 'success': completed_steps > 0}
         results['utility'] = math.sqrt(
             epoch_train_loss)*float(trained_unique_samples)
 
         if error_type is None:
-            logging.info(f"Training of (CLIENT: {clientId}) completes, {results}")
+            logging.info(f"Training of (CLIENT: {client_id}) completes, {results}")
         else:
-            logging.info(f"Training of (CLIENT: {clientId}) failed as {error_type}")
+            logging.info(f"Training of (CLIENT: {client_id}) failed as {error_type}")
 
         results['update_weight'] = model_param
         results['wall_duration'] = 0
 
         return results
 
-    def test(self, args, rank, model, device):
-        model = model.to(device=device)
+    def test(self, client_data, model, conf):
+        model = model.to(device=self.device)
         self.dqn.target_net.load_state_dict(model.state_dict())
         self.dqn.set_eval_mode()
         env = gym.make('CartPole-v0').unwrapped
         reward_sum = 0
         test_loss = 0
         s = env.reset()
         while True:
@@ -105,15 +108,15 @@
             r1 = (env.x_threshold - abs(x)) / env.x_threshold - 0.8
             r2 = (env.theta_threshold_radians - abs(theta)) / \
                 env.theta_threshold_radians - 0.5
             new_r = r1 + r2
             self.dqn.store_transition(s, a, new_r, s_)
             reward_sum += new_r
             s = s_
-            if self.dqn.memory_counter > args.memory_capacity:
+            if self.dqn.memory_counter > conf['memory_capacity']:
                 test_loss += self.dqn.learn()
 
             if done:
                 break
         logging.info('Rank {}: Test set: Average loss: {}, Reward: {}'
-                     .format(rank, test_loss, reward_sum))
+                     .format(conf['rank'], test_loss, reward_sum))
         return 0, 0, 0, {'top_1': reward_sum, 'top_5': reward_sum, 'test_loss': test_loss, 'test_len': 1}
```

### Comparing `fedscale-0.5/fedscale/core/fllibs.py` & `fedscale-1.0/fedscale/cloud/fllibs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,369 +1,369 @@
 # Standard libs
-import collections
-import copy
-import datetime
-import gc
 import json
 import logging
-import math
 import os
-import pickle
-import random
-import re
-import socket
 import sys
-import threading
-import time
-from collections import OrderedDict
-
-import numpy
-import numpy as np
-# PyTorch libs
-import torch
-import torch.distributed as dist
 import torchvision.models as tormodels
-from torch.autograd import Variable
-from torch.multiprocessing import Process, Queue
-from torch.utils.data import DataLoader
 from torchvision import datasets, transforms
 
-from fedscale.core.aggregation.optimizers import ServerOptimizer
-from fedscale.core.client_manager import clientManager
 # libs from fedscale
-from fedscale.core.config_parser import args
-from fedscale.dataloaders.divide_data import DataPartitioner, select_dataset
+import fedscale.cloud.config_parser as parser
+from fedscale.cloud import commons
 from fedscale.dataloaders.utils_data import get_data_transform
-from fedscale.utils.model_test_module import test_model
 # FedScale model libs
-from fedscale.utils.models.model_provider import get_cv_model
+from fedscale.utils.models.torch_model_provider import get_cv_model
+from fedscale.utils.models.tensorflow_model_provider import get_tensorflow_model
 
 tokenizer = None
-if args.task == 'nlp' or args.task == 'text_clf':
-    from transformers import (AdamW, AlbertTokenizer, AutoConfig,
-                              AutoModelWithLMHead, AutoTokenizer,
-                              MobileBertForPreTraining)
-
-    from fedscale.dataloaders.nlp import load_and_cache_examples, mask_tokens
-    tokenizer = AlbertTokenizer.from_pretrained(
-        'albert-base-v2', do_lower_case=True)
-elif args.task == 'speech':
-    import numba
-
-    from fedscale.dataloaders.speech import SPEECH, BackgroundNoiseDataset
-    from fedscale.dataloaders.transforms_stft import (AddBackgroundNoiseOnSTFT,
-                                                      DeleteSTFT,
-                                                      FixSTFTDimension,
-                                                      StretchAudioOnSTFT,
-                                                      TimeshiftAudioOnSTFT,
-                                                      ToMelSpectrogramFromSTFT,
-                                                      ToSTFT)
-    from fedscale.dataloaders.transforms_wav import (ChangeAmplitude,
-                                                     ChangeSpeedAndPitchAudio,
-                                                     FixAudioLength, LoadAudio,
-                                                     ToMelSpectrogram,
-                                                     ToTensor)
-elif args.task == 'detection':
-    import pickle
-
-    from fedscale.dataloaders.rcnn.lib.datasets.factory import get_imdb
-    from fedscale.dataloaders.rcnn.lib.datasets.pascal_voc import readClass
-    from fedscale.dataloaders.rcnn.lib.model.faster_rcnn.resnet import resnet
-    from fedscale.dataloaders.rcnn.lib.model.roi_layers import nms
-    from fedscale.dataloaders.rcnn.lib.model.rpn.bbox_transform import (
-        bbox_transform_inv, clip_boxes)
-    from fedscale.dataloaders.rcnn.lib.model.utils.config import (
-        cfg, cfg_from_file, cfg_from_list, get_output_dir)
-    from fedscale.dataloaders.rcnn.lib.model.utils.net_utils import (
-        adjust_learning_rate, clip_gradient, load_net, save_checkpoint,
-        save_net, weights_normal_init)
-    from fedscale.dataloaders.rcnn.lib.roi_data_layer.roibatchLoader import \
-        roibatchLoader
-    from fedscale.dataloaders.rcnn.lib.roi_data_layer.roidb import \
-        combined_roidb
-elif args.task == 'voice':
-    from torch_baidu_ctc import CTCLoss
-elif args.task == 'rl':
-    import gym
 
-    from fedscale.dataloaders.dqn import *
+
+def import_libs():
+    global tokenizer
+
+    if parser.args.task == 'nlp' or parser.args.task == 'text_clf':
+        global AdamW, AlbertTokenizer, AutoConfig, AutoModelWithLMHead, AutoTokenizer, MobileBertForPreTraining, load_and_cache_examples, mask_tokens
+
+        from transformers import (AdamW, AlbertTokenizer, AutoConfig,
+                                  AutoModelWithLMHead, AutoTokenizer,
+                                  MobileBertForPreTraining)
+
+        from fedscale.dataloaders.nlp import load_and_cache_examples, mask_tokens
+        tokenizer = AlbertTokenizer.from_pretrained(
+            'albert-base-v2', do_lower_case=True)
+    elif parser.args.task == 'speech':
+        global numba, SPEECH, BackgroundNoiseDataset, AddBackgroundNoiseOnSTFT, DeleteSTFT, FixSTFTDimension, StretchAudioOnSTFT, TimeshiftAudioOnSTFT, ToMelSpectrogramFromSTFT, ToSTFT, ChangeAmplitude, ChangeSpeedAndPitchAudio, FixAudioLength, LoadAudio, ToMelSpectrogram, ToTensor
+
+        import numba
+
+        from fedscale.dataloaders.speech import SPEECH, BackgroundNoiseDataset
+        from fedscale.dataloaders.transforms_stft import (AddBackgroundNoiseOnSTFT,
+                                                          DeleteSTFT,
+                                                          FixSTFTDimension,
+                                                          StretchAudioOnSTFT,
+                                                          TimeshiftAudioOnSTFT,
+                                                          ToMelSpectrogramFromSTFT,
+                                                          ToSTFT)
+        from fedscale.dataloaders.transforms_wav import (ChangeAmplitude,
+                                                         ChangeSpeedAndPitchAudio,
+                                                         FixAudioLength, LoadAudio,
+                                                         ToMelSpectrogram,
+                                                         ToTensor)
+    elif parser.args.task == 'detection':
+        global pickle, get_imdb, readClass, resnet, nms, bbox_transform_inv, clip_boxes, cfg, cfg_from_file, cfg_from_list, get_output_dir, adjust_learning_rate, clip_gradient, load_net, save_checkpoint, save_net, weights_normal_init, roibatchLoader, combined_roidb
+
+        import pickle
+        from fedscale.dataloaders.rcnn.lib.datasets.factory import get_imdb
+        from fedscale.dataloaders.rcnn.lib.datasets.pascal_voc import readClass
+        from fedscale.dataloaders.rcnn.lib.model.faster_rcnn.resnet import resnet
+        from fedscale.dataloaders.rcnn.lib.model.roi_layers import nms
+        from fedscale.dataloaders.rcnn.lib.model.rpn.bbox_transform import (
+            bbox_transform_inv, clip_boxes)
+        from fedscale.dataloaders.rcnn.lib.model.utils.config import (
+            cfg, cfg_from_file, cfg_from_list, get_output_dir)
+        from fedscale.dataloaders.rcnn.lib.model.utils.net_utils import (
+            adjust_learning_rate, clip_gradient, load_net, save_checkpoint,
+            save_net, weights_normal_init)
+        from fedscale.dataloaders.rcnn.lib.roi_data_layer.roibatchLoader import \
+            roibatchLoader
+        from fedscale.dataloaders.rcnn.lib.roi_data_layer.roidb import \
+            combined_roidb
+    elif parser.args.task == 'voice':
+        global CTCLoss
+
+        from torch_baidu_ctc import CTCLoss
+    elif parser.args.task == 'rl':
+        global gym, RLData, Net, DQN
+
+        import gym
+
+        from fedscale.dataloaders.dqn import RLData, Net, DQN
+
 
 # shared functions of aggregator and clients
 # initiate for nlp
 
-os.environ['MASTER_ADDR'] = args.ps_ip
-os.environ['MASTER_PORT'] = args.ps_port
-
+# Yile: are these vars used anywhere?
+os.environ['MASTER_ADDR'] = parser.args.ps_ip
+os.environ['MASTER_PORT'] = parser.args.ps_port
 
 outputClass = {'Mnist': 10, 'cifar10': 10, "imagenet": 1000, 'emnist': 47, 'amazon': 5,
                'openImg': 596, 'google_speech': 35, 'femnist': 62, 'yelp': 5, 'inaturalist': 1010
                }
 
 
 def init_model():
     global tokenizer
 
     logging.info("Initializing the model ...")
 
-    if args.task == 'nlp':
+    import_libs()
+
+    if parser.args.task == 'nlp':
         config = AutoConfig.from_pretrained(
-            os.path.join(args.data_dir, args.model+'-config.json'))
+            os.path.join(parser.args.data_dir, parser.args.model + '-config.json'))
         model = AutoModelWithLMHead.from_config(config)
         tokenizer = AlbertTokenizer.from_pretrained(
-            args.model, do_lower_case=True)
+            parser.args.model, do_lower_case=True)
 
         # model_name = 'google/mobilebert-uncased'
         # config = AutoConfig.from_pretrained(model_name)
         # tokenizer = AutoTokenizer.from_pretrained(model_name, use_fast=True)
         # model = MobileBertForPreTraining.from_pretrained(model_name)
         # model = AutoModelWithLMHead.from_config(config)
 
-    elif args.task == 'text_clf':
+    elif parser.args.task == 'text_clf':
 
-        if args.model == 'albert':
-            from transformers import (AlbertForSequenceClassification,
-                                      AutoConfig)
+        if parser.args.model == 'albert':
+            from transformers import AlbertForSequenceClassification
             config = AutoConfig.from_pretrained(os.path.join(
-                args.log_path, 'albert-small-config.json'))
-            config.num_labels = outputClass[args.data_set]
+                parser.args.log_path, 'albert-small-config.json'))
+            config.num_labels = outputClass[parser.args.data_set]
             model = AlbertForSequenceClassification(config)
-        elif args.model == 'lr':
+        elif parser.args.model == 'lr':
             from fedscale.utils.models.simple.models import LogisticRegression
-            model = LogisticRegression(300, outputClass[args.data_set])
+            model = LogisticRegression(300, outputClass[parser.args.data_set])
 
-    elif args.task == 'tag-one-sample':
+    elif parser.args.task == 'tag-one-sample':
         # Load LR model for tag prediction
-        model = LogisticRegression(args.vocab_token_size, args.vocab_tag_size)
-    elif args.task == 'speech':
-        if args.model == 'mobilenet':
+        model = LogisticRegression(parser.args.vocab_token_size, parser.args.vocab_tag_size)
+    elif parser.args.task == 'speech':
+        if parser.args.model == 'mobilenet':
             from fedscale.utils.models.specialized.resnet_speech import \
                 mobilenet_v2
-            model = mobilenet_v2(num_classes=outputClass[args.data_set])
-        elif args.model == "resnet18":
+            model = mobilenet_v2(num_classes=outputClass[parser.args.data_set])
+        elif parser.args.model == "resnet18":
             from fedscale.utils.models.specialized.resnet_speech import \
                 resnet18
             model = resnet18(
-                num_classes=outputClass[args.data_set], in_channels=1)
-        elif args.model == "resnet34":
+                num_classes=outputClass[parser.args.data_set], in_channels=1)
+        elif parser.args.model == "resnet34":
             from fedscale.utils.models.specialized.resnet_speech import \
                 resnet34
             model = resnet34(
-                num_classes=outputClass[args.data_set], in_channels=1)
-        elif args.model == "resnet50":
+                num_classes=outputClass[parser.args.data_set], in_channels=1)
+        elif parser.args.model == "resnet50":
             from fedscale.utils.models.specialized.resnet_speech import \
                 resnet50
             model = resnet50(
-                num_classes=outputClass[args.data_set], in_channels=1)
-        elif args.model == "resnet101":
+                num_classes=outputClass[parser.args.data_set], in_channels=1)
+        elif parser.args.model == "resnet101":
             from fedscale.utils.models.specialized.resnet_speech import \
                 resnet101
             model = resnet101(
-                num_classes=outputClass[args.data_set], in_channels=1)
-        elif args.model == "resnet152":
+                num_classes=outputClass[parser.args.data_set], in_channels=1)
+        elif parser.args.model == "resnet152":
             from fedscale.utils.models.specialized.resnet_speech import \
                 resnet152
             model = resnet152(
-                num_classes=outputClass[args.data_set], in_channels=1)
+                num_classes=outputClass[parser.args.data_set], in_channels=1)
         else:
             # Should not reach here
             logging.info('Model must be resnet or mobilenet')
             sys.exit(-1)
 
-    elif args.task == 'voice':
+    elif parser.args.task == 'voice':
         from fedscale.utils.models.specialized.voice_model import (
             DeepSpeech, supported_rnns)
 
         # Initialise new model training
-        with open(os.path.join(args.data_dir, "labels.json")) as label_file:
+        with open(os.path.join(parser.args.data_dir, "labels.json")) as label_file:
             labels = json.load(label_file)
 
-        audio_conf = dict(sample_rate=args.sample_rate,
-                          window_size=args.window_size,
-                          window_stride=args.window_stride,
-                          window=args.window,
-                          noise_dir=args.noise_dir,
-                          noise_prob=args.noise_prob,
-                          noise_levels=(args.noise_min, args.noise_max))
-        model = DeepSpeech(rnn_hidden_size=args.hidden_size,
-                           nb_layers=args.hidden_layers,
+        audio_conf = dict(sample_rate=parser.args.sample_rate,
+                          window_size=parser.args.window_size,
+                          window_stride=parser.args.window_stride,
+                          window=parser.args.window,
+                          noise_dir=parser.args.noise_dir,
+                          noise_prob=parser.args.noise_prob,
+                          noise_levels=(parser.args.noise_min, parser.args.noise_max))
+        model = DeepSpeech(rnn_hidden_size=parser.args.hidden_size,
+                           nb_layers=parser.args.hidden_layers,
                            labels=labels,
-                           rnn_type=supported_rnns[args.rnn_type.lower()],
+                           rnn_type=supported_rnns[parser.args.rnn_type.lower()],
                            audio_conf=audio_conf,
-                           bidirectional=args.bidirectional)
-    elif args.task == 'detection':
-        cfg_from_file(args.cfg_file)
-        cfg_from_list(['DATA_DIR', args.data_dir])
-        model = resnet(readClass(os.path.join(args.data_dir, "class.txt")), 50,
-                       pretrained=True, class_agnostic=False, pretrained_model=args.backbone)
+                           bidirectional=parser.args.bidirectional)
+    elif parser.args.task == 'detection':
+        cfg_from_file(parser.args.cfg_file)
+        cfg_from_list(['DATA_DIR', parser.args.data_dir])
+        model = resnet(readClass(os.path.join(parser.args.data_dir, "class.txt")), 50,
+                       pretrained=True, class_agnostic=False, pretrained_model=parser.args.backbone)
         model.create_architecture()
         return model
-    elif args.task == 'rl':
-        model = DQN(args).target_net
+    elif parser.args.task == 'rl':
+        model = DQN(parser.args).target_net
     else:
-        if args.model == "lr":
+        if parser.args.model == "lr":
             from fedscale.utils.models.simple.models import LogisticRegression
             model = LogisticRegression(
-                args.input_dim, outputClass[args.data_set])
-        elif args.model == 'svm':
+                parser.args.input_dim, outputClass[parser.args.data_set])
+        elif parser.args.model == 'svm':
             from fedscale.utils.models.simple.models import LinearSVM
-            model = LinearSVM(args.input_dim, outputClass[args.data_set])
+            model = LinearSVM(parser.args.input_dim, outputClass[parser.args.data_set])
+        elif parser.args.model_zoo == "fedscale-tensorflow-zoo":
+            assert parser.args.engine == commons.TENSORFLOW
+            model = get_tensorflow_model(parser.args.model, parser.args)
         else:
-            if args.model_zoo == "fedscale-zoo":
-                if args.task == "cv":
-                    model = get_cv_model()
+            if parser.args.model_zoo == "fedscale-torch-zoo":
+                if parser.args.task == "cv":
+                    model = get_cv_model(name=parser.args.model,
+                                         num_classes=outputClass[parser.args.data_set])
                 else:
-                    raise NameError(f"Model zoo {args.model_zoo} does not exist")
-            elif args.model_zoo == "torchcv":
-                model = tormodels.__dict__[args.model](
-                    num_classes=outputClass[args.data_set])
+                    raise NameError(f"Model zoo {parser.args.model_zoo} does not exist")
+            elif parser.args.model_zoo == "torchcv":
+                model = tormodels.__dict__[parser.args.model](
+                    num_classes=outputClass[parser.args.data_set])
             else:
-                raise NameError(f"Model zoo {args.model_zoo} does not exist")
+                raise NameError(f"Model zoo {parser.args.model_zoo} does not exist")
     return model
 
 
 def init_dataset():
+    import_libs()
 
-    if args.task == "detection":
-        if not os.path.exists(args.data_cache):
+    if parser.args.task == "detection":
+        if not os.path.exists(parser.args.data_cache):
             imdb_name = "voc_2007_trainval"
             imdbval_name = "voc_2007_test"
             imdb, roidb, ratio_list, ratio_index = combined_roidb(
-                imdb_name, ['DATA_DIR', args.data_dir], sizes=args.train_size_file)
+                imdb_name, ['DATA_DIR', parser.args.data_dir], sizes=parser.args.train_size_file)
             train_dataset = roibatchLoader(
-                roidb, ratio_list, ratio_index, args.batch_size, imdb.num_classes, imdb._image_index_temp,  training=True)
+                roidb, ratio_list, ratio_index, parser.args.batch_size, imdb.num_classes, imdb._image_index_temp,
+                training=True)
             imdb_, roidb_, ratio_list_, ratio_index_ = combined_roidb(
-                imdbval_name, ['DATA_DIR', args.data_dir], sizes=args.test_size_file, training=False)
+                imdbval_name, ['DATA_DIR', parser.args.data_dir], sizes=parser.args.test_size_file, training=False)
             imdb_.competition_mode(on=True)
             test_dataset = roibatchLoader(roidb_, ratio_list_, ratio_index_, 1,
                                           imdb_.num_classes, imdb_._image_index_temp, training=False, normalize=False)
-            with open(args.data_cache, 'wb') as f:
+            with open(parser.args.data_cache, 'wb') as f:
                 pickle.dump(train_dataset, f, -1)
                 pickle.dump(test_dataset, f, -1)
         else:
-            with open(args.data_cache, 'rb') as f:
+            with open(parser.args.data_cache, 'rb') as f:
                 train_dataset = pickle.load(f)
                 test_dataset = pickle.load(f)
-    elif args.task == "rl":
-        train_dataset = test_dataset = RLData(args)
+    elif parser.args.task == "rl":
+        train_dataset = test_dataset = RLData(parser.args)
     else:
 
-        if args.data_set == 'Mnist':
+        if parser.args.data_set == 'Mnist':
             train_transform, test_transform = get_data_transform('mnist')
 
-            train_dataset = datasets.MNIST(args.data_dir, train=True, download=True,
+            train_dataset = datasets.MNIST(parser.args.data_dir, train=True, download=True,
                                            transform=train_transform)
-            test_dataset = datasets.MNIST(args.data_dir, train=False, download=True,
+            test_dataset = datasets.MNIST(parser.args.data_dir, train=False, download=True,
                                           transform=test_transform)
 
-        elif args.data_set == 'cifar10':
+        elif parser.args.data_set == 'cifar10':
             train_transform, test_transform = get_data_transform('cifar')
-            train_dataset = datasets.CIFAR10(args.data_dir, train=True, download=True,
+            train_dataset = datasets.CIFAR10(parser.args.data_dir, train=True, download=True,
                                              transform=train_transform)
-            test_dataset = datasets.CIFAR10(args.data_dir, train=False, download=True,
+            test_dataset = datasets.CIFAR10(parser.args.data_dir, train=False, download=True,
                                             transform=test_transform)
 
-        elif args.data_set == "imagenet":
+        elif parser.args.data_set == "imagenet":
             train_transform, test_transform = get_data_transform('imagenet')
             train_dataset = datasets.ImageNet(
-                args.data_dir, split='train', download=False, transform=train_transform)
+                parser.args.data_dir, split='train', download=False, transform=train_transform)
             test_dataset = datasets.ImageNet(
-                args.data_dir, split='val', download=False, transform=test_transform)
+                parser.args.data_dir, split='val', download=False, transform=test_transform)
 
-        elif args.data_set == 'emnist':
+        elif parser.args.data_set == 'emnist':
             test_dataset = datasets.EMNIST(
-                args.data_dir, split='balanced', train=False, download=True, transform=transforms.ToTensor())
+                parser.args.data_dir, split='balanced', train=False, download=True, transform=transforms.ToTensor())
             train_dataset = datasets.EMNIST(
-                args.data_dir, split='balanced', train=True, download=True, transform=transforms.ToTensor())
+                parser.args.data_dir, split='balanced', train=True, download=True, transform=transforms.ToTensor())
 
-        elif args.data_set == 'femnist':
+        elif parser.args.data_set == 'femnist':
             from fedscale.dataloaders.femnist import FEMNIST
 
             train_transform, test_transform = get_data_transform('mnist')
             train_dataset = FEMNIST(
-                args.data_dir, dataset='train', transform=train_transform)
+                parser.args.data_dir, dataset='train', transform=train_transform)
             test_dataset = FEMNIST(
-                args.data_dir, dataset='test', transform=test_transform)
+                parser.args.data_dir, dataset='test', transform=test_transform)
 
-        elif args.data_set == 'openImg':
+        elif parser.args.data_set == 'openImg':
             from fedscale.dataloaders.openimage import OpenImage
 
             train_transform, test_transform = get_data_transform('openImg')
             train_dataset = OpenImage(
-                args.data_dir, dataset='train', transform=train_transform)
+                parser.args.data_dir, dataset='train', transform=train_transform)
             test_dataset = OpenImage(
-                args.data_dir, dataset='test', transform=test_transform)
+                parser.args.data_dir, dataset='test', transform=test_transform)
 
-        elif args.data_set == 'blog':
+        elif parser.args.data_set == 'blog':
             train_dataset = load_and_cache_examples(
-                args, tokenizer, evaluate=False)
+                parser.args, tokenizer, evaluate=False)
             test_dataset = load_and_cache_examples(
-                args, tokenizer, evaluate=True)
+                parser.args, tokenizer, evaluate=True)
 
-        elif args.data_set == 'stackoverflow':
+        elif parser.args.data_set == 'stackoverflow':
             from fedscale.dataloaders.stackoverflow import stackoverflow
 
-            train_dataset = stackoverflow(args.data_dir, train=True)
-            test_dataset = stackoverflow(args.data_dir, train=False)
+            train_dataset = stackoverflow(parser.args.data_dir, train=True)
+            test_dataset = stackoverflow(parser.args.data_dir, train=False)
 
-        elif args.data_set == 'amazon':
-            if args.model == 'albert':
+        elif parser.args.data_set == 'amazon':
+            if parser.args.model == 'albert':
                 import fedscale.dataloaders.amazon as fl_loader
                 train_dataset = fl_loader.AmazonReview_loader(
-                    args.data_dir, train=True, tokenizer=tokenizer, max_len=args.clf_block_size)
+                    parser.args.data_dir, train=True, tokenizer=tokenizer, max_len=parser.args.clf_block_size)
                 test_dataset = fl_loader.AmazonReview_loader(
-                    args.data_dir, train=False, tokenizer=tokenizer, max_len=args.clf_block_size)
+                    parser.args.data_dir, train=False, tokenizer=tokenizer, max_len=parser.args.clf_block_size)
 
-            elif args.model == 'lr':
+            elif parser.args.model == 'lr':
                 import fedscale.dataloaders.word2vec as fl_loader
                 train_dataset = fl_loader.AmazonReview_word2vec(
-                    args.data_dir, args.embedding_file, train=True)
+                    parser.args.data_dir, parser.args.embedding_file, train=True)
                 test_dataset = fl_loader.AmazonReview_word2vec(
-                    args.data_dir, args.embedding_file, train=False)
+                    parser.args.data_dir, parser.args.embedding_file, train=False)
 
-        elif args.data_set == 'yelp':
+        elif parser.args.data_set == 'yelp':
             import fedscale.dataloaders.yelp as fl_loader
 
             train_dataset = fl_loader.TextSentimentDataset(
-                args.data_dir, train=True, tokenizer=tokenizer, max_len=args.clf_block_size)
+                parser.args.data_dir, train=True, tokenizer=tokenizer, max_len=parser.args.clf_block_size)
             test_dataset = fl_loader.TextSentimentDataset(
-                args.data_dir, train=False, tokenizer=tokenizer, max_len=args.clf_block_size)
+                parser.args.data_dir, train=False, tokenizer=tokenizer, max_len=parser.args.clf_block_size)
 
-        elif args.data_set == 'google_speech':
+        elif parser.args.data_set == 'google_speech':
             bkg = '_background_noise_'
             data_aug_transform = transforms.Compose(
-                [ChangeAmplitude(), ChangeSpeedAndPitchAudio(), FixAudioLength(), ToSTFT(), StretchAudioOnSTFT(), TimeshiftAudioOnSTFT(), FixSTFTDimension()])
+                [ChangeAmplitude(), ChangeSpeedAndPitchAudio(), FixAudioLength(), ToSTFT(), StretchAudioOnSTFT(),
+                 TimeshiftAudioOnSTFT(), FixSTFTDimension()])
             bg_dataset = BackgroundNoiseDataset(
-                os.path.join(args.data_dir, bkg), data_aug_transform)
+                os.path.join(parser.args.data_dir, bkg), data_aug_transform)
             add_bg_noise = AddBackgroundNoiseOnSTFT(bg_dataset)
             train_feature_transform = transforms.Compose([ToMelSpectrogramFromSTFT(
                 n_mels=32), DeleteSTFT(), ToTensor('mel_spectrogram', 'input')])
-            train_dataset = SPEECH(args.data_dir, dataset='train',
+            train_dataset = SPEECH(parser.args.data_dir, dataset='train',
                                    transform=transforms.Compose([LoadAudio(),
                                                                  data_aug_transform,
                                                                  add_bg_noise,
                                                                  train_feature_transform]))
             valid_feature_transform = transforms.Compose(
                 [ToMelSpectrogram(n_mels=32), ToTensor('mel_spectrogram', 'input')])
-            test_dataset = SPEECH(args.data_dir, dataset='test',
+            test_dataset = SPEECH(parser.args.data_dir, dataset='test',
                                   transform=transforms.Compose([LoadAudio(),
                                                                 FixAudioLength(),
                                                                 valid_feature_transform]))
-        elif args.data_set == 'common_voice':
+        elif parser.args.data_set == 'common_voice':
             from fedscale.dataloaders.voice_data_loader import \
                 SpectrogramDataset
             train_dataset = SpectrogramDataset(audio_conf=model.audio_conf,
-                                               data_dir=args.data_dir,
+                                               data_dir=parser.args.data_dir,
                                                labels=model.labels,
                                                train=True,
                                                normalize=True,
-                                               speed_volume_perturb=args.speed_volume_perturb,
-                                               spec_augment=args.spec_augment,
-                                               data_mapfile=args.data_mapfile)
+                                               speed_volume_perturb=parser.args.speed_volume_perturb,
+                                               spec_augment=parser.args.spec_augment,
+                                               data_mapfile=parser.args.data_mapfile)
             test_dataset = SpectrogramDataset(audio_conf=model.audio_conf,
-                                              data_dir=args.data_dir,
+                                              data_dir=parser.args.data_dir,
                                               labels=model.labels,
                                               train=False,
                                               normalize=True,
                                               speed_volume_perturb=False,
                                               spec_augment=False)
         else:
             logging.info('DataSet must be {}!'.format(
```

### Comparing `fedscale-0.5/fedscale/core/logger/execution.py` & `fedscale-1.0/fedscale/cloud/logger/executor_logging.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# package for client
-import os
+from fedscale.cloud.fllibs import *
+import fedscale.cloud.config_parser as parser
 
-from fedscale.core.fllibs import *
-
-logDir = os.path.join(args.log_path, "logs", args.job_name,
-                      args.time_stamp, 'executor')
-logFile = os.path.join(logDir, 'log')
+logDir = None
 
 
 def init_logging():
+    global logDir
+
+    logDir = os.path.join(parser.args.log_path, "logs", parser.args.job_name,
+                          parser.args.time_stamp, 'executor')
+    logFile = os.path.join(logDir, 'log')
     if not os.path.isdir(logDir):
         os.makedirs(logDir, exist_ok=True)
 
     logging.basicConfig(
         format='%(asctime)s %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s',
         datefmt='(%m-%d) %H:%M:%S',
         level=logging.INFO,
@@ -20,11 +21,7 @@
             logging.FileHandler(logFile, mode='a'),
             logging.StreamHandler()
         ])
 
 
 def initiate_client_setting():
     init_logging()
-
-
-# initiate the log path, and executor ips
-initiate_client_setting()
```

### Comparing `fedscale-0.5/fedscale/core/resource_manager.py` & `fedscale-1.0/fedscale/cloud/resource_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import threading
 
-from fedscale.core import commons
+from fedscale.cloud import commons
 
 
 class ResourceManager(object):
     """Schedule training tasks across GPUs/CPUs"""
 
     def __init__(self, experiment_mode):
 
@@ -14,14 +14,25 @@
         self.update_lock = threading.Lock()
 
     def register_tasks(self, clientsToRun):
         # TODO: append new checkin client
         self.client_run_queue = clientsToRun.copy()
         self.client_run_queue_idx = 0
 
+    def get_task_length(self) -> int:
+        """Number of tasks left in the queue
+
+        Returns:
+            int: Number of tasks left in the queue
+        """
+        self.update_lock.acquire()
+        remaining_task_num: int = len(self.client_run_queue) - self.client_run_queue_idx
+        self.update_lock.release()
+        return remaining_task_num
+
     def remove_client_task(self, client_id):
         assert(client_id in self.client_run_queue,
                f"client task {client_id} is not in task queue")
         pass
 
     def has_next_task(self, client_id=None):
         # TODO: always has next task
```

### Comparing `fedscale-0.5/fedscale/dataloaders/amazon.py` & `fedscale-1.0/fedscale/dataloaders/amazon.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/decoder.py` & `fedscale-1.0/fedscale/dataloaders/decoder.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/divide_data.py` & `fedscale-1.0/fedscale/dataloaders/divide_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         self.data = data
         self.labels = self.data.targets
         self.args = args
         self.isTest = isTest
         np.random.seed(seed)
 
         self.data_len = len(self.data)
-        self.task = args.task
         self.numOfLabels = numOfClass
         self.client_label_cnt = defaultdict(set)
 
     def getNumOfLabels(self):
         return self.numOfLabels
 
     def getDataLen(self):
@@ -58,42 +57,42 @@
     def getClientLabel(self):
         return [len(self.client_label_cnt[i]) for i in range(self.getClientLen())]
 
     def trace_partition(self, data_map_file):
         """Read data mapping from data_map_file. Format: <client_id, sample_name, sample_category, category_id>"""
         logging.info(f"Partitioning data by profile {data_map_file}...")
 
-        clientId_maps = {}
-        unique_clientIds = {}
+        client_id_maps = {}
+        unique_client_ids = {}
         # load meta data from the data_map_file
         with open(data_map_file) as csv_file:
             csv_reader = csv.reader(csv_file, delimiter=',')
             read_first = True
             sample_id = 0
 
             for row in csv_reader:
                 if read_first:
                     logging.info(f'Trace names are {", ".join(row)}')
                     read_first = False
                 else:
                     client_id = row[0]
 
-                    if client_id not in unique_clientIds:
-                        unique_clientIds[client_id] = len(unique_clientIds)
+                    if client_id not in unique_client_ids:
+                        unique_client_ids[client_id] = len(unique_client_ids)
 
-                    clientId_maps[sample_id] = unique_clientIds[client_id]
-                    self.client_label_cnt[unique_clientIds[client_id]].add(
+                    client_id_maps[sample_id] = unique_client_ids[client_id]
+                    self.client_label_cnt[unique_client_ids[client_id]].add(
                         row[-1])
                     sample_id += 1
 
         # Partition data given mapping
-        self.partitions = [[] for _ in range(len(unique_clientIds))]
+        self.partitions = [[] for _ in range(len(unique_client_ids))]
 
         for idx in range(sample_id):
-            self.partitions[clientId_maps[idx]].append(idx)
+            self.partitions[client_id_maps[idx]].append(idx)
 
     def partition_data_helper(self, num_clients, data_map_file=None):
 
         # read mapping file to partition trace
         if data_map_file is not None:
             self.trace_partition(data_map_file)
         else:
@@ -110,15 +109,15 @@
 
         for _ in range(num_clients):
             part_len = int(1./num_clients * data_len)
             self.partitions.append(indexes[0:part_len])
             indexes = indexes[part_len:]
 
     def use(self, partition, istest):
-        resultIndex = self.partitions[partition]
+        resultIndex = self.partitions[partition % len(self.partitions)]
 
         exeuteLength = len(resultIndex) if not istest else int(
             len(resultIndex) * self.args.test_ratio)
         resultIndex = resultIndex[:exeuteLength]
         self.rng.shuffle(resultIndex)
 
         return Partition(self.data, resultIndex)
@@ -128,15 +127,18 @@
         return {'size': [len(partition) for partition in self.partitions]}
 
 
 def select_dataset(rank, partition, batch_size, args, isTest=False, collate_fn=None):
     """Load data given client Id"""
     partition = partition.use(rank - 1, isTest)
     dropLast = False if isTest else True
-    num_loaders = min(int(len(partition)/args.batch_size/2), args.num_loaders)
+    if isTest:
+        num_loaders = 0
+    else:
+        num_loaders = min(int(len(partition)/args.batch_size/2), args.num_loaders)
     if num_loaders == 0:
         time_out = 0
     else:
         time_out = 60
 
     if collate_fn is not None:
         return DataLoader(partition, batch_size=batch_size, shuffle=True, pin_memory=True, timeout=time_out, num_workers=num_loaders, drop_last=dropLast, collate_fn=collate_fn)
```

### Comparing `fedscale-0.5/fedscale/dataloaders/dqn.py` & `fedscale-1.0/fedscale/dataloaders/dqn.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/femnist.py` & `fedscale-1.0/fedscale/dataloaders/femnist.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/inaturalist.py` & `fedscale-1.0/fedscale/dataloaders/inaturalist.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/nlp.py` & `fedscale-1.0/fedscale/dataloaders/nlp.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/openimage.py` & `fedscale-1.0/fedscale/dataloaders/openimage.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/reddit.py` & `fedscale-1.0/fedscale/dataloaders/reddit.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,42 +151,42 @@
             count = 0
             clientCount = 0
             start_time = time.time()
 
             for client_data in client_data_list:
                 client_list = client_data['users']
 
-                for clientId, client in enumerate(client_list):
+                for client_id, client in enumerate(client_list):
                     tokens_list = list(client_data['user_data'][client]['x'])
 
                     for tokens in tokens_list:
 
                         tokens_list = [vocab_tokens_dict[s] for s in (
                             tokens.split()) if s in vocab_tokens_dict]
                         if not tokens_list:
                             continue
 
-                        mapping_dict[count] = clientId
+                        mapping_dict[count] = client_id
                         text.append(tokens_list)
 
                         count += 1
 
                     clientCount += 1
 
                     # num_of_remains = 1628176 - int(client)
                     #print("====In loading data, remains {} clients, may take {} sec".format(num_of_remains, (time.time() - start_time)/clientCount * num_of_remains))
                     # logging.info("====In loading  data, remains {} clients".format(num_of_remains)
 
-                    if clientId % 5000 == 0:
+                    if client_id % 5000 == 0:
                         # dump the cache
                         with open(cache_path, 'wb') as fout:
                             pickle.dump(text, fout)
                             pickle.dump(mapping_dict, fout)
 
-                        print("====Dump for {} clients".format(clientId))
+                        print("====Dump for {} clients".format(client_id))
 
             # dump the cache
             with open(cache_path, 'wb') as fout:
                 pickle.dump(text, fout)
                 pickle.dump(mapping_dict, fout)
 
         return text, mapping_dict
```

### Comparing `fedscale-0.5/fedscale/dataloaders/sparse_image_warp.py` & `fedscale-1.0/fedscale/dataloaders/sparse_image_warp.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/spec_augment.py` & `fedscale-1.0/fedscale/dataloaders/spec_augment.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/speech.py` & `fedscale-1.0/fedscale/dataloaders/speech.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/stackoverflow.py` & `fedscale-1.0/fedscale/dataloaders/stackoverflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
             print(self.train)
 
             count = 0
             clientCount = 0
             client_list = list(train_file['examples'])
             start_time = time.time()
 
-            for clientId, client in enumerate(client_list):
+            for client_id, client in enumerate(client_list):
                 tags_list = list(train_file['examples'][client]['tags'])
                 tokens_list = list(train_file['examples'][client]['tokens'])
                 title_list = list(train_file['examples'][client]['title'])
 
                 for tags, tokens, title in zip(tags_list, tokens_list, title_list):
                     tags_list = [vocab_tags_dict[s] for s in tags.decode(
                         "utf-8").split('|') if s in vocab_tags_dict]
@@ -211,34 +211,34 @@
                         continue
 
                     tokens_list = [vocab_tokens_dict[s] for s in (tokens.decode(
                         "utf-8").split()+title.decode("utf-8").split()) if s in vocab_tokens_dict]
                     if not tokens_list:
                         continue
 
-                    mapping_dict[count] = clientId
+                    mapping_dict[count] = client_id
                     text.append(tokens_list)
                     target_tags.append(tags_list)
 
                     count += 1
 
                 clientCount += 1
 
-                num_of_remains = len(client_list) - clientId
+                num_of_remains = len(client_list) - client_id
                 #print("====In loading data, remains {} clients, may take {} sec".format(num_of_remains, (time.time() - start_time)/clientCount * num_of_remains))
                 # logging.info("====In loading  data, remains {} clients".format(num_of_remains)
 
-                if clientId % 5000 == 0:
+                if client_id % 5000 == 0:
                     # dump the cache
                     with open(cache_path, 'wb') as fout:
                         pickle.dump(text, fout)
                         pickle.dump(target_tags, fout)
                         pickle.dump(mapping_dict, fout)
 
-                    #print("====Dump for {} clients".format(clientId))
+                    #print("====Dump for {} clients".format(client_id))
 
             # dump the cache
             with open(cache_path, 'wb') as fout:
                 pickle.dump(text, fout)
                 pickle.dump(target_tags, fout)
                 pickle.dump(mapping_dict, fout)
```

### Comparing `fedscale-0.5/fedscale/dataloaders/transforms_stft.py` & `fedscale-1.0/fedscale/dataloaders/transforms_stft.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/transforms_wav.py` & `fedscale-1.0/fedscale/dataloaders/transforms_wav.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/utils_data.py` & `fedscale-1.0/fedscale/dataloaders/utils_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # -*- coding: utf-8 -*-
 
 import sys
-
 from torchvision import transforms
 
-
 def get_data_transform(data: str):
     if data == 'mnist':
         train_transform = transforms.Compose([
             # transforms.Grayscale(num_output_channels=1),
-            transforms.Resize((28, 28)),
+            transforms.Resize((32, 32)),
             transforms.RandomHorizontalFlip(),
             transforms.ToTensor(),
             transforms.Normalize((0.1307,), (0.3081,))
         ])
 
         test_transform = transforms.Compose([
             # transforms.Grayscale(num_output_channels=1),
-            transforms.Resize((28, 28)),
+            transforms.Resize((32, 32)),
             transforms.RandomHorizontalFlip(),
             transforms.ToTensor(),
             transforms.Normalize((0.1307,), (0.3081,))
         ])
 
     elif data == 'cifar':
         train_transform = transforms.Compose([
@@ -153,8 +151,8 @@
             # transforms.Normalize((0.4914, 0.4822, 0.4465), (0.2023, 0.1994, 0.2010)),
             transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5)),
         ])
     else:
         print('Data must be {} or {} !'.format('mnist', 'cifar'))
         sys.exit(-1)
 
-    return train_transform, test_transform
+    return train_transform, test_transform
```

### Comparing `fedscale-0.5/fedscale/dataloaders/voice_data_loader.py` & `fedscale-1.0/fedscale/dataloaders/voice_data_loader.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/word2vec.py` & `fedscale-1.0/fedscale/dataloaders/word2vec.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/dataloaders/yelp.py` & `fedscale-1.0/fedscale/dataloaders/yelp.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/model_test_module.py` & `fedscale-1.0/fedscale/utils/model_test_module.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,30 +4,32 @@
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from torch.autograd import Variable
 
 # libs from fedscale
-from fedscale.core.config_parser import args
+import fedscale.cloud.config_parser as parser
 from fedscale.dataloaders.nlp import mask_tokens
 
-if args.task == "detection":
+if parser.args.task == "detection":
     import numpy as np
     import torch.nn as nn
     import torch.optim as optim
     from torch.autograd import Variable
 
     from fedscale.dataloaders.rcnn.lib.datasets.pascal_voc import readClass
     from fedscale.dataloaders.rcnn.lib.model.roi_layers import nms
     from fedscale.dataloaders.rcnn.lib.model.rpn.bbox_transform import (
         bbox_transform_inv, clip_boxes)
     from fedscale.dataloaders.rcnn.lib.model.utils.config import cfg
     from fedscale.dataloaders.rcnn.lib.roi_data_layer.roidb import \
         combined_roidb
+elif parser.args.task == 'voice':
+    from fedscale.dataloaders.decoder import GreedyDecoder
 
 
 def cal_accuracy(targets, outputs):
     temp_acc = 0
     temp_all_or_false = 0
 
     temp_len = 0
@@ -46,15 +48,15 @@
         temp_len += len(sample)
 
     temp_all_or_false = (temp_all_or_false/float(len(targets)) * temp_len)
 
     return temp_acc, temp_all_or_false, temp_len
 
 
-def test_model(rank, model, test_data, device='cpu', criterion=nn.NLLLoss(), tokenizer=None):
+def test_pytorch_model(rank, model, test_data, device='cpu', criterion=nn.NLLLoss(), tokenizer=None):
 
     test_loss = 0
     correct = 0
     top_5 = 0
 
     correct2 = 0
     test_len = 0
@@ -65,26 +67,26 @@
     model = model.to(device=device)  # load by pickle
     model.eval()
     targets_list = []
     preds = []
 
     decoder = None
 
-    if args.task == 'voice':
+    if parser.args.task == 'voice':
         decoder = GreedyDecoder(
             model.labels, blank_index=model.labels.index('_'))
 
     with torch.no_grad():
 
-        if args.task == 'detection':
+        if parser.args.task == 'detection':
             imdb, _, _, _ = combined_roidb(
-                "voc_2007_test", ['DATA_DIR', args.data_dir], server=True)
+                "voc_2007_test", ['DATA_DIR', parser.args.data_dir], server=True)
             data_iter = iter(test_data)
             num_images = len(test_data.dataset)
-            num_classes = len(readClass(args.data_dir + "/class.txt"))
+            num_classes = len(readClass(parser.args.data_dir + "/class.txt"))
 
             all_boxes = [[[] for _ in range(num_images)]
                          for _ in range(num_classes)]
             max_per_image = 100
             thresh = 0.0
             empty_array = np.transpose(np.array([[], [], [], [], []]), (1, 0))
             for i in range(num_images):
@@ -152,44 +154,44 @@
                         image_thresh = np.sort(image_scores)[-max_per_image]
                         for j in range(1, num_classes):
                             keep = np.where(
                                 all_boxes[j][i][:, -1] >= image_thresh)[0]
                             all_boxes[j][i] = all_boxes[j][i][keep, :]
 
                 imdb._reset_index(test_data.dataset.index)
-                output_dir = args.test_output_dir + \
-                    "/learner/" + str(args.this_rank)
+                output_dir = parser.args.test_output_dir + \
+                    "/learner/" + str(parser.args.this_rank)
                 _, mean_ap = imdb.evaluate_detections(
-                    all_boxes, output_dir, args.this_rank)
+                    all_boxes, output_dir, parser.args.this_rank)
                 return 0, mean_ap, mean_ap, {'top_1': mean_ap, 'top_5': mean_ap, 'test_loss': 0, 'test_len': num_images}
 
         for data, target in test_data:
             try:
-                if args.task == 'nlp':
+                if parser.args.task == 'nlp':
 
-                    # if args.mlm else (data, data)
+                    # if parser.args.mlm else (data, data)
                     data, target = mask_tokens(
-                        data, tokenizer, args, device=device)
+                        data, tokenizer, parser.args, device=device)
                     data, target = Variable(data).to(
                         device=device), Variable(target).to(device=device)
 
-                    # if args.mlm else model(data, labels=target)
+                    # if parser.args.mlm else model(data, labels=target)
                     outputs = model(data, labels=target)
 
                     loss = outputs[0]
                     test_loss += loss.data.item()
                     perplexity_loss += loss.data.item()
 
                     acc = accuracy(
                         outputs[1].reshape(-1, outputs[1].shape[2]), target.reshape(-1), topk=(1, 5))
 
                     correct += acc[0].item()
                     top_5 += acc[1].item()
 
-                elif args.task == 'tag':
+                elif parser.args.task == 'tag':
                     data, target = Variable(data).to(
                         device=device), Variable(target).to(device=device)
                     output = model(data)
                     loss = criterion(output, target)
 
                     # we have to scan the sample one by one
                     for idx, sample in enumerate(output):
@@ -197,29 +199,29 @@
                             target[idx]).flatten().cpu().numpy().tolist()
                         maxk = len(target_index)
                         preds += [sample.topk(maxk)[1].cpu().numpy().tolist()]
                         targets_list += [target_index]
 
                     test_loss += loss.data.item()
 
-                elif args.task == 'speech':
+                elif parser.args.task == 'speech':
                     data, target = Variable(data).to(
                         device=device), Variable(target).to(device=device)
                     data = torch.unsqueeze(data, 1)
 
                     output = model(data)
                     loss = criterion(output, target)
 
                     test_loss += loss.data.item()  # Variable.data
                     acc = accuracy(output, target, topk=(1, 5))
 
                     correct += acc[0].item()
                     top_5 += acc[1].item()
 
-                elif args.task == 'text_clf' and args.model == 'albert-base-v2':
+                elif parser.args.task == 'text_clf' and parser.args.model == 'albert-base-v2':
                     (inputs, masks) = data
                     (inputs, masks, target) = (Variable(inputs).to(device=device),
                                                Variable(masks).to(device=device), Variable(target).to(device=device))
                     outputs = model(inputs, token_type_ids=None,
                                     attention_mask=masks, labels=target)
 
                     loss = outputs.loss
@@ -227,15 +229,15 @@
 
                     test_loss += loss.item()  # Variable.data
                     acc = accuracy(output, target, topk=(1, 2))
 
                     correct += acc[0].item()
                     top_5 += acc[1].item()
 
-                elif args.task == 'voice':
+                elif parser.args.task == 'voice':
                     (inputs, target, input_percentages, target_sizes) = data
 
                     input_sizes = input_percentages.mul_(
                         int(inputs.size(3))).int()
                     inputs = Variable(inputs).to(device=device)
 
                     # unflatten targets
@@ -278,15 +280,15 @@
                     top_5 += acc[1].item()
 
             except Exception as ex:
                 logging.info(f"Testing of failed as {ex}")
                 break
             test_len += len(target)
 
-    if args.task == 'voice':
+    if parser.args.task == 'voice':
         correct,  top_5, test_len = float(
             total_wer), float(total_cer), float(num_tokens)
 
     test_len = max(test_len, 1)
     # loss function averages over batch size
     test_loss /= len(test_data)
     perplexity_loss /= len(test_data)
@@ -294,15 +296,15 @@
     sum_loss = test_loss * test_len
 
     # in NLP, we care about the perplexity of the model
     acc = round(correct / test_len, 4)
     acc_5 = round(top_5 / test_len, 4)
     test_loss = round(test_loss, 4)
 
-    if args.task == 'tag':
+    if parser.args.task == 'tag':
         # precision, recall, f1, sup = precision_recall_fscore_support(targets_list, preds, average='samples')
         top_5, correct, test_len = cal_accuracy(targets_list, preds)
 
     logging.info('Rank {}: Test set: Average loss: {}, Top-1 Accuracy: {}/{} ({}), Top-5 Accuracy: {}'
                  .format(rank, test_loss, correct, len(test_data.dataset), acc, acc_5))
 
     testRes = {'top_1': correct, 'top_5': top_5,
```

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/airnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/airnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/airnext.py` & `fedscale-1.0/fedscale/utils/models/cv_models/airnext.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/alexnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/alexnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/alphapose_coco.py` & `fedscale-1.0/fedscale/utils/models/cv_models/alphapose_coco.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/bagnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/bagnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/bamresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/bamresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/bisenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/bisenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/bninception.py` & `fedscale-1.0/fedscale/utils/models/cv_models/bninception.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/cbamresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/cbamresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/centernet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/centernet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/cgnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/cgnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/channelnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/channelnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/common.py` & `fedscale-1.0/fedscale/utils/models/cv_models/common.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/condensenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/condensenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/contextnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/contextnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/dabnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/dabnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/danet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/danet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/darknet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/darknet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/darknet53.py` & `fedscale-1.0/fedscale/utils/models/cv_models/darknet53.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/darts.py` & `fedscale-1.0/fedscale/utils/models/cv_models/darts.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/deeplabv3.py` & `fedscale-1.0/fedscale/utils/models/cv_models/deeplabv3.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/densenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/densenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/densenet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/densenet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/diapreresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/diapreresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/diapreresnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/diapreresnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/diaresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/diaresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/diaresnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/diaresnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/dicenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/dicenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/diracnetv2.py` & `fedscale-1.0/fedscale/utils/models/cv_models/diracnetv2.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/dla.py` & `fedscale-1.0/fedscale/utils/models/cv_models/dla.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/dpn.py` & `fedscale-1.0/fedscale/utils/models/cv_models/dpn.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/drn.py` & `fedscale-1.0/fedscale/utils/models/cv_models/drn.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/edanet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/edanet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/efficientnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/efficientnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/efficientnetedge.py` & `fedscale-1.0/fedscale/utils/models/cv_models/efficientnetedge.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/enet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/enet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/erfnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/erfnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/esnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/esnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/espcnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/espcnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/espnetv2.py` & `fedscale-1.0/fedscale/utils/models/cv_models/espnetv2.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/fastscnn.py` & `fedscale-1.0/fedscale/utils/models/cv_models/fastscnn.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/fastseresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/fastseresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/fbnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/fbnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/fcn8sd.py` & `fedscale-1.0/fedscale/utils/models/cv_models/fcn8sd.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/fdmobilenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/fdmobilenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/fishnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/fishnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/fpenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/fpenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/fractalnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/fractalnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/ghostnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/ghostnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/hardnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/hardnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/hrnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/hrnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/ibnbresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/ibnbresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/ibndensenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/ibndensenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/ibnresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/ibnresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/ibnresnext.py` & `fedscale-1.0/fedscale/utils/models/cv_models/ibnresnext.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/ibppose_coco.py` & `fedscale-1.0/fedscale/utils/models/cv_models/ibppose_coco.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/icnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/icnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/igcv3.py` & `fedscale-1.0/fedscale/utils/models/cv_models/igcv3.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/inceptionresnetv1.py` & `fedscale-1.0/fedscale/utils/models/cv_models/inceptionresnetv1.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/inceptionresnetv2.py` & `fedscale-1.0/fedscale/utils/models/cv_models/inceptionresnetv2.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/inceptionv3.py` & `fedscale-1.0/fedscale/utils/models/cv_models/inceptionv3.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/inceptionv4.py` & `fedscale-1.0/fedscale/utils/models/cv_models/inceptionv4.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/irevnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/irevnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/isqrtcovresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/isqrtcovresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/jasper.py` & `fedscale-1.0/fedscale/utils/models/cv_models/jasper.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/jasperdr.py` & `fedscale-1.0/fedscale/utils/models/cv_models/jasperdr.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/lednet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/lednet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/lffd.py` & `fedscale-1.0/fedscale/utils/models/cv_models/lffd.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/linknet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/linknet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/lwopenpose_cmupan.py` & `fedscale-1.0/fedscale/utils/models/cv_models/lwopenpose_cmupan.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/menet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/menet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/mixnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/mixnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/mnasnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/mnasnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/mobilenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/mobilenet_cub.py` & `fedscale-1.0/fedscale/utils/models/cv_models/mobilenet_cub.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/mobilenetb.py` & `fedscale-1.0/fedscale/utils/models/cv_models/mobilenetb.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/mobilenetv2.py` & `fedscale-1.0/fedscale/utils/models/cv_models/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/mobilenetv3.py` & `fedscale-1.0/fedscale/utils/models/cv_models/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/model_store.py` & `fedscale-1.0/fedscale/utils/models/cv_models/model_store.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/msdnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/msdnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/msdnet_cifar10.py` & `fedscale-1.0/fedscale/utils/models/cv_models/msdnet_cifar10.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/nasnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/nasnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/nin_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/nin_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/ntsnet_cub.py` & `fedscale-1.0/fedscale/utils/models/cv_models/ntsnet_cub.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/nvpattexp.py` & `fedscale-1.0/fedscale/utils/models/cv_models/nvpattexp.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/octresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/octresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/others/_espnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/others/_espnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/others/_inceptionresnetv1_.py` & `fedscale-1.0/fedscale/utils/models/cv_models/others/_inceptionresnetv1_.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/others/oth_espnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/others/oth_espnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/others/oth_inception_resnet_v1.py` & `fedscale-1.0/fedscale/utils/models/cv_models/others/oth_inception_resnet_v1.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/others/oth_quartznet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/others/oth_quartznet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/others/oth_vit.py` & `fedscale-1.0/fedscale/utils/models/cv_models/others/oth_vit.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/peleenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/peleenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/pfpcnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/pfpcnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/pnasnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/pnasnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/polynet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/polynet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/preresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/preresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/preresnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/preresnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/prnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/prnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/proxylessnas.py` & `fedscale-1.0/fedscale/utils/models/cv_models/proxylessnas.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/proxylessnas_cub.py` & `fedscale-1.0/fedscale/utils/models/cv_models/proxylessnas_cub.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/pspnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/pspnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/pyramidnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/pyramidnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/pyramidnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/pyramidnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/quartznet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/quartznet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/regnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/regnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resattnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resattnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resdropresnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resdropresnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resnesta.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resnesta.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resnet_cub.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resnet_cub.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resneta.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resneta.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resnetd.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resnetd.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resnext.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resnext.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/resnext_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/resnext_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/revnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/revnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/rir_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/rir_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/ror_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/ror_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/scnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/scnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/segnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/segnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/selecsls.py` & `fedscale-1.0/fedscale/utils/models/cv_models/selecsls.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/senet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/senet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/sepreresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/sepreresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/sepreresnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/sepreresnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/seresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/seresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/seresnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/seresnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/seresnet_cub.py` & `fedscale-1.0/fedscale/utils/models/cv_models/seresnet_cub.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/seresnext.py` & `fedscale-1.0/fedscale/utils/models/cv_models/seresnext.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/shakedropresnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/shakedropresnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/shakeshakeresnet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/shakeshakeresnet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/sharesnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/sharesnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/shufflenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/shufflenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/shufflenetv2.py` & `fedscale-1.0/fedscale/utils/models/cv_models/shufflenetv2.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/shufflenetv2b.py` & `fedscale-1.0/fedscale/utils/models/cv_models/shufflenetv2b.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/simplepose_coco.py` & `fedscale-1.0/fedscale/utils/models/cv_models/simplepose_coco.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/simpleposemobile_coco.py` & `fedscale-1.0/fedscale/utils/models/cv_models/simpleposemobile_coco.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/sinet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/sinet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/sknet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/sknet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/sparsenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/sparsenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/spnasnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/spnasnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/sqnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/sqnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/squeezenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/squeezenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/squeezenext.py` & `fedscale-1.0/fedscale/utils/models/cv_models/squeezenext.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/superpointnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/superpointnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/tresnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/tresnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/unet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/unet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/vgg.py` & `fedscale-1.0/fedscale/utils/models/cv_models/vgg.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/visemenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/visemenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/voca.py` & `fedscale-1.0/fedscale/utils/models/cv_models/voca.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/vovnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/vovnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/wrn.py` & `fedscale-1.0/fedscale/utils/models/cv_models/wrn.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/wrn1bit_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/wrn1bit_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/wrn_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/wrn_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/xception.py` & `fedscale-1.0/fedscale/utils/models/cv_models/xception.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/xdensenet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/xdensenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/xdensenet_cifar.py` & `fedscale-1.0/fedscale/utils/models/cv_models/xdensenet_cifar.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/cv_models/zfnet.py` & `fedscale-1.0/fedscale/utils/models/cv_models/zfnet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/model_provider.py` & `fedscale-1.0/fedscale/utils/models/torch_model_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1216,10 +1216,10 @@
     Returns:
     -------
     Module
         Resulted model.
     """
     name = name.lower()
     if name not in _models:
-        raise ValueError("Unsupported model: {}".format(name))
+        raise ValueError(f"Unsupported model: {name}")
     net = _models[name](**kwargs)
     return net
```

### Comparing `fedscale-0.5/fedscale/utils/models/simple/models.py` & `fedscale-1.0/fedscale/utils/models/simple/models.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/specialized/inception.py` & `fedscale-1.0/fedscale/utils/models/specialized/inception.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/specialized/mobilenet.py` & `fedscale-1.0/fedscale/utils/models/specialized/mobilenet.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/specialized/resnet_speech.py` & `fedscale-1.0/fedscale/utils/models/specialized/resnet_speech.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale/utils/models/specialized/voice_model.py` & `fedscale-1.0/fedscale/utils/models/specialized/voice_model.py`

 * *Files identical despite different names*

### Comparing `fedscale-0.5/fedscale.egg-info/SOURCES.txt` & `fedscale-1.0/fedscale.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,39 +2,49 @@
 setup.cfg
 setup.py
 fedscale/__init__.py
 fedscale.egg-info/PKG-INFO
 fedscale.egg-info/SOURCES.txt
 fedscale.egg-info/dependency_links.txt
 fedscale.egg-info/top_level.txt
-fedscale/core/__init__.py
-fedscale/core/client_manager.py
-fedscale/core/commons.py
-fedscale/core/config_parser.py
-fedscale/core/fllibs.py
-fedscale/core/resource_manager.py
-fedscale/core/aggregation/__init__.py
-fedscale/core/aggregation/aggregator.py
-fedscale/core/aggregation/optimizers.py
-fedscale/core/channels/__init__.py
-fedscale/core/channels/channel_context.py
-fedscale/core/channels/job_api_pb2.py
-fedscale/core/channels/job_api_pb2_grpc.py
-fedscale/core/execution/__init__.py
-fedscale/core/execution/client.py
-fedscale/core/execution/data_processor.py
-fedscale/core/execution/executor.py
-fedscale/core/execution/optimizers.py
-fedscale/core/execution/rlclient.py
-fedscale/core/internal/__init__.py
-fedscale/core/internal/client.py
-fedscale/core/logger/__init__.py
-fedscale/core/logger/aggragation.py
-fedscale/core/logger/execution.py
-fedscale/core/storage/__init__.py
+fedscale/cloud/__init__.py
+fedscale/cloud/client_manager.py
+fedscale/cloud/commons.py
+fedscale/cloud/config_parser.py
+fedscale/cloud/fllibs.py
+fedscale/cloud/resource_manager.py
+fedscale/cloud/aggregation/__init__.py
+fedscale/cloud/aggregation/aggregator.py
+fedscale/cloud/aggregation/aggregator_mnn.py
+fedscale/cloud/aggregation/aggregator_tflite.py
+fedscale/cloud/aggregation/async_aggregator.py
+fedscale/cloud/aggregation/optimizers.py
+fedscale/cloud/channels/__init__.py
+fedscale/cloud/channels/channel_context.py
+fedscale/cloud/channels/job_api_pb2.py
+fedscale/cloud/channels/job_api_pb2_grpc.py
+fedscale/cloud/execution/__init__.py
+fedscale/cloud/execution/client_base.py
+fedscale/cloud/execution/data_processor.py
+fedscale/cloud/execution/executor.py
+fedscale/cloud/execution/optimizers.py
+fedscale/cloud/execution/rl_client.py
+fedscale/cloud/execution/tensorflow_client.py
+fedscale/cloud/execution/torch_client.py
+fedscale/cloud/internal/__init__.py
+fedscale/cloud/internal/client_metadata.py
+fedscale/cloud/internal/model_adapter_base.py
+fedscale/cloud/internal/tensorflow_model_adapter.py
+fedscale/cloud/internal/tflite_model_adapter.py
+fedscale/cloud/internal/torch_model_adapter.py
+fedscale/cloud/logger/__init__.py
+fedscale/cloud/logger/aggregator_logging.py
+fedscale/cloud/logger/dummy_logger.py
+fedscale/cloud/logger/executor_logging.py
+fedscale/cloud/storage/__init__.py
 fedscale/dataloaders/__init__.py
 fedscale/dataloaders/amazon.py
 fedscale/dataloaders/decoder.py
 fedscale/dataloaders/divide_data.py
 fedscale/dataloaders/dqn.py
 fedscale/dataloaders/femnist.py
 fedscale/dataloaders/inaturalist.py
@@ -52,15 +62,18 @@
 fedscale/dataloaders/word2vec.py
 fedscale/dataloaders/yelp.py
 fedscale/dataloaders/rcnn/__init__.py
 fedscale/dataloaders/rcnn/_init_paths.py
 fedscale/utils/__init__.py
 fedscale/utils/model_test_module.py
 fedscale/utils/models/__init__.py
-fedscale/utils/models/model_provider.py
+fedscale/utils/models/mnn_model_provider.py
+fedscale/utils/models/tensorflow_model_provider.py
+fedscale/utils/models/tflite_model_provider.py
+fedscale/utils/models/torch_model_provider.py
 fedscale/utils/models/cv_models/__init__.py
 fedscale/utils/models/cv_models/airnet.py
 fedscale/utils/models/cv_models/airnext.py
 fedscale/utils/models/cv_models/alexnet.py
 fedscale/utils/models/cv_models/alphapose_coco.py
 fedscale/utils/models/cv_models/bagnet.py
 fedscale/utils/models/cv_models/bamresnet.py
@@ -221,8 +234,15 @@
 fedscale/utils/models/simple/models.py
 fedscale/utils/models/specialized/__init__.py
 fedscale/utils/models/specialized/inception.py
 fedscale/utils/models/specialized/mobilenet.py
 fedscale/utils/models/specialized/resnet_speech.py
 fedscale/utils/models/specialized/voice_model.py
 fedscale/utils/optimizer/__init__.py
-fedscale/utils/optimizer/yogi.py
+fedscale/utils/optimizer/yogi.py
+thirdparty/__init__.py
+thirdparty/oort/__init__.py
+thirdparty/oort/oort.py
+thirdparty/oort/utils/__init__.py
+thirdparty/oort/utils/lp.py
+thirdparty/oort/utils/lp_cplex.py
+thirdparty/oort/utils/lp_gurobi.py
```

