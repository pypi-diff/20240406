# Comparing `tmp/periflow_client-0.2.1.tar.gz` & `tmp/periflow_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "periflow_client-0.2.1.tar", max compression
+gzip compressed data, was "periflow_client-0.2.2.tar", max compression
```

## Comparing `periflow_client-0.2.1.tar` & `periflow_client-0.2.2.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0    10173 2024-01-30 05:12:55.502212 periflow_client-0.2.1/LICENSE
--rw-r--r--   0        0        0     8251 2024-02-21 07:52:43.071657 periflow_client-0.2.1/README.md
--rw-r--r--   0        0        0     1114 2024-02-21 07:52:43.071796 periflow_client-0.2.1/periflow/__init__.py
--rw-r--r--   0        0        0     4881 2024-02-21 07:56:41.130467 periflow_client-0.2.1/periflow/auth.py
--rw-r--r--   0        0        0      188 2024-02-21 07:52:43.072051 periflow_client-0.2.1/periflow/cli/__init__.py
--rw-r--r--   0        0        0     2758 2024-02-21 07:52:43.072129 periflow_client-0.2.1/periflow/cli/catalog.py
--rw-r--r--   0        0        0    29440 2024-02-21 07:52:43.072255 periflow_client-0.2.1/periflow/cli/checkpoint.py
--rw-r--r--   0        0        0    10422 2024-02-21 07:52:43.072387 periflow_client-0.2.1/periflow/cli/credential.py
--rw-r--r--   0        0        0    21020 2024-02-21 07:52:43.072484 periflow_client-0.2.1/periflow/cli/deployment.py
--rw-r--r--   0        0        0     2005 2024-02-21 07:52:43.072570 periflow_client-0.2.1/periflow/cli/gpu.py
--rw-r--r--   0        0        0     5233 2024-02-21 07:52:43.072680 periflow_client-0.2.1/periflow/cli/group.py
--rw-r--r--   0        0        0     2525 2024-02-21 07:52:43.072757 periflow_client-0.2.1/periflow/cli/key.py
--rw-r--r--   0        0        0     6753 2024-02-21 07:52:43.072858 periflow_client-0.2.1/periflow/cli/main.py
--rw-r--r--   0        0        0     9647 2024-02-21 07:52:43.072960 periflow_client-0.2.1/periflow/cli/project.py
--rw-r--r--   0        0        0      125 2024-02-21 07:52:43.073085 periflow_client-0.2.1/periflow/client/__init__.py
--rw-r--r--   0        0        0    14137 2024-02-21 07:52:43.073269 periflow_client-0.2.1/periflow/client/base.py
--rw-r--r--   0        0        0     2273 2024-02-21 07:52:43.073351 periflow_client-0.2.1/periflow/client/catalog.py
--rw-r--r--   0        0        0     4542 2024-02-21 07:52:43.073451 periflow_client-0.2.1/periflow/client/checkpoint.py
--rw-r--r--   0        0        0     2317 2024-02-21 07:52:43.073532 periflow_client-0.2.1/periflow/client/credential.py
--rw-r--r--   0        0        0     5968 2024-02-21 07:52:43.073639 periflow_client-0.2.1/periflow/client/deployment.py
--rw-r--r--   0        0        0     2687 2024-02-21 07:52:43.073722 periflow_client-0.2.1/periflow/client/file.py
--rw-r--r--   0        0        0     2424 2024-02-21 07:52:43.073819 periflow_client-0.2.1/periflow/client/group.py
--rw-r--r--   0        0        0     3073 2024-02-21 07:52:43.073906 periflow_client-0.2.1/periflow/client/project.py
--rw-r--r--   0        0        0     5859 2024-02-21 07:52:43.073992 periflow_client-0.2.1/periflow/client/user.py
--rw-r--r--   0        0        0       98 2024-02-21 07:52:43.074298 periflow_client-0.2.1/periflow/cloud/__init__.py
--rw-r--r--   0        0        0     9622 2024-02-21 07:52:43.074399 periflow_client-0.2.1/periflow/cloud/storage.py
--rw-r--r--   0        0        0      107 2024-02-21 07:52:43.074515 periflow_client-0.2.1/periflow/configurator/__init__.py
--rw-r--r--   0        0        0     1587 2024-02-21 07:52:43.074592 periflow_client-0.2.1/periflow/configurator/base.py
--rw-r--r--   0        0        0     4067 2024-02-21 07:52:43.074665 periflow_client-0.2.1/periflow/configurator/credential.py
--rw-r--r--   0        0        0     3043 2024-02-21 07:52:43.074738 periflow_client-0.2.1/periflow/configurator/deployment.py
--rw-r--r--   0        0        0     1753 2024-02-21 07:52:43.074800 periflow_client-0.2.1/periflow/context.py
--rw-r--r--   0        0        0      104 2024-02-21 07:52:43.074905 periflow_client-0.2.1/periflow/di/__init__.py
--rw-r--r--   0        0        0     1507 2024-02-21 07:52:43.074964 periflow_client-0.2.1/periflow/di/injector.py
--rw-r--r--   0        0        0      499 2024-02-21 07:52:43.075027 periflow_client-0.2.1/periflow/di/modules.py
--rw-r--r--   0        0        0     4117 2024-02-21 07:52:43.075121 periflow_client-0.2.1/periflow/enums.py
--rw-r--r--   0        0        0     6853 2024-02-21 07:52:43.075206 periflow_client-0.2.1/periflow/errors.py
--rw-r--r--   0        0        0     9572 2024-02-21 07:52:43.075295 periflow_client-0.2.1/periflow/formatter.py
--rw-r--r--   0        0        0      637 2024-02-21 07:52:43.075351 periflow_client-0.2.1/periflow/logging.py
--rw-r--r--   0        0        0       92 2024-02-21 07:52:43.075443 periflow_client-0.2.1/periflow/modules/__init__.py
--rw-r--r--   0        0        0      105 2024-02-21 07:52:43.075543 periflow_client-0.2.1/periflow/modules/converter/__init__.py
--rw-r--r--   0        0        0    17093 2024-02-21 07:52:43.075639 periflow_client-0.2.1/periflow/modules/converter/base.py
--rw-r--r--   0        0        0     7885 2024-02-21 07:52:43.075750 periflow_client-0.2.1/periflow/modules/converter/convert.py
--rw-r--r--   0        0        0     5647 2024-02-21 07:52:43.075855 periflow_client-0.2.1/periflow/modules/converter/interface.py
--rw-r--r--   0        0        0     4602 2024-02-21 07:52:43.075949 periflow_client-0.2.1/periflow/modules/converter/maps.py
--rw-r--r--   0        0        0    21328 2024-02-21 07:52:43.076130 periflow_client-0.2.1/periflow/modules/converter/models/blenderbot.py
--rw-r--r--   0        0        0    11658 2024-02-21 07:52:43.076300 periflow_client-0.2.1/periflow/modules/converter/models/bloom.py
--rw-r--r--   0        0        0    10057 2024-02-21 07:52:43.076424 periflow_client-0.2.1/periflow/modules/converter/models/codegen.py
--rw-r--r--   0        0        0    12677 2024-02-21 07:52:43.076492 periflow_client-0.2.1/periflow/modules/converter/models/falcon.py
--rw-r--r--   0        0        0    10036 2024-02-21 07:52:43.076585 periflow_client-0.2.1/periflow/modules/converter/models/gpt2.py
--rw-r--r--   0        0        0    13562 2024-02-21 07:52:43.076656 periflow_client-0.2.1/periflow/modules/converter/models/gpt_neox.py
--rw-r--r--   0        0        0    11911 2024-02-21 07:52:43.076728 periflow_client-0.2.1/periflow/modules/converter/models/gptj.py
--rw-r--r--   0        0        0    13225 2024-02-21 07:52:43.076819 periflow_client-0.2.1/periflow/modules/converter/models/llama.py
--rw-r--r--   0        0        0     4614 2024-02-21 07:52:43.076899 periflow_client-0.2.1/periflow/modules/converter/models/mistral.py
--rw-r--r--   0        0        0    10230 2024-02-21 07:52:43.077000 periflow_client-0.2.1/periflow/modules/converter/models/mpt.py
--rw-r--r--   0        0        0    12005 2024-02-21 07:52:43.077094 periflow_client-0.2.1/periflow/modules/converter/models/opt.py
--rw-r--r--   0        0        0    18734 2024-02-21 07:52:43.077181 periflow_client-0.2.1/periflow/modules/converter/models/t5.py
--rw-r--r--   0        0        0     3324 2024-02-21 07:52:43.077264 periflow_client-0.2.1/periflow/modules/converter/saver.py
--rw-r--r--   0        0        0      917 2024-02-21 07:52:43.077323 periflow_client-0.2.1/periflow/modules/converter/schema.py
--rw-r--r--   0        0        0     7959 2024-02-21 07:52:43.077422 periflow_client-0.2.1/periflow/modules/converter/utils.py
--rw-r--r--   0        0        0      105 2024-02-21 07:52:43.077530 periflow_client-0.2.1/periflow/modules/quantizer/__init__.py
--rw-r--r--   0        0        0      109 2024-02-21 07:52:43.077631 periflow_client-0.2.1/periflow/modules/quantizer/awq/__init__.py
--rw-r--r--   0        0        0    20022 2024-02-21 07:52:43.077726 periflow_client-0.2.1/periflow/modules/quantizer/awq/base.py
--rw-r--r--   0        0        0     8498 2024-02-21 07:52:43.077875 periflow_client-0.2.1/periflow/modules/quantizer/awq/models/gpt_neox.py
--rw-r--r--   0        0        0     5919 2024-02-21 07:52:43.078016 periflow_client-0.2.1/periflow/modules/quantizer/awq/models/gptj.py
--rw-r--r--   0        0        0    11209 2024-02-21 07:52:43.078094 periflow_client-0.2.1/periflow/modules/quantizer/awq/models/llama.py
--rw-r--r--   0        0        0     6666 2024-02-21 07:52:43.078196 periflow_client-0.2.1/periflow/modules/quantizer/awq/models/mpt.py
--rw-r--r--   0        0        0     7765 2024-02-21 07:52:43.078310 periflow_client-0.2.1/periflow/modules/quantizer/awq/utils.py
--rw-r--r--   0        0        0     7515 2024-02-21 07:52:43.078400 periflow_client-0.2.1/periflow/modules/quantizer/base.py
--rw-r--r--   0        0        0     3527 2024-02-21 07:52:43.078481 periflow_client-0.2.1/periflow/modules/quantizer/layers.py
--rw-r--r--   0        0        0     3665 2024-02-21 07:52:43.078548 periflow_client-0.2.1/periflow/modules/quantizer/maps.py
--rw-r--r--   0        0        0      112 2024-02-21 07:52:43.078630 periflow_client-0.2.1/periflow/modules/quantizer/schema/__init__.py
--rw-r--r--   0        0        0     1789 2024-02-21 07:52:43.078689 periflow_client-0.2.1/periflow/modules/quantizer/schema/config.py
--rw-r--r--   0        0        0     2004 2024-02-21 07:52:43.078743 periflow_client-0.2.1/periflow/modules/quantizer/schema/data.py
--rw-r--r--   0        0        0      117 2024-02-21 07:52:43.078822 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/__init__.py
--rw-r--r--   0        0        0    24940 2024-02-21 07:52:43.078881 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/base.py
--rw-r--r--   0        0        0     7501 2024-02-21 07:52:43.079031 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/bloom.py
--rw-r--r--   0        0        0     8768 2024-02-21 07:52:43.079126 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/codegen.py
--rw-r--r--   0        0        0    10442 2024-02-21 07:52:43.079200 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/falcon.py
--rw-r--r--   0        0        0     5471 2024-02-21 07:52:43.079304 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/gpt2.py
--rw-r--r--   0        0        0     9053 2024-02-21 07:52:43.079389 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/gpt_neox.py
--rw-r--r--   0        0        0     6970 2024-02-21 07:52:43.079471 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/gptj.py
--rw-r--r--   0        0        0     9244 2024-02-21 07:52:43.079575 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/llama.py
--rw-r--r--   0        0        0     5295 2024-02-21 07:52:43.079678 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/mpt.py
--rw-r--r--   0        0        0     5236 2024-02-21 07:52:43.079756 periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/opt.py
--rw-r--r--   0        0        0    16785 2024-02-21 07:52:43.079861 periflow_client-0.2.1/periflow/modules/quantizer/utils.py
--rw-r--r--   0        0        0       92 2024-02-21 07:52:43.079961 periflow_client-0.2.1/periflow/schema/__init__.py
--rw-r--r--   0        0        0       96 2024-02-21 07:52:43.080040 periflow_client-0.2.1/periflow/schema/api/__init__.py
--rw-r--r--   0        0        0       99 2024-02-21 07:52:43.080123 periflow_client-0.2.1/periflow/schema/api/v1/__init__.py
--rw-r--r--   0        0        0      114 2024-02-21 07:52:43.080232 periflow_client-0.2.1/periflow/schema/api/v1/codegen/__init__.py
--rw-r--r--   0        0        0     4229 2024-02-21 07:52:43.080328 periflow_client-0.2.1/periflow/schema/api/v1/codegen/completion_pb2.py
--rw-r--r--   0        0        0     7049 2024-02-21 07:52:43.080420 periflow_client-0.2.1/periflow/schema/api/v1/codegen/completion_pb2.pyi
--rw-r--r--   0        0        0     1142 2024-02-21 07:52:43.080486 periflow_client-0.2.1/periflow/schema/api/v1/codegen/detokenize_pb2.py
--rw-r--r--   0        0        0      681 2024-02-21 07:52:43.080543 periflow_client-0.2.1/periflow/schema/api/v1/codegen/detokenize_pb2.pyi
--rw-r--r--   0        0        0     1155 2024-02-21 07:52:43.080595 periflow_client-0.2.1/periflow/schema/api/v1/codegen/tokenize_pb2.py
--rw-r--r--   0        0        0      522 2024-02-21 07:52:43.080649 periflow_client-0.2.1/periflow/schema/api/v1/codegen/tokenize_pb2.pyi
--rw-r--r--   0        0        0     3279 2024-02-21 07:52:43.080711 periflow_client-0.2.1/periflow/schema/api/v1/completion.py
--rw-r--r--   0        0        0      430 2024-02-21 07:52:43.080772 periflow_client-0.2.1/periflow/schema/api/v1/detokenize.py
--rw-r--r--   0        0        0     1769 2024-02-21 07:52:43.080878 periflow_client-0.2.1/periflow/schema/api/v1/proto/completion.proto
--rw-r--r--   0        0        0      159 2024-02-21 07:52:43.080943 periflow_client-0.2.1/periflow/schema/api/v1/proto/detokenize.proto
--rw-r--r--   0        0        0      158 2024-02-21 07:52:43.081008 periflow_client-0.2.1/periflow/schema/api/v1/proto/tokenize.proto
--rw-r--r--   0        0        0      422 2024-02-21 07:52:43.081073 periflow_client-0.2.1/periflow/schema/api/v1/tokenize.py
--rw-r--r--   0        0        0      101 2024-02-21 07:52:43.081160 periflow_client-0.2.1/periflow/schema/resource/__init__.py
--rw-r--r--   0        0        0      104 2024-02-21 07:52:43.081243 periflow_client-0.2.1/periflow/schema/resource/v1/__init__.py
--rw-r--r--   0        0        0     4945 2024-02-21 07:55:34.577156 periflow_client-0.2.1/periflow/schema/resource/v1/attributes.py
--rw-r--r--   0        0        0     2353 2024-02-21 07:52:43.081389 periflow_client-0.2.1/periflow/schema/resource/v1/checkpoint.py
--rw-r--r--   0        0        0     1358 2024-02-21 07:52:43.081463 periflow_client-0.2.1/periflow/schema/resource/v1/credential.py
--rw-r--r--   0        0        0     2027 2024-02-21 07:52:43.081543 periflow_client-0.2.1/periflow/schema/resource/v1/deployment.py
--rw-r--r--   0        0        0      753 2024-02-21 07:52:43.081627 periflow_client-0.2.1/periflow/schema/resource/v1/transfer.py
--rw-r--r--   0        0        0       88 2024-02-21 07:52:43.081711 periflow_client-0.2.1/periflow/sdk/__init__.py
--rw-r--r--   0        0        0      102 2024-02-21 07:52:43.081789 periflow_client-0.2.1/periflow/sdk/api/__init__.py
--rw-r--r--   0        0        0     5892 2024-02-21 07:52:43.081869 periflow_client-0.2.1/periflow/sdk/api/base.py
--rw-r--r--   0        0        0    27245 2024-02-21 07:52:43.082037 periflow_client-0.2.1/periflow/sdk/api/completion.py
--rw-r--r--   0        0        0     3185 2024-02-21 07:52:43.082108 periflow_client-0.2.1/periflow/sdk/api/detokenization.py
--rw-r--r--   0        0        0     3037 2024-02-21 07:52:43.082169 periflow_client-0.2.1/periflow/sdk/api/tokenization.py
--rw-r--r--   0        0        0     1836 2024-02-21 07:52:43.082237 periflow_client-0.2.1/periflow/sdk/init.py
--rw-r--r--   0        0        0      112 2024-02-21 07:52:43.082321 periflow_client-0.2.1/periflow/sdk/resource/__init__.py
--rw-r--r--   0        0        0      733 2024-02-21 07:52:43.082374 periflow_client-0.2.1/periflow/sdk/resource/base.py
--rw-r--r--   0        0        0     1896 2024-02-21 07:52:43.082427 periflow_client-0.2.1/periflow/sdk/resource/catalog.py
--rw-r--r--   0        0        0    27872 2024-02-21 07:52:43.082546 periflow_client-0.2.1/periflow/sdk/resource/checkpoint.py
--rw-r--r--   0        0        0     4133 2024-02-21 07:52:43.082633 periflow_client-0.2.1/periflow/sdk/resource/credential.py
--rw-r--r--   0        0        0    21258 2024-02-21 07:52:43.082720 periflow_client-0.2.1/periflow/sdk/resource/deployment.py
--rw-r--r--   0        0        0       97 2024-02-21 07:52:43.082818 periflow_client-0.2.1/periflow/utils/__init__.py
--rw-r--r--   0        0        0      631 2024-02-21 07:52:43.082883 periflow_client-0.2.1/periflow/utils/decorator.py
--rw-r--r--   0        0        0     5450 2024-02-21 07:52:43.082968 periflow_client-0.2.1/periflow/utils/format.py
--rw-r--r--   0        0        0     4612 2024-02-21 07:52:43.083066 periflow_client-0.2.1/periflow/utils/fs.py
--rw-r--r--   0        0        0     1651 2024-02-21 07:52:43.083120 periflow_client-0.2.1/periflow/utils/maps.py
--rw-r--r--   0        0        0      666 2024-02-21 07:52:43.083177 periflow_client-0.2.1/periflow/utils/prompt.py
--rw-r--r--   0        0        0     1392 2024-02-21 07:52:43.083245 periflow_client-0.2.1/periflow/utils/request.py
--rw-r--r--   0        0        0     1384 2024-02-21 07:52:43.083302 periflow_client-0.2.1/periflow/utils/testing.py
--rw-r--r--   0        0        0    19778 2024-02-21 07:52:43.083383 periflow_client-0.2.1/periflow/utils/transfer.py
--rw-r--r--   0        0        0     3381 2024-02-21 07:52:43.083452 periflow_client-0.2.1/periflow/utils/url.py
--rw-r--r--   0        0        0     4521 2024-02-21 07:52:43.083527 periflow_client-0.2.1/periflow/utils/validate.py
--rw-r--r--   0        0        0     1513 2024-02-21 07:52:43.083592 periflow_client-0.2.1/periflow/utils/version.py
--rw-r--r--   0        0        0     3477 2024-02-21 08:06:19.890914 periflow_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 periflow_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-01-03 12:49:02.620986 periflow_client-0.2.2/LICENSE
+-rw-r--r--   0        0        0     8251 2024-04-06 15:33:47.697678 periflow_client-0.2.2/README.md
+-rw-r--r--   0        0        0     1114 2024-04-06 15:33:47.697965 periflow_client-0.2.2/periflow/__init__.py
+-rw-r--r--   0        0        0     4881 2024-04-06 15:33:47.698144 periflow_client-0.2.2/periflow/auth.py
+-rw-r--r--   0        0        0      188 2024-04-06 15:33:47.698870 periflow_client-0.2.2/periflow/cli/__init__.py
+-rw-r--r--   0        0        0     2758 2024-04-06 15:33:47.699015 periflow_client-0.2.2/periflow/cli/catalog.py
+-rw-r--r--   0        0        0    29440 2024-04-06 15:33:47.699699 periflow_client-0.2.2/periflow/cli/checkpoint.py
+-rw-r--r--   0        0        0    10422 2024-04-06 15:33:47.699962 periflow_client-0.2.2/periflow/cli/credential.py
+-rw-r--r--   0        0        0    21020 2024-04-06 15:33:47.700177 periflow_client-0.2.2/periflow/cli/deployment.py
+-rw-r--r--   0        0        0     2005 2024-04-06 15:33:47.701047 periflow_client-0.2.2/periflow/cli/gpu.py
+-rw-r--r--   0        0        0     5233 2024-04-06 15:33:47.701602 periflow_client-0.2.2/periflow/cli/group.py
+-rw-r--r--   0        0        0     2525 2024-04-06 15:33:47.701761 periflow_client-0.2.2/periflow/cli/key.py
+-rw-r--r--   0        0        0     6753 2024-04-06 15:33:47.701991 periflow_client-0.2.2/periflow/cli/main.py
+-rw-r--r--   0        0        0     9647 2024-04-06 15:33:47.702195 periflow_client-0.2.2/periflow/cli/project.py
+-rw-r--r--   0        0        0      125 2024-04-06 15:33:47.702399 periflow_client-0.2.2/periflow/client/__init__.py
+-rw-r--r--   0        0        0    14137 2024-04-06 15:33:47.703303 periflow_client-0.2.2/periflow/client/base.py
+-rw-r--r--   0        0        0     2273 2024-04-06 15:33:47.703716 periflow_client-0.2.2/periflow/client/catalog.py
+-rw-r--r--   0        0        0     4542 2024-04-06 15:33:47.703916 periflow_client-0.2.2/periflow/client/checkpoint.py
+-rw-r--r--   0        0        0     2317 2024-04-06 15:33:47.704059 periflow_client-0.2.2/periflow/client/credential.py
+-rw-r--r--   0        0        0     5968 2024-04-06 15:33:47.704473 periflow_client-0.2.2/periflow/client/deployment.py
+-rw-r--r--   0        0        0     2687 2024-04-06 15:33:47.704667 periflow_client-0.2.2/periflow/client/file.py
+-rw-r--r--   0        0        0     2424 2024-04-06 15:33:47.704829 periflow_client-0.2.2/periflow/client/group.py
+-rw-r--r--   0        0        0     3073 2024-04-06 15:33:47.705007 periflow_client-0.2.2/periflow/client/project.py
+-rw-r--r--   0        0        0     5859 2024-04-06 15:33:47.705153 periflow_client-0.2.2/periflow/client/user.py
+-rw-r--r--   0        0        0       98 2024-04-06 15:33:47.705341 periflow_client-0.2.2/periflow/cloud/__init__.py
+-rw-r--r--   0        0        0     9622 2024-04-06 15:33:47.705514 periflow_client-0.2.2/periflow/cloud/storage.py
+-rw-r--r--   0        0        0      107 2024-04-06 15:33:47.705702 periflow_client-0.2.2/periflow/configurator/__init__.py
+-rw-r--r--   0        0        0     1587 2024-04-06 15:33:47.705921 periflow_client-0.2.2/periflow/configurator/base.py
+-rw-r--r--   0        0        0     4067 2024-04-06 15:33:47.706115 periflow_client-0.2.2/periflow/configurator/credential.py
+-rw-r--r--   0        0        0     3043 2024-04-06 15:33:47.706243 periflow_client-0.2.2/periflow/configurator/deployment.py
+-rw-r--r--   0        0        0     1753 2024-04-06 15:33:47.706367 periflow_client-0.2.2/periflow/context.py
+-rw-r--r--   0        0        0      104 2024-04-06 15:33:47.706614 periflow_client-0.2.2/periflow/di/__init__.py
+-rw-r--r--   0        0        0     1507 2024-04-06 15:33:47.706832 periflow_client-0.2.2/periflow/di/injector.py
+-rw-r--r--   0        0        0      499 2024-04-06 15:33:47.707034 periflow_client-0.2.2/periflow/di/modules.py
+-rw-r--r--   0        0        0     4117 2024-04-06 15:33:47.707219 periflow_client-0.2.2/periflow/enums.py
+-rw-r--r--   0        0        0     6853 2024-04-06 15:33:47.708046 periflow_client-0.2.2/periflow/errors.py
+-rw-r--r--   0        0        0     9572 2024-04-06 15:33:47.708395 periflow_client-0.2.2/periflow/formatter.py
+-rw-r--r--   0        0        0      637 2024-04-06 15:33:47.708592 periflow_client-0.2.2/periflow/logging.py
+-rw-r--r--   0        0        0       92 2024-04-06 15:33:47.709488 periflow_client-0.2.2/periflow/modules/__init__.py
+-rw-r--r--   0        0        0      105 2024-04-06 15:33:47.709711 periflow_client-0.2.2/periflow/modules/converter/__init__.py
+-rw-r--r--   0        0        0    17093 2024-04-06 15:33:47.709928 periflow_client-0.2.2/periflow/modules/converter/base.py
+-rw-r--r--   0        0        0     7885 2024-04-06 15:33:47.710126 periflow_client-0.2.2/periflow/modules/converter/convert.py
+-rw-r--r--   0        0        0     5647 2024-04-06 15:33:47.710271 periflow_client-0.2.2/periflow/modules/converter/interface.py
+-rw-r--r--   0        0        0     4602 2024-04-06 15:33:47.710750 periflow_client-0.2.2/periflow/modules/converter/maps.py
+-rw-r--r--   0        0        0    21328 2024-04-06 15:33:47.711166 periflow_client-0.2.2/periflow/modules/converter/models/blenderbot.py
+-rw-r--r--   0        0        0    11658 2024-04-06 15:33:47.711603 periflow_client-0.2.2/periflow/modules/converter/models/bloom.py
+-rw-r--r--   0        0        0    10057 2024-04-06 15:33:47.712054 periflow_client-0.2.2/periflow/modules/converter/models/codegen.py
+-rw-r--r--   0        0        0    12677 2024-04-06 15:33:47.712246 periflow_client-0.2.2/periflow/modules/converter/models/falcon.py
+-rw-r--r--   0        0        0    10036 2024-04-06 15:33:47.712431 periflow_client-0.2.2/periflow/modules/converter/models/gpt2.py
+-rw-r--r--   0        0        0    13562 2024-04-06 15:33:47.712593 periflow_client-0.2.2/periflow/modules/converter/models/gpt_neox.py
+-rw-r--r--   0        0        0    11911 2024-04-06 15:33:47.712768 periflow_client-0.2.2/periflow/modules/converter/models/gptj.py
+-rw-r--r--   0        0        0    13225 2024-04-06 15:33:47.712960 periflow_client-0.2.2/periflow/modules/converter/models/llama.py
+-rw-r--r--   0        0        0     4614 2024-04-06 15:33:47.713251 periflow_client-0.2.2/periflow/modules/converter/models/mistral.py
+-rw-r--r--   0        0        0    10230 2024-04-06 15:33:47.713423 periflow_client-0.2.2/periflow/modules/converter/models/mpt.py
+-rw-r--r--   0        0        0    12005 2024-04-06 15:33:47.713979 periflow_client-0.2.2/periflow/modules/converter/models/opt.py
+-rw-r--r--   0        0        0    18734 2024-04-06 15:33:47.714175 periflow_client-0.2.2/periflow/modules/converter/models/t5.py
+-rw-r--r--   0        0        0     3324 2024-04-06 15:33:47.714366 periflow_client-0.2.2/periflow/modules/converter/saver.py
+-rw-r--r--   0        0        0      917 2024-04-06 15:33:47.714494 periflow_client-0.2.2/periflow/modules/converter/schema.py
+-rw-r--r--   0        0        0     7959 2024-04-06 15:33:47.714876 periflow_client-0.2.2/periflow/modules/converter/utils.py
+-rw-r--r--   0        0        0      105 2024-04-06 15:33:47.715085 periflow_client-0.2.2/periflow/modules/quantizer/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-06 15:33:47.715276 periflow_client-0.2.2/periflow/modules/quantizer/awq/__init__.py
+-rw-r--r--   0        0        0    20022 2024-04-06 15:33:47.715561 periflow_client-0.2.2/periflow/modules/quantizer/awq/base.py
+-rw-r--r--   0        0        0     8498 2024-04-06 15:33:47.716097 periflow_client-0.2.2/periflow/modules/quantizer/awq/models/gpt_neox.py
+-rw-r--r--   0        0        0     5919 2024-04-06 15:33:47.716322 periflow_client-0.2.2/periflow/modules/quantizer/awq/models/gptj.py
+-rw-r--r--   0        0        0    11209 2024-04-06 15:33:47.716523 periflow_client-0.2.2/periflow/modules/quantizer/awq/models/llama.py
+-rw-r--r--   0        0        0     6666 2024-04-06 15:33:47.716694 periflow_client-0.2.2/periflow/modules/quantizer/awq/models/mpt.py
+-rw-r--r--   0        0        0     7765 2024-04-06 15:33:47.716881 periflow_client-0.2.2/periflow/modules/quantizer/awq/utils.py
+-rw-r--r--   0        0        0     7515 2024-04-06 15:33:47.717041 periflow_client-0.2.2/periflow/modules/quantizer/base.py
+-rw-r--r--   0        0        0     3527 2024-04-06 15:33:47.717190 periflow_client-0.2.2/periflow/modules/quantizer/layers.py
+-rw-r--r--   0        0        0     3665 2024-04-06 15:33:47.717320 periflow_client-0.2.2/periflow/modules/quantizer/maps.py
+-rw-r--r--   0        0        0      112 2024-04-06 15:33:47.717507 periflow_client-0.2.2/periflow/modules/quantizer/schema/__init__.py
+-rw-r--r--   0        0        0     1789 2024-04-06 15:33:47.717645 periflow_client-0.2.2/periflow/modules/quantizer/schema/config.py
+-rw-r--r--   0        0        0     2004 2024-04-06 15:33:47.717824 periflow_client-0.2.2/periflow/modules/quantizer/schema/data.py
+-rw-r--r--   0        0        0      117 2024-04-06 15:33:47.718012 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/__init__.py
+-rw-r--r--   0        0        0    24940 2024-04-06 15:33:47.718151 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/base.py
+-rw-r--r--   0        0        0     7501 2024-04-06 15:33:47.718522 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/bloom.py
+-rw-r--r--   0        0        0     8768 2024-04-06 15:33:47.718704 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/codegen.py
+-rw-r--r--   0        0        0    10442 2024-04-06 15:33:47.718861 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/falcon.py
+-rw-r--r--   0        0        0     5471 2024-04-06 15:33:47.719605 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/gpt2.py
+-rw-r--r--   0        0        0     9053 2024-04-06 15:33:47.719751 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/gpt_neox.py
+-rw-r--r--   0        0        0     6970 2024-04-06 15:33:47.719888 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/gptj.py
+-rw-r--r--   0        0        0     9244 2024-04-06 15:33:47.720053 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/llama.py
+-rw-r--r--   0        0        0     5295 2024-04-06 15:33:47.720237 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/mpt.py
+-rw-r--r--   0        0        0     5236 2024-04-06 15:33:47.720380 periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/opt.py
+-rw-r--r--   0        0        0    16785 2024-04-06 15:33:47.720651 periflow_client-0.2.2/periflow/modules/quantizer/utils.py
+-rw-r--r--   0        0        0       92 2024-04-06 15:33:47.720871 periflow_client-0.2.2/periflow/schema/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-06 15:33:47.721059 periflow_client-0.2.2/periflow/schema/api/__init__.py
+-rw-r--r--   0        0        0       99 2024-04-06 15:33:47.721241 periflow_client-0.2.2/periflow/schema/api/v1/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-06 15:33:47.721449 periflow_client-0.2.2/periflow/schema/api/v1/codegen/__init__.py
+-rw-r--r--   0        0        0     4229 2024-04-06 15:33:47.721905 periflow_client-0.2.2/periflow/schema/api/v1/codegen/completion_pb2.py
+-rw-r--r--   0        0        0     7049 2024-04-06 15:33:47.722081 periflow_client-0.2.2/periflow/schema/api/v1/codegen/completion_pb2.pyi
+-rw-r--r--   0        0        0     1142 2024-04-06 15:33:47.722263 periflow_client-0.2.2/periflow/schema/api/v1/codegen/detokenize_pb2.py
+-rw-r--r--   0        0        0      681 2024-04-06 15:33:47.722386 periflow_client-0.2.2/periflow/schema/api/v1/codegen/detokenize_pb2.pyi
+-rw-r--r--   0        0        0     1155 2024-04-06 15:33:47.722503 periflow_client-0.2.2/periflow/schema/api/v1/codegen/tokenize_pb2.py
+-rw-r--r--   0        0        0      522 2024-04-06 15:33:47.722622 periflow_client-0.2.2/periflow/schema/api/v1/codegen/tokenize_pb2.pyi
+-rw-r--r--   0        0        0     3279 2024-04-06 15:33:47.722844 periflow_client-0.2.2/periflow/schema/api/v1/completion.py
+-rw-r--r--   0        0        0      430 2024-04-06 15:33:47.723098 periflow_client-0.2.2/periflow/schema/api/v1/detokenize.py
+-rw-r--r--   0        0        0     1769 2024-04-06 15:33:47.723356 periflow_client-0.2.2/periflow/schema/api/v1/proto/completion.proto
+-rw-r--r--   0        0        0      159 2024-04-06 15:33:47.723491 periflow_client-0.2.2/periflow/schema/api/v1/proto/detokenize.proto
+-rw-r--r--   0        0        0      158 2024-04-06 15:33:47.723656 periflow_client-0.2.2/periflow/schema/api/v1/proto/tokenize.proto
+-rw-r--r--   0        0        0      422 2024-04-06 15:33:47.723788 periflow_client-0.2.2/periflow/schema/api/v1/tokenize.py
+-rw-r--r--   0        0        0      101 2024-04-06 15:33:47.723974 periflow_client-0.2.2/periflow/schema/resource/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-06 15:33:47.724171 periflow_client-0.2.2/periflow/schema/resource/v1/__init__.py
+-rw-r--r--   0        0        0     4977 2024-04-06 15:43:16.743981 periflow_client-0.2.2/periflow/schema/resource/v1/attributes.py
+-rw-r--r--   0        0        0     2353 2024-04-06 15:33:47.724475 periflow_client-0.2.2/periflow/schema/resource/v1/checkpoint.py
+-rw-r--r--   0        0        0     1358 2024-04-06 15:33:47.724621 periflow_client-0.2.2/periflow/schema/resource/v1/credential.py
+-rw-r--r--   0        0        0     2027 2024-04-06 15:33:47.724759 periflow_client-0.2.2/periflow/schema/resource/v1/deployment.py
+-rw-r--r--   0        0        0      753 2024-04-06 15:33:47.725255 periflow_client-0.2.2/periflow/schema/resource/v1/transfer.py
+-rw-r--r--   0        0        0       88 2024-04-06 15:33:47.725459 periflow_client-0.2.2/periflow/sdk/__init__.py
+-rw-r--r--   0        0        0      102 2024-04-06 15:33:47.725647 periflow_client-0.2.2/periflow/sdk/api/__init__.py
+-rw-r--r--   0        0        0     5892 2024-04-06 15:33:47.725806 periflow_client-0.2.2/periflow/sdk/api/base.py
+-rw-r--r--   0        0        0    27245 2024-04-06 15:33:47.726248 periflow_client-0.2.2/periflow/sdk/api/completion.py
+-rw-r--r--   0        0        0     3185 2024-04-06 15:33:47.726420 periflow_client-0.2.2/periflow/sdk/api/detokenization.py
+-rw-r--r--   0        0        0     3037 2024-04-06 15:33:47.726594 periflow_client-0.2.2/periflow/sdk/api/tokenization.py
+-rw-r--r--   0        0        0     1836 2024-04-06 15:33:47.726979 periflow_client-0.2.2/periflow/sdk/init.py
+-rw-r--r--   0        0        0      112 2024-04-06 15:33:47.727196 periflow_client-0.2.2/periflow/sdk/resource/__init__.py
+-rw-r--r--   0        0        0      733 2024-04-06 15:33:47.727331 periflow_client-0.2.2/periflow/sdk/resource/base.py
+-rw-r--r--   0        0        0     1896 2024-04-06 15:33:47.727454 periflow_client-0.2.2/periflow/sdk/resource/catalog.py
+-rw-r--r--   0        0        0    27872 2024-04-06 15:33:47.727960 periflow_client-0.2.2/periflow/sdk/resource/checkpoint.py
+-rw-r--r--   0        0        0     4133 2024-04-06 15:33:47.728273 periflow_client-0.2.2/periflow/sdk/resource/credential.py
+-rw-r--r--   0        0        0    21258 2024-04-06 15:33:47.728577 periflow_client-0.2.2/periflow/sdk/resource/deployment.py
+-rw-r--r--   0        0        0       97 2024-04-06 15:33:47.728854 periflow_client-0.2.2/periflow/utils/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-06 15:33:47.729011 periflow_client-0.2.2/periflow/utils/decorator.py
+-rw-r--r--   0        0        0     5450 2024-04-06 15:33:47.729195 periflow_client-0.2.2/periflow/utils/format.py
+-rw-r--r--   0        0        0     4612 2024-04-06 15:33:47.729377 periflow_client-0.2.2/periflow/utils/fs.py
+-rw-r--r--   0        0        0     1651 2024-04-06 15:33:47.729573 periflow_client-0.2.2/periflow/utils/maps.py
+-rw-r--r--   0        0        0      666 2024-04-06 15:33:47.729732 periflow_client-0.2.2/periflow/utils/prompt.py
+-rw-r--r--   0        0        0     1392 2024-04-06 15:33:47.729865 periflow_client-0.2.2/periflow/utils/request.py
+-rw-r--r--   0        0        0     1384 2024-04-06 15:33:47.729981 periflow_client-0.2.2/periflow/utils/testing.py
+-rw-r--r--   0        0        0    19778 2024-04-06 15:33:47.730499 periflow_client-0.2.2/periflow/utils/transfer.py
+-rw-r--r--   0        0        0     3381 2024-04-06 15:33:47.730679 periflow_client-0.2.2/periflow/utils/url.py
+-rw-r--r--   0        0        0     4521 2024-04-06 15:33:47.730847 periflow_client-0.2.2/periflow/utils/validate.py
+-rw-r--r--   0        0        0     1513 2024-04-06 15:33:47.731224 periflow_client-0.2.2/periflow/utils/version.py
+-rw-r--r--   0        0        0     3477 2024-04-06 15:45:57.533848 periflow_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10270 1970-01-01 00:00:00.000000 periflow_client-0.2.2/PKG-INFO
```

### Comparing `periflow_client-0.2.1/LICENSE` & `periflow_client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/README.md` & `periflow_client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/__init__.py` & `periflow_client-0.2.2/periflow/__init__.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/auth.py` & `periflow_client-0.2.2/periflow/auth.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/catalog.py` & `periflow_client-0.2.2/periflow/cli/catalog.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/checkpoint.py` & `periflow_client-0.2.2/periflow/cli/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/credential.py` & `periflow_client-0.2.2/periflow/cli/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/deployment.py` & `periflow_client-0.2.2/periflow/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/gpu.py` & `periflow_client-0.2.2/periflow/cli/gpu.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/group.py` & `periflow_client-0.2.2/periflow/cli/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/key.py` & `periflow_client-0.2.2/periflow/cli/key.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/main.py` & `periflow_client-0.2.2/periflow/cli/main.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cli/project.py` & `periflow_client-0.2.2/periflow/cli/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/base.py` & `periflow_client-0.2.2/periflow/client/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/catalog.py` & `periflow_client-0.2.2/periflow/client/catalog.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/checkpoint.py` & `periflow_client-0.2.2/periflow/client/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/credential.py` & `periflow_client-0.2.2/periflow/client/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/deployment.py` & `periflow_client-0.2.2/periflow/client/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/file.py` & `periflow_client-0.2.2/periflow/client/file.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/group.py` & `periflow_client-0.2.2/periflow/client/group.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/project.py` & `periflow_client-0.2.2/periflow/client/project.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/client/user.py` & `periflow_client-0.2.2/periflow/client/user.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/cloud/storage.py` & `periflow_client-0.2.2/periflow/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/configurator/base.py` & `periflow_client-0.2.2/periflow/configurator/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/configurator/credential.py` & `periflow_client-0.2.2/periflow/configurator/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/configurator/deployment.py` & `periflow_client-0.2.2/periflow/configurator/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/context.py` & `periflow_client-0.2.2/periflow/context.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/di/injector.py` & `periflow_client-0.2.2/periflow/di/injector.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/enums.py` & `periflow_client-0.2.2/periflow/enums.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/errors.py` & `periflow_client-0.2.2/periflow/errors.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/formatter.py` & `periflow_client-0.2.2/periflow/formatter.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/logging.py` & `periflow_client-0.2.2/periflow/logging.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/base.py` & `periflow_client-0.2.2/periflow/modules/converter/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/convert.py` & `periflow_client-0.2.2/periflow/modules/converter/convert.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/interface.py` & `periflow_client-0.2.2/periflow/modules/converter/interface.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/maps.py` & `periflow_client-0.2.2/periflow/modules/converter/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/blenderbot.py` & `periflow_client-0.2.2/periflow/modules/converter/models/blenderbot.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/bloom.py` & `periflow_client-0.2.2/periflow/modules/converter/models/bloom.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/codegen.py` & `periflow_client-0.2.2/periflow/modules/converter/models/codegen.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/falcon.py` & `periflow_client-0.2.2/periflow/modules/converter/models/falcon.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/gpt2.py` & `periflow_client-0.2.2/periflow/modules/converter/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/gpt_neox.py` & `periflow_client-0.2.2/periflow/modules/converter/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/gptj.py` & `periflow_client-0.2.2/periflow/modules/converter/models/gptj.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/llama.py` & `periflow_client-0.2.2/periflow/modules/converter/models/llama.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/mistral.py` & `periflow_client-0.2.2/periflow/modules/converter/models/mistral.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/mpt.py` & `periflow_client-0.2.2/periflow/modules/converter/models/mpt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/opt.py` & `periflow_client-0.2.2/periflow/modules/converter/models/opt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/models/t5.py` & `periflow_client-0.2.2/periflow/modules/converter/models/t5.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/saver.py` & `periflow_client-0.2.2/periflow/modules/converter/saver.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/schema.py` & `periflow_client-0.2.2/periflow/modules/converter/schema.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/converter/utils.py` & `periflow_client-0.2.2/periflow/modules/converter/utils.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/awq/base.py` & `periflow_client-0.2.2/periflow/modules/quantizer/awq/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/awq/models/gpt_neox.py` & `periflow_client-0.2.2/periflow/modules/quantizer/awq/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/awq/models/gptj.py` & `periflow_client-0.2.2/periflow/modules/quantizer/awq/models/gptj.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/awq/models/llama.py` & `periflow_client-0.2.2/periflow/modules/quantizer/awq/models/llama.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/awq/models/mpt.py` & `periflow_client-0.2.2/periflow/modules/quantizer/awq/models/mpt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/awq/utils.py` & `periflow_client-0.2.2/periflow/modules/quantizer/awq/utils.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/base.py` & `periflow_client-0.2.2/periflow/modules/quantizer/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/layers.py` & `periflow_client-0.2.2/periflow/modules/quantizer/layers.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/maps.py` & `periflow_client-0.2.2/periflow/modules/quantizer/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/schema/config.py` & `periflow_client-0.2.2/periflow/modules/quantizer/schema/config.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/schema/data.py` & `periflow_client-0.2.2/periflow/modules/quantizer/schema/data.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/base.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/bloom.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/bloom.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/codegen.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/codegen.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/falcon.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/falcon.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/gpt2.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/gpt_neox.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/gptj.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/gptj.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/llama.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/llama.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/mpt.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/mpt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/smoothquant/models/opt.py` & `periflow_client-0.2.2/periflow/modules/quantizer/smoothquant/models/opt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/modules/quantizer/utils.py` & `periflow_client-0.2.2/periflow/modules/quantizer/utils.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/api/v1/codegen/completion_pb2.py` & `periflow_client-0.2.2/periflow/schema/api/v1/codegen/completion_pb2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/api/v1/codegen/completion_pb2.pyi` & `periflow_client-0.2.2/periflow/schema/api/v1/codegen/completion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/api/v1/codegen/detokenize_pb2.py` & `periflow_client-0.2.2/periflow/schema/api/v1/codegen/detokenize_pb2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/api/v1/codegen/detokenize_pb2.pyi` & `periflow_client-0.2.2/periflow/schema/api/v1/codegen/detokenize_pb2.pyi`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/api/v1/codegen/tokenize_pb2.py` & `periflow_client-0.2.2/periflow/schema/api/v1/codegen/tokenize_pb2.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/api/v1/codegen/tokenize_pb2.pyi` & `periflow_client-0.2.2/periflow/schema/api/v1/codegen/tokenize_pb2.pyi`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/api/v1/completion.py` & `periflow_client-0.2.2/periflow/schema/api/v1/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/api/v1/proto/completion.proto` & `periflow_client-0.2.2/periflow/schema/api/v1/proto/completion.proto`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/resource/v1/attributes.py` & `periflow_client-0.2.2/periflow/schema/resource/v1/attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     num_heads: int
     num_kv_heads: int
     num_layers: int
     ff_intermediate_size: int
     max_length: int
     vocab_size: int
     eos_token: int
+    rope_theta: Optional[float]
     attention_window_size: int
 
 
 class V1OPTAttributes(V1CommonAttributes):
     """V1 OPT attributes schema."""
 
     model_type: Literal["opt"]
```

### Comparing `periflow_client-0.2.1/periflow/schema/resource/v1/checkpoint.py` & `periflow_client-0.2.2/periflow/schema/resource/v1/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/resource/v1/credential.py` & `periflow_client-0.2.2/periflow/schema/resource/v1/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/resource/v1/deployment.py` & `periflow_client-0.2.2/periflow/schema/resource/v1/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/schema/resource/v1/transfer.py` & `periflow_client-0.2.2/periflow/schema/resource/v1/transfer.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/api/base.py` & `periflow_client-0.2.2/periflow/sdk/api/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/api/completion.py` & `periflow_client-0.2.2/periflow/sdk/api/completion.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/api/detokenization.py` & `periflow_client-0.2.2/periflow/sdk/api/detokenization.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/api/tokenization.py` & `periflow_client-0.2.2/periflow/sdk/api/tokenization.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/init.py` & `periflow_client-0.2.2/periflow/sdk/init.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/resource/base.py` & `periflow_client-0.2.2/periflow/sdk/resource/base.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/resource/catalog.py` & `periflow_client-0.2.2/periflow/sdk/resource/catalog.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/resource/checkpoint.py` & `periflow_client-0.2.2/periflow/sdk/resource/checkpoint.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/resource/credential.py` & `periflow_client-0.2.2/periflow/sdk/resource/credential.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/sdk/resource/deployment.py` & `periflow_client-0.2.2/periflow/sdk/resource/deployment.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/decorator.py` & `periflow_client-0.2.2/periflow/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/format.py` & `periflow_client-0.2.2/periflow/utils/format.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/fs.py` & `periflow_client-0.2.2/periflow/utils/fs.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/maps.py` & `periflow_client-0.2.2/periflow/utils/maps.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/prompt.py` & `periflow_client-0.2.2/periflow/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/request.py` & `periflow_client-0.2.2/periflow/utils/request.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/testing.py` & `periflow_client-0.2.2/periflow/utils/testing.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/transfer.py` & `periflow_client-0.2.2/periflow/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/url.py` & `periflow_client-0.2.2/periflow/utils/url.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/validate.py` & `periflow_client-0.2.2/periflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/periflow/utils/version.py` & `periflow_client-0.2.2/periflow/utils/version.py`

 * *Files identical despite different names*

### Comparing `periflow_client-0.2.1/pyproject.toml` & `periflow_client-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "periflow-client"
-version = "0.2.1"
+version = "0.2.2"
 description = "Client of PeriFlow, the fastest generative AI serving available."
 license = "Apache-2.0"
 authors = ["PeriFlow teams <eng@friendli.ai>"]
 packages = [
     { include = "periflow" },
 ]
 readme = "README.md"
```

### Comparing `periflow_client-0.2.1/PKG-INFO` & `periflow_client-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periflow-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Client of PeriFlow, the fastest generative AI serving available.
 Home-page: https://friendli.ai/periflow
 License: Apache-2.0
 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams
 Author-email: eng@friendli.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: periflow-client Version: 0.2.1 Summary: Client of
+Metadata-Version: 2.1 Name: periflow-client Version: 0.2.2 Summary: Client of
 PeriFlow, the fastest generative AI serving available. Home-page: https://
 friendli.ai/periflow License: Apache-2.0 Keywords: generative-ai,serving,llm
 Author: PeriFlow teams Author-email: eng@friendli.ai Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

