# Comparing `tmp/deepmd_kit-2.2.9.tar.gz` & `tmp/deepmd_kit-3.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepmd_kit-2.2.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "deepmd_kit-3.0.0a0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `deepmd_kit-2.2.9.tar` & `deepmd_kit-3.0.0a0.tar`

### file list

```diff
@@ -1,497 +1,655 @@
--rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/.clang-format
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/.git-blame-ignore-revs
--rw-r--r--   0        0        0       89 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/.gitattributes
--rw-r--r--   0        0        0      393 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/.gitignore
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/.license-header.txt
--rw-r--r--   0        0        0     3090 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/.readthedocs.yml
--rw-r--r--   0        0        0    10744 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/CITATIONS.bib
--rw-r--r--   0        0        0     4765 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/CONTRIBUTING.md
--rw-r--r--   0        0        0     7652 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/LICENSE
--rw-r--r--   0        0        0    13962 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/README.md
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/backend/__init__.py
--rw-r--r--   0        0        0     1173 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/backend/dp_backend.py
--rw-r--r--   0        0        0     2514 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/backend/dynamic_metadata.py
--rw-r--r--   0        0        0     7183 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/backend/find_tensorflow.py
--rw-r--r--   0        0        0     3698 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/backend/read_env.py
--rw-r--r--   0        0        0      950 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/codecov.yml
--rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/.gitignore
--rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/__about__.py
--rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/__init__.py
--rw-r--r--   0        0        0      159 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/__main__.py
--rw-r--r--   0        0        0     4334 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/calculator.py
--rw-r--r--   0        0        0      691 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/cluster/__init__.py
--rw-r--r--   0        0        0     1771 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/cluster/local.py
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/cluster/slurm.py
--rw-r--r--   0        0        0     6942 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/common.py
--rw-r--r--   0        0        0      887 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/__init__.py
--rw-r--r--   0        0        0    16295 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/descriptor.py
--rw-r--r--   0        0        0    14085 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/hybrid.py
--rw-r--r--   0        0        0    15405 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/loc_frame.py
--rw-r--r--   0        0        0     4594 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se.py
--rw-r--r--   0        0        0    51425 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_a.py
--rw-r--r--   0        0        0    20691 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_a_ebd.py
--rw-r--r--   0        0        0     1766 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_a_ebd_v2.py
--rw-r--r--   0        0        0    19821 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_a_ef.py
--rw-r--r--   0        0        0    16217 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_a_mask.py
--rw-r--r--   0        0        0    54251 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_atten.py
--rw-r--r--   0        0        0     3836 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_atten_v2.py
--rw-r--r--   0        0        0    24177 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_r.py
--rw-r--r--   0        0        0    25059 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/descriptor/se_t.py
--rw-r--r--   0        0        0      851 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/__init__.py
--rw-r--r--   0        0        0     6309 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/compress.py
--rw-r--r--   0        0        0     1316 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/convert.py
--rw-r--r--   0        0        0      142 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/doc.py
--rwxr-xr-x   0        0        0    18510 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/freeze.py
--rw-r--r--   0        0        0      134 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/gui.py
--rw-r--r--   0        0        0      664 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/ipi.py
--rw-r--r--   0        0        0     2541 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/main.py
--rw-r--r--   0        0        0     1623 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/neighbor_stat.py
--rw-r--r--   0        0        0    31240 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/test.py
--rwxr-xr-x   0        0        0    15792 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/train.py
--rw-r--r--   0        0        0     8059 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/entrypoints/transfer.py
--rw-r--r--   0        0        0    15303 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/env.py
--rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/fit/__init__.py
--rw-r--r--   0        0        0    11432 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/fit/dipole.py
--rw-r--r--   0        0        0    23647 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/fit/dos.py
--rw-r--r--   0        0        0    36575 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/fit/ener.py
--rw-r--r--   0        0        0     2495 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/fit/fitting.py
--rw-r--r--   0        0        0    25317 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/fit/polar.py
--rw-r--r--   0        0        0     3597 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/__init__.py
--rw-r--r--   0        0        0    16265 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/data_modifier.py
--rw-r--r--   0        0        0     2092 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/deep_dipole.py
--rw-r--r--   0        0        0    16639 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/deep_dos.py
--rw-r--r--   0        0        0    15599 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/deep_eval.py
--rw-r--r--   0        0        0     4749 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/deep_polar.py
--rw-r--r--   0        0        0    23827 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/deep_pot.py
--rw-r--r--   0        0        0    15224 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/deep_tensor.py
--rw-r--r--   0        0        0     1876 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/deep_wfc.py
--rw-r--r--   0        0        0     2691 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/ewald_recp.py
--rw-r--r--   0        0        0    15906 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/infer/model_devi.py
--rw-r--r--   0        0        0     2939 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/lmp.py
--rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/loggers/__init__.py
--rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/loggers/loggers.py
--rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/loss/__init__.py
--rw-r--r--   0        0        0     7930 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/loss/dos.py
--rw-r--r--   0        0        0    32591 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/loss/ener.py
--rw-r--r--   0        0        0     2284 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/loss/loss.py
--rw-r--r--   0        0        0     5683 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/loss/tensor.py
--rw-r--r--   0        0        0      392 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/__init__.py
--rw-r--r--   0        0        0     7198 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/dos.py
--rw-r--r--   0        0        0    18519 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/ener.py
--rw-r--r--   0        0        0     6241 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/frozen.py
--rw-r--r--   0        0        0     8585 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/linear.py
--rw-r--r--   0        0        0    23293 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/model.py
--rw-r--r--   0        0        0      299 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/model_stat.py
--rw-r--r--   0        0        0    24375 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/multi.py
--rw-r--r--   0        0        0     8570 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/pairtab.py
--rw-r--r--   0        0        0    14692 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/pairwise_dprc.py
--rw-r--r--   0        0        0     8166 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/model/tensor.py
--rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/__init__.py
--rw-r--r--   0        0        0     1006 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/data/__init__.py
--rw-r--r--   0        0        0    10960 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/data/data.py
--rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/descriptor/__init__.py
--rw-r--r--   0        0        0    12622 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/descriptor/se_a.py
--rw-r--r--   0        0        0    11291 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/descriptor/se_atten.py
--rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/__init__.py
--rw-r--r--   0        0        0     2809 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/freeze.py
--rw-r--r--   0        0        0    22407 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/mapt.py
--rw-r--r--   0        0        0     6264 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/train.py
--rw-r--r--   0        0        0    20955 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/wrap.py
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/fit/__init__.py
--rw-r--r--   0        0        0      334 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/fit/ener.py
--rw-r--r--   0        0        0      554 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/utils/__init__.py
--rw-r--r--   0        0        0      184 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/utils/argcheck.py
--rw-r--r--   0        0        0    15578 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/utils/config.py
--rw-r--r--   0        0        0     7755 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/utils/encode.py
--rw-r--r--   0        0        0     6129 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/utils/fio.py
--rw-r--r--   0        0        0     8572 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/utils/network.py
--rw-r--r--   0        0        0      521 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/utils/op.py
--rw-r--r--   0        0        0     4954 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/nvnmd/utils/weight.py
--rw-r--r--   0        0        0      799 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/__init__.py
--rw-r--r--   0        0        0      303 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_add_flt_nvnmd_grad.py
--rw-r--r--   0        0        0      309 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_copy_flt_nvnmd_grad.py
--rw-r--r--   0        0        0      679 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_dotmul_flt_nvnmd_grad.py
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_flt_nvnmd_grad.py
--rw-r--r--   0        0        0     1017 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_gelu.py
--rw-r--r--   0        0        0      945 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_map_flt_nvnmd_grad.py
--rw-r--r--   0        0        0      542 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_matmul_fitnet_nvnmd_grad.py
--rw-r--r--   0        0        0     1014 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_matmul_flt2fix_nvnmd.py
--rw-r--r--   0        0        0     1254 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_matmul_flt_nvnmd_grad.py
--rw-r--r--   0        0        0      871 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_mul_flt_nvnmd_grad.py
--rw-r--r--   0        0        0      579 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_prod_force_grad.py
--rw-r--r--   0        0        0      564 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_prod_force_se_a_grad.py
--rw-r--r--   0        0        0      562 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_prod_force_se_a_mask_grad.py
--rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_prod_force_se_r_grad.py
--rw-r--r--   0        0        0      622 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_prod_virial_grad.py
--rw-r--r--   0        0        0      607 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_prod_virial_se_a_grad.py
--rw-r--r--   0        0        0      486 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_prod_virial_se_r_grad.py
--rw-r--r--   0        0        0      460 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_quantize_nvnmd_grad.py
--rw-r--r--   0        0        0      566 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_soft_min_force_grad.py
--rw-r--r--   0        0        0      609 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_soft_min_virial_grad.py
--rw-r--r--   0        0        0     2956 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_tabulate_grad.py
--rw-r--r--   0        0        0     1075 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/op/_tanh4_flt_nvnmd_grad.py
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/train/__init__.py
--rw-r--r--   0        0        0     8735 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/train/run_options.py
--rw-r--r--   0        0        0    49632 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/train/trainer.py
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/__init__.py
--rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/argcheck.py
--rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/batch_size.py
--rw-r--r--   0        0        0      350 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/compat.py
--rw-r--r--   0        0        0     3410 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/compress.py
--rw-r--r--   0        0        0    12350 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/convert.py
--rw-r--r--   0        0        0      174 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/data.py
--rw-r--r--   0        0        0      289 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/data_system.py
--rw-r--r--   0        0        0      372 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/errors.py
--rw-r--r--   0        0        0     4189 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/finetune.py
--rw-r--r--   0        0        0    17492 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/graph.py
--rw-r--r--   0        0        0     3225 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/learning_rate.py
--rw-r--r--   0        0        0     7051 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/multi_init.py
--rw-r--r--   0        0        0     5629 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/neighbor_stat.py
--rw-r--r--   0        0        0    10799 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/network.py
--rw-r--r--   0        0        0      172 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/pair_tab.py
--rw-r--r--   0        0        0     2817 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/parallel_op.py
--rw-r--r--   0        0        0      226 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/path.py
--rw-r--r--   0        0        0      286 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/plugin.py
--rw-r--r--   0        0        0      244 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/random.py
--rw-r--r--   0        0        0     1611 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/sess.py
--rw-r--r--   0        0        0     2553 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/spin.py
--rw-r--r--   0        0        0    35468 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/tabulate.py
--rw-r--r--   0        0        0     6120 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/type_embed.py
--rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd/utils/weight_avg.py
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/__init__.py
--rw-r--r--   0        0        0     7113 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/common.py
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/entrypoints/__init__.py
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/entrypoints/doc.py
--rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/entrypoints/gui.py
--rw-r--r--   0        0        0      804 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/env.py
--rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/loggers/__init__.py
--rw-r--r--   0        0        0     8828 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/loggers/loggers.py
--rw-r--r--   0        0        0    20639 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/main.py
--rw-r--r--   0        0        0     1185 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/model_format/__init__.py
--rw-r--r--   0        0        0      634 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/model_format/common.py
--rw-r--r--   0        0        0     3348 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/model_format/env_mat.py
--rw-r--r--   0        0        0    19959 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/model_format/network.py
--rw-r--r--   0        0        0     8002 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/model_format/output_def.py
--rw-r--r--   0        0        0     9688 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/model_format/se_e2_a.py
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/__init__.py
--rw-r--r--   0        0        0    93328 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/argcheck.py
--rw-r--r--   0        0        0     2609 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/argcheck_nvnmd.py
--rw-r--r--   0        0        0     7656 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/batch_size.py
--rw-r--r--   0        0        0    10903 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/compat.py
--rw-r--r--   0        0        0    21796 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/data.py
--rw-r--r--   0        0        0    24262 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/data_system.py
--rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/errors.py
--rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/model_stat.py
--rw-r--r--   0        0        0     3367 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/pair_tab.py
--rw-r--r--   0        0        0     8888 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/path.py
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/plugin.py
--rw-r--r--   0        0        0     1323 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/random.py
--rw-r--r--   0        0        0     1358 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/deepmd_utils/utils/weight_avg.py
--rw-r--r--   0        0        0     8110 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/pyproject.toml
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/aarch64/config.ini
--rw-r--r--   0        0        0     2058 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/aarch64/table.S.tpl
--rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/aarch64/trampoline.S.tpl
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/arm/config.ini
--rw-r--r--   0        0        0     2486 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/arm/table.S.tpl
--rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/arm/trampoline.S.tpl
--rw-r--r--   0        0        0     4055 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/common/init.c.tpl
--rw-r--r--   0        0        0      428 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/e2k/README.md
--rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/e2k/config.ini
--rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/e2k/table.S.tpl
--rw-r--r--   0        0        0      958 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/e2k/trampoline.S.tpl
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/i386/config.ini
--rw-r--r--   0        0        0     1971 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/i386/table.S.tpl
--rw-r--r--   0        0        0      818 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/i386/trampoline.S.tpl
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips/config.ini
--rw-r--r--   0        0        0     2231 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips/table.S.tpl
--rw-r--r--   0        0        0     1185 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips/trampoline.S.tpl
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips64/config.ini
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips64/table.S.tpl
--rw-r--r--   0        0        0     1391 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips64/trampoline.S.tpl
--rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/x86_64/config.ini
--rw-r--r--   0        0        0     2547 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/x86_64/table.S.tpl
--rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/arch/x86_64/trampoline.S.tpl
--rwxr-xr-x   0        0        0    19283 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/implib/implib-gen.py
--rw-r--r--   0        0        0   926233 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/3rdparty/json.hpp
--rw-r--r--   0        0        0     9810 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/CMakeLists.txt
--rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_c/CMakeLists.txt
--rw-r--r--   0        0        0    55795 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_c/include/c_api.h
--rw-r--r--   0        0        0     1730 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_c/include/c_api_internal.h
--rw-r--r--   0        0        0    86366 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_c/include/deepmd.hpp
--rw-r--r--   0        0        0    59111 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_c/src/c_api.cc
--rw-r--r--   0        0        0     1925 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/CMakeLists.txt
--rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/AtomMap.h
--rw-r--r--   0        0        0     6076 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/DataModifier.h
--rw-r--r--   0        0        0     4574 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/DataModifierTF.h
--rw-r--r--   0        0        0    33226 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/DeepPot.h
--rw-r--r--   0        0        0    14167 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/DeepPotTF.h
--rw-r--r--   0        0        0    13697 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/DeepTensor.h
--rw-r--r--   0        0        0    12872 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/DeepTensorTF.h
--rw-r--r--   0        0        0    11789 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/common.h
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/tf_private.h
--rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/tf_public.h
--rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/include/version.h.in
--rw-r--r--   0        0        0     3579 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/src/AtomMap.cc
--rw-r--r--   0        0        0     3254 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/src/DataModifier.cc
--rw-r--r--   0        0        0    13007 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/src/DataModifierTF.cc
--rw-r--r--   0        0        0    37976 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/src/DeepPot.cc
--rw-r--r--   0        0        0    40738 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/src/DeepPotTF.cc
--rw-r--r--   0        0        0    11843 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/src/DeepTensor.cc
--rw-r--r--   0        0        0    34547 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/src/DeepTensorTF.cc
--rw-r--r--   0        0        0    45764 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/api_cc/src/common.cc
--rw-r--r--   0        0        0      159 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/Config.cmake.in
--rw-r--r--   0        0        0    17519 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/Findtensorflow.cmake
--rw-r--r--   0        0        0     1688 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/Findxdrfile.cmake
--rw-r--r--   0        0        0      568 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/cmake_lammps.cmake.in
--rw-r--r--   0        0        0     1035 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/coverage_config/CMakeLists.txt
--rw-r--r--   0        0        0      632 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/googletest.cmake.in
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/test_cxx_abi.cpp
--rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/tf_cxx_abi.cpp
--rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/cmake/tf_version.cpp
--rw-r--r--   0        0        0      211 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/config/CMakeLists.txt
--rw-r--r--   0        0        0        4 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/config/MODEL_VER
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/config/__init__.py
--rw-r--r--   0        0        0      336 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/config/run_config.ini
--rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/.gitignore
--rw-r--r--   0        0        0     1576 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/CMakeLists.txt
--rw-r--r--   0        0        0     3805 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/dp_gmx_patch
--rw-r--r--   0        0        0      713 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/include/gmx_plugin.h
--rw-r--r--   0        0        0     1077 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/patches/2020.2/CMakeLists.txt.patch.in
--rw-r--r--   0        0        0     1111 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/patches/2020.2/src/gromacs/mdlib/forcerec.cpp.patch
--rw-r--r--   0        0        0      509 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/patches/2020.2/src/gromacs/mdlib/forcerec.h.patch
--rw-r--r--   0        0        0     3472 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/patches/2020.2/src/gromacs/mdlib/sim_util.cpp.patch
--rw-r--r--   0        0        0     3087 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/gmx/src/gmx_plugin.cpp
--rwxr-xr-x   0        0        0      788 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/build_cc.sh
--rwxr-xr-x   0        0        0      642 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/build_from_c.sh
--rwxr-xr-x   0        0        0     1158 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/build_lammps.sh
--rwxr-xr-x   0        0        0    27474 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/build_tf.py
--rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/docker/Dockerfile
--rwxr-xr-x   0        0        0      427 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/docker_package_c.sh
--rwxr-xr-x   0        0        0      748 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/docker_test_package_c.sh
--rwxr-xr-x   0        0        0     1294 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/install_tf.sh
--rwxr-xr-x   0        0        0      770 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/package_c.sh
--rwxr-xr-x   0        0        0      662 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/test_cc.sh
--rwxr-xr-x   0        0        0      709 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/install/test_cc_local.sh
--rw-r--r--   0        0        0     2255 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/CMakeLists.txt
--rw-r--r--   0        0        0     7129 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/driver.cc
--rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/include/Convert.h
--rw-r--r--   0        0        0      861 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/include/StringSplit.h
--rw-r--r--   0        0        0      434 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/include/XyzFileManager.h
--rw-r--r--   0        0        0     1457 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/include/sockets.h
--rw-r--r--   0        0        0     1921 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/src/Convert.cc
--rw-r--r--   0        0        0     2510 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/src/XyzFileManager.cc
--rw-r--r--   0        0        0     4881 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/src/sockets.c
--rw-r--r--   0        0        0     7319 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/ipi/tests/test_driver.py
--rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/CMakeLists.txt
--rw-r--r--   0        0        0    44520 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/ComputeDescriptor.h
--rw-r--r--   0        0        0     4478 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/DeviceFunctor.h
--rw-r--r--   0        0        0     5638 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/SimulationRegion.h
--rw-r--r--   0        0        0    15145 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/SimulationRegion_Impl.h
--rw-r--r--   0        0        0     2825 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/coord.h
--rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/device.h
--rw-r--r--   0        0        0     2403 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/env_mat.h
--rw-r--r--   0        0        0     4818 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/env_mat_nvnmd.h
--rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/errors.h
--rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/ewald.h
--rw-r--r--   0        0        0     2951 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/fmt_nlist.h
--rw-r--r--   0        0        0     1213 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/gelu.h
--rw-r--r--   0        0        0     5646 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/gpu_cuda.h
--rw-r--r--   0        0        0     4030 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/gpu_rocm.h
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/map_aparam.h
--rw-r--r--   0        0        0     7906 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/neighbor_list.h
--rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/neighbor_stat.h
--rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/pair_tab.h
--rw-r--r--   0        0        0     1895 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/pairwise.h
--rw-r--r--   0        0        0     3520 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/prod_env_mat.h
--rw-r--r--   0        0        0     1710 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/prod_env_mat_nvnmd.h
--rw-r--r--   0        0        0     3340 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/prod_force.h
--rw-r--r--   0        0        0     1588 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/prod_force_grad.h
--rw-r--r--   0        0        0     1820 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/prod_virial.h
--rw-r--r--   0        0        0     1616 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/prod_virial_grad.h
--rw-r--r--   0        0        0     2034 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/region.cuh
--rw-r--r--   0        0        0     1331 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/region.h
--rw-r--r--   0        0        0      504 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/soft_min_switch.h
--rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/soft_min_switch_force.h
--rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/soft_min_switch_force_grad.h
--rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/soft_min_switch_virial.h
--rw-r--r--   0        0        0      501 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/soft_min_switch_virial_grad.h
--rw-r--r--   0        0        0     2266 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/switcher.h
--rw-r--r--   0        0        0    10773 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/tabulate.h
--rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/include/utilities.h
--rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/SimulationRegion.cpp
--rw-r--r--   0        0        0     5140 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/coord.cc
--rw-r--r--   0        0        0    16610 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/env_mat.cc
--rw-r--r--   0        0        0     4712 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/env_mat_nvnmd.cc
--rw-r--r--   0        0        0    10575 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/ewald.cc
--rw-r--r--   0        0        0     7678 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/fmt_nlist.cc
--rw-r--r--   0        0        0     3514 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gelu.cc
--rw-r--r--   0        0        0     3679 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/CMakeLists.txt
--rw-r--r--   0        0        0    17312 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/coord.cu
--rw-r--r--   0        0        0     1340 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/cudart/CMakeLists.txt
--rw-r--r--   0        0        0     1266 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/cudart/cudart_stub.cc
--rw-r--r--   0        0        0     5161 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/gelu.cu
--rw-r--r--   0        0        0    10958 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/neighbor_list.cu
--rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/neighbor_stat.cu
--rw-r--r--   0        0        0    36252 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/prod_env_mat.cu
--rw-r--r--   0        0        0     7770 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/prod_force.cu
--rw-r--r--   0        0        0     7135 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/prod_force_grad.cu
--rw-r--r--   0        0        0     8083 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/prod_virial.cu
--rw-r--r--   0        0        0     6230 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/prod_virial_grad.cu
--rw-r--r--   0        0        0     2580 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/region.cu
--rw-r--r--   0        0        0    45842 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/gpu/tabulate.cu
--rw-r--r--   0        0        0     1883 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/map_aparam.cc
--rw-r--r--   0        0        0    34199 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/neighbor_list.cc
--rw-r--r--   0        0        0     7232 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/pair_tab.cc
--rw-r--r--   0        0        0     4883 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/pairwise.cc
--rw-r--r--   0        0        0    12954 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/prod_env_mat.cc
--rw-r--r--   0        0        0     5435 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/prod_env_mat_nvnmd.cc
--rw-r--r--   0        0        0     8764 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/prod_force.cc
--rw-r--r--   0        0        0     5718 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/prod_force_grad.cc
--rw-r--r--   0        0        0     5851 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/prod_virial.cc
--rw-r--r--   0        0        0     5165 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/prod_virial_grad.cc
--rw-r--r--   0        0        0     5157 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/region.cc
--rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/soft_min_switch.cc
--rw-r--r--   0        0        0     2524 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/soft_min_switch_force.cc
--rw-r--r--   0        0        0     1939 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/soft_min_switch_force_grad.cc
--rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/soft_min_switch_virial.cc
--rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/soft_min_switch_virial_grad.cc
--rw-r--r--   0        0        0    35571 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/tabulate.cc
--rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lib/src/utilities.cc
--rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/CMakeLists.txt
--rw-r--r--   0        0        0     1433 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/Install.sh
--rw-r--r--   0        0        0     1390 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/builtin.cmake
--rw-r--r--   0        0        0     5420 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/compute_deeptensor_atom.cpp
--rw-r--r--   0        0        0     1101 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/compute_deeptensor_atom.h
--rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/deepmd_version.h.in
--rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/env.sh.in
--rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/env_c.sh.in
--rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/env_py.sh.in
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/env_py_c.sh.in
--rw-r--r--   0        0        0    24404 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/fix_dplr.cpp
--rw-r--r--   0        0        0     2165 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/fix_dplr.h
--rw-r--r--   0        0        0      397 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/fix_ttm_dp.h
--rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/lammps_install_list.txt.in
--rwxr-xr-x   0        0        0      290 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/lmp_version.sh
--rw-r--r--   0        0        0    51354 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/pair_deepmd.cpp
--rw-r--r--   0        0        0     4060 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/pair_deepmd.h
--rw-r--r--   0        0        0     4953 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/plugin/CMakeLists.txt
--rw-r--r--   0        0        0     1922 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/plugin/deepmdplugin.cpp
--rw-r--r--   0        0        0    12614 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/pppm_dplr.cpp
--rw-r--r--   0        0        0      802 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/lmp/pppm_dplr.h
--rw-r--r--   0        0        0     3203 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/CMakeLists.txt
--rw-r--r--   0        0        0     2308 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/AdWeight.h
--rw-r--r--   0        0        0     1596 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/Convert.h
--rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/CosSwitch.h
--rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/Gaussian.h
--rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/GroFileManager.h
--rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/HarmonicAngle.h
--rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/HarmonicBond.h
--rw-r--r--   0        0        0     1408 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/Integrator.h
--rw-r--r--   0        0        0     2773 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/Interpolation.h
--rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/LJInter.h
--rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/LJTab.h
--rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/MaxShift.h
--rw-r--r--   0        0        0     2112 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/Poly.h
--rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/RandomGenerator.h
--rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/Statistics.h
--rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/StringSplit.h
--rw-r--r--   0        0        0      539 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/TF.h
--rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/TableFileLoader.h
--rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/Tabulated.h
--rw-r--r--   0        0        0     1354 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/Trajectory.h
--rw-r--r--   0        0        0      570 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/UnitManager.h
--rw-r--r--   0        0        0      558 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/XyzFileManager.h
--rw-r--r--   0        0        0     1399 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/ZM.h
--rw-r--r--   0        0        0     1087 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/ZMFunctions.h
--rw-r--r--   0        0        0     1107 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/common.h
--rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/include/mymath.h
--rw-r--r--   0        0        0     6548 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/mdnn.cc
--rw-r--r--   0        0        0     8393 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/AdWeight.cc
--rw-r--r--   0        0        0     3997 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/Convert.cc
--rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/Gaussian.cc
--rw-r--r--   0        0        0     8092 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/GroFileManager.cc
--rw-r--r--   0        0        0     3467 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/HarmonicAngle.cc
--rw-r--r--   0        0        0     1571 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/HarmonicBond.cc
--rw-r--r--   0        0        0     3381 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/Integrator.cc
--rw-r--r--   0        0        0    16877 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/Interpolation.cpp
--rw-r--r--   0        0        0     2621 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/LJInter.cc
--rw-r--r--   0        0        0      852 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/LJTab.cc
--rw-r--r--   0        0        0     1047 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/MaxShift.cc
--rw-r--r--   0        0        0     6719 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/Poly.cpp
--rw-r--r--   0        0        0     6215 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/RandomGenerator_MT19937.cc
--rw-r--r--   0        0        0     3580 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/Statistics.cc
--rw-r--r--   0        0        0     1077 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/StringSplit.cpp
--rw-r--r--   0        0        0     1400 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/TF.cc
--rw-r--r--   0        0        0     2286 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/TableFileLoader.cpp
--rw-r--r--   0        0        0     5198 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/Tabulated.cc
--rw-r--r--   0        0        0     3355 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/Trajectory.cc
--rw-r--r--   0        0        0      963 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/UnitManager.cc
--rw-r--r--   0        0        0     3266 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/XyzFileManager.cc
--rw-r--r--   0        0        0     2227 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/ZM.cc
--rw-r--r--   0        0        0     6693 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/md/src/ZMFunctions.cpp
--rw-r--r--   0        0        0     2091 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/.gitignore
--rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/.npmignore
--rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/CMakeLists.txt
--rw-r--r--   0        0        0     1287 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/README.md
--rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/binding.gyp.in
--rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/binding.gyp.pack
--rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/index.js
--rw-r--r--   0        0        0      801 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/package.json
--rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/prepublish.py
--rw-r--r--   0        0        0     1088 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/tests/test_deeppot.js
--rw-r--r--   0        0        0    29759 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/nodejs/yarn.lock
--rw-r--r--   0        0        0     2736 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/CMakeLists.txt
--rw-r--r--   0        0        0     2726 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/add_flt_nvnmd.cc
--rw-r--r--   0        0        0     2525 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/copy_flt_nvnmd.cc
--rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/custom_op.cc
--rw-r--r--   0        0        0     2130 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/custom_op.h
--rw-r--r--   0        0        0    24439 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/descrpt.cc
--rw-r--r--   0        0        0    16142 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/descrpt_se_a_ef.cc
--rw-r--r--   0        0        0    16178 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/descrpt_se_a_ef_para.cc
--rw-r--r--   0        0        0    16178 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/descrpt_se_a_ef_vert.cc
--rw-r--r--   0        0        0    14156 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/descrpt_se_a_mask.cc
--rw-r--r--   0        0        0     4324 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/dotmul_flt_nvnmd.cc
--rw-r--r--   0        0        0     5319 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/ewald_recp.cc
--rw-r--r--   0        0        0     2269 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/flt_nvnmd.cc
--rw-r--r--   0        0        0     8314 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/gelu_multi_device.cc
--rw-r--r--   0        0        0     3576 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/map_aparam.cc
--rw-r--r--   0        0        0     4206 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/map_flt_nvnmd.cc
--rw-r--r--   0        0        0     4499 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/matmul_fitnet_nvnmd.cc
--rw-r--r--   0        0        0     3896 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/matmul_flt2fix_nvnmd.cc
--rw-r--r--   0        0        0     5575 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/matmul_flt_nvnmd.cc
--rw-r--r--   0        0        0     3207 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/mul_flt_nvnmd.cc
--rw-r--r--   0        0        0    12902 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/neighbor_stat.cc
--rw-r--r--   0        0        0     5436 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/optimizer/parallel.cc
--rw-r--r--   0        0        0     1000 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/optimizer/parallel.h
--rw-r--r--   0        0        0     7840 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/pair_tab.cc
--rw-r--r--   0        0        0    15684 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/pairwise.cc
--rw-r--r--   0        0        0    79958 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_env_mat_multi_device.cc
--rw-r--r--   0        0        0    35316 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_env_mat_multi_device_nvnmd.cc
--rw-r--r--   0        0        0     8861 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_force.cc
--rw-r--r--   0        0        0     8386 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_force_grad.cc
--rw-r--r--   0        0        0    12373 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_force_grad_multi_device.cc
--rw-r--r--   0        0        0    12601 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_force_multi_device.cc
--rw-r--r--   0        0        0     5537 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_force_se_a_grad.cc
--rw-r--r--   0        0        0     5983 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_force_se_a_mask.cc
--rw-r--r--   0        0        0     6108 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_force_se_a_mask_grad.cc
--rw-r--r--   0        0        0     4765 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_force_se_r_grad.cc
--rw-r--r--   0        0        0     9217 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_virial.cc
--rw-r--r--   0        0        0     9082 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_virial_grad.cc
--rw-r--r--   0        0        0    14592 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_virial_grad_multi_device.cc
--rw-r--r--   0        0        0    12812 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_virial_multi_device.cc
--rw-r--r--   0        0        0     6233 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_virial_se_a_grad.cc
--rw-r--r--   0        0        0     5461 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/prod_virial_se_r_grad.cc
--rw-r--r--   0        0        0     3375 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/quantize_nvnmd.cc
--rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/readme
--rw-r--r--   0        0        0     5704 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/soft_min.cc
--rw-r--r--   0        0        0     4138 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/soft_min_force.cc
--rw-r--r--   0        0        0     4936 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/soft_min_force_grad.cc
--rw-r--r--   0        0        0     5251 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/soft_min_virial.cc
--rw-r--r--   0        0        0     5964 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/soft_min_virial_grad.cc
--rw-r--r--   0        0        0    49880 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/tabulate_multi_device.cc
--rw-r--r--   0        0        0     3365 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/tanh4_flt_nvnmd.cc
--rw-r--r--   0        0        0    17595 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/op/unaggregated_grad.cc
--rw-r--r--   0        0        0      859 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/source/swig/deepmd.i
--rw-r--r--   0        0        0    32465 2022-11-09 12:37:21.000000 deepmd_kit-2.2.9/PKG-INFO
+-rw-r--r--   0        0        0       73 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/.clang-format
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      140 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/.gitattributes
+-rw-r--r--   0        0        0      404 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/.gitignore
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/.license-header.txt
+-rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/.readthedocs.yml
+-rw-r--r--   0        0        0    11799 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/CITATIONS.bib
+-rw-r--r--   0        0        0     4780 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     7652 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/LICENSE
+-rw-r--r--   0        0        0     8659 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/README.md
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/backend/__init__.py
+-rw-r--r--   0        0        0     1173 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/backend/dp_backend.py
+-rw-r--r--   0        0        0     2608 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/backend/dynamic_metadata.py
+-rw-r--r--   0        0        0     7718 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/backend/find_tensorflow.py
+-rw-r--r--   0        0        0     4017 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/backend/read_env.py
+-rw-r--r--   0        0        0      924 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/codecov.yml
+-rw-r--r--   0        0        0       26 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/.gitignore
+-rw-r--r--   0        0        0      953 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/__init__.py
+-rw-r--r--   0        0        0      153 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/__main__.py
+-rw-r--r--   0        0        0      765 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/backend/__init__.py
+-rw-r--r--   0        0        0     4929 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/backend/backend.py
+-rw-r--r--   0        0        0     2976 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/backend/dpmodel.py
+-rw-r--r--   0        0        0     3048 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/backend/pytorch.py
+-rw-r--r--   0        0        0     2638 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/backend/suffix.py
+-rw-r--r--   0        0        0     3291 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/backend/tensorflow.py
+-rw-r--r--   0        0        0     4331 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/calculator.py
+-rw-r--r--   0        0        0     8996 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/common.py
+-rw-r--r--   0        0        0      655 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/__init__.py
+-rw-r--r--   0        0        0     1051 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/atomic_model/__init__.py
+-rw-r--r--   0        0        0     3448 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/atomic_model/base_atomic_model.py
+-rw-r--r--   0        0        0     5205 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/atomic_model/dp_atomic_model.py
+-rw-r--r--   0        0        0    11634 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/atomic_model/linear_atomic_model.py
+-rw-r--r--   0        0        0     5981 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/atomic_model/make_base_atomic_model.py
+-rw-r--r--   0        0        0    11971 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/atomic_model/pairtab_atomic_model.py
+-rw-r--r--   0        0        0     1166 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/common.py
+-rw-r--r--   0        0        0      331 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/descriptor/__init__.py
+-rw-r--r--   0        0        0      189 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/descriptor/base_descriptor.py
+-rw-r--r--   0        0        0     8656 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/descriptor/hybrid.py
+-rw-r--r--   0        0        0     4577 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/descriptor/make_base_descriptor.py
+-rw-r--r--   0        0        0    14676 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/descriptor/se_e2_a.py
+-rw-r--r--   0        0        0    11539 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/descriptor/se_r.py
+-rw-r--r--   0        0        0      438 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/fitting/__init__.py
+-rw-r--r--   0        0        0      192 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/fitting/base_fitting.py
+-rw-r--r--   0        0        0     7573 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/fitting/dipole_fitting.py
+-rw-r--r--   0        0        0     2210 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/fitting/ener_fitting.py
+-rw-r--r--   0        0        0    14335 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/fitting/general_fitting.py
+-rw-r--r--   0        0        0     8515 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/fitting/invar_fitting.py
+-rw-r--r--   0        0        0     2632 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/fitting/make_base_fitting.py
+-rw-r--r--   0        0        0     8887 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/fitting/polarizability_fitting.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/infer/__init__.py
+-rw-r--r--   0        0        0    11875 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/infer/deep_eval.py
+-rw-r--r--   0        0        0      587 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/model/__init__.py
+-rw-r--r--   0        0        0     5259 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/model/base_model.py
+-rw-r--r--   0        0        0     1021 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/model/dp_model.py
+-rw-r--r--   0        0        0    13031 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/model/make_model.py
+-rw-r--r--   0        0        0     1243 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/model/model.py
+-rw-r--r--   0        0        0     2566 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/model/transform_output.py
+-rw-r--r--   0        0        0    13688 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/output_def.py
+-rw-r--r--   0        0        0     1300 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/__init__.py
+-rw-r--r--   0        0        0      677 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/batch_size.py
+-rw-r--r--   0        0        0     3813 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/env_mat.py
+-rw-r--r--   0        0        0     3539 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/exclude_mask.py
+-rw-r--r--   0        0        0     4431 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/neighbor_stat.py
+-rw-r--r--   0        0        0    21553 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/network.py
+-rw-r--r--   0        0        0     8223 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/nlist.py
+-rw-r--r--   0        0        0     2442 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/region.py
+-rw-r--r--   0        0        0      432 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/update_sel.py
+-rw-r--r--   0        0        0     2506 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/driver.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/entrypoints/__init__.py
+-rw-r--r--   0        0        0      685 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/entrypoints/convert_backend.py
+-rw-r--r--   0        0        0      538 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/entrypoints/doc.py
+-rw-r--r--   0        0        0      830 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/entrypoints/gui.py
+-rw-r--r--   0        0        0     2211 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/entrypoints/main.py
+-rw-r--r--   0        0        0     2329 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/entrypoints/neighbor_stat.py
+-rw-r--r--   0        0        0    32033 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/entrypoints/test.py
+-rw-r--r--   0        0        0     4508 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/env.py
+-rw-r--r--   0        0        0      175 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/__init__.py
+-rw-r--r--   0        0        0      825 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/deep_dipole.py
+-rw-r--r--   0        0        0     4336 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/deep_dos.py
+-rw-r--r--   0        0        0    17393 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/deep_eval.py
+-rw-r--r--   0        0        0     2770 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/deep_polar.py
+-rw-r--r--   0        0        0     5692 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/deep_pot.py
+-rw-r--r--   0        0        0     7193 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/deep_tensor.py
+-rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/deep_wfc.py
+-rw-r--r--   0        0        0    15833 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/infer/model_devi.py
+-rw-r--r--   0        0        0      167 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/loggers/__init__.py
+-rw-r--r--   0        0        0     8856 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/loggers/loggers.py
+-rw-r--r--   0        0        0      763 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/loggers/training.py
+-rw-r--r--   0        0        0    25457 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/main.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/__init__.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/entrypoints/__init__.py
+-rw-r--r--   0        0        0     9507 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/entrypoints/main.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/infer/__init__.py
+-rw-r--r--   0        0        0    20691 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/infer/deep_eval.py
+-rw-r--r--   0        0        0    14915 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/infer/inference.py
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/loss/__init__.py
+-rw-r--r--   0        0        0     3985 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/loss/denoise.py
+-rw-r--r--   0        0        0    10277 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/loss/ener.py
+-rw-r--r--   0        0        0      649 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/loss/loss.py
+-rw-r--r--   0        0        0     5854 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/loss/tensor.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/__init__.py
+-rw-r--r--   0        0        0      952 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/atomic_model/__init__.py
+-rw-r--r--   0        0        0     3749 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/atomic_model/base_atomic_model.py
+-rw-r--r--   0        0        0     7274 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/atomic_model/dp_atomic_model.py
+-rw-r--r--   0        0        0    12979 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/atomic_model/linear_atomic_model.py
+-rw-r--r--   0        0        0    13371 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/atomic_model/pairtab_atomic_model.py
+-rw-r--r--   0        0        0      197 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/backbone/__init__.py
+-rw-r--r--   0        0        0      292 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/backbone/backbone.py
+-rw-r--r--   0        0        0     3828 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/backbone/evoformer2b.py
+-rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/__init__.py
+-rw-r--r--   0        0        0      191 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/base_descriptor.py
+-rw-r--r--   0        0        0     5193 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/descriptor.py
+-rw-r--r--   0        0        0     9305 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/dpa1.py
+-rw-r--r--   0        0        0    18554 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/dpa2.py
+-rw-r--r--   0        0        0     2379 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/env_mat.py
+-rw-r--r--   0        0        0    12006 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/gaussian_lcc.py
+-rw-r--r--   0        0        0    20186 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/hybrid.py
+-rw-r--r--   0        0        0    24833 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/repformer_layer.py
+-rw-r--r--   0        0        0    10672 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/repformers.py
+-rw-r--r--   0        0        0    22144 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/se_a.py
+-rw-r--r--   0        0        0    13626 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/se_atten.py
+-rw-r--r--   0        0        0    13518 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/se_r.py
+-rw-r--r--   0        0        0     3943 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/__init__.py
+-rw-r--r--   0        0        0     2914 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/dipole_model.py
+-rw-r--r--   0        0        0     2095 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/dp_model.py
+-rw-r--r--   0        0        0     3584 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/dp_zbl_model.py
+-rw-r--r--   0        0        0     3135 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/ener_model.py
+-rw-r--r--   0        0        0     7027 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/make_hessian_model.py
+-rw-r--r--   0        0        0    13375 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/make_model.py
+-rw-r--r--   0        0        0     3689 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/model.py
+-rw-r--r--   0        0        0     2062 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/polar_model.py
+-rw-r--r--   0        0        0     8507 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/model/transform_output.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/network/__init__.py
+-rw-r--r--   0        0        0     6237 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/network/mlp.py
+-rw-r--r--   0        0        0    63478 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/network/network.py
+-rw-r--r--   0        0        0      659 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/__init__.py
+-rw-r--r--   0        0        0     2017 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/atten_lcc.py
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/base_fitting.py
+-rw-r--r--   0        0        0     4432 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/denoise.py
+-rw-r--r--   0        0        0     5918 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/dipole.py
+-rw-r--r--   0        0        0    14767 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/ener.py
+-rw-r--r--   0        0        0    21591 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/fitting.py
+-rw-r--r--   0        0        0     7391 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/polarizability.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/task.py
+-rw-r--r--   0        0        0     1332 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/model/task/type_predict.py
+-rw-r--r--   0        0        0     5358 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/optimizer/KFWrapper.py
+-rw-r--r--   0        0        0     7744 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/optimizer/LKF.py
+-rw-r--r--   0        0        0      185 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/optimizer/__init__.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/train/__init__.py
+-rw-r--r--   0        0        0    43287 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/train/training.py
+-rw-r--r--   0        0        0     7717 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/train/wrapper.py
+-rw-r--r--   0        0        0      179 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/__init__.py
+-rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/ase_calc.py
+-rw-r--r--   0        0        0      665 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/auto_batch_size.py
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/cache.py
+-rw-r--r--   0        0        0     9205 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/dataloader.py
+-rw-r--r--   0        0        0     1978 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/dataset.py
+-rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/dp_random.py
+-rw-r--r--   0        0        0     2266 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/env.py
+-rw-r--r--   0        0        0     6747 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/env_mat_stat.py
+-rw-r--r--   0        0        0     4132 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/exclude_mask.py
+-rw-r--r--   0        0        0     3962 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/finetune.py
+-rw-r--r--   0        0        0     1273 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/learning_rate.py
+-rw-r--r--   0        0        0     6440 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/multi_task.py
+-rw-r--r--   0        0        0     5636 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/neighbor_stat.py
+-rw-r--r--   0        0        0    10257 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/nlist.py
+-rw-r--r--   0        0        0      270 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/plugin.py
+-rw-r--r--   0        0        0    10299 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/preprocess.py
+-rw-r--r--   0        0        0     2896 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/region.py
+-rw-r--r--   0        0        0     2186 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/serialization.py
+-rw-r--r--   0        0        0     1617 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/stat.py
+-rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/update_sel.py
+-rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/pt/utils/utils.py
+-rw-r--r--   0        0        0       69 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/__about__.py
+-rw-r--r--   0        0        0     1069 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/__init__.py
+-rw-r--r--   0        0        0      159 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/__main__.py
+-rw-r--r--   0        0        0      112 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/calculator.py
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/cluster/__init__.py
+-rw-r--r--   0        0        0     1798 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/cluster/local.py
+-rw-r--r--   0        0        0     6941 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/common.py
+-rw-r--r--   0        0        0      887 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/__init__.py
+-rw-r--r--   0        0        0    16729 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/descriptor.py
+-rw-r--r--   0        0        0    15251 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/hybrid.py
+-rw-r--r--   0        0        0    15496 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/loc_frame.py
+-rw-r--r--   0        0        0    10344 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se.py
+-rw-r--r--   0        0        0    55628 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a.py
+-rw-r--r--   0        0        0    20700 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a_ebd.py
+-rw-r--r--   0        0        0     1769 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a_ebd_v2.py
+-rw-r--r--   0        0        0    19845 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a_ef.py
+-rw-r--r--   0        0        0    16244 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a_mask.py
+-rw-r--r--   0        0        0    55505 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_atten.py
+-rw-r--r--   0        0        0     3836 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_atten_v2.py
+-rw-r--r--   0        0        0    27858 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_r.py
+-rw-r--r--   0        0        0    25159 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_t.py
+-rw-r--r--   0        0        0      851 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/__init__.py
+-rw-r--r--   0        0        0     6437 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/compress.py
+-rw-r--r--   0        0        0     1319 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/convert.py
+-rw-r--r--   0        0        0      136 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/doc.py
+-rwxr-xr-x   0        0        0    18942 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/freeze.py
+-rw-r--r--   0        0        0      128 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/gui.py
+-rw-r--r--   0        0        0      667 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/ipi.py
+-rw-r--r--   0        0        0     2309 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/main.py
+-rw-r--r--   0        0        0      142 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/neighbor_stat.py
+-rw-r--r--   0        0        0      115 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/test.py
+-rwxr-xr-x   0        0        0     9140 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/train.py
+-rw-r--r--   0        0        0     8062 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/transfer.py
+-rw-r--r--   0        0        0    13961 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/env.py
+-rw-r--r--   0        0        0      419 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/fit/__init__.py
+-rw-r--r--   0        0        0    13717 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/fit/dipole.py
+-rw-r--r--   0        0        0    23762 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/fit/dos.py
+-rw-r--r--   0        0        0    35764 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/fit/ener.py
+-rw-r--r--   0        0        0     7618 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/fit/fitting.py
+-rw-r--r--   0        0        0    28009 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/fit/polar.py
+-rw-r--r--   0        0        0     1270 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/__init__.py
+-rw-r--r--   0        0        0    16294 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/data_modifier.py
+-rw-r--r--   0        0        0     2179 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_dipole.py
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_dos.py
+-rw-r--r--   0        0        0    53555 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_eval.py
+-rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_polar.py
+-rw-r--r--   0        0        0      110 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_pot.py
+-rw-r--r--   0        0        0    15239 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_tensor.py
+-rw-r--r--   0        0        0      126 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_wfc.py
+-rw-r--r--   0        0        0     2697 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/ewald_recp.py
+-rw-r--r--   0        0        0      386 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/infer/model_devi.py
+-rw-r--r--   0        0        0     2942 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/lmp.py
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/loggers/__init__.py
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/loggers/loggers.py
+-rw-r--r--   0        0        0      305 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/loss/__init__.py
+-rw-r--r--   0        0        0     7939 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/loss/dos.py
+-rw-r--r--   0        0        0    32600 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/loss/ener.py
+-rw-r--r--   0        0        0     2287 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/loss/loss.py
+-rw-r--r--   0        0        0     5692 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/loss/tensor.py
+-rw-r--r--   0        0        0      717 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/__init__.py
+-rw-r--r--   0        0        0     7204 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/dos.py
+-rw-r--r--   0        0        0    18531 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/ener.py
+-rw-r--r--   0        0        0     6954 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/frozen.py
+-rw-r--r--   0        0        0     8625 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/linear.py
+-rw-r--r--   0        0        0    26423 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/model.py
+-rw-r--r--   0        0        0      293 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/model_stat.py
+-rw-r--r--   0        0        0    24794 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/multi.py
+-rw-r--r--   0        0        0     8596 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/pairtab.py
+-rw-r--r--   0        0        0    14730 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/pairwise_dprc.py
+-rw-r--r--   0        0        0     8172 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/model/tensor.py
+-rw-r--r--   0        0        0      214 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/__init__.py
+-rw-r--r--   0        0        0     1006 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/data/__init__.py
+-rw-r--r--   0        0        0    10960 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/data/data.py
+-rw-r--r--   0        0        0      207 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/descriptor/__init__.py
+-rw-r--r--   0        0        0    12637 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/descriptor/se_a.py
+-rw-r--r--   0        0        0    11303 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/descriptor/se_atten.py
+-rw-r--r--   0        0        0      201 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/__init__.py
+-rw-r--r--   0        0        0     2818 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/freeze.py
+-rw-r--r--   0        0        0    22428 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/mapt.py
+-rw-r--r--   0        0        0     6288 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/train.py
+-rw-r--r--   0        0        0    20979 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/wrap.py
+-rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/fit/__init__.py
+-rw-r--r--   0        0        0      343 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/fit/ener.py
+-rw-r--r--   0        0        0      554 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/__init__.py
+-rw-r--r--   0        0        0      178 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/argcheck.py
+-rw-r--r--   0        0        0    15587 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/config.py
+-rw-r--r--   0        0        0     7758 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/encode.py
+-rw-r--r--   0        0        0     6129 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/fio.py
+-rw-r--r--   0        0        0     8584 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/network.py
+-rw-r--r--   0        0        0      521 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/op.py
+-rw-r--r--   0        0        0     4960 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/weight.py
+-rw-r--r--   0        0        0      802 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/__init__.py
+-rw-r--r--   0        0        0      306 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_add_flt_nvnmd_grad.py
+-rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_copy_flt_nvnmd_grad.py
+-rw-r--r--   0        0        0      682 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_dotmul_flt_nvnmd_grad.py
+-rw-r--r--   0        0        0      284 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_flt_nvnmd_grad.py
+-rw-r--r--   0        0        0     1020 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_gelu.py
+-rw-r--r--   0        0        0      948 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_map_flt_nvnmd_grad.py
+-rw-r--r--   0        0        0      545 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_matmul_fitnet_nvnmd_grad.py
+-rw-r--r--   0        0        0     1017 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_matmul_flt2fix_nvnmd.py
+-rw-r--r--   0        0        0     1257 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_matmul_flt_nvnmd_grad.py
+-rw-r--r--   0        0        0      874 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_mul_flt_nvnmd_grad.py
+-rw-r--r--   0        0        0      582 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_force_grad.py
+-rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_force_se_a_grad.py
+-rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_force_se_a_mask_grad.py
+-rw-r--r--   0        0        0      454 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_force_se_r_grad.py
+-rw-r--r--   0        0        0      625 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_virial_grad.py
+-rw-r--r--   0        0        0      610 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_virial_se_a_grad.py
+-rw-r--r--   0        0        0      489 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_virial_se_r_grad.py
+-rw-r--r--   0        0        0      463 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_quantize_nvnmd_grad.py
+-rw-r--r--   0        0        0      569 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_soft_min_force_grad.py
+-rw-r--r--   0        0        0      612 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_soft_min_virial_grad.py
+-rw-r--r--   0        0        0     2962 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_tabulate_grad.py
+-rw-r--r--   0        0        0     1078 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/op/_tanh4_flt_nvnmd_grad.py
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/train/__init__.py
+-rw-r--r--   0        0        0     7439 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/train/run_options.py
+-rw-r--r--   0        0        0    50613 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/train/trainer.py
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/__init__.py
+-rw-r--r--   0        0        0      346 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/argcheck.py
+-rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/batch_size.py
+-rw-r--r--   0        0        0      344 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/compat.py
+-rw-r--r--   0        0        0     3416 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/compress.py
+-rw-r--r--   0        0        0    12356 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/convert.py
+-rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/data.py
+-rw-r--r--   0        0        0      283 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/data_system.py
+-rw-r--r--   0        0        0      366 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/errors.py
+-rw-r--r--   0        0        0     4195 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/finetune.py
+-rw-r--r--   0        0        0    17317 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/graph.py
+-rw-r--r--   0        0        0     3228 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/learning_rate.py
+-rw-r--r--   0        0        0     7057 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/multi_init.py
+-rw-r--r--   0        0        0     8497 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/neighbor_stat.py
+-rw-r--r--   0        0        0    10805 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/network.py
+-rw-r--r--   0        0        0     3386 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/nlist.py
+-rw-r--r--   0        0        0      166 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/pair_tab.py
+-rw-r--r--   0        0        0     2813 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/parallel_op.py
+-rw-r--r--   0        0        0      220 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/path.py
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/plugin.py
+-rw-r--r--   0        0        0      238 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/random.py
+-rw-r--r--   0        0        0     1108 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/region.py
+-rw-r--r--   0        0        0     4034 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/serialization.py
+-rw-r--r--   0        0        0     1617 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/sess.py
+-rw-r--r--   0        0        0     2556 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/spin.py
+-rw-r--r--   0        0        0    35807 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/tabulate.py
+-rw-r--r--   0        0        0     6135 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/type_embed.py
+-rw-r--r--   0        0        0      872 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/update_sel.py
+-rw-r--r--   0        0        0      186 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/tf/utils/weight_avg.py
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/__init__.py
+-rw-r--r--   0        0        0   109554 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/argcheck.py
+-rw-r--r--   0        0        0     2609 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/argcheck_nvnmd.py
+-rw-r--r--   0        0        0     7650 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/batch_size.py
+-rw-r--r--   0        0        0    10903 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/compat.py
+-rw-r--r--   0        0        0    28689 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/data.py
+-rw-r--r--   0        0        0    28267 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/data_system.py
+-rw-r--r--   0        0        0     6482 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/env_mat_stat.py
+-rw-r--r--   0        0        0      135 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/errors.py
+-rw-r--r--   0        0        0     4761 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/finetune.py
+-rw-r--r--   0        0        0      815 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/hostlist.py
+-rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/model_stat.py
+-rw-r--r--   0        0        0     3201 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/neighbor_stat.py
+-rw-r--r--   0        0        0     3899 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/out_stat.py
+-rw-r--r--   0        0        0    11067 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/pair_tab.py
+-rw-r--r--   0        0        0    12155 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/path.py
+-rw-r--r--   0        0        0     3884 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/plugin.py
+-rw-r--r--   0        0        0     2061 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/random.py
+-rw-r--r--   0        0        0     4252 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/summary.py
+-rw-r--r--   0        0        0     5728 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/update_sel.py
+-rw-r--r--   0        0        0      935 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/version.py
+-rw-r--r--   0        0        0     1358 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/deepmd/utils/weight_avg.py
+-rw-r--r--   0        0        0     9073 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0      461 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/coverage_plugins/__init__.py
+-rw-r--r--   0        0        0     3714 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/coverage_plugins/jit_plugin.py
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/aarch64/config.ini
+-rw-r--r--   0        0        0     2058 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/aarch64/table.S.tpl
+-rw-r--r--   0        0        0      879 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/aarch64/trampoline.S.tpl
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/arm/config.ini
+-rw-r--r--   0        0        0     2486 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/arm/table.S.tpl
+-rw-r--r--   0        0        0      774 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/arm/trampoline.S.tpl
+-rw-r--r--   0        0        0     4055 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/common/init.c.tpl
+-rw-r--r--   0        0        0      428 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/e2k/README.md
+-rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/e2k/config.ini
+-rw-r--r--   0        0        0      791 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/e2k/table.S.tpl
+-rw-r--r--   0        0        0      958 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/e2k/trampoline.S.tpl
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/i386/config.ini
+-rw-r--r--   0        0        0     1971 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/i386/table.S.tpl
+-rw-r--r--   0        0        0      818 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/i386/trampoline.S.tpl
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips/config.ini
+-rw-r--r--   0        0        0     2231 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips/table.S.tpl
+-rw-r--r--   0        0        0     1185 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips/trampoline.S.tpl
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips64/config.ini
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips64/table.S.tpl
+-rw-r--r--   0        0        0     1391 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips64/trampoline.S.tpl
+-rw-r--r--   0        0        0       49 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/x86_64/config.ini
+-rw-r--r--   0        0        0     2547 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/x86_64/table.S.tpl
+-rw-r--r--   0        0        0      797 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/x86_64/trampoline.S.tpl
+-rwxr-xr-x   0        0        0    19283 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/implib/implib-gen.py
+-rw-r--r--   0        0        0   926233 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/3rdparty/json.hpp
+-rw-r--r--   0        0        0    11042 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/CMakeLists.txt
+-rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_c/CMakeLists.txt
+-rw-r--r--   0        0        0    55787 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_c/include/c_api.h
+-rw-r--r--   0        0        0     1730 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_c/include/c_api_internal.h
+-rw-r--r--   0        0        0    86362 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_c/include/deepmd.hpp
+-rw-r--r--   0        0        0    59122 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_c/src/c_api.cc
+-rw-r--r--   0        0        0     2639 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/CMakeLists.txt
+-rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/AtomMap.h
+-rw-r--r--   0        0        0     6070 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/DataModifier.h
+-rw-r--r--   0        0        0     4590 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/DataModifierTF.h
+-rw-r--r--   0        0        0    33226 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/DeepPot.h
+-rw-r--r--   0        0        0    12689 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/DeepPotPT.h
+-rw-r--r--   0        0        0    14189 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/DeepPotTF.h
+-rw-r--r--   0        0        0    13697 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/DeepTensor.h
+-rw-r--r--   0        0        0    12894 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/DeepTensorTF.h
+-rw-r--r--   0        0        0     6995 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/common.h
+-rw-r--r--   0        0        0     4937 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/commonTF.h
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/tf_private.h
+-rw-r--r--   0        0        0      347 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/tf_public.h
+-rw-r--r--   0        0        0      531 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/include/version.h.in
+-rw-r--r--   0        0        0     3579 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/AtomMap.cc
+-rw-r--r--   0        0        0     3317 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/DataModifier.cc
+-rw-r--r--   0        0        0    13059 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/DataModifierTF.cc
+-rw-r--r--   0        0        0    38449 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/DeepPot.cc
+-rw-r--r--   0        0        0    19314 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/DeepPotPT.cc
+-rw-r--r--   0        0        0    40769 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/DeepPotTF.cc
+-rw-r--r--   0        0        0    11907 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/DeepTensor.cc
+-rw-r--r--   0        0        0    34578 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/DeepTensorTF.cc
+-rw-r--r--   0        0        0    47377 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/api_cc/src/common.cc
+-rw-r--r--   0        0        0      159 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/Config.cmake.in
+-rw-r--r--   0        0        0    17519 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/Findtensorflow.cmake
+-rw-r--r--   0        0        0     1688 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/Findxdrfile.cmake
+-rw-r--r--   0        0        0      568 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/cmake_lammps.cmake.in
+-rw-r--r--   0        0        0     1035 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0        0        0      431 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/coverage_config/CMakeLists.txt
+-rw-r--r--   0        0        0      632 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/googletest.cmake.in
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/test_cxx_abi.cpp
+-rw-r--r--   0        0        0      335 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/tf_cxx_abi.cpp
+-rw-r--r--   0        0        0      358 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/cmake/tf_version.cpp
+-rw-r--r--   0        0        0      478 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/config/CMakeLists.txt
+-rw-r--r--   0        0        0        4 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/config/MODEL_VER
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/config/__init__.py
+-rw-r--r--   0        0        0      415 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/config/run_config.ini
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/.gitignore
+-rw-r--r--   0        0        0     1576 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/CMakeLists.txt
+-rw-r--r--   0        0        0     3805 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/dp_gmx_patch
+-rw-r--r--   0        0        0      713 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/include/gmx_plugin.h
+-rw-r--r--   0        0        0     1077 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/patches/2020.2/CMakeLists.txt.patch.in
+-rw-r--r--   0        0        0     1111 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/patches/2020.2/src/gromacs/mdlib/forcerec.cpp.patch
+-rw-r--r--   0        0        0      509 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/patches/2020.2/src/gromacs/mdlib/forcerec.h.patch
+-rw-r--r--   0        0        0     3472 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/patches/2020.2/src/gromacs/mdlib/sim_util.cpp.patch
+-rw-r--r--   0        0        0     3087 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/gmx/src/gmx_plugin.cpp
+-rwxr-xr-x   0        0        0      854 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/build_cc.sh
+-rwxr-xr-x   0        0        0      642 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/build_from_c.sh
+-rwxr-xr-x   0        0        0     1158 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/build_lammps.sh
+-rwxr-xr-x   0        0        0    27453 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/build_tf.py
+-rw-r--r--   0        0        0      662 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/docker/Dockerfile
+-rwxr-xr-x   0        0        0      427 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/docker_package_c.sh
+-rwxr-xr-x   0        0        0      748 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/docker_test_package_c.sh
+-rwxr-xr-x   0        0        0     1294 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/install_tf.sh
+-rwxr-xr-x   0        0        0      770 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/package_c.sh
+-rwxr-xr-x   0        0        0      662 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/test_cc.sh
+-rwxr-xr-x   0        0        0      787 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/install/test_cc_local.sh
+-rw-r--r--   0        0        0     2241 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/CMakeLists.txt
+-rw-r--r--   0        0        0     6480 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/driver.cc
+-rw-r--r--   0        0        0      673 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/include/Convert.h
+-rw-r--r--   0        0        0      861 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/include/StringSplit.h
+-rw-r--r--   0        0        0      434 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/include/XyzFileManager.h
+-rw-r--r--   0        0        0     1457 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/include/sockets.h
+-rw-r--r--   0        0        0     1921 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/src/Convert.cc
+-rw-r--r--   0        0        0     2510 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/src/XyzFileManager.cc
+-rw-r--r--   0        0        0     4881 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/src/sockets.c
+-rw-r--r--   0        0        0    11623 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/ipi/tests/test_driver.py
+-rw-r--r--   0        0        0     1737 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/CMakeLists.txt
+-rw-r--r--   0        0        0    44520 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/ComputeDescriptor.h
+-rw-r--r--   0        0        0     4478 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/DeviceFunctor.h
+-rw-r--r--   0        0        0     5638 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/SimulationRegion.h
+-rw-r--r--   0        0        0    15145 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/SimulationRegion_Impl.h
+-rw-r--r--   0        0        0     2825 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/coord.h
+-rw-r--r--   0        0        0      352 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/device.h
+-rw-r--r--   0        0        0     2403 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/env_mat.h
+-rw-r--r--   0        0        0     4818 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/env_mat_nvnmd.h
+-rw-r--r--   0        0        0      709 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/errors.h
+-rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/ewald.h
+-rw-r--r--   0        0        0     2951 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/fmt_nlist.h
+-rw-r--r--   0        0        0     1213 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/gelu.h
+-rw-r--r--   0        0        0     5646 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/gpu_cuda.h
+-rw-r--r--   0        0        0     4030 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/gpu_rocm.h
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/map_aparam.h
+-rw-r--r--   0        0        0     7906 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/neighbor_list.h
+-rw-r--r--   0        0        0      548 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/neighbor_stat.h
+-rw-r--r--   0        0        0      600 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/pair_tab.h
+-rw-r--r--   0        0        0     1895 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/pairwise.h
+-rw-r--r--   0        0        0     3520 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/prod_env_mat.h
+-rw-r--r--   0        0        0     1710 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/prod_env_mat_nvnmd.h
+-rw-r--r--   0        0        0     3340 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/prod_force.h
+-rw-r--r--   0        0        0     1588 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/prod_force_grad.h
+-rw-r--r--   0        0        0     1820 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/prod_virial.h
+-rw-r--r--   0        0        0     1616 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/prod_virial_grad.h
+-rw-r--r--   0        0        0     2034 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/region.cuh
+-rw-r--r--   0        0        0     1331 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/region.h
+-rw-r--r--   0        0        0      504 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/soft_min_switch.h
+-rw-r--r--   0        0        0      451 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/soft_min_switch_force.h
+-rw-r--r--   0        0        0      439 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/soft_min_switch_force_grad.h
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/soft_min_switch_virial.h
+-rw-r--r--   0        0        0      501 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/soft_min_switch_virial_grad.h
+-rw-r--r--   0        0        0     2266 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/switcher.h
+-rw-r--r--   0        0        0    10773 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/tabulate.h
+-rw-r--r--   0        0        0     1414 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/include/utilities.h
+-rw-r--r--   0        0        0      239 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/SimulationRegion.cpp
+-rw-r--r--   0        0        0     5140 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/coord.cc
+-rw-r--r--   0        0        0    16610 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/env_mat.cc
+-rw-r--r--   0        0        0     4712 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/env_mat_nvnmd.cc
+-rw-r--r--   0        0        0    10575 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/ewald.cc
+-rw-r--r--   0        0        0     7678 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/fmt_nlist.cc
+-rw-r--r--   0        0        0     3514 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gelu.cc
+-rw-r--r--   0        0        0     3718 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/CMakeLists.txt
+-rw-r--r--   0        0        0    17312 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/coord.cu
+-rw-r--r--   0        0        0     1340 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/cudart/CMakeLists.txt
+-rw-r--r--   0        0        0     1266 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/cudart/cudart_stub.cc
+-rw-r--r--   0        0        0     5161 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/gelu.cu
+-rw-r--r--   0        0        0    10958 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/neighbor_list.cu
+-rw-r--r--   0        0        0     3931 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/neighbor_stat.cu
+-rw-r--r--   0        0        0    36252 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_env_mat.cu
+-rw-r--r--   0        0        0     7770 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_force.cu
+-rw-r--r--   0        0        0     7135 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_force_grad.cu
+-rw-r--r--   0        0        0     8083 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_virial.cu
+-rw-r--r--   0        0        0     6230 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_virial_grad.cu
+-rw-r--r--   0        0        0     2580 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/region.cu
+-rw-r--r--   0        0        0    45842 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/gpu/tabulate.cu
+-rw-r--r--   0        0        0     1883 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/map_aparam.cc
+-rw-r--r--   0        0        0    34199 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/neighbor_list.cc
+-rw-r--r--   0        0        0     7232 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/pair_tab.cc
+-rw-r--r--   0        0        0     4883 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/pairwise.cc
+-rw-r--r--   0        0        0    12954 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/prod_env_mat.cc
+-rw-r--r--   0        0        0     5435 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/prod_env_mat_nvnmd.cc
+-rw-r--r--   0        0        0     8764 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/prod_force.cc
+-rw-r--r--   0        0        0     5718 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/prod_force_grad.cc
+-rw-r--r--   0        0        0     5851 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/prod_virial.cc
+-rw-r--r--   0        0        0     5165 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/prod_virial_grad.cc
+-rw-r--r--   0        0        0     5157 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/region.cc
+-rw-r--r--   0        0        0     3958 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch.cc
+-rw-r--r--   0        0        0     2524 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch_force.cc
+-rw-r--r--   0        0        0     1939 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch_force_grad.cc
+-rw-r--r--   0        0        0     2874 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch_virial.cc
+-rw-r--r--   0        0        0     1799 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch_virial_grad.cc
+-rw-r--r--   0        0        0    35571 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/tabulate.cc
+-rw-r--r--   0        0        0      318 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lib/src/utilities.cc
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/CMakeLists.txt
+-rw-r--r--   0        0        0     1433 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/Install.sh
+-rw-r--r--   0        0        0     1390 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/builtin.cmake
+-rw-r--r--   0        0        0     5420 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/compute_deeptensor_atom.cpp
+-rw-r--r--   0        0        0     1101 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/compute_deeptensor_atom.h
+-rw-r--r--   0        0        0      778 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/deepmd_version.h.in
+-rw-r--r--   0        0        0      635 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/env.sh.in
+-rw-r--r--   0        0        0      567 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/env_c.sh.in
+-rw-r--r--   0        0        0      873 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/env_py.sh.in
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/env_py_c.sh.in
+-rw-r--r--   0        0        0    24381 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/fix_dplr.cpp
+-rw-r--r--   0        0        0     2165 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/fix_dplr.h
+-rw-r--r--   0        0        0      397 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/fix_ttm_dp.h
+-rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/lammps_install_list.txt.in
+-rwxr-xr-x   0        0        0      290 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/lmp_version.sh
+-rw-r--r--   0        0        0    51354 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/pair_deepmd.cpp
+-rw-r--r--   0        0        0     4060 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/pair_deepmd.h
+-rw-r--r--   0        0        0     4953 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/plugin/CMakeLists.txt
+-rw-r--r--   0        0        0     1922 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/plugin/deepmdplugin.cpp
+-rw-r--r--   0        0        0    12614 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/pppm_dplr.cpp
+-rw-r--r--   0        0        0      802 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/lmp/pppm_dplr.h
+-rw-r--r--   0        0        0     3203 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/CMakeLists.txt
+-rw-r--r--   0        0        0     2308 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/AdWeight.h
+-rw-r--r--   0        0        0     1596 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/Convert.h
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/CosSwitch.h
+-rw-r--r--   0        0        0      237 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/Gaussian.h
+-rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/GroFileManager.h
+-rw-r--r--   0        0        0      722 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/HarmonicAngle.h
+-rw-r--r--   0        0        0      720 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/HarmonicBond.h
+-rw-r--r--   0        0        0     1408 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/Integrator.h
+-rw-r--r--   0        0        0     2773 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/Interpolation.h
+-rw-r--r--   0        0        0      816 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/LJInter.h
+-rw-r--r--   0        0        0      743 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/LJTab.h
+-rw-r--r--   0        0        0      613 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/MaxShift.h
+-rw-r--r--   0        0        0     2112 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/Poly.h
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/RandomGenerator.h
+-rw-r--r--   0        0        0     1079 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/Statistics.h
+-rw-r--r--   0        0        0      464 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/StringSplit.h
+-rw-r--r--   0        0        0      539 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/TF.h
+-rw-r--r--   0        0        0      648 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/TableFileLoader.h
+-rw-r--r--   0        0        0     1415 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/Tabulated.h
+-rw-r--r--   0        0        0     1354 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/Trajectory.h
+-rw-r--r--   0        0        0      570 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/UnitManager.h
+-rw-r--r--   0        0        0      558 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/XyzFileManager.h
+-rw-r--r--   0        0        0     1399 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/ZM.h
+-rw-r--r--   0        0        0     1087 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/ZMFunctions.h
+-rw-r--r--   0        0        0     1107 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/common.h
+-rw-r--r--   0        0        0     1765 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/include/mymath.h
+-rw-r--r--   0        0        0     6548 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/mdnn.cc
+-rw-r--r--   0        0        0     8393 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/AdWeight.cc
+-rw-r--r--   0        0        0     3997 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/Convert.cc
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/Gaussian.cc
+-rw-r--r--   0        0        0     8092 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/GroFileManager.cc
+-rw-r--r--   0        0        0     3467 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/HarmonicAngle.cc
+-rw-r--r--   0        0        0     1571 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/HarmonicBond.cc
+-rw-r--r--   0        0        0     3381 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/Integrator.cc
+-rw-r--r--   0        0        0    16877 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/Interpolation.cpp
+-rw-r--r--   0        0        0     2621 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/LJInter.cc
+-rw-r--r--   0        0        0      852 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/LJTab.cc
+-rw-r--r--   0        0        0     1047 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/MaxShift.cc
+-rw-r--r--   0        0        0     6719 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/Poly.cpp
+-rw-r--r--   0        0        0     6215 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/RandomGenerator_MT19937.cc
+-rw-r--r--   0        0        0     3580 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/Statistics.cc
+-rw-r--r--   0        0        0     1077 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/StringSplit.cpp
+-rw-r--r--   0        0        0     1400 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/TF.cc
+-rw-r--r--   0        0        0     2286 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/TableFileLoader.cpp
+-rw-r--r--   0        0        0     5198 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/Tabulated.cc
+-rw-r--r--   0        0        0     3355 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/Trajectory.cc
+-rw-r--r--   0        0        0      963 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/UnitManager.cc
+-rw-r--r--   0        0        0     3266 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/XyzFileManager.cc
+-rw-r--r--   0        0        0     2227 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/ZM.cc
+-rw-r--r--   0        0        0     6693 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/md/src/ZMFunctions.cpp
+-rw-r--r--   0        0        0     2091 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/.gitignore
+-rw-r--r--   0        0        0      107 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/.npmignore
+-rw-r--r--   0        0        0      681 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/CMakeLists.txt
+-rw-r--r--   0        0        0     1287 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/README.md
+-rw-r--r--   0        0        0      383 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/binding.gyp.in
+-rw-r--r--   0        0        0      388 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/binding.gyp.pack
+-rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/index.js
+-rw-r--r--   0        0        0      801 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/package.json
+-rw-r--r--   0        0        0      895 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/prepublish.py
+-rw-r--r--   0        0        0     1088 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/tests/test_deeppot.js
+-rw-r--r--   0        0        0    29759 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/nodejs/yarn.lock
+-rw-r--r--   0        0        0     2736 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/CMakeLists.txt
+-rw-r--r--   0        0        0     2726 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/add_flt_nvnmd.cc
+-rw-r--r--   0        0        0     2525 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/copy_flt_nvnmd.cc
+-rw-r--r--   0        0        0      742 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/custom_op.cc
+-rw-r--r--   0        0        0     2130 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/custom_op.h
+-rw-r--r--   0        0        0    24439 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/descrpt.cc
+-rw-r--r--   0        0        0    16142 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/descrpt_se_a_ef.cc
+-rw-r--r--   0        0        0    16178 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/descrpt_se_a_ef_para.cc
+-rw-r--r--   0        0        0    16178 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/descrpt_se_a_ef_vert.cc
+-rw-r--r--   0        0        0    14156 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/descrpt_se_a_mask.cc
+-rw-r--r--   0        0        0     4324 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/dotmul_flt_nvnmd.cc
+-rw-r--r--   0        0        0     5319 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/ewald_recp.cc
+-rw-r--r--   0        0        0     2269 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/flt_nvnmd.cc
+-rw-r--r--   0        0        0     8314 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/gelu_multi_device.cc
+-rw-r--r--   0        0        0     3576 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/map_aparam.cc
+-rw-r--r--   0        0        0     4206 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/map_flt_nvnmd.cc
+-rw-r--r--   0        0        0     4499 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/matmul_fitnet_nvnmd.cc
+-rw-r--r--   0        0        0     3896 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/matmul_flt2fix_nvnmd.cc
+-rw-r--r--   0        0        0     5575 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/matmul_flt_nvnmd.cc
+-rw-r--r--   0        0        0     3207 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/mul_flt_nvnmd.cc
+-rw-r--r--   0        0        0    12902 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/neighbor_stat.cc
+-rw-r--r--   0        0        0     5436 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/optimizer/parallel.cc
+-rw-r--r--   0        0        0     1000 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/optimizer/parallel.h
+-rw-r--r--   0        0        0     7840 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/pair_tab.cc
+-rw-r--r--   0        0        0    15684 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/pairwise.cc
+-rw-r--r--   0        0        0    79958 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_env_mat_multi_device.cc
+-rw-r--r--   0        0        0    35316 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_env_mat_multi_device_nvnmd.cc
+-rw-r--r--   0        0        0     8861 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_force.cc
+-rw-r--r--   0        0        0     8386 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_force_grad.cc
+-rw-r--r--   0        0        0    12373 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_force_grad_multi_device.cc
+-rw-r--r--   0        0        0    12601 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_force_multi_device.cc
+-rw-r--r--   0        0        0     5537 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_force_se_a_grad.cc
+-rw-r--r--   0        0        0     5983 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_force_se_a_mask.cc
+-rw-r--r--   0        0        0     6108 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_force_se_a_mask_grad.cc
+-rw-r--r--   0        0        0     4765 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_force_se_r_grad.cc
+-rw-r--r--   0        0        0     9217 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_virial.cc
+-rw-r--r--   0        0        0     9082 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_virial_grad.cc
+-rw-r--r--   0        0        0    14592 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_virial_grad_multi_device.cc
+-rw-r--r--   0        0        0    12812 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_virial_multi_device.cc
+-rw-r--r--   0        0        0     6233 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_virial_se_a_grad.cc
+-rw-r--r--   0        0        0     5461 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/prod_virial_se_r_grad.cc
+-rw-r--r--   0        0        0     3375 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/quantize_nvnmd.cc
+-rw-r--r--   0        0        0      100 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/readme
+-rw-r--r--   0        0        0     5704 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/soft_min.cc
+-rw-r--r--   0        0        0     4138 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/soft_min_force.cc
+-rw-r--r--   0        0        0     4936 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/soft_min_force_grad.cc
+-rw-r--r--   0        0        0     5251 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/soft_min_virial.cc
+-rw-r--r--   0        0        0     5964 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/soft_min_virial_grad.cc
+-rw-r--r--   0        0        0    49880 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/tabulate_multi_device.cc
+-rw-r--r--   0        0        0     3365 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/tanh4_flt_nvnmd.cc
+-rw-r--r--   0        0        0    17595 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/op/unaggregated_grad.cc
+-rw-r--r--   0        0        0      859 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/source/swig/deepmd.i
+-rw-r--r--   0        0        0    22694 2022-11-09 12:37:21.000000 deepmd_kit-3.0.0a0/PKG-INFO
```

### Comparing `deepmd_kit-2.2.9/.pre-commit-config.yaml` & `deepmd_kit-3.0.0a0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     rev: 5.13.2
     hooks:
     - id: isort
       files: \.py$
       exclude: ^source/3rdparty
 -   repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.1.14
+    rev: v0.2.2
     hooks:
     - id: ruff
       args: ["--fix"]
       exclude: ^source/3rdparty
       types_or: [python, pyi, jupyter]
     - id: ruff-format
       exclude: ^source/3rdparty
@@ -60,26 +60,26 @@
 # CSS
 -   repo: https://github.com/pre-commit/mirrors-csslint
     rev: v1.0.5
     hooks:
     -   id: csslint
 # Shell
 - repo: https://github.com/scop/pre-commit-shfmt
-  rev: v3.7.0-4
+  rev: v3.8.0-1
   hooks:
     - id: shfmt
 # CMake
 - repo: https://github.com/cheshirekow/cmake-format-precommit
   rev: v0.6.13
   hooks:
     - id: cmake-format
     #- id: cmake-lint
 # license header
 - repo: https://github.com/Lucas-C/pre-commit-hooks
-  rev: v1.5.4
+  rev: v1.5.5
   hooks:
     # C++, js
     -   id: insert-license
         files: \.(c|cc|cpp|js|ts|h|hpp)$
         args:
         - --license-filepath
         - .license-header.txt
```

### Comparing `deepmd_kit-2.2.9/CITATIONS.bib` & `deepmd_kit-3.0.0a0/CITATIONS.bib`

 * *Files 6% similar despite different names*

```diff
@@ -101,14 +101,33 @@
     author = {Zhang, Duo and Bi, Hangrui and Dai, Fu-Zhi and Jiang, Wanrun and Zhang, Linfeng and Wang, Han},
     title = {{DPA-1: Pretraining of Attention-based Deep Potential Model for Molecular Simulation}},
     publisher = {arXiv},
     year = {2022},
     doi = {10.48550/arXiv.2208.08236},
 }
 
+@misc{Zhang_2023_DPA2,
+    annote = {DPA-2},
+    author = {Duo Zhang and Xinzijian Liu and Xiangyu Zhang and Chengqian Zhang and
+              Chun Cai and Hangrui Bi and Yiming Du and Xuejian Qin and Jiameng Huang
+              and Bowen Li and Yifan Shan and Jinzhe Zeng and Yuzhi Zhang and Siyuan
+              Liu and Yifan Li and Junhan Chang and Xinyan Wang and Shuo Zhou and
+              Jianchuan Liu and Xiaoshan Luo and Zhenyu Wang and Wanrun Jiang and Jing
+              Wu and Yudi Yang and Jiyuan Yang and Manyi Yang and Fu-Qiang Gong and
+              Linshuang Zhang and Mengchao Shi and Fu-Zhi Dai and Darrin M. York and
+              Shi Liu and Tong Zhu and Zhicheng Zhong and Jian Lv and Jun Cheng and
+              Weile Jia and Mohan Chen and Guolin Ke and Weinan E and Linfeng Zhang
+              and Han Wang},
+    title = {{DPA-2: Towards a universal large atomic model for molecular and material
+              simulation}},
+    publisher = {arXiv},
+    year = {2023},
+    doi = {10.48550/arXiv.2312.15492},
+}
+
 @article{Zhang_PhysPlasmas_2020_v27_p122704,
     annote = {frame-specific parameters (e.g. electronic temperature)},
     author = {Zhang, Yuzhi and Gao, Chang and Liu, Qianrui and Zhang, Linfeng and Wang, Han and Chen, Mohan},
     title = {{Warm dense matter simulation via electron temperature dependent deep potential molecular dynamics}},
     journal = {Phys. Plasmas},
     volume = {27},
     number = {12},
```

### Comparing `deepmd_kit-2.2.9/CONTRIBUTING.md` & `deepmd_kit-3.0.0a0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ## Before you contribute
 ### Overview of DeePMD-kit
 Currently, we maintain two main branch:
 - master: stable branch with version tag
 - devel :  branch for developers
 
 ### Developer guide
-See [here](doc/development/index.md) for coding conventions, API and other needs-to-know of the code.
+See [documentation](https://deepmd.readthedocs.io/) for coding conventions, API and other needs-to-know of the code.
 
 ## How to contribute
 Please perform the following steps to create your Pull Request to this repository. If don't like to use commands, you can also use [GitHub Desktop](https://desktop.github.com/), which is easier to get started. Go to [git documentation](https://git-scm.com/doc) if you want to really master git.
 
 ### Step 1: Fork the repository
 
 1. Visit the project: <https://github.com/deepmodeling/deepmd-kit>
```

### Comparing `deepmd_kit-2.2.9/LICENSE` & `deepmd_kit-3.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/backend/dp_backend.py` & `deepmd_kit-3.0.0a0/backend/dp_backend.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/backend/dynamic_metadata.py` & `deepmd_kit-3.0.0a0/backend/dynamic_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,45 +23,46 @@
     field: str,
     settings: Optional[Dict[str, object]] = None,
 ) -> str:
     assert field in ["optional-dependencies", "entry-points", "scripts"]
     _, _, find_libpython_requires, extra_scripts, tf_version = get_argument_from_env()
     if field == "scripts":
         return {
-            "dp": "deepmd_utils.main:main",
+            "dp": "deepmd.main:main",
             **extra_scripts,
         }
     elif field == "optional-dependencies":
         return {
             "test": [
-                "dpdata>=0.1.9",
+                "dpdata>=0.2.7",
                 "ase",
                 "pytest",
                 "pytest-cov",
                 "pytest-sugar",
                 "dpgui",
             ],
             "docs": [
                 "sphinx>=3.1.1",
                 "sphinx_rtd_theme>=1.0.0rc1",
                 "sphinx_markdown_tables",
                 "myst-nb>=1.0.0rc0",
                 "myst-parser>=0.19.2",
+                "sphinx-design",
                 "breathe",
                 "exhale",
                 "numpydoc",
                 "ase",
                 "deepmodeling-sphinx>=0.1.0",
                 "dargs>=0.3.4",
                 "sphinx-argparse",
                 "pygments-lammps",
                 "sphinxcontrib-bibtex",
             ],
             "lmp": [
-                "lammps~=2023.8.2.2.0",
+                "lammps~=2023.8.2.3.0",
                 *find_libpython_requires,
             ],
             "ipi": [
                 "i-PI",
                 *find_libpython_requires,
             ],
             "gui": [
@@ -84,8 +85,11 @@
                 "nvidia-cufft-cu12",
                 "nvidia-curand-cu12",
                 "nvidia-cusolver-cu12",
                 "nvidia-cusparse-cu12",
                 "nvidia-cudnn-cu12",
                 "nvidia-cuda-nvcc-cu12",
             ],
+            "torch": [
+                "torch>=2a",
+            ],
         }
```

### Comparing `deepmd_kit-2.2.9/backend/find_tensorflow.py` & `deepmd_kit-3.0.0a0/backend/find_tensorflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 )
 
 from packaging.specifiers import (
     SpecifierSet,
 )
 
 
-@lru_cache()
+@lru_cache
 def find_tensorflow() -> Tuple[Optional[str], List[str]]:
     """Find TensorFlow library.
 
     Tries to find TensorFlow in the order of:
 
     1. Environment variable `TENSORFLOW_ROOT` if set
     2. The current Python environment.
@@ -43,14 +43,16 @@
     Returns
     -------
     str
         TensorFlow library path if found.
     list of str
         TensorFlow requirement if not found. Empty if found.
     """
+    if os.environ.get("DP_ENABLE_TENSORFLOW", "1") == "0":
+        return None, []
     requires = []
 
     tf_spec = None
 
     if (tf_spec is None or not tf_spec) and os.environ.get(
         "TENSORFLOW_ROOT"
     ) is not None:
@@ -101,15 +103,15 @@
                 raise RuntimeError("Unsupported CUDA version")
         requires.extend(get_tf_requirement()["cpu"])
         # setuptools will re-find tensorflow after installing setup_requires
         tf_install_dir = None
     return tf_install_dir, requires
 
 
-@lru_cache()
+@lru_cache
 def get_tf_requirement(tf_version: str = "") -> dict:
     """Get TensorFlow requirement (CPU) when TF is not installed.
 
     If tf_version is not given and the environment variable `TENSORFLOW_VERSION` is set, use it as the requirement.
 
     Parameters
     ----------
@@ -117,21 +119,32 @@
         TF version
 
     Returns
     -------
     dict
         TensorFlow requirement, including cpu and gpu.
     """
+    if tf_version is None:
+        return {
+            "cpu": [],
+            "gpu": [],
+            "mpi": [],
+        }
     if tf_version == "":
         tf_version = os.environ.get("TENSORFLOW_VERSION", "")
 
     extra_requires = []
     extra_select = {}
     if not (tf_version == "" or tf_version in SpecifierSet(">=2.12", prereleases=True)):
         extra_requires.append("protobuf<3.20")
+    # keras 3 is not compatible with tf.compat.v1
+    if tf_version == "" or tf_version in SpecifierSet(">=2.15.0rc0", prereleases=True):
+        extra_requires.append("tf-keras; python_version>='3.9'")
+        # only TF>=2.16 is compatible with Python 3.12
+        extra_requires.append("tf-keras>=2.16.0rc0; python_version>='3.12'")
     if tf_version == "" or tf_version in SpecifierSet(">=1.15", prereleases=True):
         extra_select["mpi"] = [
             "horovod",
             "mpi4py",
         ]
     else:
         extra_select["mpi"] = []
@@ -179,15 +192,15 @@
                 "tensorflow-metal; platform_machine=='arm64' and platform_system == 'Darwin'",
                 *extra_requires,
             ],
             **extra_select,
         }
 
 
-@lru_cache()
+@lru_cache
 def get_tf_version(tf_path: Union[str, Path]) -> str:
     """Get TF version from a TF Python library path.
 
     Parameters
     ----------
     tf_path : str or Path
         TF Python library path
```

### Comparing `deepmd_kit-2.2.9/backend/read_env.py` & `deepmd_kit-3.0.0a0/backend/read_env.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from .find_tensorflow import (
     find_tensorflow,
     get_tf_version,
 )
 
 
-@lru_cache()
+@lru_cache
 def get_argument_from_env() -> Tuple[str, list, list, dict, str]:
     """Get the arguments from environment variables.
 
     The environment variables are assumed to be not changed during the build.
 
     Returns
     -------
@@ -74,26 +74,36 @@
     else:
         cmake_args.append("-DBUILD_CPP_IF:BOOL=FALSE")
 
     if dp_lammps_version != "":
         cmake_args.append(f"-DLAMMPS_VERSION={dp_lammps_version}")
     if dp_ipi == "1":
         cmake_args.append("-DENABLE_IPI:BOOL=TRUE")
-        extra_scripts["dp_ipi"] = "deepmd.entrypoints.ipi:dp_ipi"
+        extra_scripts["dp_ipi"] = "deepmd.tf.entrypoints.ipi:dp_ipi"
 
-    tf_install_dir, _ = find_tensorflow()
-    tf_version = get_tf_version(tf_install_dir)
-    if tf_version == "" or Version(tf_version) >= Version("2.12"):
-        find_libpython_requires = []
+    if os.environ.get("DP_ENABLE_TENSORFLOW", "1") == "1":
+        tf_install_dir, _ = find_tensorflow()
+        tf_version = get_tf_version(tf_install_dir)
+        if tf_version == "" or Version(tf_version) >= Version("2.12"):
+            find_libpython_requires = []
+        else:
+            find_libpython_requires = ["find_libpython"]
+        cmake_args.extend(
+            [
+                "-DENABLE_TENSORFLOW=ON",
+                f"-DTENSORFLOW_VERSION={tf_version}",
+                f"-DTENSORFLOW_ROOT:PATH={tf_install_dir}",
+            ]
+        )
     else:
-        find_libpython_requires = ["find_libpython"]
-    cmake_args.append(f"-DTENSORFLOW_VERSION={tf_version}")
+        find_libpython_requires = []
+        cmake_args.append("-DENABLE_TENSORFLOW=OFF")
+        tf_version = None
 
     cmake_args = [
-        f"-DTENSORFLOW_ROOT:PATH={tf_install_dir}",
         "-DBUILD_PY_IF:BOOL=TRUE",
         *cmake_args,
     ]
     return (
         cmake_minimum_required_version,
         cmake_args,
         find_libpython_requires,
```

### Comparing `deepmd_kit-2.2.9/codecov.yml` & `deepmd_kit-3.0.0a0/codecov.yml`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         target: auto
         threshold: 100%
   individual_components:
     - component_id: module_python
       name: Python
       paths:
         - deepmd/**
-        - deepmd_utils/**
     - component_id: module_op
       name: OP
       paths:
         - source/op/**
     - component_id: module_core
       name: Core
       paths:
```

### Comparing `deepmd_kit-2.2.9/deepmd/__init__.py` & `deepmd_kit-3.0.0a0/deepmd/tf/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 try:
     from importlib import (
         metadata,
     )
 except ImportError:  # for Python<3.8
     import importlib_metadata as metadata
 
-import deepmd.utils.network as network
+import deepmd.tf.utils.network as network
 
 from . import (
     cluster,
     descriptor,
     fit,
     loss,
     nvnmd,
@@ -28,15 +28,15 @@
 from .infer.data_modifier import (
     DipoleChargeModifier,
 )
 
 set_mkl()
 
 try:
-    from deepmd_utils._version import version as __version__
+    from deepmd._version import version as __version__
 except ImportError:
     from .__about__ import (
         __version__,
     )
 
 # load third-party plugins
 try:
```

### Comparing `deepmd_kit-2.2.9/deepmd/calculator.py` & `deepmd_kit-3.0.0a0/deepmd/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 from ase.calculators.calculator import (
     Calculator,
     PropertyNotImplementedError,
     all_changes,
 )
 
-from deepmd import (
-    DeepPotential,
+from deepmd.infer import (
+    DeepPot,
 )
 
 if TYPE_CHECKING:
     from ase import (
         Atoms,
     )
 
@@ -49,15 +49,15 @@
         The neighbor list object. If None, then build the native neighbor list.
 
     Examples
     --------
     Compute potential energy
 
     >>> from ase import Atoms
-    >>> from deepmd.calculator import DP
+    >>> from deepmd.tf.calculator import DP
     >>> water = Atoms('H2O',
     >>>             positions=[(0.7601, 1.9270, 1),
     >>>                        (1.9575, 1, 1),
     >>>                        (1., 1., 1.)],
     >>>             cell=[100, 100, 100],
     >>>             calculator=DP(model="frozen_model.pb"))
     >>> print(water.get_potential_energy())
@@ -85,15 +85,15 @@
         model: Union[str, "Path"],
         label: str = "DP",
         type_dict: Optional[Dict[str, int]] = None,
         neighbor_list=None,
         **kwargs,
     ) -> None:
         Calculator.__init__(self, label=label, **kwargs)
-        self.dp = DeepPotential(str(Path(model).resolve()), neighbor_list=neighbor_list)
+        self.dp = DeepPot(str(Path(model).resolve()), neighbor_list=neighbor_list)
         if type_dict:
             self.type_dict = type_dict
         else:
             self.type_dict = dict(
                 zip(self.dp.get_type_map(), range(self.dp.get_ntypes()))
             )
```

### Comparing `deepmd_kit-2.2.9/deepmd/cluster/__init__.py` & `deepmd_kit-3.0.0a0/deepmd/tf/cluster/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Module that reads node resources, auto detects if running local or on SLURM."""
 
-import os
 from typing import (
     List,
     Optional,
     Tuple,
 )
 
 from .local import get_resource as get_local_res
-from .slurm import get_resource as get_slurm_res
 
 __all__ = ["get_resource"]
 
 
 def get_resource() -> Tuple[str, List[str], Optional[List[int]]]:
     """Get local or slurm resources: nodename, nodelist, and gpus.
 
     Returns
     -------
     Tuple[str, List[str], Optional[List[int]]]
         nodename, nodelist, and gpus
     """
-    if "SLURM_JOB_NODELIST" in os.environ:
-        return get_slurm_res()
-    else:
-        return get_local_res()
+    return get_local_res()
```

### Comparing `deepmd_kit-2.2.9/deepmd/cluster/local.py` & `deepmd_kit-3.0.0a0/deepmd/tf/cluster/local.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Get local GPU resources."""
 
-import socket
 import subprocess as sp
 import sys
 from typing import (
     List,
     Optional,
     Tuple,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
+from deepmd.utils.hostlist import (
+    get_host_names,
+)
 
 __all__ = ["get_gpus", "get_resource"]
 
 
 def get_gpus():
     """Get available IDs of GPU cards at local.
     These IDs are valid when used as the TensorFlow device ID.
@@ -53,11 +55,10 @@
     """Get local resources: nodename, nodelist, and gpus.
 
     Returns
     -------
     Tuple[str, List[str], Optional[List[int]]]
         nodename, nodelist, and gpus
     """
-    nodename = socket.gethostname()
-    nodelist = [nodename]
+    nodename, nodelist = get_host_names()
     gpus = get_gpus()
     return nodename, nodelist, gpus
```

### Comparing `deepmd_kit-2.2.9/deepmd/common.py` & `deepmd_kit-3.0.0a0/deepmd/tf/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,38 +13,38 @@
 )
 
 import tensorflow
 from tensorflow.python.framework import (
     tensor_util,
 )
 
-from deepmd.env import (
-    GLOBAL_TF_FLOAT_PRECISION,
-    op_module,
-    tf,
-)
-from deepmd_utils.common import (
+from deepmd.common import (
     add_data_requirement,
     data_requirement,
     expand_sys_str,
     get_np_precision,
     j_loader,
     j_must_have,
     make_default_mesh,
     select_idx_map,
 )
+from deepmd.tf.env import (
+    GLOBAL_TF_FLOAT_PRECISION,
+    op_module,
+    tf,
+)
 
 if TYPE_CHECKING:
-    from deepmd_utils.common import (
+    from deepmd.common import (
         _ACTIVATION,
         _PRECISION,
     )
 
 __all__ = [
-    # from deepmd_utils.common
+    # from deepmd.common
     "data_requirement",
     "add_data_requirement",
     "select_idx_map",
     "make_default_mesh",
     "j_must_have",
     "j_loader",
     "expand_sys_str",
@@ -239,21 +239,21 @@
     Callable
         a decorator that casts and casts back the input and
         output tensor of a method
 
     Examples
     --------
     >>> class A:
-    ...   @property
-    ...   def precision(self):
-    ...     return tf.float32
+    ...     @property
+    ...     def precision(self):
+    ...         return tf.float32
     ...
-    ...   @cast_precision
-    ...   def f(x: tf.Tensor, y: tf.Tensor) -> tf.Tensor:
-    ...     return x ** 2 + y
+    ...     @cast_precision
+    ...     def f(x: tf.Tensor, y: tf.Tensor) -> tf.Tensor:
+    ...         return x**2 + y
     """
 
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         # only convert tensors
         returned_tensor = func(
             self,
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/__init__.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/descriptor.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/descriptor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,89 +1,58 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from abc import (
     abstractmethod,
 )
 from typing import (
     Any,
-    Callable,
     Dict,
     List,
     Optional,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.common import (
+    j_get_type,
+)
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     tf,
 )
-from deepmd.utils import (
-    Plugin,
+from deepmd.tf.utils import (
     PluginVariant,
 )
+from deepmd.utils.plugin import (
+    make_plugin_registry,
+)
 
 
-class Descriptor(PluginVariant):
+class Descriptor(PluginVariant, make_plugin_registry("descriptor")):
     r"""The abstract class for descriptors. All specific descriptors should
     be based on this class.
 
     The descriptor :math:`\mathcal{D}` describes the environment of an atom,
     which should be a function of coordinates and types of its neighbour atoms.
 
     Examples
     --------
-    >>> descript = Descriptor(type="se_e2_a", rcut=6., rcut_smth=0.5, sel=[50])
+    >>> descript = Descriptor(type="se_e2_a", rcut=6.0, rcut_smth=0.5, sel=[50])
     >>> type(descript)
-    <class 'deepmd.descriptor.se_a.DescrptSeA'>
+    <class 'deepmd.tf.descriptor.se_a.DescrptSeA'>
 
     Notes
     -----
     Only methods and attributes defined in this class are generally public,
     that can be called by other classes.
     """
 
-    __plugins = Plugin()
-
-    @staticmethod
-    def register(key: str) -> Callable:
-        """Register a descriptor plugin.
-
-        Parameters
-        ----------
-        key : str
-            the key of a descriptor
-
-        Returns
-        -------
-        Descriptor
-            the registered descriptor
-
-        Examples
-        --------
-        >>> @Descriptor.register("some_descrpt")
-            class SomeDescript(Descriptor):
-                pass
-        """
-        return Descriptor.__plugins.register(key)
-
-    @classmethod
-    def get_class_by_input(cls, input: dict):
-        try:
-            descrpt_type = input["type"]
-        except KeyError:
-            raise KeyError("the type of descriptor should be set by `type`")
-        if descrpt_type in Descriptor.__plugins.plugins:
-            return Descriptor.__plugins.plugins[descrpt_type]
-        else:
-            raise RuntimeError("Unknown descriptor type: " + descrpt_type)
-
     def __new__(cls, *args, **kwargs):
         if cls is Descriptor:
-            cls = cls.get_class_by_input(kwargs)
+            cls = cls.get_class_by_type(j_get_type(kwargs, cls.__name__))
         return super().__new__(cls)
 
     @abstractmethod
     def get_rcut(self) -> float:
         """Returns the cut-off radius.
 
         Returns
@@ -170,26 +139,26 @@
         """Compute the statisitcs (avg and std) of the training data. The input will be
         normalized by the statistics.
 
         Parameters
         ----------
         data_coord : list[np.ndarray]
             The coordinates. Can be generated by
-            :meth:`deepmd.model.model_stat.make_stat_input`
+            :meth:`deepmd.tf.model.model_stat.make_stat_input`
         data_box : list[np.ndarray]
             The box. Can be generated by
-            :meth:`deepmd.model.model_stat.make_stat_input`
+            :meth:`deepmd.tf.model.model_stat.make_stat_input`
         data_atype : list[np.ndarray]
-            The atom types. Can be generated by :meth:`deepmd.model.model_stat.make_stat_input`
+            The atom types. Can be generated by :meth:`deepmd.tf.model.model_stat.make_stat_input`
         natoms_vec : list[np.ndarray]
             The vector for the number of atoms of the system and different types of
-            atoms. Can be generated by :meth:`deepmd.model.model_stat.make_stat_input`
+            atoms. Can be generated by :meth:`deepmd.tf.model.model_stat.make_stat_input`
         mesh : list[np.ndarray]
             The mesh for neighbor searching. Can be generated by
-            :meth:`deepmd.model.model_stat.make_stat_input`
+            :meth:`deepmd.tf.model.model_stat.make_stat_input`
         input_dict : dict[str, list[np.ndarray]]
             Dictionary for additional input
         **kwargs
             Additional keyword arguments which may contain `mixed_type` and `real_natoms_vec`.
 
         Notes
         -----
@@ -503,9 +472,49 @@
         ----------
         global_jdata : dict
             The global data, containing the training section
         local_jdata : dict
             The local data refer to the current class
         """
         # call subprocess
-        cls = cls.get_class_by_input(local_jdata)
+        cls = cls.get_class_by_type(j_get_type(local_jdata, cls.__name__))
         return cls.update_sel(global_jdata, local_jdata)
+
+    @classmethod
+    def deserialize(cls, data: dict, suffix: str = "") -> "Descriptor":
+        """Deserialize the model.
+
+        There is no suffix in a native DP model, but it is important
+        for the TF backend.
+
+        Parameters
+        ----------
+        data : dict
+            The serialized data
+        suffix : str, optional
+            Name suffix to identify this descriptor
+
+        Returns
+        -------
+        Descriptor
+            The deserialized descriptor
+        """
+        if cls is Descriptor:
+            return Descriptor.get_class_by_type(
+                j_get_type(data, cls.__name__)
+            ).deserialize(data, suffix=suffix)
+        raise NotImplementedError("Not implemented in class %s" % cls.__name__)
+
+    def serialize(self, suffix: str = "") -> dict:
+        """Serialize the model.
+
+        There is no suffix in a native DP model, but it is important
+        for the TF backend.
+
+        Returns
+        -------
+        dict
+            The serialized data
+        suffix : str, optional
+            Name suffix to identify this descriptor
+        """
+        raise NotImplementedError("Not implemented in class %s" % self.__name__)
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/hybrid.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/hybrid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
+    Any,
+    Dict,
     List,
     Optional,
     Tuple,
+    Union,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     tf,
 )
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
+from deepmd.utils.version import (
+    check_version_compatibility,
+)
 
-# from deepmd.descriptor import DescrptLocFrame
-# from deepmd.descriptor import DescrptSeA
-# from deepmd.descriptor import DescrptSeT
-# from deepmd.descriptor import DescrptSeAEbd
-# from deepmd.descriptor import DescrptSeAEf
-# from deepmd.descriptor import DescrptSeR
+# from deepmd.tf.descriptor import DescrptLocFrame
+# from deepmd.tf.descriptor import DescrptSeA
+# from deepmd.tf.descriptor import DescrptSeT
+# from deepmd.tf.descriptor import DescrptSeAEbd
+# from deepmd.tf.descriptor import DescrptSeAEf
+# from deepmd.tf.descriptor import DescrptSeR
 from .descriptor import (
     Descriptor,
 )
 
 
 @Descriptor.register("hybrid")
 class DescrptHybrid(Descriptor):
     """Concate a list of descriptors to form a new descriptor.
 
     Parameters
     ----------
-    list : list
+    list : list : List[Union[Descriptor, Dict[str, Any]]]
             Build a descriptor from the concatenation of the list of descriptors.
+            The descriptor can be either an object or a dictionary.
     """
 
     def __init__(
         self,
-        list: list,
+        list: List[Union[Descriptor, Dict[str, Any]]],
         multi_task: bool = False,
         ntypes: Optional[int] = None,
         spin: Optional[Spin] = None,
         **kwargs,
     ) -> None:
         """Constructor."""
         # warning: list is conflict with built-in list
@@ -142,23 +149,23 @@
         **kwargs,
     ) -> None:
         """Compute the statisitcs (avg and std) of the training data. The input will be normalized by the statistics.
 
         Parameters
         ----------
         data_coord
-            The coordinates. Can be generated by deepmd.model.make_stat_input
+            The coordinates. Can be generated by deepmd.tf.model.make_stat_input
         data_box
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         data_atype
-            The atom types. Can be generated by deepmd.model.make_stat_input
+            The atom types. Can be generated by deepmd.tf.model.make_stat_input
         natoms_vec
-            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.model.make_stat_input
+            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.tf.model.make_stat_input
         mesh
-            The mesh for neighbor searching. Can be generated by deepmd.model.make_stat_input
+            The mesh for neighbor searching. Can be generated by deepmd.tf.model.make_stat_input
         input_dict
             Dictionary for additional input
         mixed_type
             Whether to perform the mixed_type mode.
             If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
             in which frames in a system may have different natoms_vec(s), with the same nloc.
         real_natoms_vec
@@ -430,7 +437,34 @@
         """
         local_jdata_cpy = local_jdata.copy()
         local_jdata_cpy["list"] = [
             Descriptor.update_sel(global_jdata, sub_jdata)
             for sub_jdata in local_jdata["list"]
         ]
         return local_jdata_cpy
+
+    def serialize(self, suffix: str = "") -> dict:
+        return {
+            "@class": "Descriptor",
+            "type": "hybrid",
+            "@version": 1,
+            "list": [
+                descrpt.serialize(suffix=f"{suffix}_{idx}")
+                for idx, descrpt in enumerate(self.descrpt_list)
+            ],
+        }
+
+    @classmethod
+    def deserialize(cls, data: dict, suffix: str = "") -> "DescrptHybrid":
+        data = data.copy()
+        class_name = data.pop("@class")
+        assert class_name == "Descriptor"
+        class_type = data.pop("type")
+        assert class_type == "hybrid"
+        check_version_compatibility(data.pop("@version"), 1, 1)
+        obj = cls(
+            list=[
+                Descriptor.deserialize(ii, suffix=f"{suffix}_{idx}")
+                for idx, ii in enumerate(data["list"])
+            ],
+        )
+        return obj
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/loc_frame.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/loc_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
     List,
     Optional,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     default_tf_session_config,
     op_module,
     tf,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 from .descriptor import (
     Descriptor,
 )
 
@@ -164,23 +164,23 @@
         **kwargs,
     ) -> None:
         """Compute the statisitcs (avg and std) of the training data. The input will be normalized by the statistics.
 
         Parameters
         ----------
         data_coord
-            The coordinates. Can be generated by deepmd.model.make_stat_input
+            The coordinates. Can be generated by deepmd.tf.model.make_stat_input
         data_box
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         data_atype
-            The atom types. Can be generated by deepmd.model.make_stat_input
+            The atom types. Can be generated by deepmd.tf.model.make_stat_input
         natoms_vec
-            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.model.make_stat_input
+            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.tf.model.make_stat_input
         mesh
-            The mesh for neighbor searching. Can be generated by deepmd.model.make_stat_input
+            The mesh for neighbor searching. Can be generated by deepmd.tf.model.make_stat_input
         input_dict
             Dictionary for additional input
         **kwargs
             Additional keyword arguments.
         """
         all_davg = []
         all_dstd = []
@@ -339,15 +339,18 @@
         atom_virial
             The atomic virial
         """
         [net_deriv] = tf.gradients(atom_ener, self.descrpt)
         tf.summary.histogram("net_derivative", net_deriv)
         net_deriv_reshape = tf.reshape(
             net_deriv,
-            [np.cast["int64"](-1), natoms[0] * np.cast["int64"](self.ndescrpt)],
+            [
+                np.asarray(-1, dtype=np.int64),
+                natoms[0] * np.asarray(self.ndescrpt, dtype=np.int64),
+            ],
         )
         force = op_module.prod_force(
             net_deriv_reshape,
             self.descrpt_deriv,
             self.nlist,
             self.axis,
             natoms,
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_a.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,69 +3,75 @@
     List,
     Optional,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.dpmodel.utils.env_mat import (
+    EnvMat,
+)
+from deepmd.tf.common import (
     cast_precision,
     get_activation_func,
     get_np_precision,
     get_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     default_tf_session_config,
     op_module,
     tf,
 )
-from deepmd.nvnmd.descriptor.se_a import (
+from deepmd.tf.nvnmd.descriptor.se_a import (
     build_davg_dstd,
     build_op_descriptor,
     check_switch_range,
     descrpt2r4,
     filter_GR2D,
     filter_lower_R42GR,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.utils.compress import (
+from deepmd.tf.utils.compress import (
     get_extra_side_embedding_net_variable,
     get_two_side_type_embedding,
     get_type_embedding,
     make_data,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphWithoutTensorError,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_extra_embedding_net_suffix,
     get_extra_embedding_net_variables_from_graph_def,
     get_pattern_nodes_from_graph_def,
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     embedding_net,
     embedding_net_rand_seed_shift,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
-from deepmd.utils.tabulate import (
+from deepmd.tf.utils.tabulate import (
     DPTabulate,
 )
-from deepmd.utils.type_embed import (
+from deepmd.tf.utils.type_embed import (
     embed_atom_type,
 )
+from deepmd.utils.version import (
+    check_version_compatibility,
+)
 
 from .descriptor import (
     Descriptor,
 )
 from .se import (
     DescrptSe,
 )
@@ -108,15 +114,15 @@
     of a embedding network :math:`\mathcal{N}` of :math:`s(r_{ji})`:
 
     .. math::
         (\mathcal{G}^i)_j = \mathcal{N}(s(r_{ji}))
 
     :math:`\mathcal{G}^i_< \in \mathbb{R}^{N \times M_2}` takes first :math:`M_2` columns of
     :math:`\mathcal{G}^i`. The equation of embedding network :math:`\mathcal{N}` can be found at
-    :meth:`deepmd.utils.network.embedding_net`.
+    :meth:`deepmd.tf.utils.network.embedding_net`.
 
     Parameters
     ----------
     rcut
             The cut-off radius :math:`r_c`
     rcut_smth
             From where the environment matrix should be smoothed :math:`r_s`
@@ -191,16 +197,18 @@
         self.filter_resnet_dt = resnet_dt
         self.seed = seed
         self.uniform_seed = uniform_seed
         self.seed_shift = embedding_net_rand_seed_shift(self.filter_neuron)
         self.trainable = trainable
         self.compress_activation_fn = get_activation_func(activation_function)
         self.filter_activation_fn = get_activation_func(activation_function)
+        self.activation_function_name = activation_function
         self.filter_precision = get_precision(precision)
         self.filter_np_precision = get_np_precision(precision)
+        self.orig_exclude_types = exclude_types
         self.exclude_types = set()
         for tt in exclude_types:
             assert len(tt) == 2
             self.exclude_types.add((tt[0], tt[1]))
             self.exclude_types.add((tt[1], tt[0]))
         self.set_davg_zero = set_davg_zero
         self.type_one_side = type_one_side
@@ -329,23 +337,23 @@
         **kwargs,
     ) -> None:
         """Compute the statisitcs (avg and std) of the training data. The input will be normalized by the statistics.
 
         Parameters
         ----------
         data_coord
-            The coordinates. Can be generated by deepmd.model.make_stat_input
+            The coordinates. Can be generated by deepmd.tf.model.make_stat_input
         data_box
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         data_atype
-            The atom types. Can be generated by deepmd.model.make_stat_input
+            The atom types. Can be generated by deepmd.tf.model.make_stat_input
         natoms_vec
-            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.model.make_stat_input
+            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.tf.model.make_stat_input
         mesh
-            The mesh for neighbor searching. Can be generated by deepmd.model.make_stat_input
+            The mesh for neighbor searching. Can be generated by deepmd.tf.model.make_stat_input
         input_dict
             Dictionary for additional input
         **kwargs
             Additional keyword arguments.
         """
         if True:
             sumr = []
@@ -704,15 +712,18 @@
         atom_virial
             The atomic virial
         """
         [net_deriv] = tf.gradients(atom_ener, self.descrpt_reshape)
         tf.summary.histogram("net_derivative", net_deriv)
         net_deriv_reshape = tf.reshape(
             net_deriv,
-            [np.cast["int64"](-1), natoms[0] * np.cast["int64"](self.ndescrpt)],
+            [
+                np.asarray(-1, dtype=np.int64),
+                natoms[0] * np.asarray(self.ndescrpt, dtype=np.int64),
+            ],
         )
         force = op_module.prod_force_se_a(
             net_deriv_reshape,
             self.descrpt_deriv,
             self.nlist,
             natoms,
             n_a_sel=self.nnei_a,
@@ -1338,7 +1349,111 @@
 
     @property
     def explicit_ntypes(self) -> bool:
         """Explicit ntypes with type embedding."""
         if self.stripped_type_embedding:
             return True
         return False
+
+    @classmethod
+    def deserialize(cls, data: dict, suffix: str = ""):
+        """Deserialize the model.
+
+        Parameters
+        ----------
+        data : dict
+            The serialized data
+
+        Returns
+        -------
+        Model
+            The deserialized model
+        """
+        if cls is not DescrptSeA:
+            raise NotImplementedError("Not implemented in class %s" % cls.__name__)
+        data = data.copy()
+        check_version_compatibility(data.pop("@version", 1), 1, 1)
+        data.pop("@class", None)
+        data.pop("type", None)
+        embedding_net_variables = cls.deserialize_network(
+            data.pop("embeddings"), suffix=suffix
+        )
+        data.pop("env_mat")
+        variables = data.pop("@variables")
+        descriptor = cls(**data)
+        descriptor.embedding_net_variables = embedding_net_variables
+        descriptor.davg = variables["davg"].reshape(
+            descriptor.ntypes, descriptor.ndescrpt
+        )
+        descriptor.dstd = variables["dstd"].reshape(
+            descriptor.ntypes, descriptor.ndescrpt
+        )
+        return descriptor
+
+    def serialize(self, suffix: str = "") -> dict:
+        """Serialize the model.
+
+        Parameters
+        ----------
+        suffix : str, optional
+            The suffix of the scope
+
+        Returns
+        -------
+        dict
+            The serialized data
+        """
+        if type(self) is not DescrptSeA:
+            raise NotImplementedError(
+                "Not implemented in class %s" % self.__class__.__name__
+            )
+        if self.stripped_type_embedding:
+            raise NotImplementedError(
+                "stripped_type_embedding is unsupported by the native model"
+            )
+        if (self.original_sel != self.sel_a).any():
+            raise NotImplementedError(
+                "Adjusting sel is unsupported by the native model"
+            )
+        if self.embedding_net_variables is None:
+            raise RuntimeError("init_variables must be called before serialize")
+        if self.spin is not None:
+            raise NotImplementedError("spin is unsupported")
+        assert self.davg is not None
+        assert self.dstd is not None
+        # TODO: not sure how to handle type embedding - type embedding is not a model parameter,
+        # but instead a part of the input data. Maybe the interface should be refactored...
+
+        return {
+            "@class": "Descriptor",
+            "type": "se_e2_a",
+            "@version": 1,
+            "rcut": self.rcut_r,
+            "rcut_smth": self.rcut_r_smth,
+            "sel": self.sel_a,
+            "neuron": self.filter_neuron,
+            "axis_neuron": self.n_axis_neuron,
+            "resnet_dt": self.filter_resnet_dt,
+            "trainable": self.trainable,
+            "type_one_side": self.type_one_side,
+            "exclude_types": list(self.orig_exclude_types),
+            "set_davg_zero": self.set_davg_zero,
+            "activation_function": self.activation_function_name,
+            "precision": self.filter_precision.name,
+            "embeddings": self.serialize_network(
+                ntypes=self.ntypes,
+                ndim=(1 if self.type_one_side else 2),
+                in_dim=1,
+                neuron=self.filter_neuron,
+                activation_function=self.activation_function_name,
+                resnet_dt=self.filter_resnet_dt,
+                variables=self.embedding_net_variables,
+                excluded_types=self.exclude_types,
+                suffix=suffix,
+            ),
+            "env_mat": EnvMat(self.rcut_r, self.rcut_r_smth).serialize(),
+            "@variables": {
+                "davg": self.davg.reshape(self.ntypes, self.nnei_a, 4),
+                "dstd": self.dstd.reshape(self.ntypes, self.nnei_a, 4),
+            },
+            "spin": self.spin,
+        }
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_a_ebd.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a_ebd.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from typing import (
     List,
     Optional,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     add_data_requirement,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     op_module,
     tf,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     embedding_net,
     one_layer,
 )
 
 from .descriptor import (
     Descriptor,
 )
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_a_ebd_v2.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a_ebd_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 from typing import (
     List,
     Optional,
 )
 
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
 
 from .descriptor import (
     Descriptor,
 )
 from .se_a import (
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_a_ef.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a_ef.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
     List,
     Optional,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     add_data_requirement,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     default_tf_session_config,
     op_module,
     tf,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 from .descriptor import (
     Descriptor,
 )
 from .se import (
@@ -176,23 +176,23 @@
         **kwargs,
     ) -> None:
         """Compute the statisitcs (avg and std) of the training data. The input will be normalized by the statistics.
 
         Parameters
         ----------
         data_coord
-            The coordinates. Can be generated by deepmd.model.make_stat_input
+            The coordinates. Can be generated by deepmd.tf.model.make_stat_input
         data_box
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         data_atype
-            The atom types. Can be generated by deepmd.model.make_stat_input
+            The atom types. Can be generated by deepmd.tf.model.make_stat_input
         natoms_vec
-            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.model.make_stat_input
+            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.tf.model.make_stat_input
         mesh
-            The mesh for neighbor searching. Can be generated by deepmd.model.make_stat_input
+            The mesh for neighbor searching. Can be generated by deepmd.tf.model.make_stat_input
         input_dict
             Dictionary for additional input
         **kwargs
             Additional keyword arguments.
         """
         self.descrpt_vert.compute_input_stats(
             data_coord, data_box, data_atype, natoms_vec, mesh, input_dict
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_a_mask.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_a_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     List,
     Optional,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     get_activation_func,
     get_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     default_tf_session_config,
     op_module,
     tf,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     embedding_net_rand_seed_shift,
 )
 
 from .descriptor import (
     Descriptor,
 )
 from .se_a import (
@@ -69,15 +69,15 @@
     of a embedding network :math:`\mathcal{N}` of :math:`s(r_{ji})`:
 
     .. math::
         (\mathcal{G}^i)_j = \mathcal{N}(s(r_{ji}))
 
     :math:`\mathcal{G}^i_< \in \mathbb{R}^{N \times M_2}` takes first :math:`M_2` columns of
     :math:`\mathcal{G}^i`. The equation of embedding network :math:`\mathcal{N}` can be found at
-    :meth:`deepmd.utils.network.embedding_net`.
+    :meth:`deepmd.tf.utils.network.embedding_net`.
     Specially for descriptor se_a_mask is a concise implementation of se_a.
     The difference is that se_a_mask only considered a non-pbc system.
     And accept a mask matrix to indicate the atom i in frame j is a real atom or not.
     (1 means real atom, 0 means ghost atom)
     Thus se_a_mask can accept a variable number of atoms in a frame.
 
     Parameters
@@ -231,23 +231,23 @@
         **kwargs,
     ) -> None:
         """Compute the statisitcs (avg and std) of the training data. The input will be normalized by the statistics.
 
         Parameters
         ----------
         data_coord
-            The coordinates. Can be generated by deepmd.model.make_stat_input
+            The coordinates. Can be generated by deepmd.tf.model.make_stat_input
         data_box
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         data_atype
-            The atom types. Can be generated by deepmd.model.make_stat_input
+            The atom types. Can be generated by deepmd.tf.model.make_stat_input
         natoms_vec
-            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.model.make_stat_input
+            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.tf.model.make_stat_input
         mesh
-            The mesh for neighbor searching. Can be generated by deepmd.model.make_stat_input
+            The mesh for neighbor searching. Can be generated by deepmd.tf.model.make_stat_input
         input_dict
             Dictionary for additional input
         **kwargs
             Additional keyword arguments.
         """
         """
         TODO: Since not all input atoms are real in se_a_mask,
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_atten.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_atten.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,70 +8,74 @@
 )
 
 import numpy as np
 from packaging.version import (
     Version,
 )
 
-from deepmd.common import (
+from deepmd.tf.common import (
     cast_precision,
     get_np_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     TF_VERSION,
     default_tf_session_config,
     op_module,
     tf,
 )
-from deepmd.nvnmd.descriptor.se_atten import (
+from deepmd.tf.nvnmd.descriptor.se_atten import (
     build_davg_dstd,
     build_op_descriptor,
     check_switch_range,
     descrpt2r4,
     filter_GR2D,
     filter_lower_R42GR,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.utils.compress import (
+from deepmd.tf.utils.compress import (
     get_extra_side_embedding_net_variable,
     get_two_side_type_embedding,
     make_data,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_attention_layer_variables_from_graph_def,
     get_extra_embedding_net_suffix,
     get_extra_embedding_net_variables_from_graph_def,
     get_pattern_nodes_from_graph_def,
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     embedding_net,
     one_layer,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
-from deepmd.utils.tabulate import (
+from deepmd.tf.utils.tabulate import (
     DPTabulate,
 )
+from deepmd.tf.utils.update_sel import (
+    UpdateSel,
+)
 
 from .descriptor import (
     Descriptor,
 )
 from .se_a import (
     DescrptSeA,
 )
 
 log = logging.getLogger(__name__)
 
 
+@Descriptor.register("dpa1")
 @Descriptor.register("se_atten")
 class DescrptSeAtten(DescrptSeA):
     r"""Smooth version descriptor with attention.
 
     Parameters
     ----------
     rcut
@@ -148,21 +152,49 @@
         attn: int = 128,
         attn_layer: int = 2,
         attn_dotr: bool = True,
         attn_mask: bool = False,
         multi_task: bool = False,
         stripped_type_embedding: bool = False,
         smooth_type_embdding: bool = False,
+        # not implemented
+        post_ln=True,
+        ffn=False,
+        ffn_embed_dim=1024,
+        scaling_factor=1.0,
+        head_num=1,
+        normalize=True,
+        temperature=None,
+        return_rot=False,
+        concat_output_tebd: bool = True,
         **kwargs,
     ) -> None:
         if not set_davg_zero and not (stripped_type_embedding and smooth_type_embdding):
             warnings.warn(
                 "Set 'set_davg_zero' False in descriptor 'se_atten' "
                 "may cause unexpected incontinuity during model inference!"
             )
+        if not post_ln:
+            raise NotImplementedError("post_ln is not supported.")
+        if ffn:
+            raise NotImplementedError("ffn is not supported.")
+        if ffn_embed_dim != 1024:
+            raise NotImplementedError("ffn_embed_dim is not supported.")
+        if scaling_factor != 1.0:
+            raise NotImplementedError("scaling_factor is not supported.")
+        if head_num != 1:
+            raise NotImplementedError("head_num is not supported.")
+        if not normalize:
+            raise NotImplementedError("normalize is not supported.")
+        if temperature is not None:
+            raise NotImplementedError("temperature is not supported.")
+        if return_rot:
+            raise NotImplementedError("return_rot is not supported.")
+        if not concat_output_tebd:
+            raise NotImplementedError("concat_output_tebd is not supported.")
         DescrptSeA.__init__(
             self,
             rcut,
             rcut_smth,
             [sel],
             neuron=neuron,
             axis_neuron=axis_neuron,
@@ -265,24 +297,24 @@
         **kwargs,
     ) -> None:
         """Compute the statisitcs (avg and std) of the training data. The input will be normalized by the statistics.
 
         Parameters
         ----------
         data_coord
-            The coordinates. Can be generated by deepmd.model.make_stat_input
+            The coordinates. Can be generated by deepmd.tf.model.make_stat_input
         data_box
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         data_atype
-            The atom types. Can be generated by deepmd.model.make_stat_input
+            The atom types. Can be generated by deepmd.tf.model.make_stat_input
         natoms_vec
             The vector for the number of atoms of the system and different types of atoms.
             If mixed_type is True, this para is blank. See real_natoms_vec.
         mesh
-            The mesh for neighbor searching. Can be generated by deepmd.model.make_stat_input
+            The mesh for neighbor searching. Can be generated by deepmd.tf.model.make_stat_input
         input_dict
             Dictionary for additional input
         mixed_type
             Whether to perform the mixed_type mode.
             If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
             in which frames in a system may have different natoms_vec(s), with the same nloc.
         real_natoms_vec
@@ -986,14 +1018,15 @@
                     trainable=trainable,
                     uniform_seed=self.uniform_seed,
                     initial_variables=self.attention_layer_variables,
                 )
                 input_xyz = tf.keras.layers.LayerNormalization(
                     beta_initializer=tf.constant_initializer(self.beta[i]),
                     gamma_initializer=tf.constant_initializer(self.gamma[i]),
+                    dtype=self.filter_precision,
                 )(input_xyz)
                 # input_xyz = self._feedforward(input_xyz, outputs_size[-1], self.att_n)
         return input_xyz
 
     def _filter_lower(
         self,
         type_i,
@@ -1335,15 +1368,15 @@
         nei_type_vec: tf.Tensor,
     ) -> tf.Tensor:
         r"""Build the type exclude mask for the attention descriptor.
 
         Notes
         -----
         This method has the similiar way to build the type exclude mask as
-        :meth:`deepmd.descriptor.descriptor.Descriptor.build_type_exclude_mask`.
+        :meth:`deepmd.tf.descriptor.descriptor.Descriptor.build_type_exclude_mask`.
         The mathmatical expression has been explained in that method.
         The difference is that the attention descriptor has provided the type of
         the neighbors (idx_j) that is not in order, so we use it from an extra
         input.
 
         Parameters
         ----------
@@ -1369,15 +1402,15 @@
         tf.Tensor
             The type exclude mask, with the shape of (shape0, ndescrpt), and the
             precision of GLOBAL_TF_FLOAT_PRECISION. The mask has the value of 1 if the
             interaction between two types is not excluded, and 0 otherwise.
 
         See Also
         --------
-        deepmd.descriptor.descriptor.Descriptor.build_type_exclude_mask
+        deepmd.tf.descriptor.descriptor.Descriptor.build_type_exclude_mask
         """
         # generate a mask
         # op returns ntypes when the neighbor doesn't exist, so we need to add 1
         type_mask = np.array(
             [
                 [
                     1 if (tt_i, tt_j) not in exclude_types else 0
@@ -1420,13 +1453,9 @@
         Parameters
         ----------
         global_jdata : dict
             The global data, containing the training section
         local_jdata : dict
             The local data refer to the current class
         """
-        from deepmd.entrypoints.train import (
-            update_one_sel,
-        )
-
         local_jdata_cpy = local_jdata.copy()
-        return update_one_sel(global_jdata, local_jdata_cpy, True)
+        return UpdateSel().update_one_sel(global_jdata, local_jdata_cpy, True)
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_atten_v2.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_atten_v2.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_r.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_r.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,42 +3,48 @@
     List,
     Optional,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.dpmodel.utils.env_mat import (
+    EnvMat,
+)
+from deepmd.tf.common import (
     cast_precision,
     get_activation_func,
     get_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     default_tf_session_config,
     op_module,
     tf,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     embedding_net,
     embedding_net_rand_seed_shift,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
-from deepmd.utils.tabulate import (
+from deepmd.tf.utils.tabulate import (
     DPTabulate,
 )
+from deepmd.utils.version import (
+    check_version_compatibility,
+)
 
 from .descriptor import (
     Descriptor,
 )
 from .se import (
     DescrptSe,
 )
@@ -111,16 +117,17 @@
         self.filter_neuron = neuron
         self.filter_resnet_dt = resnet_dt
         self.seed = seed
         self.uniform_seed = uniform_seed
         self.seed_shift = embedding_net_rand_seed_shift(self.filter_neuron)
         self.trainable = trainable
         self.filter_activation_fn = get_activation_func(activation_function)
+        self.activation_function_name = activation_function
         self.filter_precision = get_precision(precision)
-        exclude_types = exclude_types
+        self.orig_exclude_types = exclude_types
         self.exclude_types = set()
         for tt in exclude_types:
             assert len(tt) == 2
             self.exclude_types.add((tt[0], tt[1]))
             self.exclude_types.add((tt[1], tt[0]))
         self.set_davg_zero = set_davg_zero
         self.type_one_side = type_one_side
@@ -231,23 +238,23 @@
         **kwargs,
     ):
         """Compute the statisitcs (avg and std) of the training data. The input will be normalized by the statistics.
 
         Parameters
         ----------
         data_coord
-            The coordinates. Can be generated by deepmd.model.make_stat_input
+            The coordinates. Can be generated by deepmd.tf.model.make_stat_input
         data_box
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         data_atype
-            The atom types. Can be generated by deepmd.model.make_stat_input
+            The atom types. Can be generated by deepmd.tf.model.make_stat_input
         natoms_vec
-            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.model.make_stat_input
+            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.tf.model.make_stat_input
         mesh
-            The mesh for neighbor searching. Can be generated by deepmd.model.make_stat_input
+            The mesh for neighbor searching. Can be generated by deepmd.tf.model.make_stat_input
         input_dict
             Dictionary for additional input
         **kwargs
             Additional keyword arguments.
         """
         sumr = []
         sumn = []
@@ -496,15 +503,18 @@
         atom_virial
             The atomic virial
         """
         [net_deriv] = tf.gradients(atom_ener, self.descrpt_reshape)
         tf.summary.histogram("net_derivative", net_deriv)
         net_deriv_reshape = tf.reshape(
             net_deriv,
-            [np.cast["int64"](-1), natoms[0] * np.cast["int64"](self.ndescrpt)],
+            [
+                np.asarray(-1, dtype=np.int64),
+                natoms[0] * np.asarray(self.ndescrpt, dtype=np.int64),
+            ],
         )
         force = op_module.prod_force_se_r(
             net_deriv_reshape, self.descrpt_deriv, self.nlist, natoms
         )
         virial, atom_virial = op_module.prod_virial_se_r(
             net_deriv_reshape, self.descrpt_deriv, self.rij, self.nlist, natoms
         )
@@ -691,7 +701,99 @@
             xyz_scatter = tf.concat(xyz_scatter_total, axis=1)
             # natom x outputs_size
             #
             res_rescale = 1.0 / 5.0
             result = tf.reduce_mean(xyz_scatter, axis=1) * res_rescale
 
         return result
+
+    @classmethod
+    def deserialize(cls, data: dict, suffix: str = ""):
+        """Deserialize the model.
+
+        Parameters
+        ----------
+        data : dict
+            The serialized data
+
+        Returns
+        -------
+        Model
+            The deserialized model
+        """
+        if cls is not DescrptSeR:
+            raise NotImplementedError("Not implemented in class %s" % cls.__name__)
+        data = data.copy()
+        check_version_compatibility(data.pop("@version", 1), 1, 1)
+        embedding_net_variables = cls.deserialize_network(
+            data.pop("embeddings"), suffix=suffix
+        )
+        data.pop("env_mat")
+        variables = data.pop("@variables")
+        descriptor = cls(**data)
+        descriptor.embedding_net_variables = embedding_net_variables
+        descriptor.davg = variables["davg"].reshape(
+            descriptor.ntypes, descriptor.ndescrpt
+        )
+        descriptor.dstd = variables["dstd"].reshape(
+            descriptor.ntypes, descriptor.ndescrpt
+        )
+        return descriptor
+
+    def serialize(self, suffix: str = "") -> dict:
+        """Serialize the model.
+
+        Parameters
+        ----------
+        suffix : str, optional
+            The suffix of the scope
+
+        Returns
+        -------
+        dict
+            The serialized data
+        """
+        if type(self) is not DescrptSeR:
+            raise NotImplementedError(
+                "Not implemented in class %s" % self.__class__.__name__
+            )
+        if self.embedding_net_variables is None:
+            raise RuntimeError("init_variables must be called before serialize")
+        if self.spin is not None:
+            raise NotImplementedError("spin is unsupported")
+        assert self.davg is not None
+        assert self.dstd is not None
+        # TODO: not sure how to handle type embedding - type embedding is not a model parameter,
+        # but instead a part of the input data. Maybe the interface should be refactored...
+        return {
+            "@class": "Descriptor",
+            "type": "se_r",
+            "@version": 1,
+            "rcut": self.rcut,
+            "rcut_smth": self.rcut_smth,
+            "sel": self.sel_r,
+            "neuron": self.filter_neuron,
+            "resnet_dt": self.filter_resnet_dt,
+            "trainable": self.trainable,
+            "type_one_side": self.type_one_side,
+            "exclude_types": list(self.orig_exclude_types),
+            "set_davg_zero": self.set_davg_zero,
+            "activation_function": self.activation_function_name,
+            "precision": self.filter_precision.name,
+            "embeddings": self.serialize_network(
+                ntypes=self.ntypes,
+                ndim=(1 if self.type_one_side else 2),
+                in_dim=1,
+                neuron=self.filter_neuron,
+                activation_function=self.activation_function_name,
+                resnet_dt=self.filter_resnet_dt,
+                variables=self.embedding_net_variables,
+                excluded_types=self.exclude_types,
+                suffix=suffix,
+            ),
+            "env_mat": EnvMat(self.rcut, self.rcut_smth).serialize(),
+            "@variables": {
+                "davg": self.davg.reshape(self.ntypes, self.nnei_r, 1),
+                "dstd": self.dstd.reshape(self.ntypes, self.nnei_r, 1),
+            },
+            "spin": self.spin,
+        }
```

### Comparing `deepmd_kit-2.2.9/deepmd/descriptor/se_t.py` & `deepmd_kit-3.0.0a0/deepmd/tf/descriptor/se_t.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,37 +3,37 @@
     List,
     Optional,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     cast_precision,
     get_activation_func,
     get_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     default_tf_session_config,
     op_module,
     tf,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     embedding_net,
     embedding_net_rand_seed_shift,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
-from deepmd.utils.tabulate import (
+from deepmd.tf.utils.tabulate import (
     DPTabulate,
 )
 
 from .descriptor import (
     Descriptor,
 )
 from .se import (
@@ -221,23 +221,23 @@
         **kwargs,
     ) -> None:
         """Compute the statisitcs (avg and std) of the training data. The input will be normalized by the statistics.
 
         Parameters
         ----------
         data_coord
-            The coordinates. Can be generated by deepmd.model.make_stat_input
+            The coordinates. Can be generated by deepmd.tf.model.make_stat_input
         data_box
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         data_atype
-            The atom types. Can be generated by deepmd.model.make_stat_input
+            The atom types. Can be generated by deepmd.tf.model.make_stat_input
         natoms_vec
-            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.model.make_stat_input
+            The vector for the number of atoms of the system and different types of atoms. Can be generated by deepmd.tf.model.make_stat_input
         mesh
-            The mesh for neighbor searching. Can be generated by deepmd.model.make_stat_input
+            The mesh for neighbor searching. Can be generated by deepmd.tf.model.make_stat_input
         input_dict
             Dictionary for additional input
         **kwargs
             Additional keyword arguments.
         """
         if True:
             sumr = []
@@ -509,15 +509,18 @@
             The total virial
         atom_virial
             The atomic virial
         """
         [net_deriv] = tf.gradients(atom_ener, self.descrpt_reshape)
         net_deriv_reshape = tf.reshape(
             net_deriv,
-            [np.cast["int64"](-1), natoms[0] * np.cast["int64"](self.ndescrpt)],
+            [
+                np.asarray(-1, dtype=np.int64),
+                natoms[0] * np.asarray(self.ndescrpt, dtype=np.int64),
+            ],
         )
         force = op_module.prod_force_se_a(
             net_deriv_reshape,
             self.descrpt_deriv,
             self.nlist,
             natoms,
             n_a_sel=self.nnei_a,
```

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/__init__.py` & `deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/__init__.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/compress.py` & `deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/compress.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,42 +4,43 @@
 import json
 import logging
 import os
 from typing import (
     Optional,
 )
 
-from deepmd.common import (
+from deepmd.tf.common import (
     j_loader,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_ENER_FLOAT_PRECISION,
     tf,
 )
-from deepmd.utils.argcheck import (
+from deepmd.tf.utils.argcheck import (
     normalize,
 )
-from deepmd.utils.compat import (
+from deepmd.tf.utils.compat import (
     update_deepmd_input,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphTooLargeError,
     GraphWithoutTensorError,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
     load_graph_def,
 )
+from deepmd.tf.utils.update_sel import (
+    UpdateSel,
+)
 
 from .freeze import (
     freeze,
 )
 from .train import (
-    get_min_nbor_dist,
-    get_rcut,
     train,
 )
 
 __all__ = ["compress"]
 
 log = logging.getLogger(__name__)
 
@@ -111,15 +112,18 @@
             raise RuntimeError(
                 f"The input training script {input} ({os.path.abspath(input)}) does not exist! Please check the path of the training script. "
             ) from e
         else:
             log.info("stage 0: compute the min_nbor_dist")
             jdata = j_loader(training_script)
             jdata = update_deepmd_input(jdata)
-            t_min_nbor_dist = get_min_nbor_dist(jdata, get_rcut(jdata))
+            update_sel = UpdateSel()
+            t_min_nbor_dist = update_sel.get_min_nbor_dist(
+                jdata, update_sel.get_rcut(jdata)
+            )
 
     _check_compress_type(graph)
 
     tf.constant(
         t_min_nbor_dist,
         name="train_attr/min_nbor_dist",
         dtype=GLOBAL_ENER_FLOAT_PRECISION,
```

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/convert.py` & `deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
-from deepmd.utils.convert import (
+from deepmd.tf.utils.convert import (
     convert_10_to_21,
     convert_012_to_21,
     convert_12_to_21,
     convert_13_to_21,
     convert_20_to_21,
     convert_pb_to_pbtxt,
     convert_pbtxt_to_pb,
```

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/freeze.py` & `deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/freeze.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,42 @@
 """
 
 import json
 import logging
 from os.path import (
     abspath,
 )
+from pathlib import (
+    Path,
+)
 from typing import (
     List,
     Optional,
     Union,
 )
 
 import google.protobuf.message
 
 # load grad of force module
-import deepmd.op  # noqa: F401
-from deepmd.env import (
+import deepmd.tf.op  # noqa: F401
+from deepmd.tf.env import (
     FITTING_NET_PATTERN,
     REMOVE_SUFFIX_DICT,
     tf,
 )
-from deepmd.nvnmd.entrypoints.freeze import (
+from deepmd.tf.nvnmd.entrypoints.freeze import (
     save_weight,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphTooLargeError,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_pattern_nodes_from_graph_def,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 __all__ = ["freeze"]
 
 log = logging.getLogger(__name__)
 
@@ -352,21 +355,29 @@
         Names of nodes to output, by default None.
     out_suffix : str
         The chosen suffix to freeze in the input_graph.
     """
     output_node = _make_node_names(
         freeze_type, modifier, out_suffix=out_suffix, node_names=node_names
     )
+    # see #3334
+    optional_node = [
+        "train_attr/min_nbor_dist",
+        "fitting_attr/aparam_nall",
+        "spin_attr/ntypes_spin",
+    ]
     different_set = set(output_node) - set(input_node)
     if different_set:
-        log.warning(
-            "The following nodes are not in the graph: %s. "
-            "Skip freezeing these nodes. You may be freezing "
-            "a checkpoint generated by an old version." % different_set
-        )
+        different_set -= set(optional_node)
+        if different_set:
+            log.warning(
+                "The following nodes are not in the graph: %s. "
+                "Skip freezeing these nodes. You may be freezing "
+                "a checkpoint generated by an old version." % different_set
+            )
         # use intersection as output list
         output_node = list(set(output_node) & set(input_node))
     log.info(f"The following nodes will be frozen: {output_node}")
     # We use a built-in TF helper to export variables to constants
     output_graph_def = tf.graph_util.convert_variables_to_constants(
         sess,  # The session is used to retrieve the weights
         input_graph,  # The graph_def is used to retrieve the nodes
@@ -475,29 +486,32 @@
     **kwargs,
 ):
     """Freeze the graph in supplied folder.
 
     Parameters
     ----------
     checkpoint_folder : str
-        location of the folder with model
+        location of either the folder with checkpoint or the checkpoint prefix
     output : str
         output file name
     node_names : Optional[str], optional
         names of nodes to output, by default None
     nvnmd_weight : Optional[str], optional
         nvnmd weight file
     united_model : bool
         when in multi-task mode, freeze all nodes into one unit model
     **kwargs
         other arguments
     """
     # We retrieve our checkpoint fullpath
-    checkpoint = tf.train.get_checkpoint_state(checkpoint_folder)
-    input_checkpoint = checkpoint.model_checkpoint_path
+    if Path(checkpoint_folder).is_dir():
+        checkpoint = tf.train.get_checkpoint_state(checkpoint_folder)
+        input_checkpoint = checkpoint.model_checkpoint_path
+    else:
+        input_checkpoint = checkpoint_folder
 
     # expand the output file to full path
     output_graph = abspath(output)
 
     # Before exporting our graph, we need to precise what is our output node
     # This is how TF decides what part of the Graph he has to keep
     # and what part it can dump
```

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/ipi.py` & `deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/ipi.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import subprocess
 import sys
 from typing import (
     List,
 )
 
-from deepmd.lmp import (
+from deepmd.tf.lmp import (
     get_op_dir,
 )
 
 ROOT_DIR = get_op_dir()
 
 
 def _program(name: str, args: List[str]):
```

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/main.py` & `deepmd_kit-3.0.0a0/deepmd/entrypoints/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,85 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
-"""DeePMD-Kit entry point module."""
+"""Common entrypoints."""
 
 import argparse
 from pathlib import (
     Path,
 )
-from typing import (
-    List,
-    Optional,
-    Union,
-)
 
-from deepmd.common import (
-    clear_session,
-)
-from deepmd.entrypoints import (
-    compress,
-    convert,
+from deepmd.backend.backend import (
+    Backend,
+)
+from deepmd.backend.suffix import (
+    format_model_suffix,
+)
+from deepmd.entrypoints.convert_backend import (
+    convert_backend,
+)
+from deepmd.entrypoints.doc import (
     doc_train_input,
-    freeze,
-    make_model_devi,
-    neighbor_stat,
+)
+from deepmd.entrypoints.gui import (
     start_dpgui,
-    test,
-    train_dp,
-    transfer,
 )
-from deepmd.loggers import (
-    set_log_handles,
+from deepmd.entrypoints.neighbor_stat import (
+    neighbor_stat,
 )
-from deepmd.nvnmd.entrypoints.train import (
-    train_nvnmd,
+from deepmd.entrypoints.test import (
+    test,
 )
-from deepmd_utils.main import (
-    get_ll,
-    main_parser,
-    parse_args,
+from deepmd.infer.model_devi import (
+    make_model_devi,
+)
+from deepmd.loggers.loggers import (
+    set_log_handles,
 )
-
-__all__ = ["main", "parse_args", "get_ll", "main_parser"]
 
 
-def main(args: Optional[Union[List[str], argparse.Namespace]] = None):
+def main(args: argparse.Namespace):
     """DeePMD-Kit entry point.
 
     Parameters
     ----------
     args : List[str] or argparse.Namespace, optional
         list of command line arguments, used to avoid calling from the subprocess,
         as it is quite slow to import tensorflow; if Namespace is given, it will
         be used directly
 
     Raises
     ------
     RuntimeError
         if no command was input
     """
-    if args is not None:
-        clear_session()
-
-    if not isinstance(args, argparse.Namespace):
-        args = parse_args(args=args)
-
-    # do not set log handles for None, it is useless
-    # log handles for train will be set separatelly
-    # when the use of MPI will be determined in `RunOptions`
-    if args.command not in (None, "train"):
-        set_log_handles(args.log_level, Path(args.log_path) if args.log_path else None)
+    set_log_handles(args.log_level, Path(args.log_path) if args.log_path else None)
 
     dict_args = vars(args)
 
-    if args.command == "train":
-        train_dp(**dict_args)
-    elif args.command == "freeze":
-        freeze(**dict_args)
-    elif args.command == "test":
+    if args.command == "test":
+        dict_args["model"] = format_model_suffix(
+            dict_args["model"],
+            feature=Backend.Feature.DEEP_EVAL,
+            preferred_backend=args.backend,
+            strict_prefer=False,
+        )
         test(**dict_args)
-    elif args.command == "transfer":
-        transfer(**dict_args)
-    elif args.command == "compress":
-        compress(**dict_args)
     elif args.command == "doc-train-input":
         doc_train_input(**dict_args)
     elif args.command == "model-devi":
+        dict_args["models"] = [
+            format_model_suffix(
+                mm,
+                feature=Backend.Feature.DEEP_EVAL,
+                preferred_backend=args.backend,
+                strict_prefer=False,
+            )
+            for mm in dict_args["models"]
+        ]
         make_model_devi(**dict_args)
-    elif args.command == "convert-from":
-        convert(**dict_args)
     elif args.command == "neighbor-stat":
         neighbor_stat(**dict_args)
-    elif args.command == "train-nvnmd":  # nvnmd
-        train_nvnmd(**dict_args)
     elif args.command == "gui":
         start_dpgui(**dict_args)
-    elif args.command is None:
-        pass
+    elif args.command == "convert-backend":
+        convert_backend(**dict_args)
     else:
-        raise RuntimeError(f"unknown command {args.command}")
-
-    if args is not None:
-        clear_session()
+        raise ValueError(f"Unknown command: {args.command}")
```

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/test.py` & `deepmd_kit-3.0.0a0/deepmd/entrypoints/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,37 +10,53 @@
     List,
     Optional,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd import (
-    DeepPotential,
-)
 from deepmd.common import (
     expand_sys_str,
 )
+from deepmd.infer.deep_dipole import (
+    DeepDipole,
+)
+from deepmd.infer.deep_dos import (
+    DeepDOS,
+)
+from deepmd.infer.deep_eval import (
+    DeepEval,
+)
+from deepmd.infer.deep_polar import (
+    DeepGlobalPolar,
+    DeepPolar,
+)
+from deepmd.infer.deep_pot import (
+    DeepPot,
+)
+from deepmd.infer.deep_wfc import (
+    DeepWFC,
+)
 from deepmd.utils import random as dp_random
 from deepmd.utils.data import (
     DeepmdData,
 )
 from deepmd.utils.weight_avg import (
     weighted_average,
 )
 
 if TYPE_CHECKING:
-    from deepmd.infer import (
+    from deepmd.tf.infer import (
         DeepDipole,
         DeepDOS,
         DeepPolar,
         DeepPot,
         DeepWFC,
     )
-    from deepmd.infer.deep_tensor import (
+    from deepmd.tf.infer.deep_tensor import (
         DeepTensor,
     )
 
 __all__ = ["test"]
 
 log = logging.getLogger(__name__)
 
@@ -52,14 +68,15 @@
     datafile: str,
     set_prefix: str,
     numb_test: int,
     rand_seed: Optional[int],
     shuffle_test: bool,
     detail_file: str,
     atomic: bool,
+    head: Optional[str] = None,
     **kwargs,
 ):
     """Test model predictions.
 
     Parameters
     ----------
     model : str
@@ -76,83 +93,84 @@
         seed for random generator
     shuffle_test : bool
         whether to shuffle tests
     detail_file : Optional[str]
         file where test details will be output
     atomic : bool
         whether per atom quantities should be computed
+    head : Optional[str], optional
+        (Supported backend: PyTorch) Task head to test if in multi-task mode.
     **kwargs
         additional arguments
 
     Raises
     ------
     RuntimeError
         if no valid system was found
     """
     if numb_test == 0:
         # only float has inf, but should work for min
         numb_test = float("inf")
     if datafile is not None:
-        datalist = open(datafile)
-        all_sys = datalist.read().splitlines()
-        datalist.close()
+        with open(datafile) as datalist:
+            all_sys = datalist.read().splitlines()
     else:
         all_sys = expand_sys_str(system)
 
     if len(all_sys) == 0:
         raise RuntimeError("Did not find valid system")
     err_coll = []
     siz_coll = []
 
     # init random seed
     if rand_seed is not None:
         dp_random.seed(rand_seed % (2**32))
 
     # init model
-    dp = DeepPotential(model)
+    dp = DeepEval(model, head=head)
 
     for cc, system in enumerate(all_sys):
         log.info("# ---------------output of dp test--------------- ")
         log.info(f"# testing system : {system}")
 
         # create data class
-        tmap = dp.get_type_map() if dp.model_type == "ener" else None
+        tmap = dp.get_type_map() if isinstance(dp, DeepPot) else None
         data = DeepmdData(
             system,
             set_prefix,
             shuffle_test=shuffle_test,
             type_map=tmap,
             sort_atoms=False,
         )
 
-        if dp.model_type == "ener":
+        if isinstance(dp, DeepPot):
             err = test_ener(
                 dp,
                 data,
                 system,
                 numb_test,
                 detail_file,
                 atomic,
                 append_detail=(cc != 0),
             )
-        elif dp.model_type == "dos":
+        elif isinstance(dp, DeepDOS):
             err = test_dos(
                 dp,
                 data,
                 system,
                 numb_test,
                 detail_file,
                 atomic,
                 append_detail=(cc != 0),
             )
-        elif dp.model_type == "dipole":
+        elif isinstance(dp, DeepDipole):
             err = test_dipole(dp, data, numb_test, detail_file, atomic)
-        elif dp.model_type == "polar":
+        elif isinstance(dp, DeepPolar):
             err = test_polar(dp, data, numb_test, detail_file, atomic=atomic)
-        elif dp.model_type == "global_polar":  # should not appear in this new version
+        elif isinstance(dp, DeepGlobalPolar):  # should not appear in this new version
             log.warning(
                 "Global polar model is not currently supported. Please directly use the polar mode and change loss parameters."
             )
             err = test_polar(
                 dp, data, numb_test, detail_file, atomic=False
             )  # YWolfeee: downward compatibility
         log.info("# ----------------------------------------------- ")
@@ -162,25 +180,25 @@
 
     if len(all_sys) != len(err_coll):
         log.warning("Not all systems are tested! Check if the systems are valid")
 
     if len(all_sys) > 1:
         log.info("# ----------weighted average of errors----------- ")
         log.info(f"# number of systems : {len(all_sys)}")
-        if dp.model_type == "ener":
+        if isinstance(dp, DeepPot):
             print_ener_sys_avg(avg_err)
-        elif dp.model_type == "dos":
+        elif isinstance(dp, DeepDOS):
             print_dos_sys_avg(avg_err)
-        elif dp.model_type == "dipole":
+        elif isinstance(dp, DeepDipole):
             print_dipole_sys_avg(avg_err)
-        elif dp.model_type == "polar":
+        elif isinstance(dp, DeepPolar):
             print_polar_sys_avg(avg_err)
-        elif dp.model_type == "global_polar":
+        elif isinstance(dp, DeepGlobalPolar):
             print_polar_sys_avg(avg_err)
-        elif dp.model_type == "wfc":
+        elif isinstance(dp, DeepGlobalPolar):
             print_wfc_sys_avg(avg_err)
         log.info("# ----------------------------------------------- ")
 
 
 def mae(diff: np.ndarray) -> float:
     """Calcalte mean absulote error.
 
@@ -838,14 +856,18 @@
     # YWolfeee: do summation in global polar mode
     if not atomic:
         polar = np.sum(polar.reshape((polar.shape[0], -1, 9)), axis=1)
         rmse_f = rmse(polar - test_data["polarizability"][:numb_test])
         rmse_fs = rmse_f / np.sqrt(sel_natoms)
         rmse_fa = rmse_f / sel_natoms
     else:
+        sel_mask = np.isin(atype, sel_type)
+        polar = polar.reshape((polar.shape[0], -1, 9))[:, sel_mask, :].reshape(
+            (polar.shape[0], -1)
+        )
         rmse_f = rmse(polar - test_data["atomic_polarizability"][:numb_test])
 
     log.info(f"# number of test data : {numb_test:d} ")
     log.info(f"Polarizability  RMSE       : {rmse_f:e}")
     if not atomic:
         log.info(f"Polarizability  RMSE/sqrtN : {rmse_fs:e}")
         log.info(f"Polarizability  RMSE/N     : {rmse_fa:e}")
@@ -974,14 +996,18 @@
     # do summation in atom dimension
     if not atomic:
         dipole = np.sum(dipole.reshape((dipole.shape[0], -1, 3)), axis=1)
         rmse_f = rmse(dipole - test_data["dipole"][:numb_test])
         rmse_fs = rmse_f / np.sqrt(sel_natoms)
         rmse_fa = rmse_f / sel_natoms
     else:
+        sel_mask = np.isin(atype, sel_type)
+        dipole = dipole.reshape((dipole.shape[0], -1, 3))[:, sel_mask, :].reshape(
+            (dipole.shape[0], -1)
+        )
         rmse_f = rmse(dipole - test_data["atomic_dipole"][:numb_test])
 
     log.info(f"# number of test data : {numb_test:d}")
     log.info(f"Dipole  RMSE       : {rmse_f:e}")
     if not atomic:
         log.info(f"Dipole  RMSE/sqrtN : {rmse_fs:e}")
         log.info(f"Dipole  RMSE/N     : {rmse_fa:e}")
```

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/train.py` & `deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/train.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,61 +9,49 @@
 import time
 from typing import (
     Any,
     Dict,
     Optional,
 )
 
-from deepmd.common import (
-    data_requirement,
-    expand_sys_str,
+from deepmd.tf.common import (
     j_loader,
     j_must_have,
 )
-from deepmd.env import (
-    GLOBAL_ENER_FLOAT_PRECISION,
+from deepmd.tf.env import (
     reset_default_tf_session_config,
     tf,
 )
-from deepmd.infer.data_modifier import (
+from deepmd.tf.infer.data_modifier import (
     DipoleChargeModifier,
 )
-from deepmd.model.model import (
+from deepmd.tf.model.model import (
     Model,
 )
-from deepmd.train.run_options import (
-    BUILD,
-    CITATION,
-    WELCOME,
+from deepmd.tf.train.run_options import (
     RunOptions,
 )
-from deepmd.train.trainer import (
+from deepmd.tf.train.trainer import (
     DPTrainer,
 )
-from deepmd.utils import random as dp_random
-from deepmd.utils.argcheck import (
+from deepmd.tf.utils import random as dp_random
+from deepmd.tf.utils.argcheck import (
     normalize,
 )
-from deepmd.utils.compat import (
+from deepmd.tf.utils.compat import (
     update_deepmd_input,
 )
-from deepmd.utils.data_system import (
-    DeepmdDataSystem,
-)
-from deepmd.utils.finetune import (
+from deepmd.tf.utils.finetune import (
     replace_model_params_with_pretrained_model,
 )
-from deepmd.utils.multi_init import (
+from deepmd.tf.utils.multi_init import (
     replace_model_params_with_frz_multi_model,
 )
-from deepmd.utils.neighbor_stat import (
-    NeighborStat,
-)
-from deepmd.utils.path import (
-    DPPath,
+from deepmd.utils.data_system import (
+    get_data,
 )
 
 __all__ = ["train"]
 
 log = logging.getLogger(__name__)
 
 
@@ -155,17 +143,14 @@
     # remove white spaces as it is not compressed
     tf.constant(
         json.dumps(jdata, separators=(",", ":")),
         name="train_attr/training_script",
         dtype=tf.string,
     )
 
-    for message in WELCOME + CITATION + BUILD:
-        log.info(message)
-
     run_opt.print_resource_summary()
     if origin_type_map is not None:
         jdata["model"]["origin_type_map"] = origin_type_map
     _do_work(jdata, run_opt, is_compress)
 
 
 def _do_work(jdata: Dict[str, Any], run_opt: RunOptions, is_compress: bool = False):
@@ -287,61 +272,14 @@
         log.info("finished training")
         log.info(f"wall time: {(end_time - start_time):.3f} s")
     else:
         model.save_compressed()
         log.info("finished compressing")
 
 
-def get_data(jdata: Dict[str, Any], rcut, type_map, modifier, multi_task_mode=False):
-    systems = j_must_have(jdata, "systems")
-    if isinstance(systems, str):
-        systems = expand_sys_str(systems)
-    elif isinstance(systems, list):
-        systems = systems.copy()
-    help_msg = "Please check your setting for data systems"
-    # check length of systems
-    if len(systems) == 0:
-        msg = "cannot find valid a data system"
-        log.fatal(msg)
-        raise OSError(msg, help_msg)
-    # rougly check all items in systems are valid
-    for ii in systems:
-        ii = DPPath(ii)
-        if not ii.is_dir():
-            msg = f"dir {ii} is not a valid dir"
-            log.fatal(msg)
-            raise OSError(msg, help_msg)
-        if not (ii / "type.raw").is_file():
-            msg = f"dir {ii} is not a valid data system dir"
-            log.fatal(msg)
-            raise OSError(msg, help_msg)
-
-    batch_size = j_must_have(jdata, "batch_size")
-    sys_probs = jdata.get("sys_probs", None)
-    auto_prob = jdata.get("auto_prob", "prob_sys_size")
-    optional_type_map = not multi_task_mode
-
-    data = DeepmdDataSystem(
-        systems=systems,
-        batch_size=batch_size,
-        test_size=1,  # to satisfy the old api
-        shuffle_test=True,  # to satisfy the old api
-        rcut=rcut,
-        type_map=type_map,
-        optional_type_map=optional_type_map,
-        modifier=modifier,
-        trn_all_set=True,  # sample from all sets
-        sys_probs=sys_probs,
-        auto_prob_style=auto_prob,
-    )
-    data.add_dict(data_requirement)
-
-    return data
-
-
 def get_modifier(modi_data=None):
     modifier: Optional[DipoleChargeModifier]
     if modi_data is not None:
         if modi_data["type"] == "dipole_charge":
             modifier = DipoleChargeModifier(
                 modi_data["model_name"],
                 modi_data["model_charge_map"],
@@ -352,162 +290,14 @@
         else:
             raise RuntimeError("unknown modifier type " + str(modi_data["type"]))
     else:
         modifier = None
     return modifier
 
 
-def get_rcut(jdata):
-    if jdata["model"].get("type") == "pairwise_dprc":
-        return max(
-            jdata["model"]["qm_model"]["descriptor"]["rcut"],
-            jdata["model"]["qmmm_model"]["descriptor"]["rcut"],
-        )
-    descrpt_data = jdata["model"]["descriptor"]
-    rcut_list = []
-    if descrpt_data["type"] == "hybrid":
-        for ii in descrpt_data["list"]:
-            rcut_list.append(ii["rcut"])
-    else:
-        rcut_list.append(descrpt_data["rcut"])
-    return max(rcut_list)
-
-
-def get_type_map(jdata):
-    return jdata["model"].get("type_map", None)
-
-
-def get_nbor_stat(jdata, rcut, one_type: bool = False):
-    # it seems that DeepmdDataSystem does not need rcut
-    # it's not clear why there is an argument...
-    # max_rcut = get_rcut(jdata)
-    max_rcut = rcut
-    type_map = get_type_map(jdata)
-
-    if type_map and len(type_map) == 0:
-        type_map = None
-    multi_task_mode = "data_dict" in jdata["training"]
-    if not multi_task_mode:
-        train_data = get_data(
-            jdata["training"]["training_data"], max_rcut, type_map, None
-        )
-        train_data.get_batch()
-    else:
-        assert (
-            type_map is not None
-        ), "Data stat in multi-task mode must have available type_map! "
-        train_data = None
-        for systems in jdata["training"]["data_dict"]:
-            tmp_data = get_data(
-                jdata["training"]["data_dict"][systems]["training_data"],
-                max_rcut,
-                type_map,
-                None,
-            )
-            tmp_data.get_batch()
-            assert tmp_data.get_type_map(), f"In multi-task mode, 'type_map.raw' must be defined in data systems {systems}! "
-            if train_data is None:
-                train_data = tmp_data
-            else:
-                train_data.system_dirs += tmp_data.system_dirs
-                train_data.data_systems += tmp_data.data_systems
-                train_data.natoms += tmp_data.natoms
-                train_data.natoms_vec += tmp_data.natoms_vec
-                train_data.default_mesh += tmp_data.default_mesh
-    data_ntypes = train_data.get_ntypes()
-    if type_map is not None:
-        map_ntypes = len(type_map)
-    else:
-        map_ntypes = data_ntypes
-    ntypes = max([map_ntypes, data_ntypes])
-
-    neistat = NeighborStat(ntypes, rcut, one_type=one_type)
-
-    min_nbor_dist, max_nbor_size = neistat.get_stat(train_data)
-
-    # moved from traier.py as duplicated
-    # TODO: this is a simple fix but we should have a clear
-    #       architecture to call neighbor stat
-    tf.constant(
-        min_nbor_dist,
-        name="train_attr/min_nbor_dist",
-        dtype=GLOBAL_ENER_FLOAT_PRECISION,
-    )
-    tf.constant(max_nbor_size, name="train_attr/max_nbor_size", dtype=tf.int32)
-    return min_nbor_dist, max_nbor_size
-
-
-def get_sel(jdata, rcut, one_type: bool = False):
-    _, max_nbor_size = get_nbor_stat(jdata, rcut, one_type=one_type)
-    return max_nbor_size
-
-
-def get_min_nbor_dist(jdata, rcut):
-    min_nbor_dist, _ = get_nbor_stat(jdata, rcut)
-    return min_nbor_dist
-
-
-def parse_auto_sel(sel):
-    if not isinstance(sel, str):
-        return False
-    words = sel.split(":")
-    if words[0] == "auto":
-        return True
-    else:
-        return False
-
-
-def parse_auto_sel_ratio(sel):
-    if not parse_auto_sel(sel):
-        raise RuntimeError(f"invalid auto sel format {sel}")
-    else:
-        words = sel.split(":")
-        if len(words) == 1:
-            ratio = 1.1
-        elif len(words) == 2:
-            ratio = float(words[1])
-        else:
-            raise RuntimeError(f"invalid auto sel format {sel}")
-        return ratio
-
-
-def wrap_up_4(xx):
-    return 4 * ((int(xx) + 3) // 4)
-
-
-def update_one_sel(jdata, descriptor, one_type: bool = False):
-    rcut = descriptor["rcut"]
-    tmp_sel = get_sel(
-        jdata,
-        rcut,
-        one_type=one_type,
-    )
-    sel = descriptor["sel"]
-    if isinstance(sel, int):
-        # convert to list and finnally convert back to int
-        sel = [sel]
-    if parse_auto_sel(descriptor["sel"]):
-        ratio = parse_auto_sel_ratio(descriptor["sel"])
-        descriptor["sel"] = sel = [int(wrap_up_4(ii * ratio)) for ii in tmp_sel]
-    else:
-        # sel is set by user
-        for ii, (tt, dd) in enumerate(zip(tmp_sel, sel)):
-            if dd and tt > dd:
-                # we may skip warning for sel=0, where the user is likely
-                # to exclude such type in the descriptor
-                log.warning(
-                    "sel of type %d is not enough! The expected value is "
-                    "not less than %d, but you set it to %d. The accuracy"
-                    " of your model may get worse." % (ii, tt, dd)
-                )
-    if one_type:
-        descriptor["sel"] = sel = sum(sel)
-    return descriptor
-
-
 def update_sel(jdata):
     log.info(
         "Calculate neighbor statistics... (add --skip-neighbor-stat to skip this step)"
     )
     jdata_cpy = jdata.copy()
     jdata_cpy["model"] = Model.update_sel(jdata, jdata["model"])
     return jdata_cpy
```

### Comparing `deepmd_kit-2.2.9/deepmd/entrypoints/transfer.py` & `deepmd_kit-3.0.0a0/deepmd/tf/entrypoints/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Dict,
     Optional,
     Sequence,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     TRANSFER_PATTERN,
     tf,
 )
 
 __all__ = ["transfer"]
 
 log = logging.getLogger(__name__)
```

### Comparing `deepmd_kit-2.2.9/deepmd/env.py` & `deepmd_kit-3.0.0a0/deepmd/tf/env.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Module that sets tensorflow working environment and exports inportant constants."""
 
 import ctypes
-import logging
 import os
 import platform
-from configparser import (
-    ConfigParser,
-)
 from importlib import (
     import_module,
     reload,
 )
 from pathlib import (
     Path,
 )
 from typing import (
     TYPE_CHECKING,
     Any,
-    Dict,
-    Tuple,
 )
 
 import numpy as np
 from packaging.version import (
     Version,
 )
 
-import deepmd.lib
-from deepmd_utils.env import (
+from deepmd.env import (
+    GLOBAL_CONFIG,
     GLOBAL_ENER_FLOAT_PRECISION,
     GLOBAL_NP_FLOAT_PRECISION,
+    SHARED_LIB_DIR,
+    SHARED_LIB_MODULE,
+)
+from deepmd.env import get_default_nthreads as get_tf_default_nthreads
+from deepmd.env import (
     global_float_prec,
 )
+from deepmd.env import set_default_nthreads as set_tf_default_nthreads
+from deepmd.env import (
+    set_env_if_empty,
+)
 
 if TYPE_CHECKING:
     from types import (
         ModuleType,
     )
 
 
@@ -68,15 +71,17 @@
     dlopen_library("nvidia.cublas.lib", "libcublas.so*")
     dlopen_library("nvidia.cufft.lib", "libcufft.so*")
     dlopen_library("nvidia.curand.lib", "libcurand.so*")
     dlopen_library("nvidia.cusolver.lib", "libcusolver.so*")
     dlopen_library("nvidia.cusparse.lib", "libcusparse.so*")
     dlopen_library("nvidia.cudnn.lib", "libcudnn.so*")
 
-
+# keras 3 is incompatible with tf.compat.v1
+# https://keras.io/getting_started/#tensorflow--keras-2-backwards-compatibility
+os.environ["TF_USE_LEGACY_KERAS"] = "1"
 # import tensorflow v1 compatability
 try:
     import tensorflow.compat.v1 as tf
 
     tf.disable_v2_behavior()
 except ImportError:
     import tensorflow as tf
@@ -103,59 +108,68 @@
     "TRANSFER_PATTERN",
     "FITTING_NET_PATTERN",
     "EMBEDDING_NET_PATTERN",
     "TYPE_EMBEDDING_PATTERN",
     "ATTENTION_LAYER_PATTERN",
     "REMOVE_SUFFIX_DICT",
     "TF_VERSION",
+    "tf_py_version",
 ]
 
-SHARED_LIB_MODULE = "lib"
-SHARED_LIB_DIR = Path(deepmd.lib.__path__[0])
-CONFIG_FILE = SHARED_LIB_DIR / "run_config.ini"
 
 # Python library version
 try:
     tf_py_version = tf.version.VERSION
 except AttributeError:
     tf_py_version = tf.__version__
 
+# subpatterns:
+# \1: type of centeral atom
+# \2: weight name
+# \3: layer index
+# The rest: types of neighbor atoms
+# IMPORTANT: the order is critical to match the pattern
 EMBEDDING_NET_PATTERN = str(
-    r"filter_type_\d+/matrix_\d+_\d+|"
-    r"filter_type_\d+/bias_\d+_\d+|"
-    r"filter_type_\d+/idt_\d+_\d+|"
-    r"filter_type_all/matrix_\d+|"
-    r"filter_type_all/matrix_\d+_\d+|"
-    r"filter_type_all/matrix_\d+_\d+_\d+|"
-    r"filter_type_all/bias_\d+|"
-    r"filter_type_all/bias_\d+_\d+|"
-    r"filter_type_all/bias_\d+_\d+_\d+|"
-    r"filter_type_all/idt_\d+|"
-    r"filter_type_all/idt_\d+_\d+|"
-)
-
+    r"filter_type_(\d+)/(matrix)_(\d+)_(\d+)|"
+    r"filter_type_(\d+)/(bias)_(\d+)_(\d+)|"
+    r"filter_type_(\d+)/(idt)_(\d+)_(\d+)|"
+    r"filter_type_(all)/(matrix)_(\d+)_(\d+)_(\d+)|"
+    r"filter_type_(all)/(matrix)_(\d+)_(\d+)|"
+    r"filter_type_(all)/(matrix)_(\d+)|"
+    r"filter_type_(all)/(bias)_(\d+)_(\d+)_(\d+)|"
+    r"filter_type_(all)/(bias)_(\d+)_(\d+)|"
+    r"filter_type_(all)/(bias)_(\d+)|"
+    r"filter_type_(all)/(idt)_(\d+)_(\d+)|"
+    r"filter_type_(all)/(idt)_(\d+)|"
+)[:-1]
+
+# subpatterns:
+# \1: layer index or "final"
+# \2: type of centeral atom, optional
+# the last: weight name
 FITTING_NET_PATTERN = str(
-    r"layer_\d+/matrix|"
-    r"layer_\d+_type_\d+/matrix|"
-    r"layer_\d+/bias|"
-    r"layer_\d+_type_\d+/bias|"
-    r"layer_\d+/idt|"
-    r"layer_\d+_type_\d+/idt|"
-    r"final_layer/matrix|"
-    r"final_layer_type_\d+/matrix|"
-    r"final_layer/bias|"
-    r"final_layer_type_\d+/bias|"
+    r"layer_(\d+)/(matrix)|"
+    r"layer_(\d+)_type_(\d+)/(matrix)|"
+    r"layer_(\d+)/(bias)|"
+    r"layer_(\d+)_type_(\d+)/(bias)|"
+    r"layer_(\d+)/(idt)|"
+    r"layer_(\d+)_type_(\d+)/(idt)|"
+    r"(final)_layer/(matrix)|"
+    r"(final)_layer_type_(\d+)/(matrix)|"
+    r"(final)_layer/(bias)|"
+    r"(final)_layer_type_(\d+)/(bias)|"
+    # TODO: not sure how to parse for shared layers...
     # layer_name
     r"share_.+_type_\d/matrix|"
     r"share_.+_type_\d/bias|"
     r"share_.+_type_\d/idt|"
     r"share_.+/matrix|"
     r"share_.+/bias|"
     r"share_.+/idt|"
-)
+)[:-1]
 
 TYPE_EMBEDDING_PATTERN = str(
     r"type_embed_net+/matrix_\d+|"
     r"type_embed_net+/bias_\d+|"
     r"type_embed_net+/idt_\d+|"
 )
 
@@ -212,34 +226,14 @@
     "o_dm_force_{}": "o_dm_force",
     "o_dm_virial_{}": "o_dm_virial",
     "o_dm_av_{}": "o_dm_av",
     "o_wfc_{}": "o_wfc",
 }
 
 
-def set_env_if_empty(key: str, value: str, verbose: bool = True):
-    """Set environment variable only if it is empty.
-
-    Parameters
-    ----------
-    key : str
-        env variable name
-    value : str
-        env variable value
-    verbose : bool, optional
-        if True action will be logged, by default True
-    """
-    if os.environ.get(key) is None:
-        os.environ[key] = value
-        if verbose:
-            logging.warning(
-                f"Environment variable {key} is empty. Use the default value {value}"
-            )
-
-
 def set_mkl():
     """Tuning MKL for the best performance.
 
     References
     ----------
     TF overview
     https://www.tensorflow.org/guide/performance/overview
@@ -266,52 +260,14 @@
         )
     if is_mkl:
         set_env_if_empty("KMP_BLOCKTIME", "0")
         set_env_if_empty("KMP_AFFINITY", "granularity=fine,verbose,compact,1,0")
         reload(np)
 
 
-def set_tf_default_nthreads():
-    """Set TF internal number of threads to default=automatic selection.
-
-    Notes
-    -----
-    `TF_INTRA_OP_PARALLELISM_THREADS` and `TF_INTER_OP_PARALLELISM_THREADS`
-    control TF configuration of multithreading.
-    """
-    if (
-        "OMP_NUM_THREADS" not in os.environ
-        or "TF_INTRA_OP_PARALLELISM_THREADS" not in os.environ
-        or "TF_INTER_OP_PARALLELISM_THREADS" not in os.environ
-    ):
-        logging.warning(
-            "To get the best performance, it is recommended to adjust "
-            "the number of threads by setting the environment variables "
-            "OMP_NUM_THREADS, TF_INTRA_OP_PARALLELISM_THREADS, and "
-            "TF_INTER_OP_PARALLELISM_THREADS. See "
-            "https://deepmd.rtfd.io/parallelism/ for more information."
-        )
-    set_env_if_empty("TF_INTRA_OP_PARALLELISM_THREADS", "0", verbose=False)
-    set_env_if_empty("TF_INTER_OP_PARALLELISM_THREADS", "0", verbose=False)
-
-
-def get_tf_default_nthreads() -> Tuple[int, int]:
-    """Get TF paralellism settings.
-
-    Returns
-    -------
-    Tuple[int, int]
-        number of `TF_INTRA_OP_PARALLELISM_THREADS` and
-        `TF_INTER_OP_PARALLELISM_THREADS`
-    """
-    return int(os.environ.get("TF_INTRA_OP_PARALLELISM_THREADS", "0")), int(
-        os.environ.get("TF_INTER_OP_PARALLELISM_THREADS", "0")
-    )
-
-
 def get_tf_session_config() -> Any:
     """Configure tensorflow session.
 
     Returns
     -------
     Any
         session configure object
@@ -447,41 +403,28 @@
                     "\nWARNING: devtoolset on RHEL6 and RHEL7 does not support _GLIBCXX_USE_CXX11_ABI=1. "
                     "See https://bugzilla.redhat.com/show_bug.cgi?id=1546704"
                 )
             raise RuntimeError(error_message) from e
         return module
 
 
-def _get_package_constants(
-    config_file: Path = CONFIG_FILE,
-) -> Dict[str, str]:
-    """Read package constants set at compile time by CMake to dictionary.
-
-    Parameters
-    ----------
-    config_file : str, optional
-        path to CONFIG file, by default "run_config.ini"
-
-    Returns
-    -------
-    Dict[str, str]
-        dictionary with package constants
-    """
-    config = ConfigParser()
-    config.read(config_file)
-    return dict(config.items("CONFIG"))
-
-
-GLOBAL_CONFIG = _get_package_constants()
+if GLOBAL_CONFIG["enable_tensorflow"] == "0":
+    raise RuntimeError(
+        "TensorFlow backend is not built. To enable it, "
+        "set the environmental variable DP_ENABLE_TENSORFLOW=1."
+    )
 MODEL_VERSION = GLOBAL_CONFIG["model_version"]
 TF_VERSION = GLOBAL_CONFIG["tf_version"]
 TF_CXX11_ABI_FLAG = int(GLOBAL_CONFIG["tf_cxx11_abi_flag"])
 
 op_module = get_module("deepmd_op")
 op_grads_module = get_module("op_grads")
+# prevent OOM when using with other backends
+# tf.config doesn't work for unclear reason
+set_env_if_empty("TF_FORCE_GPU_ALLOW_GROWTH", "true", verbose=False)
 
 # FLOAT_PREC
 GLOBAL_TF_FLOAT_PRECISION = tf.dtypes.as_dtype(GLOBAL_NP_FLOAT_PRECISION)
 
 
 def global_cvt_2_tf_float(xx: tf.Tensor) -> tf.Tensor:
     """Cast tensor to globally set TF precision.
```

### Comparing `deepmd_kit-2.2.9/deepmd/fit/dipole.py` & `deepmd_kit-3.0.0a0/deepmd/pt/model/descriptor/repformers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,329 +1,328 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
+    Callable,
+    Dict,
     List,
     Optional,
+    Union,
 )
 
-import numpy as np
+import torch
 
-from deepmd.common import (
-    cast_precision,
-    get_activation_func,
-    get_precision,
+from deepmd.pt.model.descriptor.descriptor import (
+    DescriptorBlock,
 )
-from deepmd.env import (
-    tf,
+from deepmd.pt.model.descriptor.env_mat import (
+    prod_env_mat,
 )
-from deepmd.fit.fitting import (
-    Fitting,
+from deepmd.pt.model.network.network import (
+    SimpleLinear,
 )
-from deepmd.loss.loss import (
-    Loss,
+from deepmd.pt.utils import (
+    env,
 )
-from deepmd.loss.tensor import (
-    TensorLoss,
+from deepmd.pt.utils.env_mat_stat import (
+    EnvMatStatSe,
 )
-from deepmd.utils.graph import (
-    get_fitting_net_variables_from_graph_def,
+from deepmd.pt.utils.utils import (
+    get_activation_fn,
 )
-from deepmd.utils.network import (
-    one_layer,
-    one_layer_rand_seed_shift,
+from deepmd.utils.env_mat_stat import (
+    StatItem,
 )
+from deepmd.utils.path import (
+    DPPath,
+)
+
+from .repformer_layer import (
+    RepformerLayer,
+)
+
+mydtype = env.GLOBAL_PT_FLOAT_PRECISION
+mydev = env.DEVICE
+
 
+def torch_linear(*args, **kwargs):
+    return torch.nn.Linear(*args, **kwargs, dtype=mydtype, device=mydev)
 
-@Fitting.register("dipole")
-class DipoleFittingSeA(Fitting):
-    r"""Fit the atomic dipole with descriptor se_a.
-
-    Parameters
-    ----------
-    descrpt : tf.Tensor
-            The descrptor
-    neuron : List[int]
-            Number of neurons in each hidden layer of the fitting net
-    resnet_dt : bool
-            Time-step `dt` in the resnet construction:
-            y = x + dt * \phi (Wx + b)
-    sel_type : List[int]
-            The atom types selected to have an atomic dipole prediction. If is None, all atoms are selected.
-    seed : int
-            Random seed for initializing the network parameters.
-    activation_function : str
-            The activation function in the embedding net. Supported options are |ACTIVATION_FN|
-    precision : str
-            The precision of the embedding net parameters. Supported options are |PRECISION|
-    uniform_seed
-            Only for the purpose of backward compatibility, retrieves the old behavior of using the random seed
-    """
 
+simple_linear = SimpleLinear
+mylinear = simple_linear
+
+
+@DescriptorBlock.register("se_repformer")
+@DescriptorBlock.register("se_uni")
+class DescrptBlockRepformers(DescriptorBlock):
     def __init__(
         self,
-        descrpt: tf.Tensor,
-        neuron: List[int] = [120, 120, 120],
-        resnet_dt: bool = True,
-        sel_type: Optional[List[int]] = None,
-        seed: Optional[int] = None,
+        rcut,
+        rcut_smth,
+        sel: int,
+        ntypes: int,
+        nlayers: int = 3,
+        g1_dim=128,
+        g2_dim=16,
+        axis_dim: int = 4,
+        direct_dist: bool = False,
+        do_bn_mode: str = "no",
+        bn_momentum: float = 0.1,
+        update_g1_has_conv: bool = True,
+        update_g1_has_drrd: bool = True,
+        update_g1_has_grrg: bool = True,
+        update_g1_has_attn: bool = True,
+        update_g2_has_g1g1: bool = True,
+        update_g2_has_attn: bool = True,
+        update_h2: bool = False,
+        attn1_hidden: int = 64,
+        attn1_nhead: int = 4,
+        attn2_hidden: int = 16,
+        attn2_nhead: int = 4,
+        attn2_has_gate: bool = False,
         activation_function: str = "tanh",
-        precision: str = "default",
-        uniform_seed: bool = False,
-        **kwargs,
-    ) -> None:
-        """Constructor."""
-        self.ntypes = descrpt.get_ntypes()
-        self.dim_descrpt = descrpt.get_dim_out()
-        self.n_neuron = neuron
-        self.resnet_dt = resnet_dt
-        self.sel_type = sel_type
-        if self.sel_type is None:
-            self.sel_type = list(range(self.ntypes))
-        self.sel_mask = np.array(
-            [ii in self.sel_type for ii in range(self.ntypes)], dtype=bool
-        )
-        self.seed = seed
-        self.uniform_seed = uniform_seed
-        self.seed_shift = one_layer_rand_seed_shift()
-        self.fitting_activation_fn = get_activation_func(activation_function)
-        self.fitting_precision = get_precision(precision)
-        self.dim_rot_mat_1 = descrpt.get_dim_rot_mat_1()
-        self.dim_rot_mat = self.dim_rot_mat_1 * 3
-        self.useBN = False
-        self.fitting_net_variables = None
-        self.mixed_prec = None
-
-    def get_sel_type(self) -> int:
-        """Get selected type."""
-        return self.sel_type
-
-    def get_out_size(self) -> int:
-        """Get the output size. Should be 3."""
-        return 3
-
-    def _build_lower(self, start_index, natoms, inputs, rot_mat, suffix="", reuse=None):
-        # cut-out inputs
-        inputs_i = tf.slice(inputs, [0, start_index, 0], [-1, natoms, -1])
-        inputs_i = tf.reshape(inputs_i, [-1, self.dim_descrpt])
-        rot_mat_i = tf.slice(rot_mat, [0, start_index, 0], [-1, natoms, -1])
-        rot_mat_i = tf.reshape(rot_mat_i, [-1, self.dim_rot_mat_1, 3])
-        layer = inputs_i
-        for ii in range(0, len(self.n_neuron)):
-            if ii >= 1 and self.n_neuron[ii] == self.n_neuron[ii - 1]:
-                layer += one_layer(
-                    layer,
-                    self.n_neuron[ii],
-                    name="layer_" + str(ii) + suffix,
-                    reuse=reuse,
-                    seed=self.seed,
-                    use_timestep=self.resnet_dt,
-                    activation_fn=self.fitting_activation_fn,
-                    precision=self.fitting_precision,
-                    uniform_seed=self.uniform_seed,
-                    initial_variables=self.fitting_net_variables,
-                    mixed_prec=self.mixed_prec,
-                )
-            else:
-                layer = one_layer(
-                    layer,
-                    self.n_neuron[ii],
-                    name="layer_" + str(ii) + suffix,
-                    reuse=reuse,
-                    seed=self.seed,
-                    activation_fn=self.fitting_activation_fn,
-                    precision=self.fitting_precision,
-                    uniform_seed=self.uniform_seed,
-                    initial_variables=self.fitting_net_variables,
-                    mixed_prec=self.mixed_prec,
+        update_style: str = "res_avg",
+        set_davg_zero: bool = True,  # TODO
+        smooth: bool = True,
+        add_type_ebd_to_seq: bool = False,
+        type: Optional[str] = None,
+    ):
+        """
+        smooth:
+            If strictly smooth, cannot be used with update_g1_has_attn
+        add_type_ebd_to_seq:
+            At the presence of seq_input (optional input to forward),
+            whether or not add an type embedding to seq_input.
+            If no seq_input is given, it has no effect.
+        """
+        super().__init__()
+        del type
+        self.epsilon = 1e-4  # protection of 1./nnei
+        self.rcut = rcut
+        self.rcut_smth = rcut_smth
+        self.ntypes = ntypes
+        self.nlayers = nlayers
+        sel = [sel] if isinstance(sel, int) else sel
+        self.nnei = sum(sel)
+        self.ndescrpt = self.nnei * 4  # use full descriptor.
+        assert len(sel) == 1
+        self.sel = sel
+        self.sec = self.sel
+        self.split_sel = self.sel
+        self.axis_dim = axis_dim
+        self.set_davg_zero = set_davg_zero
+        self.g1_dim = g1_dim
+        self.g2_dim = g2_dim
+        self.act = get_activation_fn(activation_function)
+        self.direct_dist = direct_dist
+        self.add_type_ebd_to_seq = add_type_ebd_to_seq
+
+        self.g2_embd = mylinear(1, self.g2_dim)
+        layers = []
+        for ii in range(nlayers):
+            layers.append(
+                RepformerLayer(
+                    rcut,
+                    rcut_smth,
+                    sel,
+                    ntypes,
+                    self.g1_dim,
+                    self.g2_dim,
+                    axis_dim=self.axis_dim,
+                    update_chnnl_2=(ii != nlayers - 1),
+                    do_bn_mode=do_bn_mode,
+                    bn_momentum=bn_momentum,
+                    update_g1_has_conv=update_g1_has_conv,
+                    update_g1_has_drrd=update_g1_has_drrd,
+                    update_g1_has_grrg=update_g1_has_grrg,
+                    update_g1_has_attn=update_g1_has_attn,
+                    update_g2_has_g1g1=update_g2_has_g1g1,
+                    update_g2_has_attn=update_g2_has_attn,
+                    update_h2=update_h2,
+                    attn1_hidden=attn1_hidden,
+                    attn1_nhead=attn1_nhead,
+                    attn2_has_gate=attn2_has_gate,
+                    attn2_hidden=attn2_hidden,
+                    attn2_nhead=attn2_nhead,
+                    activation_function=activation_function,
+                    update_style=update_style,
+                    smooth=smooth,
                 )
-            if (not self.uniform_seed) and (self.seed is not None):
-                self.seed += self.seed_shift
-        # (nframes x natoms) x naxis
-        final_layer = one_layer(
-            layer,
-            self.dim_rot_mat_1,
-            activation_fn=None,
-            name="final_layer" + suffix,
-            reuse=reuse,
-            seed=self.seed,
-            precision=self.fitting_precision,
-            uniform_seed=self.uniform_seed,
-            initial_variables=self.fitting_net_variables,
-            mixed_prec=self.mixed_prec,
-            final_layer=True,
-        )
-        if (not self.uniform_seed) and (self.seed is not None):
-            self.seed += self.seed_shift
-        # (nframes x natoms) x 1 * naxis
-        final_layer = tf.reshape(
-            final_layer, [tf.shape(inputs)[0] * natoms, 1, self.dim_rot_mat_1]
-        )
-        # (nframes x natoms) x 1 x 3(coord)
-        final_layer = tf.matmul(final_layer, rot_mat_i)
-        # nframes x natoms x 3
-        final_layer = tf.reshape(final_layer, [tf.shape(inputs)[0], natoms, 3])
-        return final_layer
+            )
+        self.layers = torch.nn.ModuleList(layers)
 
-    @cast_precision
-    def build(
-        self,
-        input_d: tf.Tensor,
-        rot_mat: tf.Tensor,
-        natoms: tf.Tensor,
-        input_dict: Optional[dict] = None,
-        reuse: Optional[bool] = None,
-        suffix: str = "",
-    ) -> tf.Tensor:
-        """Build the computational graph for fitting net.
+        sshape = (self.ntypes, self.nnei, 4)
+        mean = torch.zeros(sshape, dtype=mydtype, device=mydev)
+        stddev = torch.ones(sshape, dtype=mydtype, device=mydev)
+        self.register_buffer("mean", mean)
+        self.register_buffer("stddev", stddev)
+        self.stats = None
+
+    def get_rcut(self) -> float:
+        """Returns the cut-off radius."""
+        return self.rcut
+
+    def get_nsel(self) -> int:
+        """Returns the number of selected atoms in the cut-off radius."""
+        return sum(self.sel)
+
+    def get_sel(self) -> List[int]:
+        """Returns the number of selected atoms for each type."""
+        return self.sel
+
+    def get_ntypes(self) -> int:
+        """Returns the number of element types."""
+        return self.ntypes
+
+    def get_dim_out(self) -> int:
+        """Returns the output dimension."""
+        return self.dim_out
+
+    def get_dim_in(self) -> int:
+        """Returns the input dimension."""
+        return self.dim_in
+
+    def get_dim_emb(self) -> int:
+        """Returns the embedding dimension g2."""
+        return self.g2_dim
+
+    def mixed_types(self) -> bool:
+        """If true, the discriptor
+        1. assumes total number of atoms aligned across frames;
+        2. requires a neighbor list that does not distinguish different atomic types.
+
+        If false, the discriptor
+        1. assumes total number of atoms of each atom type aligned across frames;
+        2. requires a neighbor list that distinguishes different atomic types.
 
-        Parameters
-        ----------
-        input_d
-            The input descriptor
-        rot_mat
-            The rotation matrix from the descriptor.
-        natoms
-            The number of atoms. This tensor has the length of Ntypes + 2
-            natoms[0]: number of local atoms
-            natoms[1]: total number of atoms held by this processor
-            natoms[i]: 2 <= i < Ntypes+2, number of type i atoms
-        input_dict
-            Additional dict for inputs.
-        reuse
-            The weights in the networks should be reused when get the variable.
-        suffix
-            Name suffix to identify this descriptor
-
-        Returns
-        -------
-        dipole
-            The atomic dipole.
         """
-        if input_dict is None:
-            input_dict = {}
-        type_embedding = input_dict.get("type_embedding", None)
-        atype = input_dict.get("atype", None)
-        nframes = input_dict.get("nframes")
-        start_index = 0
-        inputs = tf.reshape(input_d, [-1, natoms[0], self.dim_descrpt])
-        rot_mat = tf.reshape(rot_mat, [-1, natoms[0], self.dim_rot_mat])
-
-        if type_embedding is not None:
-            nloc_mask = tf.reshape(
-                tf.tile(tf.repeat(self.sel_mask, natoms[2:]), [nframes]), [nframes, -1]
-            )
-            atype_nall = tf.reshape(atype, [-1, natoms[1]])
-            # (nframes x nloc_masked)
-            self.atype_nloc_masked = tf.reshape(
-                tf.slice(atype_nall, [0, 0], [-1, natoms[0]])[nloc_mask], [-1]
-            )  ## lammps will make error
-            self.nloc_masked = tf.shape(
-                tf.reshape(self.atype_nloc_masked, [nframes, -1])
-            )[1]
-            atype_embed = tf.nn.embedding_lookup(type_embedding, self.atype_nloc_masked)
-        else:
-            atype_embed = None
+        return True
 
-        self.atype_embed = atype_embed
+    @property
+    def dim_out(self):
+        """Returns the output dimension of this descriptor."""
+        return self.g1_dim
+
+    @property
+    def dim_in(self):
+        """Returns the atomic input dimension of this descriptor."""
+        return self.g1_dim
+
+    @property
+    def dim_emb(self):
+        """Returns the embedding dimension g2."""
+        return self.get_dim_emb()
 
-        if atype_embed is None:
-            count = 0
-            outs_list = []
-            for type_i in range(self.ntypes):
-                if type_i not in self.sel_type:
-                    start_index += natoms[2 + type_i]
-                    continue
-                final_layer = self._build_lower(
-                    start_index,
-                    natoms[2 + type_i],
-                    inputs,
-                    rot_mat,
-                    suffix="_type_" + str(type_i) + suffix,
-                    reuse=reuse,
-                )
-                start_index += natoms[2 + type_i]
-                # concat the results
-                outs_list.append(final_layer)
-                count += 1
-            outs = tf.concat(outs_list, axis=1)
+    def forward(
+        self,
+        nlist: torch.Tensor,
+        extended_coord: torch.Tensor,
+        extended_atype: torch.Tensor,
+        extended_atype_embd: Optional[torch.Tensor] = None,
+        mapping: Optional[torch.Tensor] = None,
+    ):
+        assert mapping is not None
+        assert extended_atype_embd is not None
+        nframes, nloc, nnei = nlist.shape
+        nall = extended_coord.view(nframes, -1).shape[1] // 3
+        atype = extended_atype[:, :nloc]
+        # nb x nloc x nnei x 4, nb x nloc x nnei x 3, nb x nloc x nnei x 1
+        dmatrix, diff, sw = prod_env_mat(
+            extended_coord,
+            nlist,
+            atype,
+            self.mean,
+            self.stddev,
+            self.rcut,
+            self.rcut_smth,
+        )
+        nlist_mask = nlist != -1
+        sw = torch.squeeze(sw, -1)
+        # beyond the cutoff sw should be 0.0
+        sw = sw.masked_fill(~nlist_mask, 0.0)
+
+        # [nframes, nloc, tebd_dim]
+        atype_embd = extended_atype_embd[:, :nloc, :]
+        assert list(atype_embd.shape) == [nframes, nloc, self.g1_dim]
+
+        g1 = self.act(atype_embd)
+        # nb x nloc x nnei x 1,  nb x nloc x nnei x 3
+        if not self.direct_dist:
+            g2, h2 = torch.split(dmatrix, [1, 3], dim=-1)
         else:
-            inputs = tf.reshape(
-                tf.reshape(inputs, [nframes, natoms[0], self.dim_descrpt])[nloc_mask],
-                [-1, self.dim_descrpt],
-            )
-            rot_mat = tf.reshape(
-                tf.reshape(rot_mat, [nframes, natoms[0], self.dim_rot_mat_1 * 3])[
-                    nloc_mask
-                ],
-                [-1, self.dim_rot_mat_1, 3],
-            )
-            atype_embed = tf.cast(atype_embed, self.fitting_precision)
-            type_shape = atype_embed.get_shape().as_list()
-            inputs = tf.concat([inputs, atype_embed], axis=1)
-            self.dim_descrpt = self.dim_descrpt + type_shape[1]
-            inputs = tf.reshape(inputs, [nframes, self.nloc_masked, self.dim_descrpt])
-            rot_mat = tf.reshape(
-                rot_mat, [nframes, self.nloc_masked, self.dim_rot_mat_1 * 3]
+            g2, h2 = torch.linalg.norm(diff, dim=-1, keepdim=True), diff
+            g2 = g2 / self.rcut
+            h2 = h2 / self.rcut
+        # nb x nloc x nnei x ng2
+        g2 = self.act(self.g2_embd(g2))
+
+        # set all padding positions to index of 0
+        # if the a neighbor is real or not is indicated by nlist_mask
+        nlist[nlist == -1] = 0
+        # nb x nall x ng1
+        mapping = mapping.view(nframes, nall).unsqueeze(-1).expand(-1, -1, self.g1_dim)
+        for idx, ll in enumerate(self.layers):
+            # g1:     nb x nloc x ng1
+            # g1_ext: nb x nall x ng1
+            g1_ext = torch.gather(g1, 1, mapping)
+            g1, g2, h2 = ll.forward(
+                g1_ext,
+                g2,
+                h2,
+                nlist,
+                nlist_mask,
+                sw,
             )
-            final_layer = self._build_lower(
-                0, self.nloc_masked, inputs, rot_mat, suffix=suffix, reuse=reuse
-            )
-            # nframes x natoms x 3
-            outs = tf.reshape(final_layer, [nframes, self.nloc_masked, 3])
 
-        tf.summary.histogram("fitting_net_output", outs)
-        return tf.reshape(outs, [-1])
-        # return tf.reshape(outs, [tf.shape(inputs)[0] * natoms[0] * 3 // 3])
+        # uses the last layer.
+        # nb x nloc x 3 x ng2
+        h2g2 = ll._cal_h2g2(g2, h2, nlist_mask, sw)
+        # (nb x nloc) x ng2 x 3
+        rot_mat = torch.permute(h2g2, (0, 1, 3, 2))
 
-    def init_variables(
-        self,
-        graph: tf.Graph,
-        graph_def: tf.GraphDef,
-        suffix: str = "",
-    ) -> None:
-        """Init the fitting net variables with the given dict.
+        return g1, g2, h2, rot_mat.view(-1, nloc, self.dim_emb, 3), sw
 
-        Parameters
-        ----------
-        graph : tf.Graph
-            The input frozen model graph
-        graph_def : tf.GraphDef
-            The input frozen model graph_def
-        suffix : str
-            suffix to name scope
+    def compute_input_stats(
+        self,
+        merged: Union[Callable[[], List[dict]], List[dict]],
+        path: Optional[DPPath] = None,
+    ):
         """
-        self.fitting_net_variables = get_fitting_net_variables_from_graph_def(
-            graph_def, suffix=suffix
-        )
-
-    def enable_mixed_precision(self, mixed_prec: Optional[dict] = None) -> None:
-        """Reveive the mixed precision setting.
+        Compute the input statistics (e.g. mean and stddev) for the descriptors from packed data.
 
         Parameters
         ----------
-        mixed_prec
-            The mixed precision setting used in the embedding net
-        """
-        self.mixed_prec = mixed_prec
-        self.fitting_precision = get_precision(mixed_prec["output_prec"])
+        merged : Union[Callable[[], List[dict]], List[dict]]
+            - List[dict]: A list of data samples from various data systems.
+                Each element, `merged[i]`, is a data dictionary containing `keys`: `torch.Tensor`
+                originating from the `i`-th data system.
+            - Callable[[], List[dict]]: A lazy function that returns data samples in the above format
+                only when needed. Since the sampling process can be slow and memory-intensive,
+                the lazy function helps by only sampling once.
+        path : Optional[DPPath]
+            The path to the stat file.
 
-    def get_loss(self, loss: dict, lr) -> Loss:
-        """Get the loss function.
-
-        Parameters
-        ----------
-        loss : dict
-            the loss dict
-        lr : LearningRateExp
-            the learning rate
-
-        Returns
-        -------
-        Loss
-            the loss function
         """
-        return TensorLoss(
-            loss,
-            model=self,
-            tensor_name="dipole",
-            tensor_size=3,
-            label_name="dipole",
-        )
+        env_mat_stat = EnvMatStatSe(self)
+        if path is not None:
+            path = path / env_mat_stat.get_hash()
+        if path is None or not path.is_dir():
+            if callable(merged):
+                # only get data for once
+                sampled = merged()
+            else:
+                sampled = merged
+        else:
+            sampled = []
+        env_mat_stat.load_or_compute_stats(sampled, path)
+        self.stats = env_mat_stat.stats
+        mean, stddev = env_mat_stat()
+        if not self.set_davg_zero:
+            self.mean.copy_(torch.tensor(mean, device=env.DEVICE))
+        self.stddev.copy_(torch.tensor(stddev, device=env.DEVICE))
+
+    def get_stats(self) -> Dict[str, StatItem]:
+        """Get the statistics of the descriptor."""
+        if self.stats is None:
+            raise RuntimeError(
+                "The statistics of the descriptor has not been computed."
+            )
+        return self.stats
```

### Comparing `deepmd_kit-2.2.9/deepmd/fit/dos.py` & `deepmd_kit-3.0.0a0/deepmd/tf/fit/dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,50 +3,53 @@
 from typing import (
     List,
     Optional,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     add_data_requirement,
     cast_precision,
     get_activation_func,
     get_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     tf,
 )
-from deepmd.fit.fitting import (
+from deepmd.tf.fit.fitting import (
     Fitting,
 )
-from deepmd.loss.dos import (
+from deepmd.tf.loss.dos import (
     DOSLoss,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.loss.loss import (
     Loss,
 )
-from deepmd.nvnmd.fit.ener import (
+from deepmd.tf.nvnmd.fit.ener import (
     one_layer_nvnmd,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphWithoutTensorError,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_fitting_net_variables_from_graph_def,
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.network import one_layer as one_layer_deepmd
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import one_layer as one_layer_deepmd
+from deepmd.tf.utils.network import (
     one_layer_rand_seed_shift,
 )
+from deepmd.utils.out_stat import (
+    compute_stats_from_redu,
+)
 
 log = logging.getLogger(__name__)
 
 
 @Fitting.register("dos")
 class DOSFitting(Fitting):
     r"""Fitting the density of states (DOS) of the system.
@@ -221,16 +224,18 @@
             nsys = len(data)
             for ss in range(len(data)):
                 sys_tynatom.append(data[ss][0].astype(np.float64))
         sys_tynatom = np.array(sys_tynatom)
         sys_tynatom = np.reshape(sys_tynatom, [nsys, -1])
         sys_tynatom = sys_tynatom[:, 2:]
 
-        dos_shift, resd, rank, s_value = np.linalg.lstsq(
-            sys_tynatom, sys_dos, rcond=rcond
+        dos_shift, _ = compute_stats_from_redu(
+            sys_dos,
+            sys_tynatom,
+            rcond=rcond,
         )
 
         return dos_shift
 
     def compute_input_stats(self, all_stat: dict, protection: float = 1e-2) -> None:
         """Compute the input statistics.
```

### Comparing `deepmd_kit-2.2.9/deepmd/fit/ener.py` & `deepmd_kit-3.0.0a0/deepmd/tf/fit/ener.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,61 +1,74 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 from typing import (
+    TYPE_CHECKING,
     List,
     Optional,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     add_data_requirement,
     cast_precision,
     get_activation_func,
     get_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     global_cvt_2_tf_float,
     tf,
 )
-from deepmd.fit.fitting import (
+from deepmd.tf.fit.fitting import (
     Fitting,
 )
-from deepmd.infer import (
+from deepmd.tf.infer import (
     DeepPotential,
 )
-from deepmd.loss.ener import (
+from deepmd.tf.loss.ener import (
     EnerDipoleLoss,
     EnerSpinLoss,
     EnerStdLoss,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.loss.loss import (
     Loss,
 )
-from deepmd.nvnmd.fit.ener import (
+from deepmd.tf.nvnmd.fit.ener import (
     one_layer_nvnmd,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphWithoutTensorError,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_fitting_net_variables_from_graph_def,
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.network import one_layer as one_layer_deepmd
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import one_layer as one_layer_deepmd
+from deepmd.tf.utils.network import (
     one_layer_rand_seed_shift,
 )
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
+from deepmd.utils.finetune import (
+    change_energy_bias_lower,
+)
+from deepmd.utils.out_stat import (
+    compute_stats_from_redu,
+)
+from deepmd.utils.version import (
+    check_version_compatibility,
+)
+
+if TYPE_CHECKING:
+    pass
 
 log = logging.getLogger(__name__)
 
 
 @Fitting.register("ener")
 class EnerFitting(Fitting):
     r"""Fitting the energy of the system. The force and the virial can also be trained.
@@ -87,16 +100,18 @@
     where :math:`\mathbf{x} \in \mathbb{R}^{N_{n-1}}` is the input vector and :math:`\mathbf{y} \in \mathbb{R}`
     is the output scalar. :math:`\mathbf{w} \in \mathbb{R}^{N_{n-1}}` and
     :math:`\mathbf{b} \in \mathbb{R}` are weights and bias, respectively,
     both of which are trainable if `trainable[n]` is `True`.
 
     Parameters
     ----------
-    descrpt
-            The descrptor :math:`\mathcal{D}`
+    ntypes
+            The ntypes of the descrptor :math:`\mathcal{D}`
+    dim_descrpt
+            The dimension of the descrptor :math:`\mathcal{D}`
     neuron
             Number of neurons :math:`N` in each hidden layer of the fitting net
     resnet_dt
             Time-step `dt` in the resnet construction:
             :math:`y = x + dt * \phi (Wx + b)`
     numb_fparam
             Number of frame parameter
@@ -126,15 +141,16 @@
     use_aparam_as_mask: bool, optional
             If True, the atomic parameters will be used as a mask that determines the atom is real/virtual.
             And the aparam will not be used as the atomic parameters for embedding.
     """
 
     def __init__(
         self,
-        descrpt: tf.Tensor,
+        ntypes: int,
+        dim_descrpt: int,
         neuron: List[int] = [120, 120, 120],
         resnet_dt: bool = True,
         numb_fparam: int = 0,
         numb_aparam: int = 0,
         rcond: Optional[float] = None,
         tot_ener_zero: bool = False,
         trainable: Optional[List[bool]] = None,
@@ -146,16 +162,16 @@
         layer_name: Optional[List[Optional[str]]] = None,
         use_aparam_as_mask: bool = False,
         spin: Optional[Spin] = None,
         **kwargs,
     ) -> None:
         """Constructor."""
         # model param
-        self.ntypes = descrpt.get_ntypes()
-        self.dim_descrpt = descrpt.get_dim_out()
+        self.ntypes = ntypes
+        self.dim_descrpt = dim_descrpt
         self.use_aparam_as_mask = use_aparam_as_mask
         # args = ()\
         #        .add('numb_fparam',      int,    default = 0)\
         #        .add('numb_aparam',      int,    default = 0)\
         #        .add('neuron',           list,   default = [120,120,120], alias = 'n_neuron')\
         #        .add('resnet_dt',        bool,   default = True)\
         #        .add('rcond',            float,  default = 1e-3) \
@@ -172,50 +188,51 @@
         self.rcond = rcond
         self.seed = seed
         self.uniform_seed = uniform_seed
         self.spin = spin
         self.ntypes_spin = self.spin.get_ntypes_spin() if self.spin is not None else 0
         self.seed_shift = one_layer_rand_seed_shift()
         self.tot_ener_zero = tot_ener_zero
+        self.activation_function_name = activation_function
         self.fitting_activation_fn = get_activation_func(activation_function)
         self.fitting_precision = get_precision(precision)
         self.trainable = trainable
         if self.trainable is None:
             self.trainable = [True for ii in range(len(self.n_neuron) + 1)]
         if isinstance(self.trainable, bool):
             self.trainable = [self.trainable] * (len(self.n_neuron) + 1)
         assert (
             len(self.trainable) == len(self.n_neuron) + 1
         ), "length of trainable should be that of n_neuron + 1"
         self.atom_ener = []
         self.atom_ener_v = atom_ener
-        for at, ae in enumerate(atom_ener):
+        for at, ae in enumerate(atom_ener if atom_ener is not None else []):
             if ae is not None:
                 self.atom_ener.append(
                     tf.constant(ae, GLOBAL_TF_FLOAT_PRECISION, name="atom_%d_ener" % at)
                 )
             else:
                 self.atom_ener.append(None)
         self.useBN = False
         self.bias_atom_e = np.zeros(self.ntypes, dtype=np.float64)
         # data requirement
         if self.numb_fparam > 0:
             add_data_requirement(
                 "fparam", self.numb_fparam, atomic=False, must=True, high_prec=False
             )
-            self.fparam_avg = None
-            self.fparam_std = None
-            self.fparam_inv_std = None
+        self.fparam_avg = None
+        self.fparam_std = None
+        self.fparam_inv_std = None
         if self.numb_aparam > 0:
             add_data_requirement(
                 "aparam", self.numb_aparam, atomic=True, must=True, high_prec=False
             )
-            self.aparam_avg = None
-            self.aparam_std = None
-            self.aparam_inv_std = None
+        self.aparam_avg = None
+        self.aparam_std = None
+        self.aparam_inv_std = None
 
         self.fitting_net_variables = None
         self.mixed_prec = None
         self.layer_name = layer_name
         if self.layer_name is not None:
             assert isinstance(self.layer_name, list), "layer_name should be a list"
             assert (
@@ -280,29 +297,25 @@
         sys_tynatom = np.reshape(sys_tynatom, [nsys, -1])
         sys_tynatom = sys_tynatom[:, 2:]
         if len(self.atom_ener) > 0:
             # Atomic energies stats are incorrect if atomic energies are assigned.
             # In this situation, we directly use these assigned energies instead of computing stats.
             # This will make the loss decrease quickly
             assigned_atom_ener = np.array(
-                [ee for ee in self.atom_ener_v if ee is not None]
+                [ee if ee is not None else np.nan for ee in self.atom_ener_v]
             )
-            assigned_ener_idx = [
-                ii for ii, ee in enumerate(self.atom_ener_v) if ee is not None
-            ]
-            # np.dot out size: nframe
-            sys_ener -= np.dot(sys_tynatom[:, assigned_ener_idx], assigned_atom_ener)
-            sys_tynatom[:, assigned_ener_idx] = 0.0
-        energy_shift, resd, rank, s_value = np.linalg.lstsq(
-            sys_tynatom, sys_ener, rcond=rcond
+        else:
+            assigned_atom_ener = None
+        energy_shift, _ = compute_stats_from_redu(
+            sys_ener.reshape(-1, 1),
+            sys_tynatom,
+            assigned_bias=assigned_atom_ener,
+            rcond=rcond,
         )
-        if len(self.atom_ener) > 0:
-            for ii in assigned_ener_idx:
-                energy_shift[ii] = self.atom_ener_v[ii]
-        return energy_shift
+        return energy_shift.ravel()
 
     def compute_input_stats(self, all_stat: dict, protection: float = 1e-2) -> None:
         """Compute the input statistics.
 
         Parameters
         ----------
         all_stat
@@ -779,114 +792,26 @@
         data,
         frozen_model,
         origin_type_map,
         full_type_map,
         bias_shift="delta",
         ntest=10,
     ) -> None:
-        """Change the energy bias according to the input data and the pretrained model.
-
-        Parameters
-        ----------
-        data : DeepmdDataSystem
-            The training data.
-        frozen_model : str
-            The path file of frozen model.
-        origin_type_map : list
-            The original type_map in dataset, they are targets to change the energy bias.
-        full_type_map : str
-            The full type_map in pretrained model
-        bias_shift : str
-            The mode for changing energy bias : ['delta', 'statistic']
-            'delta' : perform predictions on energies of target dataset,
-                    and do least sqaure on the errors to obtain the target shift as bias.
-            'statistic' : directly use the statistic energy bias in the target dataset.
-        ntest : int
-            The number of test samples in a system to change the energy bias.
-        """
-        type_numbs = []
-        energy_ground_truth = []
-        energy_predict = []
-        sorter = np.argsort(full_type_map)
-        idx_type_map = sorter[
-            np.searchsorted(full_type_map, origin_type_map, sorter=sorter)
-        ]
-        mixed_type = data.mixed_type
-        numb_type = len(full_type_map)
         dp = None
         if bias_shift == "delta":
             # init model
             dp = DeepPotential(frozen_model)
-        for sys in data.data_systems:
-            test_data = sys.get_test()
-            nframes = test_data["box"].shape[0]
-            numb_test = min(nframes, ntest)
-            if mixed_type:
-                atype = test_data["type"][:numb_test].reshape([numb_test, -1])
-            else:
-                atype = test_data["type"][0]
-            assert np.array(
-                [i in idx_type_map for i in list(set(atype.reshape(-1)))]
-            ).all(), "Some types are not in 'type_map'!"
-            energy_ground_truth.append(
-                test_data["energy"][:numb_test].reshape([numb_test, 1])
-            )
-            if mixed_type:
-                type_numbs.append(
-                    np.array(
-                        [(atype == i).sum(axis=-1) for i in idx_type_map],
-                        dtype=np.int32,
-                    ).T
-                )
-            else:
-                type_numbs.append(
-                    np.tile(
-                        np.bincount(atype, minlength=numb_type)[idx_type_map],
-                        (numb_test, 1),
-                    )
-                )
-            if bias_shift == "delta":
-                coord = test_data["coord"][:numb_test].reshape([numb_test, -1])
-                if sys.pbc:
-                    box = test_data["box"][:numb_test]
-                else:
-                    box = None
-                ret = dp.eval(coord, box, atype, mixed_type=mixed_type)
-                energy_predict.append(ret[0].reshape([numb_test, 1]))
-        type_numbs = np.concatenate(type_numbs)
-        energy_ground_truth = np.concatenate(energy_ground_truth)
-        old_bias = self.bias_atom_e[idx_type_map]
-        if bias_shift == "delta":
-            energy_predict = np.concatenate(energy_predict)
-            bias_diff = energy_ground_truth - energy_predict
-            delta_bias = np.linalg.lstsq(type_numbs, bias_diff, rcond=None)[0]
-            unbias_e = energy_predict + type_numbs @ delta_bias
-            atom_numbs = type_numbs.sum(-1)
-            rmse_ae = np.sqrt(
-                np.mean(
-                    np.square(
-                        (unbias_e.ravel() - energy_ground_truth.ravel()) / atom_numbs
-                    )
-                )
-            )
-            self.bias_atom_e[idx_type_map] += delta_bias.reshape(-1)
-            log.info(
-                f"RMSE of atomic energy after linear regression is: {rmse_ae} eV/atom."
-            )
-        elif bias_shift == "statistic":
-            statistic_bias = np.linalg.lstsq(
-                type_numbs, energy_ground_truth, rcond=None
-            )[0]
-            self.bias_atom_e[idx_type_map] = statistic_bias.reshape(-1)
-        else:
-            raise RuntimeError("Unknown bias_shift mode: " + bias_shift)
-        log.info(
-            "Change energy bias of {} from {} to {}.".format(
-                str(origin_type_map), str(old_bias), str(self.bias_atom_e[idx_type_map])
-            )
+        self.bias_atom_e = change_energy_bias_lower(
+            data,
+            dp,
+            origin_type_map,
+            full_type_map,
+            self.bias_atom_e,
+            bias_shift=bias_shift,
+            ntest=ntest,
         )
 
     def enable_mixed_precision(self, mixed_prec: Optional[dict] = None) -> None:
         """Reveive the mixed precision setting.
 
         Parameters
         ----------
@@ -917,7 +842,91 @@
             return EnerStdLoss(**loss)
         elif _loss_type == "ener_dipole":
             return EnerDipoleLoss(**loss)
         elif _loss_type == "ener_spin":
             return EnerSpinLoss(**loss, use_spin=self.spin.use_spin)
         else:
             raise RuntimeError("unknown loss type")
+
+    @classmethod
+    def deserialize(cls, data: dict, suffix: str = ""):
+        """Deserialize the model.
+
+        Parameters
+        ----------
+        data : dict
+            The serialized data
+
+        Returns
+        -------
+        Model
+            The deserialized model
+        """
+        data = data.copy()
+        check_version_compatibility(data.pop("@version", 1), 1, 1)
+        fitting = cls(**data)
+        fitting.fitting_net_variables = cls.deserialize_network(
+            data["nets"],
+            suffix=suffix,
+        )
+        fitting.bias_atom_e = data["@variables"]["bias_atom_e"]
+        if fitting.numb_fparam > 0:
+            fitting.fparam_avg = data["@variables"]["fparam_avg"]
+            fitting.fparam_inv_std = data["@variables"]["fparam_inv_std"]
+        if fitting.numb_aparam > 0:
+            fitting.aparam_avg = data["@variables"]["aparam_avg"]
+            fitting.aparam_inv_std = data["@variables"]["aparam_inv_std"]
+        return fitting
+
+    def serialize(self, suffix: str = "") -> dict:
+        """Serialize the model.
+
+        Returns
+        -------
+        dict
+            The serialized data
+        """
+        data = {
+            "@class": "Fitting",
+            "type": "ener",
+            "@version": 1,
+            "var_name": "energy",
+            "ntypes": self.ntypes,
+            "dim_descrpt": self.dim_descrpt,
+            # very bad design: type embedding is not passed to the class
+            # TODO: refactor the class
+            "mixed_types": False,
+            "dim_out": 1,
+            "neuron": self.n_neuron,
+            "resnet_dt": self.resnet_dt,
+            "numb_fparam": self.numb_fparam,
+            "numb_aparam": self.numb_aparam,
+            "rcond": self.rcond,
+            "tot_ener_zero": self.tot_ener_zero,
+            "trainable": self.trainable,
+            "atom_ener": self.atom_ener_v,
+            "activation_function": self.activation_function_name,
+            "precision": self.fitting_precision.name,
+            "layer_name": self.layer_name,
+            "use_aparam_as_mask": self.use_aparam_as_mask,
+            "spin": self.spin,
+            "exclude_types": [],
+            "nets": self.serialize_network(
+                ntypes=self.ntypes,
+                # TODO: consider type embeddings
+                ndim=1,
+                in_dim=self.dim_descrpt + self.numb_fparam + self.numb_aparam,
+                neuron=self.n_neuron,
+                activation_function=self.activation_function_name,
+                resnet_dt=self.resnet_dt,
+                variables=self.fitting_net_variables,
+                suffix=suffix,
+            ),
+            "@variables": {
+                "bias_atom_e": self.bias_atom_e,
+                "fparam_avg": self.fparam_avg,
+                "fparam_inv_std": self.fparam_inv_std,
+                "aparam_avg": self.aparam_avg,
+                "aparam_inv_std": self.aparam_inv_std,
+            },
+        }
+        return data
```

### Comparing `deepmd_kit-2.2.9/deepmd/fit/fitting.py` & `deepmd_kit-3.0.0a0/deepmd/tf/lmp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,126 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
-from abc import (
-    abstractmethod,
+"""Register entry points for lammps-wheel."""
+import os
+import platform
+from importlib import (
+    import_module,
+)
+from pathlib import (
+    Path,
 )
 from typing import (
-    Callable,
+    List,
+    Optional,
+)
+
+from packaging.version import (
+    Version,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
+    SHARED_LIB_DIR,
+    TF_VERSION,
     tf,
 )
-from deepmd.loss.loss import (
-    Loss,
+
+if Version(TF_VERSION) < Version("2.12"):
+    from find_libpython import (
+        find_libpython,
+    )
+else:
+    find_libpython = None
+
+
+def get_env(paths: List[Optional[str]]) -> str:
+    """Get the environment variable from given paths."""
+    return ":".join(p for p in paths if p is not None)
+
+
+def get_library_path(module: str, filename: str) -> List[str]:
+    """Get library path from a module.
+
+    Parameters
+    ----------
+    module : str
+        The module name.
+    filename : str
+        The library filename pattern.
+
+    Returns
+    -------
+    list[str]
+        The library path.
+    """
+    try:
+        m = import_module(module)
+    except ModuleNotFoundError:
+        return []
+    else:
+        libs = sorted(Path(m.__path__[0]).glob(filename))
+        return [str(lib) for lib in libs]
+
+
+if platform.system() == "Linux":
+    lib_env = "LD_LIBRARY_PATH"
+elif platform.system() == "Darwin":
+    lib_env = "DYLD_FALLBACK_LIBRARY_PATH"
+else:
+    raise RuntimeError("Unsupported platform")
+
+if platform.system() == "Linux":
+    preload_env = "LD_PRELOAD"
+elif platform.system() == "Darwin":
+    preload_env = "DYLD_INSERT_LIBRARIES"
+else:
+    raise RuntimeError("Unsupported platform")
+
+tf_dir = tf.sysconfig.get_lib()
+op_dir = str(SHARED_LIB_DIR)
+
+
+cuda_library_paths = []
+if platform.system() == "Linux":
+    cuda_library_paths.extend(
+        [
+            *get_library_path("nvidia.cuda_runtime.lib", "libcudart.so*"),
+            *get_library_path("nvidia.cublas.lib", "libcublasLt.so*"),
+            *get_library_path("nvidia.cublas.lib", "libcublas.so*"),
+            *get_library_path("nvidia.cufft.lib", "libcufft.so*"),
+            *get_library_path("nvidia.curand.lib", "libcurand.so*"),
+            *get_library_path("nvidia.cusolver.lib", "libcusolver.so*"),
+            *get_library_path("nvidia.cusparse.lib", "libcusparse.so*"),
+            *get_library_path("nvidia.cudnn.lib", "libcudnn.so*"),
+        ]
+    )
+
+os.environ[preload_env] = get_env(
+    [
+        os.environ.get(preload_env),
+        *cuda_library_paths,
+    ]
 )
-from deepmd.utils import (
-    Plugin,
-    PluginVariant,
-)
-
-
-class Fitting(PluginVariant):
-    __plugins = Plugin()
-
-    @staticmethod
-    def register(key: str) -> Callable:
-        """Register a Fitting plugin.
-
-        Parameters
-        ----------
-        key : str
-            the key of a Fitting
-
-        Returns
-        -------
-        Fitting
-            the registered Fitting
-
-        Examples
-        --------
-        >>> @Fitting.register("some_fitting")
-            class SomeFitting(Fitting):
-                pass
-        """
-        return Fitting.__plugins.register(key)
-
-    def __new__(cls, *args, **kwargs):
-        if cls is Fitting:
-            try:
-                fitting_type = kwargs["type"]
-            except KeyError:
-                raise KeyError("the type of fitting should be set by `type`")
-            if fitting_type in Fitting.__plugins.plugins:
-                cls = Fitting.__plugins.plugins[fitting_type]
-            else:
-                raise RuntimeError("Unknown descriptor type: " + fitting_type)
-        return super().__new__(cls)
-
-    @property
-    def precision(self) -> tf.DType:
-        """Precision of fitting network."""
-        return self.fitting_precision
-
-    def init_variables(
-        self,
-        graph: tf.Graph,
-        graph_def: tf.GraphDef,
-        suffix: str = "",
-    ) -> None:
-        """Init the fitting net variables with the given dict.
-
-        Parameters
-        ----------
-        graph : tf.Graph
-            The input frozen model graph
-        graph_def : tf.GraphDef
-            The input frozen model graph_def
-        suffix : str
-            suffix to name scope
-
-        Notes
-        -----
-        This method is called by others when the fitting supported initialization from the given variables.
-        """
-        raise NotImplementedError(
-            "Fitting %s doesn't support initialization from the given variables!"
-            % type(self).__name__
-        )
-
-    @abstractmethod
-    def get_loss(self, loss: dict, lr) -> Loss:
-        """Get the loss function.
-
-        Parameters
-        ----------
-        loss : dict
-            the loss dict
-        lr : LearningRateExp
-            the learning rate
-
-        Returns
-        -------
-        Loss
-            the loss function
-        """
+
+# set LD_LIBRARY_PATH
+os.environ[lib_env] = get_env(
+    [
+        os.environ.get(lib_env),
+        tf_dir,
+        os.path.join(tf_dir, "python"),
+        op_dir,
+    ]
+)
+
+# preload python library, only for TF<2.12
+if find_libpython is not None:
+    libpython = find_libpython()
+    os.environ[preload_env] = get_env(
+        [
+            os.environ.get(preload_env),
+            libpython,
+        ]
+    )
+
+
+def get_op_dir() -> str:
+    """Get the directory of the deepmd-kit OP library."""
+    return op_dir
```

### Comparing `deepmd_kit-2.2.9/deepmd/fit/polar.py` & `deepmd_kit-3.0.0a0/deepmd/tf/fit/polar.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,51 +3,58 @@
 from typing import (
     List,
     Optional,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     cast_precision,
     get_activation_func,
     get_precision,
 )
-from deepmd.descriptor import (
+from deepmd.tf.descriptor import (
     DescrptSeA,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
-from deepmd.fit.fitting import (
+from deepmd.tf.fit.fitting import (
     Fitting,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.loss.loss import (
     Loss,
 )
-from deepmd.loss.tensor import (
+from deepmd.tf.loss.tensor import (
     TensorLoss,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_fitting_net_variables_from_graph_def,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     one_layer,
     one_layer_rand_seed_shift,
 )
+from deepmd.utils.version import (
+    check_version_compatibility,
+)
 
 
 @Fitting.register("polar")
 class PolarFittingSeA(Fitting):
     r"""Fit the atomic polarizability with descriptor se_a.
 
     Parameters
     ----------
-    descrpt : tf.Tensor
-            The descrptor
+    ntypes
+            The ntypes of the descrptor :math:`\mathcal{D}`
+    dim_descrpt
+            The dimension of the descrptor :math:`\mathcal{D}`
+    embedding_width
+            The rotation matrix dimension of the descrptor :math:`\mathcal{D}`
     neuron : List[int]
             Number of neurons in each hidden layer of the fitting net
     resnet_dt : bool
             Time-step `dt` in the resnet construction:
             y = x + dt * \phi (Wx + b)
     sel_type : List[int]
             The atom types selected to have an atomic polarizability prediction. If is None, all atoms are selected.
@@ -65,87 +72,97 @@
             The precision of the embedding net parameters. Supported options are |PRECISION|
     uniform_seed
             Only for the purpose of backward compatibility, retrieves the old behavior of using the random seed
     """
 
     def __init__(
         self,
-        descrpt: tf.Tensor,
+        ntypes: int,
+        dim_descrpt: int,
+        embedding_width: int,
         neuron: List[int] = [120, 120, 120],
         resnet_dt: bool = True,
         sel_type: Optional[List[int]] = None,
         fit_diag: bool = True,
         scale: Optional[List[float]] = None,
         shift_diag: bool = True,  # YWolfeee: will support the user to decide whether to use this function
         # diag_shift : List[float] = None, YWolfeee: will not support the user to assign a shift
         seed: Optional[int] = None,
         activation_function: str = "tanh",
         precision: str = "default",
         uniform_seed: bool = False,
         **kwargs,
     ) -> None:
         """Constructor."""
-        self.ntypes = descrpt.get_ntypes()
-        self.dim_descrpt = descrpt.get_dim_out()
+        self.ntypes = ntypes
+        self.dim_descrpt = dim_descrpt
         self.n_neuron = neuron
         self.resnet_dt = resnet_dt
         self.sel_type = sel_type
         self.fit_diag = fit_diag
         self.seed = seed
         self.uniform_seed = uniform_seed
         self.seed_shift = one_layer_rand_seed_shift()
         # self.diag_shift = diag_shift
         self.shift_diag = shift_diag
         self.scale = scale
+        self.activation_function_name = activation_function
         self.fitting_activation_fn = get_activation_func(activation_function)
         self.fitting_precision = get_precision(precision)
         if self.sel_type is None:
             self.sel_type = list(range(self.ntypes))
         self.sel_mask = np.array(
             [ii in self.sel_type for ii in range(self.ntypes)], dtype=bool
         )
         if self.scale is None:
-            self.scale = [1.0 for ii in range(self.ntypes)]
+            self.scale = np.array([1.0 for ii in range(self.ntypes)])
+        else:
+            if isinstance(self.scale, list):
+                assert (
+                    len(self.scale) == ntypes
+                ), "Scale should be a list of length ntypes."
+            elif isinstance(self.scale, float):
+                self.scale = [self.scale for _ in range(ntypes)]
+            else:
+                raise ValueError(
+                    "Scale must be a list of float of length ntypes or a float."
+                )
+            self.scale = np.array(self.scale)
         # if self.diag_shift is None:
         #    self.diag_shift = [0.0 for ii in range(self.ntypes)]
         if not isinstance(self.sel_type, list):
             self.sel_type = [self.sel_type]
         self.sel_type = sorted(self.sel_type)
         self.constant_matrix = np.zeros(
             self.ntypes
         )  # self.ntypes x 1, store the average diagonal value
         # if type(self.diag_shift) is not list:
         #    self.diag_shift = [self.diag_shift]
-        if not isinstance(self.scale, list):
-            self.scale = [self.scale for ii in range(self.ntypes)]
-        self.scale = np.array(self.scale)
-        self.dim_rot_mat_1 = descrpt.get_dim_rot_mat_1()
+        self.dim_rot_mat_1 = embedding_width
         self.dim_rot_mat = self.dim_rot_mat_1 * 3
         self.useBN = False
         self.fitting_net_variables = None
         self.mixed_prec = None
 
     def get_sel_type(self) -> List[int]:
         """Get selected atom types."""
         return self.sel_type
 
     def get_out_size(self) -> int:
         """Get the output size. Should be 9."""
         return 9
 
-    def compute_input_stats(self, all_stat, protection=1e-2):
-        """Compute the input statistics.
+    def compute_output_stats(self, all_stat):
+        """Compute the output statistics.
 
         Parameters
         ----------
         all_stat
             Dictionary of inputs.
             can be prepared by model.make_stat_input
-        protection
-            Divided-by-zero protection
         """
         if "polarizability" not in all_stat.keys():
             self.avgeig = np.zeros([9])
             warnings.warn(
                 "no polarizability data, cannot do data stat. use zeros as guess"
             )
             return
@@ -505,14 +522,80 @@
             loss,
             model=self,
             tensor_name="polar",
             tensor_size=9,
             label_name="polarizability",
         )
 
+    def serialize(self, suffix: str) -> dict:
+        """Serialize the model.
+
+        Returns
+        -------
+        dict
+            The serialized data
+        """
+        data = {
+            "@class": "Fitting",
+            "type": "polar",
+            "@version": 1,
+            "var_name": "polar",
+            "ntypes": self.ntypes,
+            "dim_descrpt": self.dim_descrpt,
+            "embedding_width": self.dim_rot_mat_1,
+            # very bad design: type embedding is not passed to the class
+            # TODO: refactor the class
+            "mixed_types": False,
+            "dim_out": 3,
+            "neuron": self.n_neuron,
+            "resnet_dt": self.resnet_dt,
+            "activation_function": self.activation_function_name,
+            "precision": self.fitting_precision.name,
+            "exclude_types": [],
+            "fit_diag": self.fit_diag,
+            "scale": list(self.scale),
+            "shift_diag": self.shift_diag,
+            "nets": self.serialize_network(
+                ntypes=self.ntypes,
+                # TODO: consider type embeddings
+                ndim=1,
+                in_dim=self.dim_descrpt,
+                out_dim=self.dim_rot_mat_1,
+                neuron=self.n_neuron,
+                activation_function=self.activation_function_name,
+                resnet_dt=self.resnet_dt,
+                variables=self.fitting_net_variables,
+                suffix=suffix,
+            ),
+        }
+        return data
+
+    @classmethod
+    def deserialize(cls, data: dict, suffix: str):
+        """Deserialize the model.
+
+        Parameters
+        ----------
+        data : dict
+            The serialized data
+
+        Returns
+        -------
+        Model
+            The deserialized model
+        """
+        data = data.copy()
+        check_version_compatibility(data.pop("@version", 1), 1, 1)
+        fitting = cls(**data)
+        fitting.fitting_net_variables = cls.deserialize_network(
+            data["nets"],
+            suffix=suffix,
+        )
+        return fitting
+
 
 class GlobalPolarFittingSeA:
     r"""Fit the system polarizability with descriptor se_a.
 
     Parameters
     ----------
     descrpt : tf.Tensor
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/data_modifier.py` & `deepmd_kit-3.0.0a0/deepmd/tf/infer/data_modifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,34 +3,32 @@
 from typing import (
     List,
     Tuple,
 )
 
 import numpy as np
 
-import deepmd.op  # noqa: F401
-from deepmd.common import (
+import deepmd.tf.op  # noqa: F401
+from deepmd.tf.common import (
     make_default_mesh,
     select_idx_map,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     op_module,
     tf,
 )
-from deepmd.infer.deep_dipole import (
-    DeepDipole,
-)
-from deepmd.infer.ewald_recp import (
+from deepmd.tf.infer.deep_dipole import DeepDipoleOld as DeepDipole
+from deepmd.tf.infer.ewald_recp import (
     EwaldRecp,
 )
-from deepmd.utils.data import (
+from deepmd.tf.utils.data import (
     DeepmdData,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 
 class DipoleChargeModifier(DeepDipole):
     """Parameters
     ----------
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/deep_dipole.py` & `deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_dipole.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
+from pathlib import (
+    Path,
+)
 from typing import (
-    TYPE_CHECKING,
     Optional,
 )
 
-from deepmd.infer.deep_tensor import (
+from deepmd.infer.deep_dipole import (
+    DeepDipole,
+)
+from deepmd.tf.infer.deep_tensor import (
     DeepTensor,
 )
 
-if TYPE_CHECKING:
-    from pathlib import (
-        Path,
-    )
+__all__ = [
+    "DeepDipole",
+]
 
 
-class DeepDipole(DeepTensor):
+class DeepDipoleOld(DeepTensor):
+    # used for DipoleChargeModifier only
     """Constructor.
 
     Parameters
     ----------
     model_file : Path
         The name of the frozen model file.
     load_prefix: str
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/deep_dos.py` & `deepmd_kit-3.0.0a0/deepmd/tf/infer/deep_tensor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,506 +1,444 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
-import logging
 from typing import (
     TYPE_CHECKING,
-    Callable,
+    ClassVar,
+    Dict,
     List,
     Optional,
     Tuple,
-    Union,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     make_default_mesh,
 )
-from deepmd.infer.deep_eval import (
-    DeepEval,
-)
-from deepmd.utils.batch_size import (
-    AutoBatchSize,
-)
-from deepmd.utils.sess import (
+from deepmd.tf.infer.deep_eval import DeepEvalOld as DeepEval
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 if TYPE_CHECKING:
     from pathlib import (
         Path,
     )
 
-log = logging.getLogger(__name__)
 
-
-class DeepDOS(DeepEval):
-    """Constructor.
+class DeepTensor(DeepEval):
+    """Evaluates a tensor model.
 
     Parameters
     ----------
-    model_file : Path
+    model_file: str
         The name of the frozen model file.
     load_prefix: str
         The prefix in the load computational graph
     default_tf_graph : bool
         If uses the default tf graph, otherwise build a new tf graph for evaluation
-    auto_batch_size : bool or int or AutomaticBatchSize, default: True
-        If True, automatic batch size will be used. If int, it will be used
-        as the initial batch size.
     input_map : dict, optional
         The input map for tf.import_graph_def. Only work with default tf graph
-
-    Warnings
-    --------
-    For developers: `DeepTensor` initializer must be called at the end after
-    `self.tensors` are modified because it uses the data in `self.tensors` dict.
-    Do not chanage the order!
+    neighbor_list : ase.neighborlist.NeighborList, optional
+        The neighbor list object. If None, then build the native neighbor list.
     """
 
+    tensors: ClassVar[Dict[str, str]] = {
+        # descriptor attrs
+        "t_ntypes": "descrpt_attr/ntypes:0",
+        "t_rcut": "descrpt_attr/rcut:0",
+        # model attrs
+        "t_tmap": "model_attr/tmap:0",
+        "t_sel_type": "model_attr/sel_type:0",
+        "t_ouput_dim": "model_attr/output_dim:0",
+        # inputs
+        "t_coord": "t_coord:0",
+        "t_type": "t_type:0",
+        "t_natoms": "t_natoms:0",
+        "t_box": "t_box:0",
+        "t_mesh": "t_mesh:0",
+    }
+
     def __init__(
         self,
         model_file: "Path",
         load_prefix: str = "load",
         default_tf_graph: bool = False,
-        auto_batch_size: Union[bool, int, AutoBatchSize] = True,
         input_map: Optional[dict] = None,
+        neighbor_list=None,
     ) -> None:
-        # add these tensors on top of what is defined by DeepTensor Class
-        # use this in favor of dict update to move attribute from class to
-        # instance namespace
-        self.tensors = {
-            # descrpt attrs
-            "t_ntypes": "descrpt_attr/ntypes:0",
-            "t_rcut": "descrpt_attr/rcut:0",
-            # fitting attrs
-            "t_dfparam": "fitting_attr/dfparam:0",
-            "t_daparam": "fitting_attr/daparam:0",
-            "t_numb_dos": "fitting_attr/numb_dos:0",
-            # model attrs
-            "t_tmap": "model_attr/tmap:0",
-            # inputs
-            "t_coord": "t_coord:0",
-            "t_type": "t_type:0",
-            "t_natoms": "t_natoms:0",
-            "t_box": "t_box:0",
-            "t_mesh": "t_mesh:0",
-            # add output tensors
-            "t_dos": "o_dos:0",
-            "t_atom_dos": "o_atom_dos:0",
-            "t_descriptor": "o_descriptor:0",
-        }
+        """Constructor."""
         DeepEval.__init__(
             self,
             model_file,
             load_prefix=load_prefix,
             default_tf_graph=default_tf_graph,
-            auto_batch_size=auto_batch_size,
             input_map=input_map,
+            neighbor_list=neighbor_list,
         )
-
-        # load optional tensors
-        operations = [op.name for op in self.graph.get_operations()]
-        # check if the graph has these operations:
-        # if yes add them
-        if "load/t_fparam" in operations:
-            self.tensors.update({"t_fparam": "t_fparam:0"})
-            self.has_fparam = True
-        else:
-            log.debug("Could not get tensor 't_fparam:0'")
-            self.t_fparam = None
-            self.has_fparam = False
-
-        if "load/t_aparam" in operations:
-            self.tensors.update({"t_aparam": "t_aparam:0"})
-            self.has_aparam = True
-        else:
-            log.debug("Could not get tensor 't_aparam:0'")
-            self.t_aparam = None
-            self.has_aparam = False
+        # check model type
+        model_type = self.tensors["t_tensor"][2:-2]
+        assert (
+            self.model_type == model_type
+        ), f"expect {model_type} model but got {self.model_type}"
 
         # now load tensors to object attributes
         for attr_name, tensor_name in self.tensors.items():
-            try:
+            self._get_tensor(tensor_name, attr_name)
+
+        # load optional tensors if possible
+        optional_tensors = {
+            "t_global_tensor": f"o_global_{model_type}:0",
+            "t_force": "o_force:0",
+            "t_virial": "o_virial:0",
+            "t_atom_virial": "o_atom_virial:0",
+        }
+        try:
+            # first make sure these tensor all exists (but do not modify self attr)
+            for attr_name, tensor_name in optional_tensors.items():
+                self._get_tensor(tensor_name)
+            # then put those into self.attrs
+            for attr_name, tensor_name in optional_tensors.items():
                 self._get_tensor(tensor_name, attr_name)
-            except KeyError:
-                if attr_name != "t_descriptor":
-                    raise
+        except KeyError:
+            self._support_gfv = False
+        else:
+            self.tensors.update(optional_tensors)
+            self._support_gfv = True
 
         self._run_default_sess()
         self.tmap = self.tmap.decode("UTF-8").split()
 
-        # setup modifier
-        try:
-            t_modifier_type = self._get_tensor("modifier_attr/type:0")
-            self.modifier_type = run_sess(self.sess, t_modifier_type).decode("UTF-8")
-        except (ValueError, KeyError):
-            self.modifier_type = None
-
     def _run_default_sess(self):
-        [
-            self.ntypes,
-            self.rcut,
-            self.numb_dos,
-            self.dfparam,
-            self.daparam,
-            self.tmap,
-        ] = run_sess(
+        [self.ntypes, self.rcut, self.tmap, self.tselt, self.output_dim] = run_sess(
             self.sess,
             [
                 self.t_ntypes,
                 self.t_rcut,
-                self.t_numb_dos,
-                self.t_dfparam,
-                self.t_daparam,
                 self.t_tmap,
+                self.t_sel_type,
+                self.t_ouput_dim,
             ],
         )
 
     def get_ntypes(self) -> int:
         """Get the number of atom types of this model."""
         return self.ntypes
 
     def get_rcut(self) -> float:
         """Get the cut-off radius of this model."""
         return self.rcut
 
-    def get_numb_dos(self) -> int:
-        """Get the length of DOS output of this DP model."""
-        return self.numb_dos
-
     def get_type_map(self) -> List[str]:
         """Get the type map (element name of the atom types) of this model."""
         return self.tmap
 
     def get_sel_type(self) -> List[int]:
-        """Unsupported in this model."""
-        raise NotImplementedError("This model type does not support this attribute")
+        """Get the selected atom types of this model."""
+        return self.tselt
 
     def get_dim_fparam(self) -> int:
         """Get the number (dimension) of frame parameters of this DP."""
         return self.dfparam
 
     def get_dim_aparam(self) -> int:
         """Get the number (dimension) of atomic parameters of this DP."""
         return self.daparam
 
-    def _eval_func(self, inner_func: Callable, numb_test: int, natoms: int) -> Callable:
-        """Wrapper method with auto batch size.
-
-        Parameters
-        ----------
-        inner_func : Callable
-            the method to be wrapped
-        numb_test : int
-            number of tests
-        natoms : int
-            number of atoms
-
-        Returns
-        -------
-        Callable
-            the wrapper
-        """
-        if self.auto_batch_size is not None:
-
-            def eval_func(*args, **kwargs):
-                return self.auto_batch_size.execute_all(
-                    inner_func, numb_test, natoms, *args, **kwargs
-                )
-
-        else:
-            eval_func = inner_func
-        return eval_func
-
-    def _get_natoms_and_nframes(
-        self,
-        coords: np.ndarray,
-        atom_types: Union[List[int], np.ndarray],
-        mixed_type: bool = False,
-    ) -> Tuple[int, int]:
-        if mixed_type:
-            natoms = len(atom_types[0])
-        else:
-            natoms = len(atom_types)
-        coords = np.reshape(np.array(coords), [-1, natoms * 3])
-        nframes = coords.shape[0]
-        return natoms, nframes
-
     def eval(
         self,
         coords: np.ndarray,
         cells: np.ndarray,
         atom_types: List[int],
-        atomic: bool = False,
+        atomic: bool = True,
         fparam: Optional[np.ndarray] = None,
         aparam: Optional[np.ndarray] = None,
+        efield: Optional[np.ndarray] = None,
         mixed_type: bool = False,
-    ) -> Tuple[np.ndarray, ...]:
-        """Evaluate the dos, atom_dos by using this model.
+    ) -> np.ndarray:
+        """Evaluate the model.
 
         Parameters
         ----------
         coords
             The coordinates of atoms.
             The array should be of size nframes x natoms x 3
         cells
             The cell of the region.
             If None then non-PBC is assumed, otherwise using PBC.
             The array should be of size nframes x 9
         atom_types
             The atom types
             The list should contain natoms ints
         atomic
-            Calculate the atomic energy and virial
+            If True (default), return the atomic tensor
+            Otherwise return the global tensor
         fparam
-            The frame parameter.
-            The array can be of size :
-            - nframes x dim_fparam.
-            - dim_fparam. Then all frames are assumed to be provided with the same fparam.
+            Not used in this model
         aparam
-            The atomic parameter
-            The array can be of size :
-            - nframes x natoms x dim_aparam.
-            - natoms x dim_aparam. Then all frames are assumed to be provided with the same aparam.
-            - dim_aparam. Then all frames and atoms are provided with the same aparam.
+            Not used in this model
+        efield
+            Not used in this model
         mixed_type
             Whether to perform the mixed_type mode.
             If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
             in which frames in a system may have different natoms_vec(s), with the same nloc.
 
         Returns
         -------
-        dos
-            The electron density of state.
-        atom_dos
-            The atom-sited density of state. Only returned when atomic == True
+        tensor
+            The returned tensor
+            If atomic == False then of size nframes x output_dim
+            else of size nframes x natoms x output_dim
         """
-        # reshape coords before getting shape
-        natoms, numb_test = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        output = self._eval_func(self._eval_inner, numb_test, natoms)(
-            coords,
-            cells,
-            atom_types,
-            fparam=fparam,
-            aparam=aparam,
-            atomic=atomic,
-            mixed_type=mixed_type,
-        )
-
-        return output
-
-    def _prepare_feed_dict(
-        self,
-        coords,
-        cells,
-        atom_types,
-        fparam=None,
-        aparam=None,
-        atomic=False,
-        mixed_type=False,
-    ):
         # standarize the shape of inputs
-        natoms, nframes = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
         if mixed_type:
+            natoms = atom_types[0].size
             atom_types = np.array(atom_types, dtype=int).reshape([-1, natoms])
         else:
             atom_types = np.array(atom_types, dtype=int).reshape([-1])
+            natoms = atom_types.size
         coords = np.reshape(np.array(coords), [-1, natoms * 3])
+        nframes = coords.shape[0]
         if cells is None:
             pbc = False
-            # make cells to work around the requirement of pbc
             cells = np.tile(np.eye(3), [nframes, 1]).reshape([nframes, 9])
         else:
             pbc = True
             cells = np.array(cells).reshape([nframes, 9])
 
-        if self.has_fparam:
-            assert fparam is not None
-            fparam = np.array(fparam)
-        if self.has_aparam:
-            assert aparam is not None
-            aparam = np.array(aparam)
-
-        # reshape the inputs
-        if self.has_fparam:
-            fdim = self.get_dim_fparam()
-            if fparam.size == nframes * fdim:
-                fparam = np.reshape(fparam, [nframes, fdim])
-            elif fparam.size == fdim:
-                fparam = np.tile(fparam.reshape([-1]), [nframes, 1])
-            else:
-                raise RuntimeError(
-                    "got wrong size of frame param, should be either %d x %d or %d"
-                    % (nframes, fdim, fdim)
-                )
-        if self.has_aparam:
-            fdim = self.get_dim_aparam()
-            if aparam.size == nframes * natoms * fdim:
-                aparam = np.reshape(aparam, [nframes, natoms * fdim])
-            elif aparam.size == natoms * fdim:
-                aparam = np.tile(aparam.reshape([-1]), [nframes, 1])
-            elif aparam.size == fdim:
-                aparam = np.tile(aparam.reshape([-1]), [nframes, natoms])
-            else:
-                raise RuntimeError(
-                    "got wrong size of frame param, should be either %d x %d x %d or %d x %d or %d"
-                    % (nframes, natoms, fdim, natoms, fdim, fdim)
-                )
-
         # sort inputs
-        coords, atom_types, imap = self.sort_input(
-            coords, atom_types, mixed_type=mixed_type
+        coords, atom_types, imap, sel_at, sel_imap = self.sort_input(
+            coords, atom_types, sel_atoms=self.get_sel_type(), mixed_type=mixed_type
         )
 
         # make natoms_vec and default_mesh
-        natoms_vec = self.make_natoms_vec(atom_types, mixed_type=mixed_type)
-        assert natoms_vec[0] == natoms
+        if self.neighbor_list is None:
+            natoms_vec = self.make_natoms_vec(atom_types, mixed_type=mixed_type)
+            assert natoms_vec[0] == natoms
+            mesh = make_default_mesh(pbc, mixed_type)
+        else:
+            if nframes > 1:
+                raise NotImplementedError(
+                    "neighbor_list does not support multiple frames"
+                )
+            (
+                natoms_vec,
+                coords,
+                atom_types,
+                mesh,
+                imap,
+                _,
+            ) = self.build_neighbor_list(
+                coords,
+                cells if cells is not None else None,
+                atom_types,
+                imap,
+                self.neighbor_list,
+            )
 
         # evaluate
         feed_dict_test = {}
         feed_dict_test[self.t_natoms] = natoms_vec
         if mixed_type:
             feed_dict_test[self.t_type] = atom_types.reshape([-1])
         else:
             feed_dict_test[self.t_type] = np.tile(atom_types, [nframes, 1]).reshape(
                 [-1]
             )
         feed_dict_test[self.t_coord] = np.reshape(coords, [-1])
+        feed_dict_test[self.t_box] = np.reshape(cells, [-1])
+        feed_dict_test[self.t_mesh] = mesh
 
-        if len(self.t_box.shape) == 1:
-            feed_dict_test[self.t_box] = np.reshape(cells, [-1])
-        elif len(self.t_box.shape) == 2:
-            feed_dict_test[self.t_box] = cells
-        else:
-            raise RuntimeError
-        feed_dict_test[self.t_mesh] = make_default_mesh(pbc, mixed_type)
-        if self.has_fparam:
-            feed_dict_test[self.t_fparam] = np.reshape(fparam, [-1])
-        if self.has_aparam:
-            feed_dict_test[self.t_aparam] = np.reshape(aparam, [-1])
-        return feed_dict_test, imap
-
-    def _eval_inner(
-        self,
-        coords,
-        cells,
-        atom_types,
-        fparam=None,
-        aparam=None,
-        atomic=False,
-        mixed_type=False,
-    ):
-        natoms, nframes = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        feed_dict_test, imap = self._prepare_feed_dict(
-            coords, cells, atom_types, fparam, aparam, mixed_type=mixed_type
-        )
-        t_out = [self.t_dos]
         if atomic:
-            t_out += [self.t_atom_dos]
-
-        v_out = run_sess(self.sess, t_out, feed_dict=feed_dict_test)
-        dos = v_out[0]
-        if atomic:
-            atom_dos = v_out[1]
+            assert (
+                "global" not in self.model_type
+            ), f"cannot do atomic evaluation with model type {self.model_type}"
+            t_out = [self.t_tensor]
+        else:
+            assert (
+                self._support_gfv or "global" in self.model_type
+            ), f"do not support global tensor evaluation with old {self.model_type} model"
+            t_out = [self.t_global_tensor if self._support_gfv else self.t_tensor]
+        v_out = self.sess.run(t_out, feed_dict=feed_dict_test)
+        tensor = v_out[0]
 
         # reverse map of the outputs
         if atomic:
-            atom_dos = self.reverse_map(
-                np.reshape(atom_dos, [nframes, -1, self.numb_dos]), imap
+            tensor = np.array(tensor)
+            tensor = self.reverse_map(
+                np.reshape(tensor, [nframes, -1, self.output_dim]), sel_imap
             )
-            dos = np.sum(atom_dos, axis=1)
-
-        dos = np.reshape(dos, [nframes, self.numb_dos])
-        if atomic:
-            atom_dos = np.reshape(atom_dos, [nframes, natoms, self.numb_dos])
-            return dos, atom_dos
+            tensor = np.reshape(tensor, [nframes, len(sel_at), self.output_dim])
         else:
-            return dos
+            tensor = np.reshape(tensor, [nframes, self.output_dim])
+
+        return tensor
 
-    def eval_descriptor(
+    def eval_full(
         self,
         coords: np.ndarray,
         cells: np.ndarray,
         atom_types: List[int],
-        fparam: Optional[np.ndarray] = None,
-        aparam: Optional[np.ndarray] = None,
-        efield: Optional[np.ndarray] = None,
+        atomic: bool = False,
+        fparam: Optional[np.array] = None,
+        aparam: Optional[np.array] = None,
+        efield: Optional[np.array] = None,
         mixed_type: bool = False,
-    ) -> np.array:
-        """Evaluate descriptors by using this DP.
+    ) -> Tuple[np.ndarray, ...]:
+        """Evaluate the model with interface similar to the energy model.
+        Will return global tensor, component-wise force and virial
+        and optionally atomic tensor and atomic virial.
 
         Parameters
         ----------
         coords
             The coordinates of atoms.
             The array should be of size nframes x natoms x 3
         cells
             The cell of the region.
             If None then non-PBC is assumed, otherwise using PBC.
             The array should be of size nframes x 9
         atom_types
             The atom types
             The list should contain natoms ints
+        atomic
+            Whether to calculate atomic tensor and virial
         fparam
-            The frame parameter.
-            The array can be of size :
-            - nframes x dim_fparam.
-            - dim_fparam. Then all frames are assumed to be provided with the same fparam.
+            Not used in this model
         aparam
-            The atomic parameter
-            The array can be of size :
-            - nframes x natoms x dim_aparam.
-            - natoms x dim_aparam. Then all frames are assumed to be provided with the same aparam.
-            - dim_aparam. Then all frames and atoms are provided with the same aparam.
+            Not used in this model
         efield
-            The external field on atoms.
-            The array should be of size nframes x natoms x 3
+            Not used in this model
         mixed_type
             Whether to perform the mixed_type mode.
             If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
             in which frames in a system may have different natoms_vec(s), with the same nloc.
 
         Returns
         -------
-        descriptor
-            Descriptors.
+        tensor
+            The global tensor.
+            shape: [nframes x nout]
+        force
+            The component-wise force (negative derivative) on each atom.
+            shape: [nframes x nout x natoms x 3]
+        virial
+            The component-wise virial of the tensor.
+            shape: [nframes x nout x 9]
+        atom_tensor
+            The atomic tensor. Only returned when atomic == True
+            shape: [nframes x natoms x nout]
+        atom_virial
+            The atomic virial. Only returned when atomic == True
+            shape: [nframes x nout x natoms x 9]
         """
-        natoms, numb_test = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        descriptor = self._eval_func(self._eval_descriptor_inner, numb_test, natoms)(
-            coords,
-            cells,
-            atom_types,
-            fparam=fparam,
-            aparam=aparam,
-            efield=efield,
-            mixed_type=mixed_type,
-        )
-        return descriptor
+        assert self._support_gfv, "do not support eval_full with old tensor model"
 
-    def _eval_descriptor_inner(
-        self,
-        coords: np.ndarray,
-        cells: np.ndarray,
-        atom_types: List[int],
-        fparam: Optional[np.ndarray] = None,
-        aparam: Optional[np.ndarray] = None,
-        efield: Optional[np.ndarray] = None,
-        mixed_type: bool = False,
-    ) -> np.array:
-        natoms, nframes = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        feed_dict_test, imap = self._prepare_feed_dict(
-            coords, cells, atom_types, fparam, aparam, efield, mixed_type=mixed_type
-        )
-        (descriptor,) = run_sess(
-            self.sess, [self.t_descriptor], feed_dict=feed_dict_test
+        # standarize the shape of inputs
+        if mixed_type:
+            natoms = atom_types[0].size
+            atom_types = np.array(atom_types, dtype=int).reshape([-1, natoms])
+        else:
+            atom_types = np.array(atom_types, dtype=int).reshape([-1])
+            natoms = atom_types.size
+        coords = np.reshape(np.array(coords), [-1, natoms * 3])
+        nframes = coords.shape[0]
+        if cells is None:
+            pbc = False
+            cells = np.tile(np.eye(3), [nframes, 1]).reshape([nframes, 9])
+        else:
+            pbc = True
+            cells = np.array(cells).reshape([nframes, 9])
+        nout = self.output_dim
+
+        # sort inputs
+        coords, atom_types, imap, sel_at, sel_imap = self.sort_input(
+            coords, atom_types, sel_atoms=self.get_sel_type(), mixed_type=mixed_type
         )
-        return self.reverse_map(np.reshape(descriptor, [nframes, natoms, -1]), imap)
+
+        # make natoms_vec and default_mesh
+        if self.neighbor_list is None:
+            natoms_vec = self.make_natoms_vec(atom_types, mixed_type=mixed_type)
+            assert natoms_vec[0] == natoms
+            mesh = make_default_mesh(pbc, mixed_type)
+            ghost_map = None
+        else:
+            if nframes > 1:
+                raise NotImplementedError(
+                    "neighbor_list does not support multiple frames"
+                )
+            (
+                natoms_vec,
+                coords,
+                atom_types,
+                mesh,
+                imap,
+                ghost_map,
+            ) = self.build_neighbor_list(
+                coords,
+                cells if cells is not None else None,
+                atom_types,
+                imap,
+                self.neighbor_list,
+            )
+
+        # evaluate
+        feed_dict_test = {}
+        feed_dict_test[self.t_natoms] = natoms_vec
+        if mixed_type:
+            feed_dict_test[self.t_type] = atom_types.reshape([-1])
+        else:
+            feed_dict_test[self.t_type] = np.tile(atom_types, [nframes, 1]).reshape(
+                [-1]
+            )
+        feed_dict_test[self.t_coord] = np.reshape(coords, [-1])
+        feed_dict_test[self.t_box] = np.reshape(cells, [-1])
+        feed_dict_test[self.t_mesh] = mesh
+
+        t_out = [self.t_global_tensor, self.t_force, self.t_virial]
+        if atomic:
+            t_out += [self.t_tensor, self.t_atom_virial]
+
+        v_out = self.sess.run(t_out, feed_dict=feed_dict_test)
+        gt = v_out[0]  # global tensor
+        force = v_out[1]
+        virial = v_out[2]
+        if atomic:
+            at = v_out[3]  # atom tensor
+            av = v_out[4]  # atom virial
+
+        nloc = natoms_vec[0]
+        nall = natoms_vec[1]
+
+        if ghost_map is not None:
+            # add the value of ghost atoms to real atoms
+            force = np.reshape(force, [nframes * nout, -1, 3])
+            # TODO: is there some way not to use for loop?
+            for ii in range(nframes * nout):
+                np.add.at(force[ii], ghost_map, force[ii, nloc:])
+            if atomic:
+                av = np.reshape(av, [nframes * nout, -1, 9])
+                for ii in range(nframes * nout):
+                    np.add.at(av[ii], ghost_map, av[ii, nloc:])
+
+        # please note here the shape are wrong!
+        force = self.reverse_map(np.reshape(force, [nframes * nout, nall, 3]), imap)
+        if atomic:
+            at = self.reverse_map(
+                np.reshape(at, [nframes, len(sel_at), nout]), sel_imap
+            )
+            av = self.reverse_map(np.reshape(av, [nframes * nout, nall, 9]), imap)
+
+        # make sure the shapes are correct here
+        gt = np.reshape(gt, [nframes, nout])
+        force = np.reshape(force, [nframes, nout, nall, 3])
+        if nloc < nall:
+            force = force[:, :, :nloc, :]
+        virial = np.reshape(virial, [nframes, nout, 9])
+        if atomic:
+            at = np.reshape(at, [nframes, len(sel_at), self.output_dim])
+            av = np.reshape(av, [nframes, nout, nall, 9])
+            if nloc < nall:
+                av = av[:, :, :nloc, :]
+            return gt, force, virial, at, av
+        else:
+            return gt, force, virial
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/deep_eval.py` & `deepmd_kit-3.0.0a0/deepmd/pt/model/atomic_model/pairtab_atomic_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,457 +1,397 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
-from functools import (
-    lru_cache,
-)
+import copy
 from typing import (
-    TYPE_CHECKING,
+    Dict,
     List,
     Optional,
     Union,
 )
 
-import numpy as np
+import torch
 
-from deepmd.env import (
-    MODEL_VERSION,
-    default_tf_session_config,
-    tf,
+from deepmd.dpmodel import (
+    FittingOutputDef,
+    OutputVariableDef,
+)
+from deepmd.utils.pair_tab import (
+    PairTab,
 )
-from deepmd.utils.batch_size import (
-    AutoBatchSize,
+from deepmd.utils.version import (
+    check_version_compatibility,
 )
-from deepmd.utils.sess import (
-    run_sess,
+
+from .base_atomic_model import (
+    BaseAtomicModel,
 )
 
-if TYPE_CHECKING:
-    from pathlib import (
-        Path,
-    )
 
+class PairTabAtomicModel(torch.nn.Module, BaseAtomicModel):
+    """Pairwise tabulation energy model.
+
+    This model can be used to tabulate the pairwise energy between atoms for either
+    short-range or long-range interactions, such as D3, LJ, ZBL, etc. It should not
+    be used alone, but rather as one submodel of a linear (sum) model, such as
+    DP+D3.
+
+    Do not put the model on the first model of a linear model, since the linear
+    model fetches the type map from the first model.
 
-class DeepEval:
-    """Common methods for DeepPot, DeepWFC, DeepPolar, ...
+    At this moment, the model does not smooth the energy at the cutoff radius, so
+    one needs to make sure the energy has been smoothed to zero.
 
     Parameters
     ----------
-    model_file : Path
-        The name of the frozen model file.
-    load_prefix: str
-        The prefix in the load computational graph
-    default_tf_graph : bool
-        If uses the default tf graph, otherwise build a new tf graph for evaluation
-    auto_batch_size : bool or int or AutomaticBatchSize, default: False
-        If True, automatic batch size will be used. If int, it will be used
-        as the initial batch size.
-    input_map : dict, optional
-        The input map for tf.import_graph_def. Only work with default tf graph
-    neighbor_list : ase.neighborlist.NewPrimitiveNeighborList, optional
-        The ASE neighbor list class to produce the neighbor list. If None, the
-        neighbor list will be built natively in the model.
+    tab_file : str
+        The path to the tabulation file.
+    rcut : float
+        The cutoff radius.
+    sel : int or list[int]
+        The maxmum number of atoms in the cut-off radius.
     """
 
-    load_prefix: str  # set by subclass
-
     def __init__(
-        self,
-        model_file: "Path",
-        load_prefix: str = "load",
-        default_tf_graph: bool = False,
-        auto_batch_size: Union[bool, int, AutoBatchSize] = False,
-        input_map: Optional[dict] = None,
-        neighbor_list=None,
+        self, tab_file: str, rcut: float, sel: Union[int, List[int]], **kwargs
     ):
-        self.graph = self._load_graph(
-            model_file,
-            prefix=load_prefix,
-            default_tf_graph=default_tf_graph,
-            input_map=input_map,
-        )
-        self.load_prefix = load_prefix
+        torch.nn.Module.__init__(self)
+        self.model_def_script = ""
+        self.tab_file = tab_file
+        self.rcut = rcut
+        self.tab = self._set_pairtab(tab_file, rcut)
+        BaseAtomicModel.__init__(self, **kwargs)
+
+        # handle deserialization with no input file
+        if self.tab_file is not None:
+            (
+                tab_info,
+                tab_data,
+            ) = self.tab.get()  # this returns -> Tuple[np.array, np.array]
+            self.register_buffer("tab_info", torch.from_numpy(tab_info))
+            self.register_buffer("tab_data", torch.from_numpy(tab_data))
+        else:
+            self.register_buffer("tab_info", None)
+            self.register_buffer("tab_data", None)
 
-        # graph_compatable should be called after graph and prefix are set
-        if not self._graph_compatable():
-            raise RuntimeError(
-                f"model in graph (version {self.model_version}) is incompatible"
-                f"with the model (version {MODEL_VERSION}) supported by the current code."
-                "See https://deepmd.rtfd.io/compatability/ for details."
-            )
-
-        # set default to False, as subclasses may not support
-        if isinstance(auto_batch_size, bool):
-            if auto_batch_size:
-                self.auto_batch_size = AutoBatchSize()
-            else:
-                self.auto_batch_size = None
-        elif isinstance(auto_batch_size, int):
-            self.auto_batch_size = AutoBatchSize(auto_batch_size)
-        elif isinstance(auto_batch_size, AutoBatchSize):
-            self.auto_batch_size = auto_batch_size
+        # self.model_type = "ener"
+        # self.model_version = MODEL_VERSION ## this shoud be in the parent class
+
+        if isinstance(sel, int):
+            self.sel = sel
+        elif isinstance(sel, list):
+            self.sel = sum(sel)
         else:
-            raise TypeError("auto_batch_size should be bool, int, or AutoBatchSize")
+            raise TypeError("sel must be int or list[int]")
 
-        self.neighbor_list = neighbor_list
+    @torch.jit.ignore
+    def _set_pairtab(self, tab_file: str, rcut: float) -> PairTab:
+        return PairTab(tab_file, rcut)
+
+    def fitting_output_def(self) -> FittingOutputDef:
+        return FittingOutputDef(
+            [
+                OutputVariableDef(
+                    name="energy",
+                    shape=[1],
+                    reduciable=True,
+                    r_differentiable=True,
+                    c_differentiable=True,
+                )
+            ]
+        )
 
-    @property
-    @lru_cache(maxsize=None)
-    def model_type(self) -> str:
-        """Get type of model.
+    @torch.jit.export
+    def get_rcut(self) -> float:
+        return self.rcut
+
+    @torch.jit.export
+    def get_type_map(self) -> Optional[List[str]]:
+        raise NotImplementedError("TODO: implement this method")
+
+    def get_sel(self) -> List[int]:
+        return [self.sel]
+
+    def get_nsel(self) -> int:
+        return self.sel
+
+    def mixed_types(self) -> bool:
+        """If true, the model
+        1. assumes total number of atoms aligned across frames;
+        2. uses a neighbor list that does not distinguish different atomic types.
+
+        If false, the model
+        1. assumes total number of atoms of each atom type aligned across frames;
+        2. uses a neighbor list that distinguishes different atomic types.
 
-        :type:str
         """
-        t_mt = self._get_tensor("model_attr/model_type:0")
-        [mt] = run_sess(self.sess, [t_mt], feed_dict={})
-        return mt.decode("utf-8")
-
-    @property
-    @lru_cache(maxsize=None)
-    def model_version(self) -> str:
-        """Get version of model.
+        # to match DPA1 and DPA2.
+        return True
 
-        Returns
-        -------
-        str
-            version of model
-        """
-        try:
-            t_mt = self._get_tensor("model_attr/model_version:0")
-        except KeyError:
-            # For deepmd-kit version 0.x - 1.x, set model version to 0.0
-            return "0.0"
-        else:
-            [mt] = run_sess(self.sess, [t_mt], feed_dict={})
-            return mt.decode("utf-8")
+    def serialize(self) -> dict:
+        dd = BaseAtomicModel.serialize(self)
+        dd.update(
+            {
+                "@class": "Model",
+                "@version": 1,
+                "type": "pairtab",
+                "tab": self.tab.serialize(),
+                "rcut": self.rcut,
+                "sel": self.sel,
+            }
+        )
+        return dd
 
-    @property
-    @lru_cache(maxsize=None)
-    def sess(self) -> tf.Session:
-        """Get TF session."""
-        # start a tf session associated to the graph
-        return tf.Session(graph=self.graph, config=default_tf_session_config)
+    @classmethod
+    def deserialize(cls, data) -> "PairTabAtomicModel":
+        data = copy.deepcopy(data)
+        check_version_compatibility(data.pop("@version", 1), 1, 1)
+        rcut = data.pop("rcut")
+        sel = data.pop("sel")
+        tab = PairTab.deserialize(data.pop("tab"))
+        data.pop("@class", None)
+        data.pop("type", None)
+        tab_model = cls(None, rcut, sel, **data)
+        tab_model.tab = tab
+        tab_model.register_buffer("tab_info", torch.from_numpy(tab_model.tab.tab_info))
+        tab_model.register_buffer("tab_data", torch.from_numpy(tab_model.tab.tab_data))
+        return tab_model
 
-    def _graph_compatable(self) -> bool:
-        """Check the model compatability.
+    def forward_atomic(
+        self,
+        extended_coord: torch.Tensor,
+        extended_atype: torch.Tensor,
+        nlist: torch.Tensor,
+        mapping: Optional[torch.Tensor] = None,
+        fparam: Optional[torch.Tensor] = None,
+        aparam: Optional[torch.Tensor] = None,
+        do_atomic_virial: bool = False,
+    ) -> Dict[str, torch.Tensor]:
+        nframes, nloc, nnei = nlist.shape
+        extended_coord = extended_coord.view(nframes, -1, 3)
+        if self.do_grad_r() or self.do_grad_c():
+            extended_coord.requires_grad_(True)
+
+        # this will mask all -1 in the nlist
+        mask = nlist >= 0
+        masked_nlist = nlist * mask
+
+        atype = extended_atype[:, :nloc]  # (nframes, nloc)
+        pairwise_rr = self._get_pairwise_dist(
+            extended_coord, masked_nlist
+        )  # (nframes, nloc, nnei)
+        self.tab_data = self.tab_data.to(device=extended_coord.device).view(
+            int(self.tab_info[-1]), int(self.tab_info[-1]), int(self.tab_info[2]), 4
+        )
 
-        Returns
-        -------
-        bool
-            If the model stored in the graph file is compatable with the current code
-        """
-        model_version_major = int(self.model_version.split(".")[0])
-        model_version_minor = int(self.model_version.split(".")[1])
-        MODEL_VERSION_MAJOR = int(MODEL_VERSION.split(".")[0])
-        MODEL_VERSION_MINOR = int(MODEL_VERSION.split(".")[1])
-        if (model_version_major != MODEL_VERSION_MAJOR) or (
-            model_version_minor > MODEL_VERSION_MINOR
-        ):
-            return False
-        else:
-            return True
+        # to calculate the atomic_energy, we need 3 tensors, i_type, j_type, pairwise_rr
+        # i_type : (nframes, nloc), this is atype.
+        # j_type : (nframes, nloc, nnei)
+        j_type = extended_atype[
+            torch.arange(extended_atype.size(0), device=extended_coord.device)[
+                :, None, None
+            ],
+            masked_nlist,
+        ]
+
+        raw_atomic_energy = self._pair_tabulated_inter(
+            nlist, atype, j_type, pairwise_rr
+        )
 
-    def _get_tensor(
-        self, tensor_name: str, attr_name: Optional[str] = None
-    ) -> tf.Tensor:
-        """Get TF graph tensor and assign it to class namespace.
+        atomic_energy = 0.5 * torch.sum(
+            torch.where(
+                nlist != -1, raw_atomic_energy, torch.zeros_like(raw_atomic_energy)
+            ),
+            dim=-1,
+        ).unsqueeze(-1)
+
+        return {"energy": atomic_energy}
+
+    def _pair_tabulated_inter(
+        self,
+        nlist: torch.Tensor,
+        i_type: torch.Tensor,
+        j_type: torch.Tensor,
+        rr: torch.Tensor,
+    ) -> torch.Tensor:
+        """Pairwise tabulated energy.
 
         Parameters
         ----------
-        tensor_name : str
-            name of tensor to get
-        attr_name : Optional[str], optional
-            if specified, class attribute with this name will be created and tensor will
-            be assigned to it, by default None
+        nlist : torch.Tensor
+            The unmasked neighbour list. (nframes, nloc)
+        i_type : torch.Tensor
+            The integer representation of atom type for all local atoms for all frames. (nframes, nloc)
+        j_type : torch.Tensor
+            The integer representation of atom type for all neighbour atoms of all local atoms for all frames. (nframes, nloc, nnei)
+        rr : torch.Tensor
+            The salar distance vector between two atoms. (nframes, nloc, nnei)
 
         Returns
         -------
-        tf.Tensor
-            loaded tensor
+        torch.Tensor
+            The masked atomic energy for all local atoms for all frames. (nframes, nloc, nnei)
+
+        Raises
+        ------
+        Exception
+            If the distance is beyond the table.
+
+        Notes
+        -----
+        This function is used to calculate the pairwise energy between two atoms.
+        It uses a table containing cubic spline coefficients calculated in PairTab.
         """
-        # do not use os.path.join as it doesn't work on Windows
-        tensor_path = "/".join((self.load_prefix, tensor_name))
-        tensor = self.graph.get_tensor_by_name(tensor_path)
-        if attr_name:
-            setattr(self, attr_name, tensor)
-            return tensor
-        else:
-            return tensor
+        nframes, nloc, nnei = nlist.shape
+        rmin = self.tab_info[0]
+        hh = self.tab_info[1]
+        hi = 1.0 / hh
 
-    @staticmethod
-    def _load_graph(
-        frozen_graph_filename: "Path",
-        prefix: str = "load",
-        default_tf_graph: bool = False,
-        input_map: Optional[dict] = None,
-    ):
-        # We load the protobuf file from the disk and parse it to retrieve the
-        # unserialized graph_def
-        with tf.gfile.GFile(str(frozen_graph_filename), "rb") as f:
-            graph_def = tf.GraphDef()
-            graph_def.ParseFromString(f.read())
-
-            if default_tf_graph:
-                tf.import_graph_def(
-                    graph_def,
-                    input_map=input_map,
-                    return_elements=None,
-                    name=prefix,
-                    producer_op_list=None,
-                )
-                graph = tf.get_default_graph()
-            else:
-                # Then, we can use again a convenient built-in function to import
-                # a graph_def into the  current default Graph
-                with tf.Graph().as_default() as graph:
-                    tf.import_graph_def(
-                        graph_def,
-                        input_map=None,
-                        return_elements=None,
-                        name=prefix,
-                        producer_op_list=None,
-                    )
+        nspline = int(self.tab_info[2] + 0.1)
 
-            return graph
+        uu = (rr - rmin) * hi  # this is broadcasted to (nframes,nloc,nnei)
 
-    @staticmethod
-    def sort_input(
-        coord: np.ndarray,
-        atom_type: np.ndarray,
-        sel_atoms: Optional[List[int]] = None,
-        mixed_type: bool = False,
-    ):
-        """Sort atoms in the system according their types.
+        # if nnei of atom 0 has -1 in the nlist, uu would be 0.
+        # this is to handle the nlist where the mask is set to 0, so that we don't raise exception for those atoms.
+        uu = torch.where(nlist != -1, uu, nspline + 1)
 
-        Parameters
-        ----------
-        coord
-            The coordinates of atoms.
-            Should be of shape [nframes, natoms, 3]
-        atom_type
-            The type of atoms
-            Should be of shape [natoms]
-        sel_atoms
-            The selected atoms by type
-        mixed_type
-            Whether to perform the mixed_type mode.
-            If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
-            in which frames in a system may have different natoms_vec(s), with the same nloc.
+        if torch.any(uu < 0):
+            raise Exception("coord go beyond table lower boundary")
 
-        Returns
-        -------
-        coord_out
-            The coordinates after sorting
-        atom_type_out
-            The atom types after sorting
-        idx_map
-            The index mapping from the input to the output.
-            For example coord_out = coord[:,idx_map,:]
-        sel_atom_type
-            Only output if sel_atoms is not None
-            The sorted selected atom types
-        sel_idx_map
-            Only output if sel_atoms is not None
-            The index mapping from the selected atoms to sorted selected atoms.
-        """
-        if mixed_type:
-            # mixed_type need not to resort
-            natoms = atom_type[0].size
-            idx_map = np.arange(natoms)
-            return coord, atom_type, idx_map
-        if sel_atoms is not None:
-            selection = [False] * np.size(atom_type)
-            for ii in sel_atoms:
-                selection += atom_type == ii
-            sel_atom_type = atom_type[selection]
-        natoms = atom_type.size
-        idx = np.arange(natoms)
-        idx_map = np.lexsort((idx, atom_type))
-        nframes = coord.shape[0]
-        coord = coord.reshape([nframes, -1, 3])
-        coord = np.reshape(coord[:, idx_map, :], [nframes, -1])
-        atom_type = atom_type[idx_map]
-        if sel_atoms is not None:
-            sel_natoms = np.size(sel_atom_type)
-            sel_idx = np.arange(sel_natoms)
-            sel_idx_map = np.lexsort((sel_idx, sel_atom_type))
-            sel_atom_type = sel_atom_type[sel_idx_map]
-            return coord, atom_type, idx_map, sel_atom_type, sel_idx_map
-        else:
-            return coord, atom_type, idx_map
+        idx = uu.to(torch.int)
+
+        uu -= idx
+
+        table_coef = self._extract_spline_coefficient(
+            i_type, j_type, idx, self.tab_data, nspline
+        )
+        table_coef = table_coef.view(nframes, nloc, nnei, 4)
+        ener = self._calculate_ener(table_coef, uu)
+
+        # here we need to overwrite energy to zero at rcut and beyond.
+        mask_beyond_rcut = rr >= self.rcut
+        # also overwrite values beyond extrapolation to zero
+        extrapolation_mask = rr >= rmin + nspline * hh
+        ener[mask_beyond_rcut] = 0
+        ener[extrapolation_mask] = 0
+
+        return ener
 
     @staticmethod
-    def reverse_map(vec: np.ndarray, imap: List[int]) -> np.ndarray:
-        """Reverse mapping of a vector according to the index map.
+    def _get_pairwise_dist(coords: torch.Tensor, nlist: torch.Tensor) -> torch.Tensor:
+        """Get pairwise distance `dr`.
 
         Parameters
         ----------
-        vec
-            Input vector. Be of shape [nframes, natoms, -1]
-        imap
-            Index map. Be of shape [natoms]
+        coords : torch.Tensor
+            The coordinate of the atoms, shape of (nframes, nall, 3).
+        nlist
+            The masked nlist, shape of (nframes, nloc, nnei)
 
         Returns
         -------
-        vec_out
-            Reverse mapped vector.
+        torch.Tensor
+            The pairwise distance between the atoms (nframes, nloc, nnei).
         """
-        ret = np.zeros(vec.shape)
-        # for idx,ii in enumerate(imap) :
-        #     ret[:,ii,:] = vec[:,idx,:]
-        ret[:, imap, :] = vec
-        return ret
-
-    def make_natoms_vec(
-        self, atom_types: np.ndarray, mixed_type: bool = False
-    ) -> np.ndarray:
-        """Make the natom vector used by deepmd-kit.
+        nframes, nloc, nnei = nlist.shape
+        coord_l = coords[:, :nloc].view(nframes, -1, 1, 3)
+        index = nlist.view(nframes, -1).unsqueeze(-1).expand(-1, -1, 3)
+        coord_r = torch.gather(coords, 1, index)
+        coord_r = coord_r.view(nframes, nloc, nnei, 3)
+        diff = coord_r - coord_l
+        pairwise_rr = torch.linalg.norm(diff, dim=-1, keepdim=True).squeeze(-1)
+        return pairwise_rr
+
+    @staticmethod
+    def _extract_spline_coefficient(
+        i_type: torch.Tensor,
+        j_type: torch.Tensor,
+        idx: torch.Tensor,
+        tab_data: torch.Tensor,
+        nspline: int,
+    ) -> torch.Tensor:
+        """Extract the spline coefficient from the table.
 
         Parameters
         ----------
-        atom_types
-            The type of atoms
-        mixed_type
-            Whether to perform the mixed_type mode.
-            If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
-            in which frames in a system may have different natoms_vec(s), with the same nloc.
+        i_type : torch.Tensor
+            The integer representation of atom type for all local atoms for all frames. (nframes, nloc)
+        j_type : torch.Tensor
+            The integer representation of atom type for all neighbour atoms of all local atoms for all frames. (nframes, nloc, nnei)
+        idx : torch.Tensor
+            The index of the spline coefficient. (nframes, nloc, nnei)
+        tab_data : torch.Tensor
+            The table storing all the spline coefficient. (ntype, ntype, nspline, 4)
+        nspline : int
+            The number of splines in the table.
 
         Returns
         -------
-        natoms
-            The number of atoms. This tensor has the length of Ntypes + 2
-            natoms[0]: number of local atoms
-            natoms[1]: total number of atoms held by this processor
-            natoms[i]: 2 <= i < Ntypes+2, number of type i atoms
+        torch.Tensor
+            The spline coefficient. (nframes, nloc, nnei, 4), shape may be squeezed.
 
         """
-        natoms_vec = np.zeros(self.ntypes + 2).astype(int)
-        if mixed_type:
-            natoms = atom_types[0].size
-        else:
-            natoms = atom_types.size
-        natoms_vec[0] = natoms
-        natoms_vec[1] = natoms
-        if mixed_type:
-            natoms_vec[2] = natoms
-            return natoms_vec
-        for ii in range(self.ntypes):
-            natoms_vec[ii + 2] = np.count_nonzero(atom_types == ii)
-        return natoms_vec
+        # (nframes, nloc, nnei)
+        expanded_i_type = i_type.unsqueeze(-1).expand(-1, -1, j_type.shape[-1])
 
-    def eval_typeebd(self) -> np.ndarray:
-        """Evaluate output of type embedding network by using this model.
+        # (nframes, nloc, nnei, nspline, 4)
+        expanded_tab_data = tab_data[expanded_i_type, j_type]
 
-        Returns
-        -------
-        np.ndarray
-            The output of type embedding network. The shape is [ntypes, o_size],
-            where ntypes is the number of types, and o_size is the number of nodes
-            in the output layer.
+        # (nframes, nloc, nnei, 1, 4)
+        expanded_idx = idx.unsqueeze(-1).unsqueeze(-1).expand(-1, -1, -1, -1, 4)
 
-        Raises
-        ------
-        KeyError
-            If the model does not enable type embedding.
+        # handle the case where idx is beyond the number of splines
+        clipped_indices = torch.clamp(expanded_idx, 0, nspline - 1).to(torch.int64)
 
-        See Also
-        --------
-        deepmd.utils.type_embed.TypeEmbedNet : The type embedding network.
-
-        Examples
-        --------
-        Get the output of type embedding network of `graph.pb`:
-
-        >>> from deepmd.infer import DeepPotential
-        >>> dp = DeepPotential('graph.pb')
-        >>> dp.eval_typeebd()
-        """
-        t_typeebd = self._get_tensor("t_typeebd:0")
-        [typeebd] = run_sess(self.sess, [t_typeebd], feed_dict={})
-        return typeebd
+        # (nframes, nloc, nnei, 4)
+        final_coef = torch.gather(expanded_tab_data, 3, clipped_indices).squeeze()
 
-    def build_neighbor_list(
-        self,
-        coords: np.ndarray,
-        cell: Optional[np.ndarray],
-        atype: np.ndarray,
-        imap: np.ndarray,
-        neighbor_list,
-    ):
-        """Make the mesh with neighbor list for a single frame.
+        # when the spline idx is beyond the table, all spline coefficients are set to `0`, and the resulting ener corresponding to the idx is also `0`.
+        final_coef[expanded_idx.squeeze() > nspline] = 0
+        return final_coef
+
+    @staticmethod
+    def _calculate_ener(coef: torch.Tensor, uu: torch.Tensor) -> torch.Tensor:
+        """Calculate energy using spline coeeficients.
 
         Parameters
         ----------
-        coords : np.ndarray
-            The coordinates of atoms. Should be of shape [natoms, 3]
-        cell : Optional[np.ndarray]
-            The cell of the system. Should be of shape [3, 3]
-        atype : np.ndarray
-            The type of atoms. Should be of shape [natoms]
-        imap : np.ndarray
-            The index map of atoms. Should be of shape [natoms]
-        neighbor_list : ase.neighborlist.NewPrimitiveNeighborList
-            ASE neighbor list. The following method or attribute will be
-            used/set: bothways, self_interaction, update, build, first_neigh,
-            pair_second, offset_vec.
+        coef : torch.Tensor
+            The spline coefficients. (nframes, nloc, nnei, 4)
+        uu : torch.Tensor
+            The atom displancemnt used in interpolation and extrapolation (nframes, nloc, nnei)
 
         Returns
         -------
-        natoms_vec : np.ndarray
-            The number of atoms. This tensor has the length of Ntypes + 2
-            natoms[0]: nloc
-            natoms[1]: nall
-            natoms[i]: 2 <= i < Ntypes+2, number of type i atoms for nloc
-        coords : np.ndarray
-            The coordinates of atoms, including ghost atoms. Should be of
-            shape [nframes, nall, 3]
-        atype : np.ndarray
-            The type of atoms, including ghost atoms. Should be of shape [nall]
-        mesh : np.ndarray
-            The mesh in nei_mode=4.
-        imap : np.ndarray
-            The index map of atoms. Should be of shape [nall]
-        ghost_map : np.ndarray
-            The index map of ghost atoms. Should be of shape [nghost]
+        torch.Tensor
+            The atomic energy for all local atoms for all frames. (nframes, nloc, nnei)
+        """
+        a3, a2, a1, a0 = torch.unbind(coef, dim=-1)
+        etmp = (a3 * uu + a2) * uu + a1  # this should be elementwise operations.
+        ener = etmp * uu + a0  # this energy has the extrapolated value when rcut > rmax
+        return ener
+
+    @torch.jit.export
+    def get_dim_fparam(self) -> int:
+        """Get the number (dimension) of frame parameters of this atomic model."""
+        return 0
+
+    @torch.jit.export
+    def get_dim_aparam(self) -> int:
+        """Get the number (dimension) of atomic parameters of this atomic model."""
+        return 0
+
+    @torch.jit.export
+    def get_sel_type(self) -> List[int]:
+        """Get the selected atom types of this model.
+
+        Only atoms with selected atom types have atomic contribution
+        to the result of the model.
+        If returning an empty list, all atom types are selected.
+        """
+        return []
+
+    @torch.jit.export
+    def is_aparam_nall(self) -> bool:
+        """Check whether the shape of atomic parameters is (nframes, nall, ndim).
+
+        If False, the shape is (nframes, nloc, ndim).
         """
-        pbc = np.repeat(cell is not None, 3)
-        cell = cell.reshape(3, 3)
-        positions = coords.reshape(-1, 3)
-        neighbor_list.bothways = True
-        neighbor_list.self_interaction = False
-        if neighbor_list.update(pbc, cell, positions):
-            neighbor_list.build(pbc, cell, positions)
-        first_neigh = neighbor_list.first_neigh.copy()
-        pair_second = neighbor_list.pair_second.copy()
-        offset_vec = neighbor_list.offset_vec.copy()
-        # get out-of-box neighbors
-        out_mask = np.any(offset_vec != 0, axis=1)
-        out_idx = pair_second[out_mask]
-        out_offset = offset_vec[out_mask]
-        out_coords = positions[out_idx] + out_offset.dot(cell)
-        atype = np.array(atype, dtype=int)
-        out_atype = atype[out_idx]
-
-        nloc = positions.shape[0]
-        nghost = out_idx.size
-        all_coords = np.concatenate((positions, out_coords), axis=0)
-        all_atype = np.concatenate((atype, out_atype), axis=0)
-        # convert neighbor indexes
-        ghost_map = pair_second[out_mask]
-        pair_second[out_mask] = np.arange(nloc, nloc + nghost)
-        # get the mesh
-        mesh = np.zeros(16 + nloc * 2 + pair_second.size, dtype=int)
-        mesh[0] = nloc
-        # ilist
-        mesh[16 : 16 + nloc] = np.arange(nloc)
-        # numnei
-        mesh[16 + nloc : 16 + nloc * 2] = first_neigh[1:] - first_neigh[:-1]
-        # jlist
-        mesh[16 + nloc * 2 :] = pair_second
-
-        # natoms_vec
-        natoms_vec = np.zeros(self.ntypes + 2).astype(int)
-        natoms_vec[0] = nloc
-        natoms_vec[1] = nloc + nghost
-        for ii in range(self.ntypes):
-            natoms_vec[ii + 2] = np.count_nonzero(atype == ii)
-        # imap append ghost atoms
-        imap = np.concatenate((imap, np.arange(nloc, nloc + nghost)))
-        return natoms_vec, all_coords, all_atype, mesh, imap, ghost_map
+        return False
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/deep_polar.py` & `deepmd_kit-3.0.0a0/deepmd/dpmodel/descriptor/make_base_descriptor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,165 +1,159 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
+from abc import (
+    ABC,
+    abstractmethod,
+)
 from typing import (
-    TYPE_CHECKING,
+    Callable,
     List,
     Optional,
+    Union,
 )
 
-import numpy as np
-
-from deepmd.infer.deep_tensor import (
-    DeepTensor,
+from deepmd.common import (
+    j_get_type,
+)
+from deepmd.utils.path import (
+    DPPath,
+)
+from deepmd.utils.plugin import (
+    PluginVariant,
+    make_plugin_registry,
 )
-
-if TYPE_CHECKING:
-    from pathlib import (
-        Path,
-    )
 
 
-class DeepPolar(DeepTensor):
-    """Constructor.
+def make_base_descriptor(
+    t_tensor,
+    fwd_method_name: str = "forward",
+):
+    """Make the base class for the descriptor.
 
     Parameters
     ----------
-    model_file : Path
-        The name of the frozen model file.
-    load_prefix: str
-        The prefix in the load computational graph
-    default_tf_graph : bool
-        If uses the default tf graph, otherwise build a new tf graph for evaluation
-    input_map : dict, optional
-        The input map for tf.import_graph_def. Only work with default tf graph
-    neighbor_list : ase.neighborlist.NeighborList, optional
-        The neighbor list object. If None, then build the native neighbor list.
-
-    Warnings
-    --------
-    For developers: `DeepTensor` initializer must be called at the end after
-    `self.tensors` are modified because it uses the data in `self.tensors` dict.
-    Do not chanage the order!
-    """
+    t_tensor
+        The type of the tensor. used in the type hint.
+    fwd_method_name
+        Name of the forward method. For dpmodels, it should be "call".
+        For torch models, it should be "forward".
 
-    def __init__(
-        self,
-        model_file: "Path",
-        load_prefix: str = "load",
-        default_tf_graph: bool = False,
-        input_map: Optional[dict] = None,
-        neighbor_list=None,
-    ) -> None:
-        # use this in favor of dict update to move attribute from class to
-        # instance namespace
-        self.tensors = dict(
-            {
-                # output tensor
-                "t_tensor": "o_polar:0",
-            },
-            **self.tensors,
-        )
+    """
 
-        DeepTensor.__init__(
-            self,
-            model_file,
-            load_prefix=load_prefix,
-            default_tf_graph=default_tf_graph,
-            input_map=input_map,
-            neighbor_list=neighbor_list,
-        )
-
-    def get_dim_fparam(self) -> int:
-        """Unsupported in this model."""
-        raise NotImplementedError("This model type does not support this attribute")
-
-    def get_dim_aparam(self) -> int:
-        """Unsupported in this model."""
-        raise NotImplementedError("This model type does not support this attribute")
+    class BD(ABC, PluginVariant, make_plugin_registry("descriptor")):
+        """Base descriptor provides the interfaces of descriptor."""
 
+        def __new__(cls, *args, **kwargs):
+            if cls is BD:
+                cls = cls.get_class_by_type(j_get_type(kwargs, cls.__name__))
+            return super().__new__(cls)
+
+        @abstractmethod
+        def get_rcut(self) -> float:
+            """Returns the cut-off radius."""
+            pass
+
+        @abstractmethod
+        def get_sel(self) -> List[int]:
+            """Returns the number of selected neighboring atoms for each type."""
+            pass
+
+        def get_nsel(self) -> int:
+            """Returns the total number of selected neighboring atoms in the cut-off radius."""
+            return sum(self.get_sel())
+
+        def get_nnei(self) -> int:
+            """Returns the total number of selected neighboring atoms in the cut-off radius."""
+            return self.get_nsel()
+
+        @abstractmethod
+        def get_ntypes(self) -> int:
+            """Returns the number of element types."""
+            pass
+
+        @abstractmethod
+        def get_dim_out(self) -> int:
+            """Returns the output descriptor dimension."""
+            pass
+
+        @abstractmethod
+        def get_dim_emb(self) -> int:
+            """Returns the embedding dimension of g2."""
+            pass
+
+        @abstractmethod
+        def mixed_types(self) -> bool:
+            """Returns if the descriptor requires a neighbor list that distinguish different
+            atomic types or not.
+            """
+            pass
+
+        @abstractmethod
+        def share_params(self, base_class, shared_level, resume=False):
+            """
+            Share the parameters of self to the base_class with shared_level during multitask training.
+            If not start from checkpoint (resume is False),
+            some seperated parameters (e.g. mean and stddev) will be re-calculated across different classes.
+            """
+            pass
 
-class DeepGlobalPolar(DeepTensor):
-    """Constructor.
+        def compute_input_stats(
+            self,
+            merged: Union[Callable[[], List[dict]], List[dict]],
+            path: Optional[DPPath] = None,
+        ):
+            """Update mean and stddev for descriptor elements."""
+            raise NotImplementedError
 
-    Parameters
-    ----------
-    model_file : str
-        The name of the frozen model file.
-    load_prefix: str
-        The prefix in the load computational graph
-    default_tf_graph : bool
-        If uses the default tf graph, otherwise build a new tf graph for evaluation
-    neighbor_list : ase.neighborlist.NeighborList, optional
-        The neighbor list object. If None, then build the native neighbor list.
-    """
+        @abstractmethod
+        def fwd(
+            self,
+            extended_coord,
+            extended_atype,
+            nlist,
+            mapping: Optional[t_tensor] = None,
+        ):
+            """Calculate descriptor."""
+            pass
+
+        @abstractmethod
+        def serialize(self) -> dict:
+            """Serialize the obj to dict."""
+            pass
+
+        @classmethod
+        def deserialize(cls, data: dict) -> "BD":
+            """Deserialize the model.
+
+            Parameters
+            ----------
+            data : dict
+                The serialized data
+
+            Returns
+            -------
+            BD
+                The deserialized descriptor
+            """
+            if cls is BD:
+                return BD.get_class_by_type(data["type"]).deserialize(data)
+            raise NotImplementedError("Not implemented in class %s" % cls.__name__)
+
+        @classmethod
+        @abstractmethod
+        def update_sel(cls, global_jdata: dict, local_jdata: dict):
+            """Update the selection and perform neighbor statistics.
+
+            Parameters
+            ----------
+            global_jdata : dict
+                The global data, containing the training section
+            local_jdata : dict
+                The local data refer to the current class
+            """
+            # call subprocess
+            cls = cls.get_class_by_type(j_get_type(local_jdata, cls.__name__))
+            return cls.update_sel(global_jdata, local_jdata)
 
-    def __init__(
-        self,
-        model_file: str,
-        load_prefix: str = "load",
-        default_tf_graph: bool = False,
-        neighbor_list=None,
-    ) -> None:
-        self.tensors.update(
-            {
-                "t_sel_type": "model_attr/sel_type:0",
-                # output tensor
-                "t_tensor": "o_global_polar:0",
-            }
-        )
+    setattr(BD, fwd_method_name, BD.fwd)
+    delattr(BD, "fwd")
 
-        DeepTensor.__init__(
-            self,
-            model_file,
-            load_prefix=load_prefix,
-            default_tf_graph=default_tf_graph,
-            neighbor_list=None,
-        )
-
-    def eval(
-        self,
-        coords: np.ndarray,
-        cells: np.ndarray,
-        atom_types: List[int],
-        atomic: bool = False,
-        fparam: Optional[np.ndarray] = None,
-        aparam: Optional[np.ndarray] = None,
-        efield: Optional[np.ndarray] = None,
-    ) -> np.ndarray:
-        """Evaluate the model.
-
-        Parameters
-        ----------
-        coords
-            The coordinates of atoms.
-            The array should be of size nframes x natoms x 3
-        cells
-            The cell of the region.
-            If None then non-PBC is assumed, otherwise using PBC.
-            The array should be of size nframes x 9
-        atom_types
-            The atom types
-            The list should contain natoms ints
-        atomic
-            Not used in this model
-        fparam
-            Not used in this model
-        aparam
-            Not used in this model
-        efield
-            Not used in this model
-
-        Returns
-        -------
-        tensor
-            The returned tensor
-            If atomic == False then of size nframes x variable_dof
-            else of size nframes x natoms x variable_dof
-        """
-        return DeepTensor.eval(self, coords, cells, atom_types, atomic=False)
-
-    def get_dim_fparam(self) -> int:
-        """Unsupported in this model."""
-        raise NotImplementedError("This model type does not support this attribute")
-
-    def get_dim_aparam(self) -> int:
-        """Unsupported in this model."""
-        raise NotImplementedError("This model type does not support this attribute")
+    return BD
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/deep_pot.py` & `deepmd_kit-3.0.0a0/deepmd/utils/data_system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,691 +1,813 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
+import collections
 import logging
+import warnings
+from functools import (
+    lru_cache,
+)
 from typing import (
-    TYPE_CHECKING,
-    Callable,
+    Any,
+    Dict,
     List,
     Optional,
-    Tuple,
     Union,
 )
 
 import numpy as np
 
+import deepmd.utils.random as dp_random
 from deepmd.common import (
+    data_requirement,
+    expand_sys_str,
+    j_must_have,
     make_default_mesh,
 )
-from deepmd.infer.data_modifier import (
-    DipoleChargeModifier,
+from deepmd.env import (
+    GLOBAL_NP_FLOAT_PRECISION,
 )
-from deepmd.infer.deep_eval import (
-    DeepEval,
+from deepmd.utils.data import (
+    DeepmdData,
 )
-from deepmd.utils.batch_size import (
-    AutoBatchSize,
+from deepmd.utils.out_stat import (
+    compute_stats_from_redu,
 )
-from deepmd.utils.sess import (
-    run_sess,
+from deepmd.utils.path import (
+    DPPath,
 )
 
-if TYPE_CHECKING:
-    from pathlib import (
-        Path,
-    )
-
 log = logging.getLogger(__name__)
 
 
-class DeepPot(DeepEval):
-    """Constructor.
+class DeepmdDataSystem:
+    """Class for manipulating many data systems.
 
-    Parameters
-    ----------
-    model_file : Path
-        The name of the frozen model file.
-    load_prefix: str
-        The prefix in the load computational graph
-    default_tf_graph : bool
-        If uses the default tf graph, otherwise build a new tf graph for evaluation
-    auto_batch_size : bool or int or AutomaticBatchSize, default: True
-        If True, automatic batch size will be used. If int, it will be used
-        as the initial batch size.
-    input_map : dict, optional
-        The input map for tf.import_graph_def. Only work with default tf graph
-    neighbor_list : ase.neighborlist.NewPrimitiveNeighborList, optional
-        The ASE neighbor list class to produce the neighbor list. If None, the
-        neighbor list will be built natively in the model.
-
-    Examples
-    --------
-    >>> from deepmd.infer import DeepPot
-    >>> import numpy as np
-    >>> dp = DeepPot('graph.pb')
-    >>> coord = np.array([[1,0,0], [0,0,1.5], [1,0,3]]).reshape([1, -1])
-    >>> cell = np.diag(10 * np.ones(3)).reshape([1, -1])
-    >>> atype = [1,0,1]
-    >>> e, f, v = dp.eval(coord, cell, atype)
-
-    where `e`, `f` and `v` are predicted energy, force and virial of the system, respectively.
-
-    Warnings
-    --------
-    For developers: `DeepTensor` initializer must be called at the end after
-    `self.tensors` are modified because it uses the data in `self.tensors` dict.
-    Do not chanage the order!
+    It is implemented with the help of DeepmdData
     """
 
     def __init__(
         self,
-        model_file: "Path",
-        load_prefix: str = "load",
-        default_tf_graph: bool = False,
-        auto_batch_size: Union[bool, int, AutoBatchSize] = True,
-        input_map: Optional[dict] = None,
-        neighbor_list=None,
-    ) -> None:
-        # add these tensors on top of what is defined by DeepTensor Class
-        # use this in favor of dict update to move attribute from class to
-        # instance namespace
-        self.tensors = {
-            # descrpt attrs
-            "t_ntypes": "descrpt_attr/ntypes:0",
-            "t_rcut": "descrpt_attr/rcut:0",
-            # fitting attrs
-            "t_dfparam": "fitting_attr/dfparam:0",
-            "t_daparam": "fitting_attr/daparam:0",
-            # model attrs
-            "t_tmap": "model_attr/tmap:0",
-            # inputs
-            "t_coord": "t_coord:0",
-            "t_type": "t_type:0",
-            "t_natoms": "t_natoms:0",
-            "t_box": "t_box:0",
-            "t_mesh": "t_mesh:0",
-            # add output tensors
-            "t_energy": "o_energy:0",
-            "t_force": "o_force:0",
-            "t_virial": "o_virial:0",
-            "t_ae": "o_atom_energy:0",
-            "t_av": "o_atom_virial:0",
-            "t_descriptor": "o_descriptor:0",
-        }
-        DeepEval.__init__(
-            self,
-            model_file,
-            load_prefix=load_prefix,
-            default_tf_graph=default_tf_graph,
-            auto_batch_size=auto_batch_size,
-            input_map=input_map,
-            neighbor_list=neighbor_list,
-        )
+        systems: List[str],
+        batch_size: int,
+        test_size: int,
+        rcut: Optional[float] = None,
+        set_prefix: str = "set",
+        shuffle_test: bool = True,
+        type_map: Optional[List[str]] = None,
+        optional_type_map: bool = True,
+        modifier=None,
+        trn_all_set=False,
+        sys_probs=None,
+        auto_prob_style="prob_sys_size",
+        sort_atoms: bool = True,
+    ):
+        """Constructor.
 
-        # load optional tensors
-        operations = [op.name for op in self.graph.get_operations()]
-        # check if the graph has these operations:
-        # if yes add them
-
-        if ("%s/t_efield" % load_prefix) in operations:
-            self.tensors.update({"t_efield": "t_efield:0"})
-            self.has_efield = True
-        else:
-            log.debug("Could not get tensor 't_efield:0'")
-            self.t_efield = None
-            self.has_efield = False
-
-        if ("%s/t_fparam" % load_prefix) in operations:
-            self.tensors.update({"t_fparam": "t_fparam:0"})
-            self.has_fparam = True
-        else:
-            log.debug("Could not get tensor 't_fparam:0'")
-            self.t_fparam = None
-            self.has_fparam = False
-
-        if ("%s/t_aparam" % load_prefix) in operations:
-            self.tensors.update({"t_aparam": "t_aparam:0"})
-            self.has_aparam = True
-        else:
-            log.debug("Could not get tensor 't_aparam:0'")
-            self.t_aparam = None
-            self.has_aparam = False
-
-        if ("%s/spin_attr/ntypes_spin" % load_prefix) in operations:
-            self.tensors.update({"t_ntypes_spin": "spin_attr/ntypes_spin:0"})
-            self.has_spin = True
-        else:
-            self.ntypes_spin = 0
-            self.has_spin = False
+        Parameters
+        ----------
+        systems
+            Specifying the paths to systems
+        batch_size
+            The batch size
+        test_size
+            The size of test data
+        rcut
+            The cut-off radius. Not used.
+        set_prefix
+            Prefix for the directories of different sets
+        shuffle_test
+            If the test data are shuffled
+        type_map
+            Gives the name of different atom types
+        optional_type_map
+            If the type_map.raw in each system is optional
+        modifier
+            Data modifier that has the method `modify_data`
+        trn_all_set
+            Use all sets as training dataset. Otherwise, if the number of sets is more than 1, the last set is left for test.
+        sys_probs : list of float
+            The probabilitis of systems to get the batch.
+            Summation of positive elements of this list should be no greater than 1.
+            Element of this list can be negative, the probability of the corresponding system is determined
+                automatically by the number of batches in the system.
+        auto_prob_style : str
+            Determine the probability of systems automatically. The method is assigned by this key and can be
+            - "prob_uniform"  : the probability all the systems are equal, namely 1.0/self.get_nsystems()
+            - "prob_sys_size" : the probability of a system is proportional to the number of batches in the system
+            - "prob_sys_size;stt_idx:end_idx:weight;stt_idx:end_idx:weight;..." :
+                                the list of systems is devided into blocks. A block is specified by `stt_idx:end_idx:weight`,
+                                where `stt_idx` is the starting index of the system, `end_idx` is then ending (not including) index of the system,
+                                the probabilities of the systems in this block sums up to `weight`, and the relatively probabilities within this block is proportional
+                to the number of batches in the system.
+        sort_atoms : bool
+            Sort atoms by atom types. Required to enable when the data is directly feeded to
+            descriptors except mixed types.
+        """
+        # init data
+        del rcut
+        self.system_dirs = systems
+        self.nsystems = len(self.system_dirs)
+        self.data_systems = []
+        for ii in self.system_dirs:
+            self.data_systems.append(
+                DeepmdData(
+                    ii,
+                    set_prefix=set_prefix,
+                    shuffle_test=shuffle_test,
+                    type_map=type_map,
+                    optional_type_map=optional_type_map,
+                    modifier=modifier,
+                    trn_all_set=trn_all_set,
+                    sort_atoms=sort_atoms,
+                )
+            )
+        # check mix_type format
+        error_format_msg = (
+            "if one of the system is of mixed_type format, "
+            "then all of the systems should be of mixed_type format!"
+        )
+        if self.data_systems[0].mixed_type:
+            for data_sys in self.data_systems[1:]:
+                assert data_sys.mixed_type, error_format_msg
+            self.mixed_type = True
+        else:
+            for data_sys in self.data_systems[1:]:
+                assert not data_sys.mixed_type, error_format_msg
+            self.mixed_type = False
+        # batch size
+        self.batch_size = batch_size
+        is_auto_bs = False
+        self.mixed_systems = False
+        if isinstance(self.batch_size, int):
+            self.batch_size = self.batch_size * np.ones(self.nsystems, dtype=int)
+        elif isinstance(self.batch_size, str):
+            words = self.batch_size.split(":")
+            if "auto" == words[0]:
+                is_auto_bs = True
+                rule = 32
+                if len(words) == 2:
+                    rule = int(words[1])
+                self.batch_size = self._make_auto_bs(rule)
+            elif "mixed" == words[0]:
+                self.mixed_type = True
+                self.mixed_systems = True
+                if len(words) == 2:
+                    rule = int(words[1])
+                else:
+                    raise RuntimeError("batch size must be specified for mixed systems")
+                self.batch_size = rule * np.ones(self.nsystems, dtype=int)
+            else:
+                raise RuntimeError("unknown batch_size rule " + words[0])
+        elif isinstance(self.batch_size, list):
+            pass
+        else:
+            raise RuntimeError("invalid batch_size")
+        assert isinstance(self.batch_size, (list, np.ndarray))
+        assert len(self.batch_size) == self.nsystems
+
+        # natoms, nbatches
+        ntypes = []
+        for ii in self.data_systems:
+            ntypes.append(ii.get_ntypes())
+        self.sys_ntypes = max(ntypes)
+        self.natoms = []
+        self.natoms_vec = []
+        self.nbatches = []
+        type_map_list = []
+        for ii in range(self.nsystems):
+            self.natoms.append(self.data_systems[ii].get_natoms())
+            self.natoms_vec.append(
+                self.data_systems[ii].get_natoms_vec(self.sys_ntypes).astype(int)
+            )
+            self.nbatches.append(
+                self.data_systems[ii].get_sys_numb_batch(self.batch_size[ii])
+            )
+            type_map_list.append(self.data_systems[ii].get_type_map())
+        self.type_map = self._check_type_map_consistency(type_map_list)
 
-        # now load tensors to object attributes
-        for attr_name, tensor_name in self.tensors.items():
+        # ! altered by Marián Rynik
+        # test size
+        # now test size can be set as a percentage of systems data or test size
+        # can be set for each system individualy in the same manner as batch
+        # size. This enables one to use systems with diverse number of
+        # structures and different number of atoms.
+        self.test_size = test_size
+        if isinstance(self.test_size, int):
+            self.test_size = self.test_size * np.ones(self.nsystems, dtype=int)
+        elif isinstance(self.test_size, str):
+            words = self.test_size.split("%")
             try:
-                self._get_tensor(tensor_name, attr_name)
-            except KeyError:
-                if attr_name != "t_descriptor":
-                    raise
-
-        self._run_default_sess()
-        self.tmap = self.tmap.decode("UTF-8").split()
-
-        # setup modifier
-        try:
-            t_modifier_type = self._get_tensor("modifier_attr/type:0")
-            self.modifier_type = run_sess(self.sess, t_modifier_type).decode("UTF-8")
-        except (ValueError, KeyError):
-            self.modifier_type = None
-
-        try:
-            t_jdata = self._get_tensor("train_attr/training_script:0")
-            jdata = run_sess(self.sess, t_jdata).decode("UTF-8")
-            import json
-
-            jdata = json.loads(jdata)
-            self.descriptor_type = jdata["model"]["descriptor"]["type"]
-        except (ValueError, KeyError):
-            self.descriptor_type = None
-
-        if self.modifier_type == "dipole_charge":
-            t_mdl_name = self._get_tensor("modifier_attr/mdl_name:0")
-            t_mdl_charge_map = self._get_tensor("modifier_attr/mdl_charge_map:0")
-            t_sys_charge_map = self._get_tensor("modifier_attr/sys_charge_map:0")
-            t_ewald_h = self._get_tensor("modifier_attr/ewald_h:0")
-            t_ewald_beta = self._get_tensor("modifier_attr/ewald_beta:0")
-            [mdl_name, mdl_charge_map, sys_charge_map, ewald_h, ewald_beta] = run_sess(
-                self.sess,
-                [
-                    t_mdl_name,
-                    t_mdl_charge_map,
-                    t_sys_charge_map,
-                    t_ewald_h,
-                    t_ewald_beta,
-                ],
-            )
-            mdl_name = mdl_name.decode("UTF-8")
-            mdl_charge_map = [int(ii) for ii in mdl_charge_map.decode("UTF-8").split()]
-            sys_charge_map = [int(ii) for ii in sys_charge_map.decode("UTF-8").split()]
-            self.dm = DipoleChargeModifier(
-                mdl_name,
-                mdl_charge_map,
-                sys_charge_map,
-                ewald_h=ewald_h,
-                ewald_beta=ewald_beta,
+                percent = int(words[0])
+            except ValueError:
+                raise RuntimeError("unknown test_size rule " + words[0])
+            self.test_size = self._make_auto_ts(percent)
+        elif isinstance(self.test_size, list):
+            pass
+        else:
+            raise RuntimeError("invalid test_size")
+        assert isinstance(self.test_size, (list, np.ndarray))
+        assert len(self.test_size) == self.nsystems
+
+        # init pick idx
+        self.pick_idx = 0
+
+        # derive system probabilities
+        self.sys_probs = None
+        self.set_sys_probs(sys_probs, auto_prob_style)
+
+        # check batch and test size
+        for ii in range(self.nsystems):
+            chk_ret = self.data_systems[ii].check_batch_size(self.batch_size[ii])
+            if chk_ret is not None and not is_auto_bs and not self.mixed_systems:
+                warnings.warn(
+                    "system %s required batch size is larger than the size of the dataset %s (%d > %d)"
+                    % (
+                        self.system_dirs[ii],
+                        chk_ret[0],
+                        self.batch_size[ii],
+                        chk_ret[1],
+                    )
+                )
+            chk_ret = self.data_systems[ii].check_test_size(self.test_size[ii])
+            if chk_ret is not None and not is_auto_bs and not self.mixed_systems:
+                warnings.warn(
+                    "system %s required test size is larger than the size of the dataset %s (%d > %d)"
+                    % (self.system_dirs[ii], chk_ret[0], self.test_size[ii], chk_ret[1])
+                )
+
+    def _load_test(self, ntests=-1):
+        self.test_data = collections.defaultdict(list)
+        for ii in range(self.nsystems):
+            test_system_data = self.data_systems[ii].get_test(ntests=ntests)
+            for nn in test_system_data:
+                self.test_data[nn].append(test_system_data[nn])
+
+    @property
+    @lru_cache(maxsize=None)
+    def default_mesh(self) -> List[np.ndarray]:
+        """Mesh for each system."""
+        return [
+            make_default_mesh(
+                self.data_systems[ii].pbc, self.data_systems[ii].mixed_type
             )
+            for ii in range(self.nsystems)
+        ]
+
+    def compute_energy_shift(self, rcond=None, key="energy"):
+        sys_ener = []
+        for ss in self.data_systems:
+            sys_ener.append(ss.avg(key))
+        sys_ener = np.concatenate(sys_ener)
+        sys_tynatom = np.array(self.natoms_vec, dtype=GLOBAL_NP_FLOAT_PRECISION)
+        sys_tynatom = np.reshape(sys_tynatom, [self.nsystems, -1])
+        sys_tynatom = sys_tynatom[:, 2:]
+        energy_shift, _ = compute_stats_from_redu(
+            sys_ener.reshape(-1, 1),
+            sys_tynatom,
+            rcond=rcond,
+        )
+        return energy_shift.ravel()
+
+    def add_dict(self, adict: dict) -> None:
+        """Add items to the data system by a `dict`.
+        `adict` should have items like
+        .. code-block:: python.
+
+           adict[key] = {
+               "ndof": ndof,
+               "atomic": atomic,
+               "must": must,
+               "high_prec": high_prec,
+               "type_sel": type_sel,
+               "repeat": repeat,
+           }
 
-    def _run_default_sess(self):
-        if self.has_spin is True:
-            [
-                self.ntypes,
-                self.ntypes_spin,
-                self.rcut,
-                self.dfparam,
-                self.daparam,
-                self.tmap,
-            ] = run_sess(
-                self.sess,
-                [
-                    self.t_ntypes,
-                    self.t_ntypes_spin,
-                    self.t_rcut,
-                    self.t_dfparam,
-                    self.t_daparam,
-                    self.t_tmap,
-                ],
+        For the explaination of the keys see `add`
+        """
+        for kk in adict:
+            self.add(
+                kk,
+                adict[kk]["ndof"],
+                atomic=adict[kk]["atomic"],
+                must=adict[kk]["must"],
+                high_prec=adict[kk]["high_prec"],
+                type_sel=adict[kk]["type_sel"],
+                repeat=adict[kk]["repeat"],
+                default=adict[kk]["default"],
+                dtype=adict[kk].get("dtype"),
+                output_natoms_for_type_sel=adict[kk].get(
+                    "output_natoms_for_type_sel", False
+                ),
             )
-        else:
-            [self.ntypes, self.rcut, self.dfparam, self.daparam, self.tmap] = run_sess(
-                self.sess,
-                [
-                    self.t_ntypes,
-                    self.t_rcut,
-                    self.t_dfparam,
-                    self.t_daparam,
-                    self.t_tmap,
-                ],
+
+    def add(
+        self,
+        key: str,
+        ndof: int,
+        atomic: bool = False,
+        must: bool = False,
+        high_prec: bool = False,
+        type_sel: Optional[List[int]] = None,
+        repeat: int = 1,
+        default: float = 0.0,
+        dtype: Optional[np.dtype] = None,
+        output_natoms_for_type_sel: bool = False,
+    ):
+        """Add a data item that to be loaded.
+
+        Parameters
+        ----------
+        key
+            The key of the item. The corresponding data is stored in `sys_path/set.*/key.npy`
+        ndof
+            The number of dof
+        atomic
+            The item is an atomic property.
+            If False, the size of the data should be nframes x ndof
+            If True, the size of data should be nframes x natoms x ndof
+        must
+            The data file `sys_path/set.*/key.npy` must exist.
+            If must is False and the data file does not exist, the `data_dict[find_key]` is set to 0.0
+        high_prec
+            Load the data and store in float64, otherwise in float32
+        type_sel
+            Select certain type of atoms
+        repeat
+            The data will be repeated `repeat` times.
+        default, default=0.
+            Default value of data
+        dtype
+            The dtype of data, overwrites `high_prec` if provided
+        output_natoms_for_type_sel : bool
+            If True and type_sel is True, the atomic dimension will be natoms instead of nsel
+        """
+        for ii in self.data_systems:
+            ii.add(
+                key,
+                ndof,
+                atomic=atomic,
+                must=must,
+                high_prec=high_prec,
+                repeat=repeat,
+                type_sel=type_sel,
+                default=default,
+                dtype=dtype,
+                output_natoms_for_type_sel=output_natoms_for_type_sel,
             )
 
-    def get_ntypes(self) -> int:
-        """Get the number of atom types of this model."""
-        return self.ntypes
+    def reduce(self, key_out, key_in):
+        """Generate a new item from the reduction of another atom.
 
-    def get_ntypes_spin(self):
-        """Get the number of spin atom types of this model."""
-        return self.ntypes_spin
-
-    def get_rcut(self) -> float:
-        """Get the cut-off radius of this model."""
-        return self.rcut
+        Parameters
+        ----------
+        key_out
+            The name of the reduced item
+        key_in
+            The name of the data item to be reduced
+        """
+        for ii in self.data_systems:
+            ii.reduce(key_out, key_in)
 
-    def get_type_map(self) -> List[str]:
-        """Get the type map (element name of the atom types) of this model."""
-        return self.tmap
+    def get_data_dict(self, ii: int = 0) -> dict:
+        return self.data_systems[ii].get_data_dict()
 
-    def get_sel_type(self) -> List[int]:
-        """Unsupported in this model."""
-        raise NotImplementedError("This model type does not support this attribute")
-
-    def get_descriptor_type(self) -> List[int]:
-        """Get the descriptor type of this model."""
-        return self.descriptor_type
-
-    def get_dim_fparam(self) -> int:
-        """Get the number (dimension) of frame parameters of this DP."""
-        return self.dfparam
-
-    def get_dim_aparam(self) -> int:
-        """Get the number (dimension) of atomic parameters of this DP."""
-        return self.daparam
+    def set_sys_probs(self, sys_probs=None, auto_prob_style: str = "prob_sys_size"):
+        if sys_probs is None:
+            if auto_prob_style == "prob_uniform":
+                prob_v = 1.0 / float(self.nsystems)
+                probs = [prob_v for ii in range(self.nsystems)]
+            elif auto_prob_style[:13] == "prob_sys_size":
+                if auto_prob_style == "prob_sys_size":
+                    prob_style = f"prob_sys_size;0:{self.get_nsystems()}:1.0"
+                else:
+                    prob_style = auto_prob_style
+                probs = prob_sys_size_ext(
+                    prob_style, self.get_nsystems(), self.nbatches
+                )
+            else:
+                raise RuntimeError("Unknown auto prob style: " + auto_prob_style)
+        else:
+            probs = process_sys_probs(sys_probs, self.nbatches)
+        self.sys_probs = probs
 
-    def _eval_func(self, inner_func: Callable, numb_test: int, natoms: int) -> Callable:
-        """Wrapper method with auto batch size.
+    def get_batch(self, sys_idx: Optional[int] = None) -> dict:
+        # batch generation style altered by Ziyao Li:
+        # one should specify the "sys_prob" and "auto_prob_style" params
+        # via set_sys_prob() function. The sys_probs this function uses is
+        # defined as a private variable, self.sys_probs, initialized in __init__().
+        # This is to optimize the (vain) efforts in evaluating sys_probs every batch.
+        """Get a batch of data from the data systems.
 
         Parameters
         ----------
-        inner_func : Callable
-            the method to be wrapped
-        numb_test : int
-            number of tests
-        natoms : int
-            number of atoms
+        sys_idx : int
+            The index of system from which the batch is get.
+            If sys_idx is not None, `sys_probs` and `auto_prob_style` are ignored
+            If sys_idx is None, automatically determine the system according to `sys_probs` or `auto_prob_style`, see the following.
+            This option does not work for mixed systems.
 
         Returns
         -------
-        Callable
-            the wrapper
+        dict
+            The batch data
         """
-        if self.auto_batch_size is not None:
-
-            def eval_func(*args, **kwargs):
-                return self.auto_batch_size.execute_all(
-                    inner_func, numb_test, natoms, *args, **kwargs
-                )
-
+        if not self.mixed_systems:
+            b_data = self.get_batch_standard(sys_idx)
         else:
-            eval_func = inner_func
-        return eval_func
+            b_data = self.get_batch_mixed()
+        return b_data
 
-    def _get_natoms_and_nframes(
-        self,
-        coords: np.ndarray,
-        atom_types: Union[List[int], np.ndarray],
-        mixed_type: bool = False,
-    ) -> Tuple[int, int]:
-        if mixed_type:
-            natoms = len(atom_types[0])
-        else:
-            natoms = len(atom_types)
-        if natoms == 0:
-            assert coords.size == 0
-        else:
-            coords = np.reshape(np.array(coords), [-1, natoms * 3])
-        nframes = coords.shape[0]
-        return natoms, nframes
-
-    def eval(
-        self,
-        coords: np.ndarray,
-        cells: np.ndarray,
-        atom_types: List[int],
-        atomic: bool = False,
-        fparam: Optional[np.ndarray] = None,
-        aparam: Optional[np.ndarray] = None,
-        efield: Optional[np.ndarray] = None,
-        mixed_type: bool = False,
-    ) -> Tuple[np.ndarray, ...]:
-        """Evaluate the energy, force and virial by using this DP.
+    def get_batch_standard(self, sys_idx: Optional[int] = None) -> dict:
+        """Get a batch of data from the data systems in the standard way.
 
         Parameters
         ----------
-        coords
-            The coordinates of atoms.
-            The array should be of size nframes x natoms x 3
-        cells
-            The cell of the region.
-            If None then non-PBC is assumed, otherwise using PBC.
-            The array should be of size nframes x 9
-        atom_types
-            The atom types
-            The list should contain natoms ints
-        atomic
-            Calculate the atomic energy and virial
-        fparam
-            The frame parameter.
-            The array can be of size :
-            - nframes x dim_fparam.
-            - dim_fparam. Then all frames are assumed to be provided with the same fparam.
-        aparam
-            The atomic parameter
-            The array can be of size :
-            - nframes x natoms x dim_aparam.
-            - natoms x dim_aparam. Then all frames are assumed to be provided with the same aparam.
-            - dim_aparam. Then all frames and atoms are provided with the same aparam.
-        efield
-            The external field on atoms.
-            The array should be of size nframes x natoms x 3
-        mixed_type
-            Whether to perform the mixed_type mode.
-            If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
-            in which frames in a system may have different natoms_vec(s), with the same nloc.
+        sys_idx : int
+            The index of system from which the batch is get.
+            If sys_idx is not None, `sys_probs` and `auto_prob_style` are ignored
+            If sys_idx is None, automatically determine the system according to `sys_probs` or `auto_prob_style`, see the following.
 
         Returns
         -------
-        energy
-            The system energy.
-        force
-            The force on each atom
-        virial
-            The virial
-        atom_energy
-            The atomic energy. Only returned when atomic == True
-        atom_virial
-            The atomic virial. Only returned when atomic == True
+        dict
+            The batch data
         """
-        # reshape coords before getting shape
-        natoms, numb_test = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        output = self._eval_func(self._eval_inner, numb_test, natoms)(
-            coords,
-            cells,
-            atom_types,
-            fparam=fparam,
-            aparam=aparam,
-            atomic=atomic,
-            efield=efield,
-            mixed_type=mixed_type,
-        )
+        if sys_idx is not None:
+            self.pick_idx = sys_idx
+        else:
+            # prob = self._get_sys_probs(sys_probs, auto_prob_style)
+            self.pick_idx = dp_random.choice(np.arange(self.nsystems), p=self.sys_probs)
+        b_data = self.data_systems[self.pick_idx].get_batch(
+            self.batch_size[self.pick_idx]
+        )
+        b_data["natoms_vec"] = self.natoms_vec[self.pick_idx]
+        b_data["default_mesh"] = self.default_mesh[self.pick_idx]
+        return b_data
 
-        if self.modifier_type is not None:
-            if atomic:
-                raise RuntimeError("modifier does not support atomic modification")
-            me, mf, mv = self.dm.eval(coords, cells, atom_types)
-            output = list(output)  # tuple to list
-            e, f, v = output[:3]
-            output[0] += me.reshape(e.shape)
-            output[1] += mf.reshape(f.shape)
-            output[2] += mv.reshape(v.shape)
-            output = tuple(output)
-        return output
+    def get_batch_mixed(self) -> dict:
+        """Get a batch of data from the data systems in the mixed way.
 
-    def _prepare_feed_dict(
-        self,
-        coords,
-        cells,
-        atom_types,
-        fparam=None,
-        aparam=None,
-        efield=None,
-        mixed_type=False,
-    ):
-        # standarize the shape of inputs
-        natoms, nframes = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        if mixed_type:
-            atom_types = np.array(atom_types, dtype=int).reshape([-1, natoms])
-        else:
-            atom_types = np.array(atom_types, dtype=int).reshape([-1])
-        coords = np.reshape(np.array(coords), [nframes, natoms * 3])
-        if cells is None:
-            pbc = False
-            # make cells to work around the requirement of pbc
-            cells = np.tile(np.eye(3), [nframes, 1]).reshape([nframes, 9])
-        else:
-            pbc = True
-            cells = np.array(cells).reshape([nframes, 9])
+        Returns
+        -------
+        dict
+            The batch data
+        """
+        # mixed systems have a global batch size
+        batch_size = self.batch_size[0]
+        batch_data = []
+        for _ in range(batch_size):
+            self.pick_idx = dp_random.choice(np.arange(self.nsystems), p=self.sys_probs)
+            bb_data = self.data_systems[self.pick_idx].get_batch(1)
+            bb_data["natoms_vec"] = self.natoms_vec[self.pick_idx]
+            bb_data["default_mesh"] = self.default_mesh[self.pick_idx]
+            batch_data.append(bb_data)
+        b_data = self._merge_batch_data(batch_data)
+        return b_data
 
-        if self.has_fparam:
-            assert fparam is not None
-            fparam = np.array(fparam)
-        if self.has_aparam:
-            assert aparam is not None
-            aparam = np.array(aparam)
-        if self.has_efield:
-            assert (
-                efield is not None
-            ), "you are using a model with external field, parameter efield should be provided"
-            efield = np.array(efield)
-
-        # reshape the inputs
-        if self.has_fparam:
-            fdim = self.get_dim_fparam()
-            if fparam.size == nframes * fdim:
-                fparam = np.reshape(fparam, [nframes, fdim])
-            elif fparam.size == fdim:
-                fparam = np.tile(fparam.reshape([-1]), [nframes, 1])
-            else:
-                raise RuntimeError(
-                    "got wrong size of frame param, should be either %d x %d or %d"
-                    % (nframes, fdim, fdim)
-                )
-        if self.has_aparam:
-            fdim = self.get_dim_aparam()
-            if aparam.size == nframes * natoms * fdim:
-                aparam = np.reshape(aparam, [nframes, natoms * fdim])
-            elif aparam.size == natoms * fdim:
-                aparam = np.tile(aparam.reshape([-1]), [nframes, 1])
-            elif aparam.size == fdim:
-                aparam = np.tile(aparam.reshape([-1]), [nframes, natoms])
+    def _merge_batch_data(self, batch_data: List[dict]) -> dict:
+        """Merge batch data from different systems.
+
+        Parameters
+        ----------
+        batch_data : list of dict
+            A list of batch data from different systems.
+
+        Returns
+        -------
+        dict
+            The merged batch data.
+        """
+        b_data = {}
+        max_natoms = max(bb["natoms_vec"][0] for bb in batch_data)
+        # natoms_vec
+        natoms_vec = np.zeros(2 + self.get_ntypes(), dtype=int)
+        natoms_vec[0:3] = max_natoms
+        b_data["natoms_vec"] = natoms_vec
+        # real_natoms_vec
+        real_natoms_vec = np.vstack([bb["natoms_vec"] for bb in batch_data])
+        b_data["real_natoms_vec"] = real_natoms_vec
+        # type
+        type_vec = np.full((len(batch_data), max_natoms), -1, dtype=int)
+        for ii, bb in enumerate(batch_data):
+            type_vec[ii, : bb["type"].shape[1]] = bb["type"][0]
+        b_data["type"] = type_vec
+        # default_mesh
+        default_mesh = np.mean([bb["default_mesh"] for bb in batch_data], axis=0)
+        b_data["default_mesh"] = default_mesh
+        # other data
+        data_dict = self.get_data_dict(0)
+        for kk, vv in data_dict.items():
+            if kk not in batch_data[0]:
+                continue
+            b_data["find_" + kk] = batch_data[0]["find_" + kk]
+            if not vv["atomic"]:
+                b_data[kk] = np.concatenate([bb[kk] for bb in batch_data], axis=0)
             else:
-                raise RuntimeError(
-                    "got wrong size of frame param, should be either %d x %d x %d or %d x %d or %d"
-                    % (nframes, natoms, fdim, natoms, fdim, fdim)
+                b_data[kk] = np.zeros(
+                    (len(batch_data), max_natoms * vv["ndof"] * vv["repeat"]),
+                    dtype=batch_data[0][kk].dtype,
                 )
+                for ii, bb in enumerate(batch_data):
+                    b_data[kk][ii, : bb[kk].shape[1]] = bb[kk][0]
+        return b_data
+
+    # ! altered by Marián Rynik
+    def get_test(self, sys_idx: Optional[int] = None, n_test: int = -1):  # depreciated
+        """Get test data from the the data systems.
 
-        # sort inputs
-        coords, atom_types, imap = self.sort_input(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        if self.has_efield:
-            efield = np.reshape(efield, [nframes, natoms, 3])
-            efield = efield[:, imap, :]
-            efield = np.reshape(efield, [nframes, natoms * 3])
-        if self.has_aparam:
-            aparam = np.reshape(aparam, [nframes, natoms, fdim])
-            aparam = aparam[:, imap, :]
-            aparam = np.reshape(aparam, [nframes, natoms * fdim])
-
-        # make natoms_vec and default_mesh
-        if self.neighbor_list is None:
-            natoms_vec = self.make_natoms_vec(atom_types, mixed_type=mixed_type)
-            assert natoms_vec[0] == natoms
-            mesh = make_default_mesh(pbc, mixed_type)
-            ghost_map = None
+        Parameters
+        ----------
+        sys_idx
+            The test dat of system with index `sys_idx` will be returned.
+            If is None, the currently selected system will be returned.
+        n_test
+            Number of test data. If set to -1 all test data will be get.
+        """
+        if not hasattr(self, "test_data"):
+            self._load_test(ntests=n_test)
+        if sys_idx is not None:
+            idx = sys_idx
+        else:
+            idx = self.pick_idx
+
+        test_system_data = {}
+        for nn in self.test_data:
+            test_system_data[nn] = self.test_data[nn][idx]
+        test_system_data["natoms_vec"] = self.natoms_vec[idx]
+        test_system_data["default_mesh"] = self.default_mesh[idx]
+        return test_system_data
+
+    def get_sys_ntest(self, sys_idx=None):
+        """Get number of tests for the currently selected system,
+        or one defined by sys_idx.
+        """
+        if sys_idx is not None:
+            return self.test_size[sys_idx]
         else:
-            if nframes > 1:
-                raise NotImplementedError(
-                    "neighbor_list does not support multiple frames"
-                )
-            (
-                natoms_vec,
-                coords,
-                atom_types,
-                mesh,
-                imap,
-                ghost_map,
-            ) = self.build_neighbor_list(
-                coords,
-                cells if cells is not None else None,
-                atom_types,
-                imap,
-                self.neighbor_list,
-            )
+            return self.test_size[self.pick_idx]
 
-        # evaluate
-        feed_dict_test = {}
-        feed_dict_test[self.t_natoms] = natoms_vec
-        if mixed_type:
-            feed_dict_test[self.t_type] = atom_types.reshape([-1])
-        else:
-            feed_dict_test[self.t_type] = np.tile(atom_types, [nframes, 1]).reshape(
-                [-1]
-            )
-        feed_dict_test[self.t_coord] = np.reshape(coords, [-1])
+    def get_type_map(self) -> List[str]:
+        """Get the type map."""
+        return self.type_map
 
-        if len(self.t_box.shape) == 1:
-            feed_dict_test[self.t_box] = np.reshape(cells, [-1])
-        elif len(self.t_box.shape) == 2:
-            feed_dict_test[self.t_box] = cells
-        else:
-            raise RuntimeError
-        if self.has_efield:
-            feed_dict_test[self.t_efield] = np.reshape(efield, [-1])
-        feed_dict_test[self.t_mesh] = mesh
-        if self.has_fparam:
-            feed_dict_test[self.t_fparam] = np.reshape(fparam, [-1])
-        if self.has_aparam:
-            feed_dict_test[self.t_aparam] = np.reshape(aparam, [-1])
-        return feed_dict_test, imap, natoms_vec, ghost_map
+    def get_nbatches(self) -> int:
+        """Get the total number of batches."""
+        return self.nbatches
 
-    def _eval_inner(
-        self,
-        coords,
-        cells,
-        atom_types,
-        fparam=None,
-        aparam=None,
-        atomic=False,
-        efield=None,
-        mixed_type=False,
-    ):
-        natoms, nframes = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        feed_dict_test, imap, natoms_vec, ghost_map = self._prepare_feed_dict(
-            coords, cells, atom_types, fparam, aparam, efield, mixed_type=mixed_type
-        )
+    def get_ntypes(self) -> int:
+        """Get the number of types."""
+        return self.sys_ntypes
 
-        nloc = natoms_vec[0]
-        nall = natoms_vec[1]
+    def get_nsystems(self) -> int:
+        """Get the number of data systems."""
+        return self.nsystems
+
+    def get_sys(self, idx: int) -> DeepmdData:
+        """Get a certain data system."""
+        return self.data_systems[idx]
+
+    def get_batch_size(self) -> int:
+        """Get the batch size."""
+        return self.batch_size
+
+    def print_summary(self, name: str):
+        print_summary(
+            name,
+            self.nsystems,
+            self.system_dirs,
+            self.natoms,
+            self.batch_size,
+            self.nbatches,
+            self.sys_probs,
+            [ii.pbc for ii in self.data_systems],
+        )
+
+    def _make_auto_bs(self, rule):
+        bs = []
+        for ii in self.data_systems:
+            ni = ii.get_natoms()
+            bsi = rule // ni
+            if bsi * ni < rule:
+                bsi += 1
+            bs.append(bsi)
+        return bs
+
+    # ! added by Marián Rynik
+    def _make_auto_ts(self, percent):
+        ts = []
+        for ii in range(self.nsystems):
+            ni = self.batch_size[ii] * self.nbatches[ii]
+            tsi = int(ni * percent / 100)
+            ts.append(tsi)
+
+        return ts
+
+    def _check_type_map_consistency(self, type_map_list):
+        ret = []
+        for ii in type_map_list:
+            if ii is not None:
+                min_len = min([len(ii), len(ret)])
+                for idx in range(min_len):
+                    if ii[idx] != ret[idx]:
+                        raise RuntimeError(f"inconsistent type map: {ret!s} {ii!s}")
+                if len(ii) > len(ret):
+                    ret = ii
+        return ret
+
+
+def _format_name_length(name, width):
+    if len(name) <= width:
+        return "{: >{}}".format(name, width)
+    else:
+        name = name[-(width - 3) :]
+        name = "-- " + name
+        return name
+
+
+def print_summary(
+    name: str,
+    nsystems: int,
+    system_dirs: List[str],
+    natoms: List[int],
+    batch_size: List[int],
+    nbatches: List[int],
+    sys_probs: List[float],
+    pbc: List[bool],
+):
+    """Print summary of systems.
 
-        t_out = [self.t_energy, self.t_force, self.t_virial]
-        if atomic:
-            t_out += [self.t_ae, self.t_av]
-
-        v_out = run_sess(self.sess, t_out, feed_dict=feed_dict_test)
-        energy = v_out[0]
-        force = v_out[1]
-        virial = v_out[2]
-        if atomic:
-            ae = v_out[3]
-            av = v_out[4]
-
-        if self.has_spin:
-            ntypes_real = self.ntypes - self.ntypes_spin
-            natoms_real = sum(
-                [
-                    np.count_nonzero(np.array(atom_types) == ii)
-                    for ii in range(ntypes_real)
-                ]
+    Parameters
+    ----------
+    name : str
+        The name of the system
+    nsystems : int
+        The number of systems
+    system_dirs : list of str
+        The directories of the systems
+    natoms : list of int
+        The number of atoms
+    batch_size : list of int
+        The batch size
+    nbatches : list of int
+        The number of batches
+    sys_probs : list of float
+        The probabilities
+    pbc : list of bool
+        The periodic boundary conditions
+    """
+    # width 65
+    sys_width = 42
+    log.info(
+        f"---Summary of DataSystem: {name:13s}-----------------------------------------------"
+    )
+    log.info("found %d system(s):" % nsystems)
+    log.info(
+        ("%s  " % _format_name_length("system", sys_width))
+        + ("%6s  %6s  %6s  %9s  %3s" % ("natoms", "bch_sz", "n_bch", "prob", "pbc"))
+    )
+    for ii in range(nsystems):
+        log.info(
+            "%s  %6d  %6d  %6d  %9.3e  %3s"
+            % (
+                _format_name_length(system_dirs[ii], sys_width),
+                natoms[ii],
+                # TODO batch size * nbatches = number of structures
+                batch_size[ii],
+                nbatches[ii],
+                sys_probs[ii],
+                "T" if pbc[ii] else "F",
             )
-        else:
-            natoms_real = natoms
-        if ghost_map is not None:
-            # add the value of ghost atoms to real atoms
-            force = np.reshape(force, [nframes, -1, 3])
-            np.add.at(force[0], ghost_map, force[0, nloc:])
-            if atomic:
-                av = np.reshape(av, [nframes, -1, 9])
-                np.add.at(av[0], ghost_map, av[0, nloc:])
-
-        # reverse map of the outputs
-        force = self.reverse_map(np.reshape(force, [nframes, -1, 3]), imap)
-        if atomic:
-            ae = self.reverse_map(np.reshape(ae, [nframes, -1, 1]), imap[:natoms_real])
-            av = self.reverse_map(np.reshape(av, [nframes, -1, 9]), imap)
-
-        energy = np.reshape(energy, [nframes, 1])
-        force = np.reshape(force, [nframes, nall, 3])
-        if nloc < nall:
-            force = force[:, :nloc, :]
-        virial = np.reshape(virial, [nframes, 9])
-        if atomic:
-            ae = np.reshape(ae, [nframes, natoms_real, 1])
-            av = np.reshape(av, [nframes, nall, 9])
-            if nloc < nall:
-                av = av[:, :nloc, :]
-            return energy, force, virial, ae, av
-        else:
-            return energy, force, virial
+        )
+    log.info(
+        "--------------------------------------------------------------------------------------"
+    )
 
-    def eval_descriptor(
-        self,
-        coords: np.ndarray,
-        cells: np.ndarray,
-        atom_types: List[int],
-        fparam: Optional[np.ndarray] = None,
-        aparam: Optional[np.ndarray] = None,
-        efield: Optional[np.ndarray] = None,
-        mixed_type: bool = False,
-    ) -> np.array:
-        """Evaluate descriptors by using this DP.
 
-        Parameters
-        ----------
-        coords
-            The coordinates of atoms.
-            The array should be of size nframes x natoms x 3
-        cells
-            The cell of the region.
-            If None then non-PBC is assumed, otherwise using PBC.
-            The array should be of size nframes x 9
-        atom_types
-            The atom types
-            The list should contain natoms ints
-        fparam
-            The frame parameter.
-            The array can be of size :
-            - nframes x dim_fparam.
-            - dim_fparam. Then all frames are assumed to be provided with the same fparam.
-        aparam
-            The atomic parameter
-            The array can be of size :
-            - nframes x natoms x dim_aparam.
-            - natoms x dim_aparam. Then all frames are assumed to be provided with the same aparam.
-            - dim_aparam. Then all frames and atoms are provided with the same aparam.
-        efield
-            The external field on atoms.
-            The array should be of size nframes x natoms x 3
-        mixed_type
-            Whether to perform the mixed_type mode.
-            If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
-            in which frames in a system may have different natoms_vec(s), with the same nloc.
+def process_sys_probs(sys_probs, nbatch):
+    sys_probs = np.array(sys_probs)
+    type_filter = sys_probs >= 0
+    assigned_sum_prob = np.sum(type_filter * sys_probs)
+    # 1e-8 is to handle floating point error; See #1917
+    assert (
+        assigned_sum_prob <= 1.0 + 1e-8
+    ), "the sum of assigned probability should be less than 1"
+    rest_sum_prob = 1.0 - assigned_sum_prob
+    if not np.isclose(rest_sum_prob, 0):
+        rest_nbatch = (1 - type_filter) * nbatch
+        rest_prob = rest_sum_prob * rest_nbatch / np.sum(rest_nbatch)
+        ret_prob = rest_prob + type_filter * sys_probs
+    else:
+        ret_prob = sys_probs
+    assert np.isclose(np.sum(ret_prob), 1), "sum of probs should be 1"
+    return ret_prob
+
+
+def prob_sys_size_ext(keywords, nsystems, nbatch):
+    block_str = keywords.split(";")[1:]
+    block_stt = []
+    block_end = []
+    block_weights = []
+    for ii in block_str:
+        stt = int(ii.split(":")[0])
+        end = int(ii.split(":")[1])
+        weight = float(ii.split(":")[2])
+        assert weight >= 0, "the weight of a block should be no less than 0"
+        block_stt.append(stt)
+        block_end.append(end)
+        block_weights.append(weight)
+    nblocks = len(block_str)
+    block_probs = np.array(block_weights) / np.sum(block_weights)
+    sys_probs = np.zeros([nsystems])
+    for ii in range(nblocks):
+        nbatch_block = nbatch[block_stt[ii] : block_end[ii]]
+        tmp_prob = [float(i) for i in nbatch_block] / np.sum(nbatch_block)
+        sys_probs[block_stt[ii] : block_end[ii]] = tmp_prob * block_probs[ii]
+    return sys_probs
 
-        Returns
-        -------
-        descriptor
-            Descriptors.
-        """
-        natoms, numb_test = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        descriptor = self._eval_func(self._eval_descriptor_inner, numb_test, natoms)(
-            coords,
-            cells,
-            atom_types,
-            fparam=fparam,
-            aparam=aparam,
-            efield=efield,
-            mixed_type=mixed_type,
-        )
-        return descriptor
 
-    def _eval_descriptor_inner(
-        self,
-        coords: np.ndarray,
-        cells: np.ndarray,
-        atom_types: List[int],
-        fparam: Optional[np.ndarray] = None,
-        aparam: Optional[np.ndarray] = None,
-        efield: Optional[np.ndarray] = None,
-        mixed_type: bool = False,
-    ) -> np.array:
-        natoms, nframes = self._get_natoms_and_nframes(
-            coords, atom_types, mixed_type=mixed_type
-        )
-        feed_dict_test, imap, natoms_vec, ghost_map = self._prepare_feed_dict(
-            coords, cells, atom_types, fparam, aparam, efield, mixed_type=mixed_type
-        )
-        (descriptor,) = run_sess(
-            self.sess, [self.t_descriptor], feed_dict=feed_dict_test
-        )
-        imap = imap[:natoms]
-        return self.reverse_map(np.reshape(descriptor, [nframes, natoms, -1]), imap)
+def process_systems(systems: Union[str, List[str]]) -> List[str]:
+    """Process the user-input systems.
+
+    If it is a single directory, search for all the systems in the directory.
+    Check if the systems are valid.
+
+    Parameters
+    ----------
+    systems : str or list of str
+        The user-input systems
+
+    Returns
+    -------
+    list of str
+        The valid systems
+    """
+    if isinstance(systems, str):
+        systems = expand_sys_str(systems)
+    elif isinstance(systems, list):
+        systems = systems.copy()
+    help_msg = "Please check your setting for data systems"
+    # check length of systems
+    if len(systems) == 0:
+        msg = "cannot find valid a data system"
+        log.fatal(msg)
+        raise OSError(msg, help_msg)
+    # rougly check all items in systems are valid
+    for ii in systems:
+        ii = DPPath(ii)
+        if not ii.is_dir():
+            msg = f"dir {ii} is not a valid dir"
+            log.fatal(msg)
+            raise OSError(msg, help_msg)
+        if not (ii / "type.raw").is_file():
+            msg = f"dir {ii} is not a valid data system dir"
+            log.fatal(msg)
+            raise OSError(msg, help_msg)
+    return systems
+
+
+def get_data(
+    jdata: Dict[str, Any], rcut, type_map, modifier, multi_task_mode=False
+) -> DeepmdDataSystem:
+    """Get the data system.
+
+    Parameters
+    ----------
+    jdata
+        The json data
+    rcut
+        The cut-off radius, not used
+    type_map
+        The type map
+    modifier
+        The data modifier
+    multi_task_mode
+        If in multi task mode
+
+    Returns
+    -------
+    DeepmdDataSystem
+        The data system
+    """
+    systems = j_must_have(jdata, "systems")
+    systems = process_systems(systems)
+
+    batch_size = j_must_have(jdata, "batch_size")
+    sys_probs = jdata.get("sys_probs", None)
+    auto_prob = jdata.get("auto_prob", "prob_sys_size")
+    optional_type_map = not multi_task_mode
+
+    data = DeepmdDataSystem(
+        systems=systems,
+        batch_size=batch_size,
+        test_size=1,  # to satisfy the old api
+        shuffle_test=True,  # to satisfy the old api
+        rcut=rcut,
+        type_map=type_map,
+        optional_type_map=optional_type_map,
+        modifier=modifier,
+        trn_all_set=True,  # sample from all sets
+        sys_probs=sys_probs,
+        auto_prob_style=auto_prob,
+    )
+    data.add_dict(data_requirement)
+
+    return data
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/deep_tensor.py` & `deepmd_kit-3.0.0a0/deepmd/pt/model/model/make_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,446 +1,385 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
-    TYPE_CHECKING,
-    ClassVar,
     Dict,
     List,
     Optional,
     Tuple,
 )
 
-import numpy as np
+import torch
 
-from deepmd.common import (
-    make_default_mesh,
+from deepmd.dpmodel import (
+    ModelOutputDef,
 )
-from deepmd.infer.deep_eval import (
-    DeepEval,
+from deepmd.dpmodel.output_def import (
+    OutputVariableCategory,
+    OutputVariableOperation,
+    check_operation_applied,
 )
-from deepmd.utils.sess import (
-    run_sess,
+from deepmd.pt.model.model.transform_output import (
+    communicate_extended_output,
+    fit_output_to_model_output,
 )
+from deepmd.pt.utils.env import (
+    GLOBAL_PT_ENER_FLOAT_PRECISION,
+    GLOBAL_PT_FLOAT_PRECISION,
+    PRECISION_DICT,
+    RESERVED_PRECISON_DICT,
+)
+from deepmd.pt.utils.nlist import (
+    extend_input_and_build_neighbor_list,
+    nlist_distinguish_types,
+)
+
+
+def make_model(T_AtomicModel):
+    """Make a model as a derived class of an atomic model.
 
-if TYPE_CHECKING:
-    from pathlib import (
-        Path,
-    )
+    The model provide two interfaces.
 
+    1. the `forward_common_lower`, that takes extended coordinates, atyps and neighbor list,
+    and outputs the atomic and property and derivatives (if required) on the extended region.
 
-class DeepTensor(DeepEval):
-    """Evaluates a tensor model.
+    2. the `forward_common`, that takes coordinates, atypes and cell and predicts
+    the atomic and reduced property, and derivatives (if required) on the local region.
 
     Parameters
     ----------
-    model_file: str
-        The name of the frozen model file.
-    load_prefix: str
-        The prefix in the load computational graph
-    default_tf_graph : bool
-        If uses the default tf graph, otherwise build a new tf graph for evaluation
-    input_map : dict, optional
-        The input map for tf.import_graph_def. Only work with default tf graph
-    neighbor_list : ase.neighborlist.NeighborList, optional
-        The neighbor list object. If None, then build the native neighbor list.
+    T_AtomicModel
+        The atomic model.
+
+    Returns
+    -------
+    CM
+        The model.
+
     """
 
-    tensors: ClassVar[Dict[str, str]] = {
-        # descriptor attrs
-        "t_ntypes": "descrpt_attr/ntypes:0",
-        "t_rcut": "descrpt_attr/rcut:0",
-        # model attrs
-        "t_tmap": "model_attr/tmap:0",
-        "t_sel_type": "model_attr/sel_type:0",
-        "t_ouput_dim": "model_attr/output_dim:0",
-        # inputs
-        "t_coord": "t_coord:0",
-        "t_type": "t_type:0",
-        "t_natoms": "t_natoms:0",
-        "t_box": "t_box:0",
-        "t_mesh": "t_mesh:0",
-    }
-
-    def __init__(
-        self,
-        model_file: "Path",
-        load_prefix: str = "load",
-        default_tf_graph: bool = False,
-        input_map: Optional[dict] = None,
-        neighbor_list=None,
-    ) -> None:
-        """Constructor."""
-        DeepEval.__init__(
+    class CM(T_AtomicModel):
+        def __init__(
             self,
-            model_file,
-            load_prefix=load_prefix,
-            default_tf_graph=default_tf_graph,
-            input_map=input_map,
-            neighbor_list=neighbor_list,
-        )
-        # check model type
-        model_type = self.tensors["t_tensor"][2:-2]
-        assert (
-            self.model_type == model_type
-        ), f"expect {model_type} model but got {self.model_type}"
-
-        # now load tensors to object attributes
-        for attr_name, tensor_name in self.tensors.items():
-            self._get_tensor(tensor_name, attr_name)
-
-        # load optional tensors if possible
-        optional_tensors = {
-            "t_global_tensor": f"o_global_{model_type}:0",
-            "t_force": "o_force:0",
-            "t_virial": "o_virial:0",
-            "t_atom_virial": "o_atom_virial:0",
-        }
-        try:
-            # first make sure these tensor all exists (but do not modify self attr)
-            for attr_name, tensor_name in optional_tensors.items():
-                self._get_tensor(tensor_name)
-            # then put those into self.attrs
-            for attr_name, tensor_name in optional_tensors.items():
-                self._get_tensor(tensor_name, attr_name)
-        except KeyError:
-            self._support_gfv = False
-        else:
-            self.tensors.update(optional_tensors)
-            self._support_gfv = True
-
-        self._run_default_sess()
-        self.tmap = self.tmap.decode("UTF-8").split()
-
-    def _run_default_sess(self):
-        [self.ntypes, self.rcut, self.tmap, self.tselt, self.output_dim] = run_sess(
-            self.sess,
-            [
-                self.t_ntypes,
-                self.t_rcut,
-                self.t_tmap,
-                self.t_sel_type,
-                self.t_ouput_dim,
-            ],
-        )
-
-    def get_ntypes(self) -> int:
-        """Get the number of atom types of this model."""
-        return self.ntypes
-
-    def get_rcut(self) -> float:
-        """Get the cut-off radius of this model."""
-        return self.rcut
-
-    def get_type_map(self) -> List[str]:
-        """Get the type map (element name of the atom types) of this model."""
-        return self.tmap
-
-    def get_sel_type(self) -> List[int]:
-        """Get the selected atom types of this model."""
-        return self.tselt
-
-    def get_dim_fparam(self) -> int:
-        """Get the number (dimension) of frame parameters of this DP."""
-        return self.dfparam
-
-    def get_dim_aparam(self) -> int:
-        """Get the number (dimension) of atomic parameters of this DP."""
-        return self.daparam
-
-    def eval(
-        self,
-        coords: np.ndarray,
-        cells: np.ndarray,
-        atom_types: List[int],
-        atomic: bool = True,
-        fparam: Optional[np.ndarray] = None,
-        aparam: Optional[np.ndarray] = None,
-        efield: Optional[np.ndarray] = None,
-        mixed_type: bool = False,
-    ) -> np.ndarray:
-        """Evaluate the model.
-
-        Parameters
-        ----------
-        coords
-            The coordinates of atoms.
-            The array should be of size nframes x natoms x 3
-        cells
-            The cell of the region.
-            If None then non-PBC is assumed, otherwise using PBC.
-            The array should be of size nframes x 9
-        atom_types
-            The atom types
-            The list should contain natoms ints
-        atomic
-            If True (default), return the atomic tensor
-            Otherwise return the global tensor
-        fparam
-            Not used in this model
-        aparam
-            Not used in this model
-        efield
-            Not used in this model
-        mixed_type
-            Whether to perform the mixed_type mode.
-            If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
-            in which frames in a system may have different natoms_vec(s), with the same nloc.
-
-        Returns
-        -------
-        tensor
-            The returned tensor
-            If atomic == False then of size nframes x output_dim
-            else of size nframes x natoms x output_dim
-        """
-        # standarize the shape of inputs
-        if mixed_type:
-            natoms = atom_types[0].size
-            atom_types = np.array(atom_types, dtype=int).reshape([-1, natoms])
-        else:
-            atom_types = np.array(atom_types, dtype=int).reshape([-1])
-            natoms = atom_types.size
-        coords = np.reshape(np.array(coords), [-1, natoms * 3])
-        nframes = coords.shape[0]
-        if cells is None:
-            pbc = False
-            cells = np.tile(np.eye(3), [nframes, 1]).reshape([nframes, 9])
-        else:
-            pbc = True
-            cells = np.array(cells).reshape([nframes, 9])
-
-        # sort inputs
-        coords, atom_types, imap, sel_at, sel_imap = self.sort_input(
-            coords, atom_types, sel_atoms=self.get_sel_type(), mixed_type=mixed_type
-        )
-
-        # make natoms_vec and default_mesh
-        if self.neighbor_list is None:
-            natoms_vec = self.make_natoms_vec(atom_types, mixed_type=mixed_type)
-            assert natoms_vec[0] == natoms
-            mesh = make_default_mesh(pbc, mixed_type)
-        else:
-            if nframes > 1:
-                raise NotImplementedError(
-                    "neighbor_list does not support multiple frames"
-                )
-            (
-                natoms_vec,
-                coords,
-                atom_types,
-                mesh,
-                imap,
-                _,
-            ) = self.build_neighbor_list(
-                coords,
-                cells if cells is not None else None,
-                atom_types,
-                imap,
-                self.neighbor_list,
+            *args,
+            **kwargs,
+        ):
+            super().__init__(
+                *args,
+                **kwargs,
             )
+            self.precision_dict = PRECISION_DICT
+            self.reverse_precision_dict = RESERVED_PRECISON_DICT
+            self.global_pt_float_precision = GLOBAL_PT_FLOAT_PRECISION
+            self.global_pt_ener_float_precision = GLOBAL_PT_ENER_FLOAT_PRECISION
+
+        def model_output_def(self):
+            """Get the output def for the model."""
+            return ModelOutputDef(self.atomic_output_def())
+
+        @torch.jit.export
+        def model_output_type(self) -> List[str]:
+            """Get the output type for the model."""
+            output_def = self.model_output_def()
+            var_defs = output_def.var_defs
+            # jit: Comprehension ifs are not supported yet
+            # type hint is critical for JIT
+            vars: List[str] = []
+            for kk, vv in var_defs.items():
+                # .value is critical for JIT
+                if vv.category == OutputVariableCategory.OUT.value:
+                    vars.append(kk)
+            return vars
 
-        # evaluate
-        feed_dict_test = {}
-        feed_dict_test[self.t_natoms] = natoms_vec
-        if mixed_type:
-            feed_dict_test[self.t_type] = atom_types.reshape([-1])
-        else:
-            feed_dict_test[self.t_type] = np.tile(atom_types, [nframes, 1]).reshape(
-                [-1]
-            )
-        feed_dict_test[self.t_coord] = np.reshape(coords, [-1])
-        feed_dict_test[self.t_box] = np.reshape(cells, [-1])
-        feed_dict_test[self.t_mesh] = mesh
-
-        if atomic:
-            assert (
-                "global" not in self.model_type
-            ), f"cannot do atomic evaluation with model type {self.model_type}"
-            t_out = [self.t_tensor]
-        else:
-            assert (
-                self._support_gfv or "global" in self.model_type
-            ), f"do not support global tensor evaluation with old {self.model_type} model"
-            t_out = [self.t_global_tensor if self._support_gfv else self.t_tensor]
-        v_out = self.sess.run(t_out, feed_dict=feed_dict_test)
-        tensor = v_out[0]
-
-        # reverse map of the outputs
-        if atomic:
-            tensor = np.array(tensor)
-            tensor = self.reverse_map(
-                np.reshape(tensor, [nframes, -1, self.output_dim]), sel_imap
+        # cannot use the name forward. torch script does not work
+        def forward_common(
+            self,
+            coord,
+            atype,
+            box: Optional[torch.Tensor] = None,
+            fparam: Optional[torch.Tensor] = None,
+            aparam: Optional[torch.Tensor] = None,
+            do_atomic_virial: bool = False,
+        ) -> Dict[str, torch.Tensor]:
+            """Return model prediction.
+
+            Parameters
+            ----------
+            coord
+                The coordinates of the atoms.
+                shape: nf x (nloc x 3)
+            atype
+                The type of atoms. shape: nf x nloc
+            box
+                The simulation box. shape: nf x 9
+            fparam
+                frame parameter. nf x ndf
+            aparam
+                atomic parameter. nf x nloc x nda
+            do_atomic_virial
+                If calculate the atomic virial.
+
+            Returns
+            -------
+            ret_dict
+                The result dict of type Dict[str,torch.Tensor].
+                The keys are defined by the `ModelOutputDef`.
+
+            """
+            cc, bb, fp, ap, input_prec = self.input_type_cast(
+                coord, box=box, fparam=fparam, aparam=aparam
             )
-            tensor = np.reshape(tensor, [nframes, len(sel_at), self.output_dim])
-        else:
-            tensor = np.reshape(tensor, [nframes, self.output_dim])
-
-        return tensor
-
-    def eval_full(
-        self,
-        coords: np.ndarray,
-        cells: np.ndarray,
-        atom_types: List[int],
-        atomic: bool = False,
-        fparam: Optional[np.array] = None,
-        aparam: Optional[np.array] = None,
-        efield: Optional[np.array] = None,
-        mixed_type: bool = False,
-    ) -> Tuple[np.ndarray, ...]:
-        """Evaluate the model with interface similar to the energy model.
-        Will return global tensor, component-wise force and virial
-        and optionally atomic tensor and atomic virial.
-
-        Parameters
-        ----------
-        coords
-            The coordinates of atoms.
-            The array should be of size nframes x natoms x 3
-        cells
-            The cell of the region.
-            If None then non-PBC is assumed, otherwise using PBC.
-            The array should be of size nframes x 9
-        atom_types
-            The atom types
-            The list should contain natoms ints
-        atomic
-            Whether to calculate atomic tensor and virial
-        fparam
-            Not used in this model
-        aparam
-            Not used in this model
-        efield
-            Not used in this model
-        mixed_type
-            Whether to perform the mixed_type mode.
-            If True, the input data has the mixed_type format (see doc/model/train_se_atten.md),
-            in which frames in a system may have different natoms_vec(s), with the same nloc.
-
-        Returns
-        -------
-        tensor
-            The global tensor.
-            shape: [nframes x nout]
-        force
-            The component-wise force (negative derivative) on each atom.
-            shape: [nframes x nout x natoms x 3]
-        virial
-            The component-wise virial of the tensor.
-            shape: [nframes x nout x 9]
-        atom_tensor
-            The atomic tensor. Only returned when atomic == True
-            shape: [nframes x natoms x nout]
-        atom_virial
-            The atomic virial. Only returned when atomic == True
-            shape: [nframes x nout x natoms x 9]
-        """
-        assert self._support_gfv, "do not support eval_full with old tensor model"
-
-        # standarize the shape of inputs
-        if mixed_type:
-            natoms = atom_types[0].size
-            atom_types = np.array(atom_types, dtype=int).reshape([-1, natoms])
-        else:
-            atom_types = np.array(atom_types, dtype=int).reshape([-1])
-            natoms = atom_types.size
-        coords = np.reshape(np.array(coords), [-1, natoms * 3])
-        nframes = coords.shape[0]
-        if cells is None:
-            pbc = False
-            cells = np.tile(np.eye(3), [nframes, 1]).reshape([nframes, 9])
-        else:
-            pbc = True
-            cells = np.array(cells).reshape([nframes, 9])
-        nout = self.output_dim
-
-        # sort inputs
-        coords, atom_types, imap, sel_at, sel_imap = self.sort_input(
-            coords, atom_types, sel_atoms=self.get_sel_type(), mixed_type=mixed_type
-        )
-
-        # make natoms_vec and default_mesh
-        if self.neighbor_list is None:
-            natoms_vec = self.make_natoms_vec(atom_types, mixed_type=mixed_type)
-            assert natoms_vec[0] == natoms
-            mesh = make_default_mesh(pbc, mixed_type)
-            ghost_map = None
-        else:
-            if nframes > 1:
-                raise NotImplementedError(
-                    "neighbor_list does not support multiple frames"
-                )
+            del coord, box, fparam, aparam
             (
-                natoms_vec,
-                coords,
-                atom_types,
-                mesh,
-                imap,
-                ghost_map,
-            ) = self.build_neighbor_list(
-                coords,
-                cells if cells is not None else None,
-                atom_types,
-                imap,
-                self.neighbor_list,
+                extended_coord,
+                extended_atype,
+                mapping,
+                nlist,
+            ) = extend_input_and_build_neighbor_list(
+                cc,
+                atype,
+                self.get_rcut(),
+                self.get_sel(),
+                mixed_types=self.mixed_types(),
+                box=bb,
+            )
+            model_predict_lower = self.forward_common_lower(
+                extended_coord,
+                extended_atype,
+                nlist,
+                mapping,
+                do_atomic_virial=do_atomic_virial,
+                fparam=fp,
+                aparam=ap,
+            )
+            model_predict = communicate_extended_output(
+                model_predict_lower,
+                self.model_output_def(),
+                mapping,
+                do_atomic_virial=do_atomic_virial,
             )
+            model_predict = self.output_type_cast(model_predict, input_prec)
+            return model_predict
 
-        # evaluate
-        feed_dict_test = {}
-        feed_dict_test[self.t_natoms] = natoms_vec
-        if mixed_type:
-            feed_dict_test[self.t_type] = atom_types.reshape([-1])
-        else:
-            feed_dict_test[self.t_type] = np.tile(atom_types, [nframes, 1]).reshape(
-                [-1]
+        def forward_common_lower(
+            self,
+            extended_coord,
+            extended_atype,
+            nlist,
+            mapping: Optional[torch.Tensor] = None,
+            fparam: Optional[torch.Tensor] = None,
+            aparam: Optional[torch.Tensor] = None,
+            do_atomic_virial: bool = False,
+        ):
+            """Return model prediction. Lower interface that takes
+            extended atomic coordinates and types, nlist, and mapping
+            as input, and returns the predictions on the extended region.
+            The predictions are not reduced.
+
+            Parameters
+            ----------
+            extended_coord
+                coodinates in extended region. nf x (nall x 3)
+            extended_atype
+                atomic type in extended region. nf x nall
+            nlist
+                neighbor list. nf x nloc x nsel.
+            mapping
+                mapps the extended indices to local indices. nf x nall.
+            fparam
+                frame parameter. nf x ndf
+            aparam
+                atomic parameter. nf x nloc x nda
+            do_atomic_virial
+                whether calculate atomic virial.
+
+            Returns
+            -------
+            result_dict
+                the result dict, defined by the `FittingOutputDef`.
+
+            """
+            nframes, nall = extended_atype.shape[:2]
+            extended_coord = extended_coord.view(nframes, -1, 3)
+            nlist = self.format_nlist(extended_coord, extended_atype, nlist)
+            cc_ext, _, fp, ap, input_prec = self.input_type_cast(
+                extended_coord, fparam=fparam, aparam=aparam
+            )
+            del extended_coord, fparam, aparam
+            atomic_ret = self.forward_common_atomic(
+                cc_ext,
+                extended_atype,
+                nlist,
+                mapping=mapping,
+                fparam=fp,
+                aparam=ap,
             )
-        feed_dict_test[self.t_coord] = np.reshape(coords, [-1])
-        feed_dict_test[self.t_box] = np.reshape(cells, [-1])
-        feed_dict_test[self.t_mesh] = mesh
-
-        t_out = [self.t_global_tensor, self.t_force, self.t_virial]
-        if atomic:
-            t_out += [self.t_tensor, self.t_atom_virial]
-
-        v_out = self.sess.run(t_out, feed_dict=feed_dict_test)
-        gt = v_out[0]  # global tensor
-        force = v_out[1]
-        virial = v_out[2]
-        if atomic:
-            at = v_out[3]  # atom tensor
-            av = v_out[4]  # atom virial
-
-        nloc = natoms_vec[0]
-        nall = natoms_vec[1]
-
-        if ghost_map is not None:
-            # add the value of ghost atoms to real atoms
-            force = np.reshape(force, [nframes * nout, -1, 3])
-            # TODO: is there some way not to use for loop?
-            for ii in range(nframes * nout):
-                np.add.at(force[ii], ghost_map, force[ii, nloc:])
-            if atomic:
-                av = np.reshape(av, [nframes * nout, -1, 9])
-                for ii in range(nframes * nout):
-                    np.add.at(av[ii], ghost_map, av[ii, nloc:])
-
-        # please note here the shape are wrong!
-        force = self.reverse_map(np.reshape(force, [nframes * nout, nall, 3]), imap)
-        if atomic:
-            at = self.reverse_map(
-                np.reshape(at, [nframes, len(sel_at), nout]), sel_imap
+            model_predict = fit_output_to_model_output(
+                atomic_ret,
+                self.atomic_output_def(),
+                cc_ext,
+                do_atomic_virial=do_atomic_virial,
             )
-            av = self.reverse_map(np.reshape(av, [nframes * nout, nall, 9]), imap)
+            model_predict = self.output_type_cast(model_predict, input_prec)
+            return model_predict
+
+        def input_type_cast(
+            self,
+            coord: torch.Tensor,
+            box: Optional[torch.Tensor] = None,
+            fparam: Optional[torch.Tensor] = None,
+            aparam: Optional[torch.Tensor] = None,
+        ) -> Tuple[
+            torch.Tensor,
+            Optional[torch.Tensor],
+            Optional[torch.Tensor],
+            Optional[torch.Tensor],
+            str,
+        ]:
+            """Cast the input data to global float type."""
+            input_prec = self.reverse_precision_dict[coord.dtype]
+            ###
+            ### type checking would not pass jit, convert to coord prec anyway
+            ###
+            # for vv, kk in zip([fparam, aparam], ["frame", "atomic"]):
+            #     if vv is not None and self.reverse_precision_dict[vv.dtype] != input_prec:
+            #         log.warning(
+            #           f"type of {kk} parameter {self.reverse_precision_dict[vv.dtype]}"
+            #           " does not match"
+            #           f" that of the coordinate {input_prec}"
+            #         )
+            _lst: List[Optional[torch.Tensor]] = [
+                vv.to(coord.dtype) if vv is not None else None
+                for vv in [box, fparam, aparam]
+            ]
+            box, fparam, aparam = _lst
+            if (
+                input_prec
+                == self.reverse_precision_dict[self.global_pt_float_precision]
+            ):
+                return coord, box, fparam, aparam, input_prec
+            else:
+                pp = self.global_pt_float_precision
+                return (
+                    coord.to(pp),
+                    box.to(pp) if box is not None else None,
+                    fparam.to(pp) if fparam is not None else None,
+                    aparam.to(pp) if aparam is not None else None,
+                    input_prec,
+                )
+
+        def output_type_cast(
+            self,
+            model_ret: Dict[str, torch.Tensor],
+            input_prec: str,
+        ) -> Dict[str, torch.Tensor]:
+            """Convert the model output to the input prec."""
+            do_cast = (
+                input_prec
+                != self.reverse_precision_dict[self.global_pt_float_precision]
+            )
+            pp = self.precision_dict[input_prec]
+            odef = self.model_output_def()
+            for kk in odef.keys():
+                if kk not in model_ret.keys():
+                    # do not return energy_derv_c if not do_atomic_virial
+                    continue
+                if check_operation_applied(odef[kk], OutputVariableOperation.REDU):
+                    model_ret[kk] = (
+                        model_ret[kk].to(self.global_pt_ener_float_precision)
+                        if model_ret[kk] is not None
+                        else None
+                    )
+                elif do_cast:
+                    model_ret[kk] = (
+                        model_ret[kk].to(pp) if model_ret[kk] is not None else None
+                    )
+            return model_ret
+
+        def format_nlist(
+            self,
+            extended_coord: torch.Tensor,
+            extended_atype: torch.Tensor,
+            nlist: torch.Tensor,
+        ):
+            """Format the neighbor list.
+
+            1. If the number of neighbors in the `nlist` is equal to sum(self.sel),
+            it does nothong
+
+            2. If the number of neighbors in the `nlist` is smaller than sum(self.sel),
+            the `nlist` is pad with -1.
+
+            3. If the number of neighbors in the `nlist` is larger than sum(self.sel),
+            the nearest sum(sel) neighbors will be preseved.
+
+            Known limitations:
+
+            In the case of not self.mixed_types, the nlist is always formatted.
+            May have side effact on the efficiency.
+
+            Parameters
+            ----------
+            extended_coord
+                coodinates in extended region. nf x nall x 3
+            extended_atype
+                atomic type in extended region. nf x nall
+            nlist
+                neighbor list. nf x nloc x nsel
+
+            Returns
+            -------
+            formated_nlist
+                the formated nlist.
+
+            """
+            mixed_types = self.mixed_types()
+            nlist = self._format_nlist(extended_coord, nlist, sum(self.get_sel()))
+            if not mixed_types:
+                nlist = nlist_distinguish_types(nlist, extended_atype, self.get_sel())
+            return nlist
+
+        def _format_nlist(
+            self,
+            extended_coord: torch.Tensor,
+            nlist: torch.Tensor,
+            nnei: int,
+        ):
+            n_nf, n_nloc, n_nnei = nlist.shape
+            # nf x nall x 3
+            extended_coord = extended_coord.view([n_nf, -1, 3])
+            rcut = self.get_rcut()
+
+            if n_nnei < nnei:
+                nlist = torch.cat(
+                    [
+                        nlist,
+                        -1
+                        * torch.ones(
+                            [n_nf, n_nloc, nnei - n_nnei],
+                            dtype=nlist.dtype,
+                            device=nlist.device,
+                        ),
+                    ],
+                    dim=-1,
+                )
+            elif n_nnei > nnei:
+                m_real_nei = nlist >= 0
+                nlist = torch.where(m_real_nei, nlist, 0)
+                # nf x nloc x 3
+                coord0 = extended_coord[:, :n_nloc, :]
+                # nf x (nloc x nnei) x 3
+                index = nlist.view(n_nf, n_nloc * n_nnei, 1).expand(-1, -1, 3)
+                coord1 = torch.gather(extended_coord, 1, index)
+                # nf x nloc x nnei x 3
+                coord1 = coord1.view(n_nf, n_nloc, n_nnei, 3)
+                # nf x nloc x nnei
+                rr = torch.linalg.norm(coord0[:, :, None, :] - coord1, dim=-1)
+                rr = torch.where(m_real_nei, rr, float("inf"))
+                rr, nlist_mapping = torch.sort(rr, dim=-1)
+                nlist = torch.gather(nlist, 2, nlist_mapping)
+                nlist = torch.where(rr > rcut, -1, nlist)
+                nlist = nlist[..., :nnei]
+            else:  # n_nnei == nnei:
+                pass  # great!
+            assert nlist.shape[-1] == nnei
+            return nlist
 
-        # make sure the shapes are correct here
-        gt = np.reshape(gt, [nframes, nout])
-        force = np.reshape(force, [nframes, nout, nall, 3])
-        if nloc < nall:
-            force = force[:, :, :nloc, :]
-        virial = np.reshape(virial, [nframes, nout, 9])
-        if atomic:
-            at = np.reshape(at, [nframes, len(sel_at), self.output_dim])
-            av = np.reshape(av, [nframes, nout, nall, 9])
-            if nloc < nall:
-                av = av[:, :, :nloc, :]
-            return gt, force, virial, at, av
-        else:
-            return gt, force, virial
+    return CM
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/ewald_recp.py` & `deepmd_kit-3.0.0a0/deepmd/tf/infer/ewald_recp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     default_tf_session_config,
     op_module,
     tf,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 
 class EwaldRecp:
     """Evaluate the reciprocal part of the Ewald sum."""
```

### Comparing `deepmd_kit-2.2.9/deepmd/infer/model_devi.py` & `deepmd_kit-3.0.0a0/deepmd/infer/model_devi.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,20 @@
 )
 
 import numpy as np
 
 from deepmd.common import (
     expand_sys_str,
 )
-
-from ..utils.batch_size import (
-    AutoBatchSize,
+from deepmd.infer.deep_pot import (
+    DeepPot,
 )
-from ..utils.data import (
+from deepmd.utils.data import (
     DeepmdData,
 )
-from .deep_pot import (
-    DeepPot,
-)
 
 try:
     from typing import Literal  # python >=3.8
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
 
@@ -293,20 +289,20 @@
     -------
     model_devi : numpy.ndarray, `n_frames x 8`
         Model deviation results. The first column is index of steps, the other 7 columns are
         max_devi_v, min_devi_v, avg_devi_v, max_devi_f, min_devi_f, avg_devi_f, devi_e.
 
     Examples
     --------
-    >>> from deepmd.infer import calc_model_devi
-    >>> from deepmd.infer import DeepPot as DP
+    >>> from deepmd.tf.infer import calc_model_devi
+    >>> from deepmd.tf.infer import DeepPot as DP
     >>> import numpy as np
-    >>> coord = np.array([[1,0,0], [0,0,1.5], [1,0,3]]).reshape([1, -1])
+    >>> coord = np.array([[1, 0, 0], [0, 0, 1.5], [1, 0, 3]]).reshape([1, -1])
     >>> cell = np.diag(10 * np.ones(3)).reshape([1, -1])
-    >>> atype = [1,0,1]
+    >>> atype = [1, 0, 1]
     >>> graphs = [DP("graph.000.pb"), DP("graph.001.pb")]
     >>> model_devi = calc_model_devi(coord, cell, atype, graphs)
     """
     energies = []
     forces = []
     virials = []
     natom = atype.shape[-1]
@@ -392,17 +388,16 @@
     relative_v : float, default: None
         If given, calculate the relative model deviation of virial. The
         value is the level parameter for computing the relative model
         deviation of the virial.
     **kwargs
         Arbitrary keyword arguments.
     """
-    auto_batch_size = AutoBatchSize()
     # init models
-    dp_models = [DeepPot(model, auto_batch_size=auto_batch_size) for model in models]
+    dp_models = [DeepPot(model, auto_batch_size=True) for model in models]
 
     # check type maps
     tmaps = [dp.get_type_map() for dp in dp_models]
     if _check_tmaps(tmaps):
         tmap = tmaps[0]
     else:
         raise RuntimeError("The models does not have the same type map.")
```

### Comparing `deepmd_kit-2.2.9/deepmd/loss/dos.py` & `deepmd_kit-3.0.0a0/deepmd/tf/loss/dos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     add_data_requirement,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     global_cvt_2_ener_float,
     global_cvt_2_tf_float,
     tf,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 from .loss import (
     Loss,
 )
```

### Comparing `deepmd_kit-2.2.9/deepmd/loss/ener.py` & `deepmd_kit-3.0.0a0/deepmd/tf/loss/ener.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
     Optional,
 )
 
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     add_data_requirement,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     global_cvt_2_ener_float,
     global_cvt_2_tf_float,
     tf,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 from .loss import (
     Loss,
 )
```

### Comparing `deepmd_kit-2.2.9/deepmd/loss/loss.py` & `deepmd_kit-3.0.0a0/deepmd/tf/loss/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import (
     Dict,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
 
 
 class Loss(metaclass=ABCMeta):
     """The abstract class for the loss function."""
```

### Comparing `deepmd_kit-2.2.9/deepmd/loss/tensor.py` & `deepmd_kit-3.0.0a0/deepmd/tf/loss/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     add_data_requirement,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     global_cvt_2_tf_float,
     tf,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 from .loss import (
     Loss,
 )
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/dos.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/dos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
     List,
     Optional,
     Union,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     MODEL_VERSION,
     global_cvt_2_ener_float,
     tf,
 )
-from deepmd.utils.type_embed import (
+from deepmd.tf.utils.type_embed import (
     TypeEmbedNet,
 )
 
 from .model import (
     StandardModel,
 )
 from .model_stat import (
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/ener.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/ener.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
     List,
     Optional,
     Union,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     MODEL_VERSION,
     global_cvt_2_ener_float,
     op_module,
     tf,
 )
-from deepmd.utils.data_system import (
+from deepmd.tf.utils.data_system import (
     DeepmdDataSystem,
 )
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
-from deepmd.utils.type_embed import (
+from deepmd.tf.utils.type_embed import (
     TypeEmbedNet,
 )
 
 from .model import (
     StandardModel,
 )
 from .model_stat import (
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/frozen.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/frozen.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,48 +3,57 @@
     Enum,
 )
 from typing import (
     Optional,
     Union,
 )
 
-from deepmd.env import (
+from deepmd.infer.deep_pot import (
+    DeepPot,
+)
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     MODEL_VERSION,
     tf,
 )
-from deepmd.fit.fitting import (
+from deepmd.tf.fit.fitting import (
     Fitting,
 )
-from deepmd.infer import (
+from deepmd.tf.infer import (
     DeepPotential,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.loss.loss import (
     Loss,
 )
 
 from .model import (
     Model,
 )
 
 
+@Model.register("frozen")
 class FrozenModel(Model):
     """Load model from a frozen model, which cannot be trained.
 
     Parameters
     ----------
     model_file : str
         The path to the frozen model
     """
 
     def __init__(self, model_file: str, **kwargs):
         super().__init__(**kwargs)
         self.model_file = model_file
         self.model = DeepPotential(model_file)
-        self.model_type = self.model.model_type
+        if isinstance(self.model, DeepPot):
+            self.model_type = "ener"
+        else:
+            raise NotImplementedError(
+                "This model type has not been implemented. " "Contribution is welcome!"
+            )
 
     def build(
         self,
         coord_: tf.Tensor,
         atype_: tf.Tensor,
         natoms: tf.Tensor,
         box: tf.Tensor,
@@ -118,22 +127,34 @@
                 self.model.get_dim_fparam(), name="dfparam", dtype=tf.int32
             )
             t_daparam = tf.constant(
                 self.model.get_dim_aparam(), name="daparam", dtype=tf.int32
             )
         if self.model_type == "ener":
             return {
-                "energy": tf.identity(self.model.t_energy, name="o_energy" + suffix),
-                "force": tf.identity(self.model.t_force, name="o_force" + suffix),
-                "virial": tf.identity(self.model.t_virial, name="o_virial" + suffix),
+                # must visit the backend class
+                "energy": tf.identity(
+                    self.model.deep_eval.output_tensors["energy_redu"],
+                    name="o_energy" + suffix,
+                ),
+                "force": tf.identity(
+                    self.model.deep_eval.output_tensors["energy_derv_r"],
+                    name="o_force" + suffix,
+                ),
+                "virial": tf.identity(
+                    self.model.deep_eval.output_tensors["energy_derv_c_redu"],
+                    name="o_virial" + suffix,
+                ),
                 "atom_ener": tf.identity(
-                    self.model.t_ae, name="o_atom_energy" + suffix
+                    self.model.deep_eval.output_tensors["energy"],
+                    name="o_atom_energy" + suffix,
                 ),
                 "atom_virial": tf.identity(
-                    self.model.t_av, name="o_atom_virial" + suffix
+                    self.model.deep_eval.output_tensors["energy_derv_c"],
+                    name="o_atom_virial" + suffix,
                 ),
                 "coord": coord_,
                 "atype": atype_,
             }
         else:
             raise NotImplementedError(
                 f"Model type {self.model_type} has not been implemented. "
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/linear.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 )
 from typing import (
     List,
     Optional,
     Union,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     MODEL_VERSION,
     tf,
 )
-from deepmd.fit.fitting import (
+from deepmd.tf.fit.fitting import (
     Fitting,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.loss.loss import (
     Loss,
 )
 
 from .model import (
     Model,
 )
 
@@ -143,14 +143,15 @@
         local_jdata_cpy["models"] = [
             Model.update_sel(global_jdata, sub_jdata)
             for sub_jdata in local_jdata["models"]
         ]
         return local_jdata_cpy
 
 
+@Model.register("linear_ener")
 class LinearEnergyModel(LinearModel):
     """Linear energy model make linear combinations of several existing energy models."""
 
     model_type = "ener"
 
     def build(
         self,
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/model.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,78 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
+import copy
 from abc import (
     ABC,
     abstractmethod,
 )
 from enum import (
     Enum,
 )
 from typing import (
     Dict,
     List,
     Optional,
     Union,
 )
 
-from deepmd.descriptor.descriptor import (
+from deepmd.common import (
+    j_get_type,
+)
+from deepmd.tf.descriptor.descriptor import (
     Descriptor,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     tf,
 )
-from deepmd.fit.fitting import (
+from deepmd.tf.fit.dipole import (
+    DipoleFittingSeA,
+)
+from deepmd.tf.fit.dos import (
+    DOSFitting,
+)
+from deepmd.tf.fit.ener import (
+    EnerFitting,
+)
+from deepmd.tf.fit.fitting import (
     Fitting,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.fit.polar import (
+    PolarFittingSeA,
+)
+from deepmd.tf.loss.loss import (
     Loss,
 )
-from deepmd.utils.argcheck import (
+from deepmd.tf.utils.argcheck import (
     type_embedding_args,
 )
-from deepmd.utils.data_system import (
+from deepmd.tf.utils.data_system import (
     DeepmdDataSystem,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     load_graph_def,
 )
-from deepmd.utils.pair_tab import (
+from deepmd.tf.utils.pair_tab import (
     PairTab,
 )
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
-from deepmd.utils.type_embed import (
+from deepmd.tf.utils.type_embed import (
     TypeEmbedNet,
 )
+from deepmd.utils.plugin import (
+    make_plugin_registry,
+)
+from deepmd.utils.version import (
+    check_version_compatibility,
+)
 
 
-class Model(ABC):
+class Model(ABC, make_plugin_registry("model")):
     """Abstract base model.
 
     Parameters
     ----------
     type_embedding
         Type embedding net
     type_map
@@ -74,60 +96,18 @@
         Whether add energy bias from the statistics of the data to short-range tabulated atomic energy. It only takes effect when `use_srtab` is provided.
     spin
         spin
     compress
         Compression information for internal use
     """
 
-    @classmethod
-    def get_class_by_input(cls, input: dict):
-        """Get the class by input data.
-
-        Parameters
-        ----------
-        input : dict
-            The input data
-        """
-        # infer model type by fitting_type
-        from deepmd.model.frozen import (
-            FrozenModel,
-        )
-        from deepmd.model.linear import (
-            LinearEnergyModel,
-        )
-        from deepmd.model.multi import (
-            MultiModel,
-        )
-        from deepmd.model.pairtab import (
-            PairTabModel,
-        )
-        from deepmd.model.pairwise_dprc import (
-            PairwiseDPRc,
-        )
-
-        model_type = input.get("type", "standard")
-        if model_type == "standard":
-            return StandardModel
-        elif model_type == "multi":
-            return MultiModel
-        elif model_type == "pairwise_dprc":
-            return PairwiseDPRc
-        elif model_type == "frozen":
-            return FrozenModel
-        elif model_type == "linear_ener":
-            return LinearEnergyModel
-        elif model_type == "pairtab":
-            return PairTabModel
-        else:
-            raise ValueError(f"unknown model type: {model_type}")
-
     def __new__(cls, *args, **kwargs):
         if cls is Model:
             # init model
-            cls = cls.get_class_by_input(kwargs)
+            cls = cls.get_class_by_type(kwargs.get("type", "standard"))
             return cls.__new__(cls, *args, **kwargs)
         return super().__new__(cls)
 
     def __init__(
         self,
         type_embedding: Optional[Union[dict, TypeEmbedNet]] = None,
         type_map: Optional[List[str]] = None,
@@ -511,15 +491,15 @@
             The type of atoms
         natoms : tf.Tensor
             The number of atoms. This tensor has the length of Ntypes + 2
             natoms[0]: number of local atoms
             natoms[1]: total number of atoms held by this processor
             natoms[i]: 2 <= i < Ntypes+2, number of type i atoms
         box : tf.Tensor
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         mesh : tf.Tensor
             For historical reasons, only the length of the Tensor matters.
             if size of mesh == 6, pbc is assumed.
             if size of mesh == 0, no-pbc is assumed.
         **kwargs : dict
             The additional arguments
 
@@ -558,18 +538,59 @@
             The local data refer to the current class
 
         Returns
         -------
         dict
             The updated local data
         """
-        cls = cls.get_class_by_input(local_jdata)
+        cls = cls.get_class_by_type(local_jdata.get("type", "standard"))
         return cls.update_sel(global_jdata, local_jdata)
 
+    @classmethod
+    def deserialize(cls, data: dict, suffix: str = "") -> "Model":
+        """Deserialize the model.
+
+        There is no suffix in a native DP model, but it is important
+        for the TF backend.
+
+        Parameters
+        ----------
+        data : dict
+            The serialized data
+        suffix : str, optional
+            Name suffix to identify this model
+
+        Returns
+        -------
+        Model
+            The deserialized Model
+        """
+        if cls is Model:
+            return Model.get_class_by_type(data.get("type", "standard")).deserialize(
+                data
+            )
+        raise NotImplementedError("Not implemented in class %s" % cls.__name__)
+
+    def serialize(self, suffix: str = "") -> dict:
+        """Serialize the model.
 
+        There is no suffix in a native DP model, but it is important
+        for the TF backend.
+
+        Returns
+        -------
+        dict
+            The serialized data
+        suffix : str, optional
+            Name suffix to identify this descriptor
+        """
+        raise NotImplementedError("Not implemented in class %s" % self.__name__)
+
+
+@Model.register("standard")
 class StandardModel(Model):
     """Standard model, which must contain a descriptor and a fitting.
 
     Parameters
     ----------
     descriptor : Union[dict, Descriptor]
         The descriptor
@@ -590,24 +611,31 @@
         )
         from .tensor import (
             DipoleModel,
             PolarModel,
         )
 
         if cls is StandardModel:
-            fitting_type = kwargs["fitting_net"]["type"]
+            if isinstance(kwargs["fitting_net"], dict):
+                fitting_type = Fitting.get_class_by_type(
+                    j_get_type(kwargs["fitting_net"], cls.__name__)
+                )
+            elif isinstance(kwargs["fitting_net"], Fitting):
+                fitting_type = type(kwargs["fitting_net"])
+            else:
+                raise RuntimeError("get unknown fitting type when building model")
             # init model
             # infer model type by fitting_type
-            if fitting_type == "ener":
+            if issubclass(fitting_type, EnerFitting):
                 cls = EnerModel
-            elif fitting_type == "dos":
+            elif issubclass(fitting_type, DOSFitting):
                 cls = DOSModel
-            elif fitting_type == "dipole":
+            elif issubclass(fitting_type, DipoleFittingSeA):
                 cls = DipoleModel
-            elif fitting_type == "polar":
+            elif issubclass(fitting_type, PolarFittingSeA):
                 cls = PolarModel
             else:
                 raise RuntimeError("get unknown fitting type when building model")
             return cls.__new__(cls)
         return super().__new__(cls)
 
     def __init__(
@@ -627,15 +655,23 @@
             self.descrpt = Descriptor(
                 **descriptor, ntypes=len(self.get_type_map()), spin=self.spin
             )
 
         if isinstance(fitting_net, Fitting):
             self.fitting = fitting_net
         else:
-            self.fitting = Fitting(**fitting_net, descrpt=self.descrpt, spin=self.spin)
+            if fitting_net["type"] in ["dipole", "polar"]:
+                fitting_net["embedding_width"] = self.descrpt.get_dim_rot_mat_1()
+            self.fitting = Fitting(
+                **fitting_net,
+                descrpt=self.descrpt,
+                spin=self.spin,
+                ntypes=self.descrpt.get_ntypes(),
+                dim_descrpt=self.descrpt.get_dim_out(),
+            )
         self.rcut = self.descrpt.get_rcut()
         self.ntypes = self.descrpt.get_ntypes()
 
         # type embedding
         if type_embedding is not None and isinstance(type_embedding, TypeEmbedNet):
             self.typeebd = type_embedding
         elif type_embedding is not None:
@@ -720,7 +756,67 @@
             The local data refer to the current class
         """
         local_jdata_cpy = local_jdata.copy()
         local_jdata_cpy["descriptor"] = Descriptor.update_sel(
             global_jdata, local_jdata["descriptor"]
         )
         return local_jdata_cpy
+
+    @classmethod
+    def deserialize(cls, data: dict, suffix: str = "") -> "Descriptor":
+        """Deserialize the model.
+
+        There is no suffix in a native DP model, but it is important
+        for the TF backend.
+
+        Parameters
+        ----------
+        data : dict
+            The serialized data
+        suffix : str, optional
+            Name suffix to identify this descriptor
+
+        Returns
+        -------
+        Descriptor
+            The deserialized descriptor
+        """
+        data = copy.deepcopy(data)
+        check_version_compatibility(data.pop("@version", 1), 1, 1)
+        descriptor = Descriptor.deserialize(data.pop("descriptor"), suffix=suffix)
+        fitting = Fitting.deserialize(data.pop("fitting"), suffix=suffix)
+        data.pop("atom_exclude_types")
+        data.pop("pair_exclude_types")
+        return cls(
+            descriptor=descriptor,
+            fitting_net=fitting,
+            **data,
+        )
+
+    def serialize(self, suffix: str = "") -> dict:
+        """Serialize the model.
+
+        There is no suffix in a native DP model, but it is important
+        for the TF backend.
+
+        Returns
+        -------
+        dict
+            The serialized data
+        suffix : str, optional
+            Name suffix to identify this descriptor
+        """
+        if self.typeebd is not None:
+            raise NotImplementedError("type embedding is not supported")
+        if self.spin is not None:
+            raise NotImplementedError("spin is not supported")
+        return {
+            "@class": "Model",
+            "type": "standard",
+            "@version": 1,
+            "type_map": self.type_map,
+            "descriptor": self.descrpt.serialize(suffix=suffix),
+            "fitting": self.fitting.serialize(suffix=suffix),
+            # not supported yet
+            "atom_exclude_types": [],
+            "pair_exclude_types": [],
+        }
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/multi.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/multi.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,61 +4,62 @@
     Dict,
     List,
     Optional,
 )
 
 import numpy as np
 
-from deepmd.descriptor.descriptor import (
+from deepmd.tf.descriptor.descriptor import (
     Descriptor,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     MODEL_VERSION,
     global_cvt_2_ener_float,
     op_module,
     tf,
 )
-from deepmd.fit import (
+from deepmd.tf.fit import (
     DipoleFittingSeA,
     DOSFitting,
     EnerFitting,
     GlobalPolarFittingSeA,
     PolarFittingSeA,
 )
-from deepmd.fit.fitting import (
+from deepmd.tf.fit.fitting import (
     Fitting,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.loss.loss import (
     Loss,
 )
-from deepmd.utils.argcheck import (
+from deepmd.tf.utils.argcheck import (
     type_embedding_args,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.pair_tab import (
+from deepmd.tf.utils.pair_tab import (
     PairTab,
 )
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
-from deepmd.utils.type_embed import (
+from deepmd.tf.utils.type_embed import (
     TypeEmbedNet,
 )
 
 from .model import (
     Model,
 )
 from .model_stat import (
     make_stat_input,
     merge_sys_stat,
 )
 
 
+@Model.register("multi")
 class MultiModel(Model):
     """Multi-task model.
 
     Parameters
     ----------
     descriptor
             Descriptor
@@ -129,16 +130,24 @@
 
         fitting_dict = {}
         for item in fitting_net_dict:
             item_fitting_param = fitting_net_dict[item]
             if isinstance(item_fitting_param, Fitting):
                 fitting_dict[item] = item_fitting_param
             else:
+                if item_fitting_param["type"] in ["dipole", "polar"]:
+                    item_fitting_param[
+                        "embedding_width"
+                    ] = self.descrpt.get_dim_rot_mat_1()
                 fitting_dict[item] = Fitting(
-                    **item_fitting_param, descrpt=self.descrpt, spin=self.spin
+                    **item_fitting_param,
+                    descrpt=self.descrpt,
+                    spin=self.spin,
+                    ntypes=self.descrpt.get_ntypes(),
+                    dim_descrpt=self.descrpt.get_dim_out(),
                 )
 
         # type embedding
         if type_embedding is not None and isinstance(type_embedding, TypeEmbedNet):
             self.typeebd = type_embedding
         elif type_embedding is not None:
             self.typeebd = TypeEmbedNet(
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/pairtab.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/pairtab.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,35 +6,39 @@
     List,
     Optional,
     Union,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     MODEL_VERSION,
     global_cvt_2_ener_float,
     op_module,
     tf,
 )
-from deepmd.fit.fitting import (
+from deepmd.tf.fit.fitting import (
     Fitting,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.loss.loss import (
     Loss,
 )
-from deepmd.model.model import (
+from deepmd.tf.model.model import (
     Model,
 )
-from deepmd.utils.pair_tab import (
+from deepmd.tf.utils.pair_tab import (
     PairTab,
 )
+from deepmd.tf.utils.update_sel import (
+    UpdateSel,
+)
 
 
+@Model.register("pairtab")
 class PairTabModel(Model):
     """Pairwise tabulation energy model.
 
     This model can be used to tabulate the pairwise energy between atoms for either
     short-range or long-range interactions, such as D3, LJ, ZBL, etc. It should not
     be used alone, but rather as one submodel of a linear (sum) model, such as
     DP+D3.
@@ -276,13 +280,9 @@
             The local data refer to the current class
 
         Returns
         -------
         dict
             The updated local data
         """
-        from deepmd.entrypoints.train import (
-            update_one_sel,
-        )
-
         local_jdata_cpy = local_jdata.copy()
-        return update_one_sel(global_jdata, local_jdata_cpy, True)
+        return UpdateSel().update_one_sel(global_jdata, local_jdata_cpy, True)
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/pairwise_dprc.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/pairwise_dprc.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,45 @@
 from typing import (
     Dict,
     List,
     Optional,
     Union,
 )
 
-from deepmd.common import (
+from deepmd.tf.common import (
     add_data_requirement,
     make_default_mesh,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     MODEL_VERSION,
     op_module,
     tf,
 )
-from deepmd.loss.loss import (
+from deepmd.tf.loss.loss import (
     Loss,
 )
-from deepmd.model.model import (
+from deepmd.tf.model.model import (
     Model,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     load_graph_def,
 )
-from deepmd.utils.spin import (
+from deepmd.tf.utils.spin import (
     Spin,
 )
-from deepmd.utils.type_embed import (
+from deepmd.tf.utils.type_embed import (
     TypeEmbedNet,
 )
+from deepmd.tf.utils.update_sel import (
+    UpdateSel,
+)
 
 
+@Model.register("pairwise_dprc")
 class PairwiseDPRc(Model):
     """Pairwise Deep Potential - Range Correction."""
 
     model_type = "ener"
 
     def __init__(
         self,
@@ -373,15 +377,15 @@
             The type of atoms
         natoms : tf.Tensor
             The number of atoms. This tensor has the length of Ntypes + 2
             natoms[0]: number of local atoms
             natoms[1]: total number of atoms held by this processor
             natoms[i]: 2 <= i < Ntypes+2, number of type i atoms
         box : tf.Tensor
-            The box. Can be generated by deepmd.model.make_stat_input
+            The box. Can be generated by deepmd.tf.model.make_stat_input
         mesh : tf.Tensor
             For historical reasons, only the length of the Tensor matters.
             if size of mesh == 6, pbc is assumed.
             if size of mesh == 0, no-pbc is assumed.
         aparam : tf.Tensor
             The parameters of the descriptor
         **kwargs : dict
@@ -408,21 +412,17 @@
         Parameters
         ----------
         global_jdata : dict
             The global data, containing the training section
         local_jdata : dict
             The local data refer to the current class
         """
-        from deepmd.entrypoints.train import (
-            get_min_nbor_dist,
-        )
-
         # do not update sel; only find min distance
         # rcut is not important here
-        get_min_nbor_dist(global_jdata, 6.0)
+        UpdateSel().get_min_nbor_dist(global_jdata, 6.0)
         return local_jdata
 
 
 def gather_placeholder(
     params: tf.Tensor, indices: tf.Tensor, placeholder: float = 0.0, **kwargs
 ) -> tf.Tensor:
     """Call tf.gather but allow indices to contain placeholders (-1)."""
```

### Comparing `deepmd_kit-2.2.9/deepmd/model/tensor.py` & `deepmd_kit-3.0.0a0/deepmd/tf/model/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
     List,
     Optional,
     Union,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     MODEL_VERSION,
     tf,
 )
-from deepmd.utils.type_embed import (
+from deepmd.tf.utils.type_embed import (
     TypeEmbedNet,
 )
 
 from .model import (
     StandardModel,
 )
 from .model_stat import (
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/data/__init__.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/data/data.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/data/data.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/descriptor/se_a.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/descriptor/se_a.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     op_module,
     tf,
 )
 
 #
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.nvnmd.utils.weight import (
+from deepmd.tf.nvnmd.utils.weight import (
     get_normalize,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     embedding_net,
 )
 
 log = logging.getLogger(__name__)
 
 
 def build_davg_dstd():
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/descriptor/se_atten.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/descriptor/se_atten.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_NP_FLOAT_PRECISION,
     op_module,
     tf,
 )
 
 #
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.nvnmd.utils.weight import (
+from deepmd.tf.nvnmd.utils.weight import (
     get_normalize,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
 )
 
 log = logging.getLogger(__name__)
 
 
 def build_davg_dstd():
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/freeze.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/freeze.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
-from deepmd.nvnmd.utils.fio import (
+from deepmd.tf.nvnmd.utils.fio import (
     FioDic,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
 )
 
 
 def filter_tensorVariableList(tensorVariableList) -> dict:
     r"""Get the name of variable for NVNMD.
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/mapt.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/mapt.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 import logging
 from typing import (
     Optional,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
-from deepmd.nvnmd.data.data import (
+from deepmd.tf.nvnmd.data.data import (
     jdata_deepmd_input_v0,
     jdata_sys,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.nvnmd.utils.fio import (
+from deepmd.tf.nvnmd.utils.fio import (
     FioDic,
 )
-from deepmd.nvnmd.utils.network import (
+from deepmd.tf.nvnmd.utils.network import (
     get_sess,
 )
-from deepmd.nvnmd.utils.weight import (
+from deepmd.tf.nvnmd.utils.weight import (
     get_filter_type_weight,
     get_filter_weight,
     get_normalize,
     get_type_embedding_weight,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 log = logging.getLogger(__name__)
 
 
 class MapTable:
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/train.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 import os
 from typing import (
     Optional,
 )
 
-from deepmd.entrypoints.freeze import (
+from deepmd.tf.entrypoints.freeze import (
     freeze,
 )
-from deepmd.entrypoints.train import (
+from deepmd.tf.entrypoints.train import (
     train,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
-from deepmd.nvnmd.data.data import (
+from deepmd.tf.nvnmd.data.data import (
     jdata_deepmd_input_v0,
 )
-from deepmd.nvnmd.entrypoints.mapt import (
+from deepmd.tf.nvnmd.entrypoints.mapt import (
     mapt,
 )
-from deepmd.nvnmd.entrypoints.wrap import (
+from deepmd.tf.nvnmd.entrypoints.wrap import (
     wrap,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.nvnmd.utils.fio import (
+from deepmd.tf.nvnmd.utils.fio import (
     FioDic,
 )
 
 log = logging.getLogger(__name__)
 
 jdata_cmd_train = {
     "INPUT": "train.json",
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/entrypoints/wrap.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/entrypoints/wrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 import logging
 from typing import (
     Optional,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
-from deepmd.nvnmd.data.data import (
+from deepmd.tf.nvnmd.data.data import (
     jdata_deepmd_input_v0,
     jdata_sys,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.nvnmd.utils.encode import (
+from deepmd.tf.nvnmd.utils.encode import (
     Encode,
 )
-from deepmd.nvnmd.utils.fio import (
+from deepmd.tf.nvnmd.utils.fio import (
     FioBin,
     FioTxt,
 )
-from deepmd.nvnmd.utils.network import (
+from deepmd.tf.nvnmd.utils.network import (
     get_sess,
 )
-from deepmd.nvnmd.utils.weight import (
+from deepmd.tf.nvnmd.utils.weight import (
     get_fitnet_weight,
     get_type_weight,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 log = logging.getLogger(__name__)
 
 
 class Wrap:
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/utils/__init__.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/utils/config.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 
 import numpy as np
 
-from deepmd.nvnmd.data.data import (
+from deepmd.tf.nvnmd.data.data import (
     NVNMD_CITATION,
     NVNMD_WELCOME,
     jdata_config_v0,
     jdata_config_v0_ni128,
     jdata_config_v0_ni256,
     jdata_config_v1_ni128,
     jdata_config_v1_ni256,
     jdata_deepmd_input_v0,
     jdata_deepmd_input_v0_ni128,
     jdata_deepmd_input_v0_ni256,
     jdata_deepmd_input_v1_ni128,
     jdata_deepmd_input_v1_ni256,
 )
-from deepmd.nvnmd.utils.fio import (
+from deepmd.tf.nvnmd.utils.fio import (
     FioDic,
 )
-from deepmd.nvnmd.utils.op import (
+from deepmd.tf.nvnmd.utils.op import (
     r2s,
 )
 
 log = logging.getLogger(__name__)
 
 
 class NvnmdConfig:
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/utils/encode.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/encode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 
 import numpy as np
 
-from deepmd.nvnmd.data.data import (
+from deepmd.tf.nvnmd.data.data import (
     jdata_sys,
 )
 
 log = logging.getLogger(__name__)
 
 
 class Encode:
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/utils/fio.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/fio.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/utils/network.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     op_module,
     tf,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.nvnmd.utils.weight import (
+from deepmd.tf.nvnmd.utils.weight import (
     get_constant_initializer,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     variable_summaries,
 )
 
 log = logging.getLogger(__name__)
 
 
 def get_sess():
```

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/utils/op.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/op.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd/nvnmd/utils/weight.py` & `deepmd_kit-3.0.0a0/deepmd/tf/nvnmd/utils/weight.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
 
 log = logging.getLogger(__name__)
 
 
 def get_weight(weights, key):
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/__init__.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib
 import logging
 from pathlib import (
     Path,
 )
 
 NOT_LOADABLE = ("__init__.py",)
-PACKAGE_BASE = "deepmd.op"
+PACKAGE_BASE = "deepmd.tf.op"
 
 log = logging.getLogger(__name__)
 
 
 def import_ops():
     """Import all custom TF ops that are present in this submodule.
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_dotmul_flt_nvnmd_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_dotmul_flt_nvnmd_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
 
 
 @ops.RegisterGradient("DotmulFltNvnmd")
 def _DotmulFltNvnmdGrad(op, grad):
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_gelu.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_gelu.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """First-order derivatives and second-order derivatives for gelu function."""
 import tensorflow
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
 )
 
 try:
     gelu = tensorflow.nn.gelu
 except AttributeError:
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_map_flt_nvnmd_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_map_flt_nvnmd_grad.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
 
 
 @ops.RegisterGradient("MapFltNvnmd")
 def _MapFltNvnmdGrad(op, grad):
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_matmul_fitnet_nvnmd_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_matmul_fitnet_nvnmd_grad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
 
 
 @ops.RegisterGradient("MatmulFitnetNvnmd")
 def _MatmulFitnetNvnmdGrad(op, grad):
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_matmul_flt2fix_nvnmd.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_matmul_flt2fix_nvnmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
 
 
 @ops.RegisterGradient("MatmulFlt2fixNvnmd")
 def _MatmulFlt2fixNvnmdGrad(op, grad):
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_matmul_flt_nvnmd_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_matmul_flt_nvnmd_grad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
 
 
 @ops.RegisterGradient("MatmulFltNvnmd")
 def _MatmulFltNvnmdGrad(op, grad):
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_mul_flt_nvnmd_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_mul_flt_nvnmd_grad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
 
 
 @ops.RegisterGradient("MulFltNvnmd")
 def _MulFltNvnmdGrad(op, grad):
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_prod_force_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_soft_min_force_grad.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: LGPL-3.0-or-later
-"""Gradients for prod force."""
+"""Gradients for soft min force."""
 
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_grads_module,
 )
 
 
-@ops.RegisterGradient("ProdForce")
-def _prod_force_grad_cc(op, grad):
-    net_grad = op_grads_module.prod_force_grad(
+@ops.RegisterGradient("SoftMinForce")
+def _soft_min_force_grad_cc(op, grad):
+    net_grad = op_grads_module.soft_min_force_grad(
         grad,
         op.inputs[0],
         op.inputs[1],
         op.inputs[2],
         op.inputs[3],
-        op.inputs[4],
         n_a_sel=op.get_attr("n_a_sel"),
         n_r_sel=op.get_attr("n_r_sel"),
     )
-    return [net_grad, None, None, None, None]
+    return [net_grad, None, None, None]
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_prod_force_se_a_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_force_se_a_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Gradients for prod force."""
 
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_grads_module,
 )
 
 
 @ops.RegisterGradient("ProdForceSeA")
 def _prod_force_se_a_grad_cc(op, grad):
     net_grad = op_grads_module.prod_force_se_a_grad(
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_prod_force_se_a_mask_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_force_se_a_mask_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Gradients for prod force se_a_mask."""
 
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_grads_module,
 )
 
 
 @ops.RegisterGradient("ProdForceSeAMask")
 def _prod_force_se_a_mask_grad_cc(op, grad):
     net_grad = op_grads_module.prod_force_se_a_mask_grad(
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_prod_virial_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_force_grad.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: LGPL-3.0-or-later
-"""Gradients for prod virial."""
+"""Gradients for prod force."""
 
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_grads_module,
 )
 
 
-@ops.RegisterGradient("ProdVirial")
-def _prod_virial_grad_cc(op, grad, grad_atom):
-    net_grad = op_grads_module.prod_virial_grad(
+@ops.RegisterGradient("ProdForce")
+def _prod_force_grad_cc(op, grad):
+    net_grad = op_grads_module.prod_force_grad(
         grad,
         op.inputs[0],
         op.inputs[1],
         op.inputs[2],
         op.inputs[3],
         op.inputs[4],
-        op.inputs[5],
         n_a_sel=op.get_attr("n_a_sel"),
         n_r_sel=op.get_attr("n_r_sel"),
     )
-    return [net_grad, None, None, None, None, None]
+    return [net_grad, None, None, None, None]
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_prod_virial_se_a_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_prod_virial_se_a_grad.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Gradients for prod virial."""
 
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_grads_module,
 )
 
 
 @ops.RegisterGradient("ProdVirialSeA")
 def _prod_virial_se_a_grad_cc(op, grad, grad_atom):
     net_grad = op_grads_module.prod_virial_se_a_grad(
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_soft_min_force_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_soft_min_virial_grad.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: LGPL-3.0-or-later
-"""Gradients for soft min force."""
+"""Gradients for soft min virial."""
 
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_grads_module,
 )
 
 
-@ops.RegisterGradient("SoftMinForce")
-def _soft_min_force_grad_cc(op, grad):
-    net_grad = op_grads_module.soft_min_force_grad(
+@ops.RegisterGradient("SoftMinVirial")
+def _soft_min_virial_grad_cc(op, grad, grad_atom):
+    net_grad = op_grads_module.soft_min_virial_grad(
         grad,
         op.inputs[0],
         op.inputs[1],
         op.inputs[2],
         op.inputs[3],
+        op.inputs[4],
         n_a_sel=op.get_attr("n_a_sel"),
         n_r_sel=op.get_attr("n_r_sel"),
     )
-    return [net_grad, None, None, None]
+    return [net_grad, None, None, None, None]
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_tabulate_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_tabulate_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Gradients for tabulate."""
 
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
 )
 
-# from deepmd.DescrptSeATabulate import last_layer_size
+# from deepmd.tf.DescrptSeATabulate import last_layer_size
 
 
 @ops.RegisterGradient("TabulateFusion")
 @ops.RegisterGradient("TabulateFusionSeA")
 def _tabulate_fusion_se_a_grad_cc(op, dy):
     dy_dx, dy_df = op_module.tabulate_fusion_se_a_grad(
         op.inputs[0],
```

### Comparing `deepmd_kit-2.2.9/deepmd/op/_tanh4_flt_nvnmd_grad.py` & `deepmd_kit-3.0.0a0/deepmd/tf/op/_tanh4_flt_nvnmd_grad.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from tensorflow.python.framework import (
     ops,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
 
 
 @ops.RegisterGradient("Tanh4FltNvnmd")
 def _Tanh4FltNvnmdGrad(op, grad):
     prechi = 2**23
```

### Comparing `deepmd_kit-2.2.9/deepmd/train/run_options.py` & `deepmd_kit-3.0.0a0/deepmd/tf/train/run_options.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,71 +12,71 @@
     Optional,
 )
 
 from packaging.version import (
     Version,
 )
 
-from deepmd.cluster import (
+from deepmd.tf.cluster import (
     get_resource,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_CONFIG,
     TF_VERSION,
-    get_tf_default_nthreads,
-    global_float_prec,
     tf,
 )
-from deepmd.loggers import (
+from deepmd.tf.loggers import (
     set_log_handles,
 )
+from deepmd.utils.summary import SummaryPrinter as BaseSummaryPrinter
 
 if TYPE_CHECKING:
     import horovod.tensorflow as HVD
 
 
 __all__ = [
-    "WELCOME",
-    "CITATION",
-    "BUILD",
     "RunOptions",
 ]
 
 log = logging.getLogger(__name__)
 
 
-# http://patorjk.com/software/taag. Font:Big"
-WELCOME = (
-    r" _____               _____   __  __  _____           _     _  _   ",
-    r"|  __ \             |  __ \ |  \/  ||  __ \         | |   (_)| |  ",
-    r"| |  | |  ___   ___ | |__) || \  / || |  | | ______ | | __ _ | |_ ",
-    r"| |  | | / _ \ / _ \|  ___/ | |\/| || |  | ||______|| |/ /| || __|",
-    r"| |__| ||  __/|  __/| |     | |  | || |__| |        |   < | || |_ ",
-    r"|_____/  \___| \___||_|     |_|  |_||_____/         |_|\_\|_| \__|",
-)
-
-CITATION = (
-    "Please read and cite:",
-    "Wang, Zhang, Han and E, Comput.Phys.Comm. 228, 178-184 (2018)",
-    "Zeng et al, J. Chem. Phys., 159, 054801 (2023)",
-    "See https://deepmd.rtfd.io/credits/ for details.",
-)
+class SummaryPrinter(BaseSummaryPrinter):
+    """Summary printer for TensorFlow."""
 
-_sep = "\n                      "
-BUILD = (
-    f"installed to:         {GLOBAL_CONFIG['install_prefix']}",
-    f"source :              {GLOBAL_CONFIG['git_summ']}",
-    f"source brach:         {GLOBAL_CONFIG['git_branch']}",
-    f"source commit:        {GLOBAL_CONFIG['git_hash']}",
-    f"source commit at:     {GLOBAL_CONFIG['git_date']}",
-    f"build float prec:     {global_float_prec}",
-    f"build variant:        {GLOBAL_CONFIG['dp_variant']}",
-    f"build with tf inc:    {GLOBAL_CONFIG['tf_include_dir']}",
-    f"build with tf lib:    {GLOBAL_CONFIG['tf_libs'].replace(';', _sep)}",
-)
+    def __init__(self, compute_device: str, ngpus: int) -> None:
+        super().__init__()
+        self.compute_device = compute_device
+        self.ngpus = ngpus
+
+    def is_built_with_cuda(self) -> bool:
+        """Check if the backend is built with CUDA."""
+        return tf.test.is_built_with_cuda()
+
+    def is_built_with_rocm(self) -> bool:
+        """Check if the backend is built with ROCm."""
+        return tf.test.is_built_with_rocm()
+
+    def get_compute_device(self) -> str:
+        """Get Compute device."""
+        return self.compute_device
+
+    def get_ngpus(self) -> int:
+        """Get the number of GPUs."""
+        return self.ngpus
+
+    def get_backend_info(self) -> dict:
+        """Get backend information."""
+        return {
+            "Backend": "TensorFlow",
+            "TF ver": tf.version.GIT_VERSION,
+            "build with TF ver": TF_VERSION,
+            "build with TF inc": GLOBAL_CONFIG["tf_include_dir"].replace(";", "\n"),
+            "build with TF lib": GLOBAL_CONFIG["tf_libs"].replace(";", "\n"),
+        }
 
 
 class RunOptions:
     """Class with info on how to run training (cluster, MPI and GPU config).
 
     Attributes
     ----------
@@ -144,33 +144,15 @@
     @property
     def is_chief(self):
         """Whether my rank is 0."""
         return self.my_rank == 0
 
     def print_resource_summary(self):
         """Print build and current running cluster configuration summary."""
-        log.info("---Summary of the training---------------------------------------")
-        if self.is_distrib:
-            log.info("distributed")
-            log.info(f"world size:           {self.world_size}")
-            log.info(f"my rank:              {self.my_rank}")
-            log.info(f"node list:            {self.nodelist}")
-        log.info(f"running on:           {self.nodename}")
-        log.info(f"computing device:     {self.my_device}")
-        if tf.test.is_built_with_cuda():
-            env_value = os.environ.get("CUDA_VISIBLE_DEVICES", "unset")
-            log.info(f"CUDA_VISIBLE_DEVICES: {env_value}")
-        if hasattr(tf.test, "is_built_with_rocm") and tf.test.is_built_with_rocm():
-            env_value = os.environ.get("HIP_VISIBLE_DEVICES", "unset")
-            log.info(f"HIP_VISIBLE_DEVICES:  {env_value}")
-        log.info(f"Count of visible GPU: {len(self.gpus or [])}")
-        intra, inter = get_tf_default_nthreads()
-        log.info(f"num_intra_threads:    {intra:d}")
-        log.info(f"num_inter_threads:    {inter:d}")
-        log.info("-----------------------------------------------------------------")
+        SummaryPrinter(self.my_device, len(self.gpus or []))()
 
     def _setup_logger(
         self,
         log_path: Optional[Path],
         log_level: int,
         mpi_log: Optional[str],
     ):
```

### Comparing `deepmd_kit-2.2.9/deepmd/train/trainer.py` & `deepmd_kit-3.0.0a0/deepmd/tf/train/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: LGPL-3.0-or-later
-import glob
 import logging
 import os
-import platform
 import shutil
 import time
 from typing import (
     Dict,
     List,
 )
 
@@ -17,60 +15,67 @@
     Version,
 )
 from tensorflow.python.client import (
     timeline,
 )
 
 # load grad of force module
-import deepmd.op  # noqa: F401
+import deepmd.tf.op  # noqa: F401
 from deepmd.common import (
+    symlink_prefix_files,
+)
+from deepmd.loggers.training import (
+    format_training_message,
+    format_training_message_per_task,
+)
+from deepmd.tf.common import (
     data_requirement,
     get_precision,
     j_must_have,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_ENER_FLOAT_PRECISION,
     GLOBAL_TF_FLOAT_PRECISION,
     TF_VERSION,
     get_tf_session_config,
     tf,
     tfv2,
 )
-from deepmd.fit.ener import (
+from deepmd.tf.fit.ener import (
     EnerFitting,
 )
-from deepmd.model import (
+from deepmd.tf.model import (
     MultiModel,
 )
-from deepmd.model.model import (
+from deepmd.tf.model.model import (
     Model,
 )
-from deepmd.utils import random as dp_random
-from deepmd.utils.data_system import (
+from deepmd.tf.utils import random as dp_random
+from deepmd.tf.utils.data_system import (
     DeepmdDataSystem,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphTooLargeError,
     GraphWithoutTensorError,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name_from_graph,
     load_graph_def,
 )
-from deepmd.utils.learning_rate import (
+from deepmd.tf.utils.learning_rate import (
     LearningRateExp,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 log = logging.getLogger(__name__)
 
 # nvnmd
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
 
 
 def _is_subdir(path, directory):
     path = os.path.realpath(path)
     directory = os.path.realpath(directory)
@@ -769,16 +774,18 @@
                             fp, train_batches, valid_batches, fitting_key=fitting_key
                         )
                 if self.timing_in_training:
                     toc = time.time()
                     test_time = toc - tic
                     wall_time = toc - wall_time_tic
                     log.info(
-                        "batch %7d training time %.2f s, testing time %.2f s, total wall time %.2f s"
-                        % (cur_batch, train_time, test_time, wall_time)
+                        format_training_message(
+                            batch=cur_batch,
+                            wall_time=wall_time,
+                        )
                     )
                     # the first training time is not accurate
                     if cur_batch > self.disp_freq or stop_batch < 2 * self.disp_freq:
                         total_train_time += train_time
                     train_time = 0
                     wall_time_tic = toc
                 if (
@@ -826,27 +833,15 @@
             raise GraphTooLargeError(
                 "The graph size exceeds 2 GB, the hard limitation of protobuf."
                 " Then a DecodeError was raised by protobuf. You should "
                 "reduce the size of your model."
             ) from e
         # make symlinks from prefix with step to that without step to break nothing
         # get all checkpoint files
-        original_files = glob.glob(ckpt_prefix + ".*")
-        for ori_ff in original_files:
-            new_ff = self.save_ckpt + ori_ff[len(ckpt_prefix) :]
-            try:
-                # remove old one
-                os.remove(new_ff)
-            except OSError:
-                pass
-            if platform.system() != "Windows":
-                # by default one does not have access to create symlink on Windows
-                os.symlink(os.path.relpath(ori_ff, os.path.dirname(new_ff)), new_ff)
-            else:
-                shutil.copyfile(ori_ff, new_ff)
+        symlink_prefix_files(ckpt_prefix, self.save_ckpt)
         log.info("saved checkpoint %s" % self.save_ckpt)
 
     def get_feed_dict(self, batch, is_training):
         feed_dict = {}
         for kk in batch.keys():
             if kk == "find_type" or kk == "type" or kk == "real_natoms_vec":
                 continue
@@ -966,14 +961,31 @@
                     # assert k in train_results.keys()
                     print_str += prop_fmt % (valid_results[k], train_results[k])
             else:
                 prop_fmt = "   %11.2e"
                 for k in train_results.keys():
                     print_str += prop_fmt % (train_results[k])
             print_str += "   %8.1e\n" % cur_lr
+            log.info(
+                format_training_message_per_task(
+                    batch=cur_batch,
+                    task_name="trn",
+                    rmse=train_results,
+                    learning_rate=cur_lr,
+                )
+            )
+            if valid_results is not None:
+                log.info(
+                    format_training_message_per_task(
+                        batch=cur_batch,
+                        task_name="val",
+                        rmse=valid_results,
+                        learning_rate=None,
+                    )
+                )
         else:
             for fitting_key in train_results:
                 if valid_results[fitting_key] is not None:
                     prop_fmt = "   %11.2e %11.2e"
                     for k in valid_results[fitting_key].keys():
                         # assert k in train_results[fitting_key].keys()
                         print_str += prop_fmt % (
@@ -981,14 +993,31 @@
                             train_results[fitting_key][k],
                         )
                 else:
                     prop_fmt = "   %11.2e"
                     for k in train_results[fitting_key].keys():
                         print_str += prop_fmt % (train_results[fitting_key][k])
                 print_str += "   %8.1e\n" % cur_lr_dict[fitting_key]
+                log.info(
+                    format_training_message_per_task(
+                        batch=cur_batch,
+                        task_name=f"{fitting_key}_trn",
+                        rmse=train_results[fitting_key],
+                        learning_rate=cur_lr_dict[fitting_key],
+                    )
+                )
+                if valid_results is not None:
+                    log.info(
+                        format_training_message_per_task(
+                            batch=cur_batch,
+                            task_name=f"{fitting_key}_val",
+                            rmse=valid_results[fitting_key],
+                            learning_rate=None,
+                        )
+                    )
         fp.write(print_str)
         fp.flush()
 
     @staticmethod
     def eval_single_list(single_batch_list, loss, sess, get_feed_dict_func, prefix=""):
         if single_batch_list is None:
             return None
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/batch_size.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/batch_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from packaging.version import (
     Version,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     TF_VERSION,
     tf,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     OutOfMemoryError,
 )
-from deepmd_utils.utils.batch_size import AutoBatchSize as AutoBatchSizeBase
+from deepmd.utils.batch_size import AutoBatchSize as AutoBatchSizeBase
 
 
 class AutoBatchSize(AutoBatchSizeBase):
     def is_gpu_available(self) -> bool:
         """Check if GPU is available.
 
         Returns
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/compress.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import logging
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_pattern_nodes_from_graph_def,
     get_tensor_by_name_from_graph,
 )
 
 log = logging.getLogger(__name__)
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/convert.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
     text_format,
 )
 from packaging.specifiers import (
     SpecifierSet,
 )
 from packaging.version import parse as parse_version
 
-from deepmd import (
+from deepmd.tf import (
     __version__,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
 
 log = logging.getLogger(__name__)
 
 
 def detect_model_version(input_model: str):
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/finetune.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/finetune.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import json
 import logging
 from typing import (
     Any,
     Dict,
 )
 
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphWithoutTensorError,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name,
 )
 
 log = logging.getLogger(__name__)
 
 
 def replace_model_params_with_pretrained_model(
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/graph.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from typing import (
     Dict,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     ATTENTION_LAYER_PATTERN,
     EMBEDDING_NET_PATTERN,
     FITTING_NET_PATTERN,
     TYPE_EMBEDDING_PATTERN,
     tf,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphWithoutTensorError,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 
 # TODO (JZ): I think in this file we can merge some duplicated lines into one method...
 def load_graph_def(model_file: str) -> Tuple[tf.Graph, tf.GraphDef]:
     """Load graph as well as the graph_def from the frozen model(model_file).
@@ -162,28 +162,24 @@
     -------
     Dict
         The embedding net nodes within the given tf.GraphDef object
     """
     # embedding_net_pattern = f"filter_type_\d+{suffix}/matrix_\d+_\d+|filter_type_\d+{suffix}/bias_\d+_\d+|filter_type_\d+{suffix}/idt_\d+_\d+|filter_type_all{suffix}/matrix_\d+_\d+|filter_type_all{suffix}/matrix_\d+_\d+_\d+|filter_type_all{suffix}/bias_\d+_\d+|filter_type_all{suffix}/bias_\d+_\d+_\d+|filter_type_all{suffix}/idt_\d+_\d+"
     if suffix != "":
         embedding_net_pattern = (
-            EMBEDDING_NET_PATTERN.replace("/idt", suffix + "/idt")
-            .replace("/bias", suffix + "/bias")
-            .replace("/matrix", suffix + "/matrix")
+            EMBEDDING_NET_PATTERN.replace("/(idt)", suffix + "/(idt)")
+            .replace("/(bias)", suffix + "/(bias)")
+            .replace("/(matrix)", suffix + "/(matrix)")
         )
     else:
         embedding_net_pattern = EMBEDDING_NET_PATTERN
 
     embedding_net_nodes = get_pattern_nodes_from_graph_def(
         graph_def, embedding_net_pattern
     )
-    for key in embedding_net_nodes.keys():
-        assert (
-            key.find("bias") > 0 or key.find("matrix") > 0
-        ), "currently, only support weight matrix and bias matrix at the tabulation op!"
     return embedding_net_nodes
 
 
 def get_embedding_net_nodes(model_file: str, suffix: str = "") -> Dict:
     """Get the embedding net nodes with the given frozen model(model_file).
 
     Parameters
@@ -356,17 +352,17 @@
     Returns
     -------
     Dict
         The fitting net nodes within the given tf.GraphDef object
     """
     if suffix != "":
         fitting_net_pattern = (
-            FITTING_NET_PATTERN.replace("/idt", suffix + "/idt")
-            .replace("/bias", suffix + "/bias")
-            .replace("/matrix", suffix + "/matrix")
+            FITTING_NET_PATTERN.replace("/(idt)", suffix + "/(idt)")
+            .replace("/(bias)", suffix + "/(bias)")
+            .replace("/(matrix)", suffix + "/(matrix)")
         )
     else:
         fitting_net_pattern = FITTING_NET_PATTERN
     fitting_net_nodes = get_pattern_nodes_from_graph_def(graph_def, fitting_net_pattern)
     for key in fitting_net_nodes.keys():
         assert (
             key.find("bias") > 0 or key.find("matrix") > 0 or key.find("idt") > 0
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/learning_rate.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/learning_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
     Optional,
 )
 
 import numpy as np
 
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
 
 
 class LearningRateExp:
     r"""The exponentially decaying learning rate.
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/multi_init.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/multi_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import json
 import logging
 from typing import (
     Any,
     Dict,
 )
 
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     GraphWithoutTensorError,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_tensor_by_name,
 )
 
 log = logging.getLogger(__name__)
 
 
 def replace_model_params_with_frz_multi_model(
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/network.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import numpy as np
 
-from deepmd.common import (
+from deepmd.tf.common import (
     get_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     tf,
 )
 
 
 def one_layer_rand_seed_shift():
     return 3
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/parallel_op.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/parallel_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
     Callable,
     Dict,
     Generator,
     Optional,
     Tuple,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
-from deepmd.utils.sess import (
+from deepmd.tf.utils.sess import (
     run_sess,
 )
 
 
 class ParallelOp:
     """Run an op with data parallelism.
 
@@ -26,25 +26,23 @@
     nthreads : int, optional
         the number of threads
     config : tf.ConfigProto, optional
         tf.ConfigProto
 
     Examples
     --------
-    >>> from deepmd.env import tf
-    >>> from deepmd.utils.parallel_op import ParallelOp
+    >>> from deepmd.tf.env import tf
+    >>> from deepmd.tf.utils.parallel_op import ParallelOp
     >>> def builder():
     ...     x = tf.placeholder(tf.int32, [1])
     ...     return {"x": x}, (x + 1)
-    ...
     >>> p = ParallelOp(builder, nthreads=4)
     >>> def feed():
     ...     for ii in range(10):
     ...         yield {"x": [ii]}
-    ...
     >>> print(*p.generate(tf.Session(), feed()))
     [1] [2] [3] [4] [5] [6] [7] [8] [9] [10]
     """
 
     def __init__(
         self,
         builder: Callable[..., Tuple[Dict[str, tf.Tensor], Tuple[tf.Tensor]]],
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/sess.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/sess.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 import os
 
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
-from deepmd.utils.errors import (
+from deepmd.tf.utils.errors import (
     OutOfMemoryError,
 )
 
 
 def run_sess(sess: tf.Session, *args, **kwargs):
     """Run session with erorrs caught.
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/spin.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/spin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
     List,
     Optional,
 )
 
-from deepmd.env import (
+from deepmd.tf.env import (
     GLOBAL_TF_FLOAT_PRECISION,
     tf,
 )
 
 
 class Spin:
     """Class for spin.
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/tabulate.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/tabulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 import numpy as np
 from scipy.special import (
     comb,
 )
 
 import deepmd
-from deepmd.common import (
+from deepmd.tf.common import (
     ACTIVATION_FN_DICT,
 )
-from deepmd.descriptor import (
+from deepmd.tf.descriptor import (
     Descriptor,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     op_module,
     tf,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_embedding_net_nodes_from_graph_def,
     get_tensor_by_name_from_graph,
 )
 
 log = logging.getLogger(__name__)
 
 
@@ -103,23 +103,23 @@
         self.activation_fn = activation_fn
 
         # self.sess = tf.Session(graph = self.graph)
 
         self.sub_graph, self.sub_graph_def = self._load_sub_graph()
         self.sub_sess = tf.Session(graph=self.sub_graph)
 
-        if isinstance(self.descrpt, deepmd.descriptor.DescrptSeR):
+        if isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeR):
             self.sel_a = self.descrpt.sel_r
             self.rcut = self.descrpt.rcut
             self.rcut_smth = self.descrpt.rcut_smth
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeA):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeA):
             self.sel_a = self.descrpt.sel_a
             self.rcut = self.descrpt.rcut_r
             self.rcut_smth = self.descrpt.rcut_r_smth
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeT):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeT):
             self.sel_a = self.descrpt.sel_a
             self.rcut = self.descrpt.rcut_r
             self.rcut_smth = self.descrpt.rcut_r_smth
         else:
             raise RuntimeError("Unsupported descriptor")
 
         self.davg = get_tensor_by_name_from_graph(
@@ -129,14 +129,18 @@
             self.graph, f"descrpt_attr{self.suffix}/t_std"
         )
         self.ntypes = get_tensor_by_name_from_graph(self.graph, "descrpt_attr/ntypes")
 
         self.embedding_net_nodes = get_embedding_net_nodes_from_graph_def(
             self.graph_def, suffix=self.suffix
         )
+        for key in self.embedding_net_nodes.keys():
+            assert (
+                key.find("bias") > 0 or key.find("matrix") > 0
+            ), "currently, only support weight matrix and bias matrix at the tabulation op!"
 
         # move it to the descriptor class
         # for tt in self.exclude_types:
         #     if (tt[0] not in range(self.ntypes)) or (tt[1] not in range(self.ntypes)):
         #         raise RuntimeError("exclude types" + str(tt) + " must within the number of atomic types " + str(self.ntypes) + "!")
         # if (self.ntypes * self.ntypes - len(self.exclude_types) == 0):
         #     raise RuntimeError("empty embedding-net are not supported in model compression!")
@@ -175,16 +179,16 @@
         lower : dict[str, int]
             The lower boundary of environment matrix by net
         upper : dict[str, int]
             The upper boundary of environment matrix by net
         """
         # tabulate range [lower, upper] with stride0 'stride0'
         lower, upper = self._get_env_mat_range(min_nbor_dist)
-        if isinstance(self.descrpt, deepmd.descriptor.DescrptSeAtten) or isinstance(
-            self.descrpt, deepmd.descriptor.DescrptSeAEbdV2
+        if isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeAtten) or isinstance(
+            self.descrpt, deepmd.tf.descriptor.DescrptSeAEbdV2
         ):
             uu = np.max(upper)
             ll = np.min(lower)
             xx = np.arange(ll, uu, stride0, dtype=self.data_type)
             xx = np.append(
                 xx,
                 np.arange(uu, extrapolate * uu, stride1, dtype=self.data_type),
@@ -192,15 +196,15 @@
             xx = np.append(xx, np.array([extrapolate * uu], dtype=self.data_type))
             nspline = ((uu - ll) / stride0 + (extrapolate * uu - uu) / stride1).astype(
                 int
             )
             self._build_lower(
                 "filter_net", xx, 0, uu, ll, stride0, stride1, extrapolate, nspline
             )
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeA):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeA):
             for ii in range(self.table_size):
                 if (self.type_one_side and not self._all_excluded(ii)) or (
                     not self.type_one_side
                     and (ii // self.ntypes, ii % self.ntypes) not in self.exclude_types
                 ):
                     if self.type_one_side:
                         net = "filter_-1_net_" + str(ii)
@@ -229,15 +233,15 @@
                     )
                     nspline = (
                         (uu - ll) / stride0 + (extrapolate * uu - uu) / stride1
                     ).astype(int)
                     self._build_lower(
                         net, xx, ii, uu, ll, stride0, stride1, extrapolate, nspline
                     )
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeT):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeT):
             xx_all = []
             for ii in range(self.ntypes):
                 xx = np.arange(
                     extrapolate * lower[ii], lower[ii], stride1, dtype=self.data_type
                 )
                 xx = np.append(
                     xx, np.arange(lower[ii], upper[ii], stride0, dtype=self.data_type)
@@ -271,15 +275,15 @@
                         lower[ii],
                         stride0,
                         stride1,
                         extrapolate,
                         nspline[ii],
                     )
                     idx += 1
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeR):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeR):
             for ii in range(self.table_size):
                 if (self.type_one_side and not self._all_excluded(ii)) or (
                     not self.type_one_side
                     and (ii // self.ntypes, ii % self.ntypes) not in self.exclude_types
                 ):
                     if self.type_one_side:
                         net = "filter_-1_net_" + str(ii)
@@ -323,27 +327,27 @@
     ):
         vv, dd, d2 = self._make_data(xx, idx)
         self.data[net] = np.zeros(
             [nspline, 6 * self.last_layer_size], dtype=self.data_type
         )
 
         # tt.shape: [nspline, self.last_layer_size]
-        if isinstance(self.descrpt, deepmd.descriptor.DescrptSeA):
+        if isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeA):
             tt = np.full((nspline, self.last_layer_size), stride1)
             tt[: int((upper - lower) / stride0), :] = stride0
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeT):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeT):
             tt = np.full((nspline, self.last_layer_size), stride1)
             tt[
                 int((lower - extrapolate * lower) / stride1) + 1 : (
                     int((lower - extrapolate * lower) / stride1)
                     + int((upper - lower) / stride0)
                 ),
                 :,
             ] = stride0
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeR):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeR):
             tt = np.full((nspline, self.last_layer_size), stride1)
             tt[: int((upper - lower) / stride0), :] = stride0
         else:
             raise RuntimeError("Unsupported descriptor")
 
         # hh.shape: [nspline, self.last_layer_size]
         hh = (
@@ -419,22 +423,22 @@
             tf.import_graph_def(sub_graph_def, name="")
         return sub_graph, sub_graph_def
 
     def _get_bias(self):
         bias = {}
         for layer in range(1, self.layer_size + 1):
             bias["layer_" + str(layer)] = []
-            if isinstance(self.descrpt, deepmd.descriptor.DescrptSeAtten) or isinstance(
-                self.descrpt, deepmd.descriptor.DescrptSeAEbdV2
-            ):
+            if isinstance(
+                self.descrpt, deepmd.tf.descriptor.DescrptSeAtten
+            ) or isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeAEbdV2):
                 node = self.embedding_net_nodes[
                     f"filter_type_all{self.suffix}/bias_{layer}"
                 ]
                 bias["layer_" + str(layer)].append(tf.make_ndarray(node))
-            elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeA):
+            elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeA):
                 if self.type_one_side:
                     for ii in range(0, self.ntypes):
                         if not self._all_excluded(ii):
                             node = self.embedding_net_nodes[
                                 f"filter_type_all{self.suffix}/bias_{layer}_{ii}"
                             ]
                             bias["layer_" + str(layer)].append(tf.make_ndarray(node))
@@ -448,22 +452,22 @@
                         ) not in self.exclude_types:
                             node = self.embedding_net_nodes[
                                 f"filter_type_{ii // self.ntypes}{self.suffix}/bias_{layer}_{ii % self.ntypes}"
                             ]
                             bias["layer_" + str(layer)].append(tf.make_ndarray(node))
                         else:
                             bias["layer_" + str(layer)].append(np.array([]))
-            elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeT):
+            elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeT):
                 for ii in range(self.ntypes):
                     for jj in range(ii, self.ntypes):
                         node = self.embedding_net_nodes[
                             f"filter_type_all{self.suffix}/bias_{layer}_{ii}_{jj}"
                         ]
                         bias["layer_" + str(layer)].append(tf.make_ndarray(node))
-            elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeR):
+            elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeR):
                 if self.type_one_side:
                     for ii in range(0, self.ntypes):
                         if not self._all_excluded(ii):
                             node = self.embedding_net_nodes[
                                 f"filter_type_all{self.suffix}/bias_{layer}_{ii}"
                             ]
                             bias["layer_" + str(layer)].append(tf.make_ndarray(node))
@@ -485,22 +489,22 @@
                 raise RuntimeError("Unsupported descriptor")
         return bias
 
     def _get_matrix(self):
         matrix = {}
         for layer in range(1, self.layer_size + 1):
             matrix["layer_" + str(layer)] = []
-            if isinstance(self.descrpt, deepmd.descriptor.DescrptSeAtten) or isinstance(
-                self.descrpt, deepmd.descriptor.DescrptSeAEbdV2
-            ):
+            if isinstance(
+                self.descrpt, deepmd.tf.descriptor.DescrptSeAtten
+            ) or isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeAEbdV2):
                 node = self.embedding_net_nodes[
                     f"filter_type_all{self.suffix}/matrix_{layer}"
                 ]
                 matrix["layer_" + str(layer)].append(tf.make_ndarray(node))
-            elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeA):
+            elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeA):
                 if self.type_one_side:
                     for ii in range(0, self.ntypes):
                         if not self._all_excluded(ii):
                             node = self.embedding_net_nodes[
                                 f"filter_type_all{self.suffix}/matrix_{layer}_{ii}"
                             ]
                             matrix["layer_" + str(layer)].append(tf.make_ndarray(node))
@@ -514,22 +518,22 @@
                         ) not in self.exclude_types:
                             node = self.embedding_net_nodes[
                                 f"filter_type_{ii // self.ntypes}{self.suffix}/matrix_{layer}_{ii % self.ntypes}"
                             ]
                             matrix["layer_" + str(layer)].append(tf.make_ndarray(node))
                         else:
                             matrix["layer_" + str(layer)].append(np.array([]))
-            elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeT):
+            elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeT):
                 for ii in range(self.ntypes):
                     for jj in range(ii, self.ntypes):
                         node = self.embedding_net_nodes[
                             f"filter_type_all{self.suffix}/matrix_{layer}_{ii}_{jj}"
                         ]
                         matrix["layer_" + str(layer)].append(tf.make_ndarray(node))
-            elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeR):
+            elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeR):
                 if self.type_one_side:
                     for ii in range(0, self.ntypes):
                         if not self._all_excluded(ii):
                             node = self.embedding_net_nodes[
                                 f"filter_type_all{self.suffix}/matrix_{layer}_{ii}"
                             ]
                             matrix["layer_" + str(layer)].append(tf.make_ndarray(node))
@@ -708,22 +712,22 @@
     def _layer_1(self, x, w, b):
         t = tf.concat([x, x], axis=1)
         return t, self.activation_fn(tf.matmul(x, w) + b) + t
 
     # Change the embedding net range to sw / min_nbor_dist
     def _get_env_mat_range(self, min_nbor_dist):
         sw = self._spline5_switch(min_nbor_dist, self.rcut_smth, self.rcut)
-        if isinstance(self.descrpt, deepmd.descriptor.DescrptSeA):
+        if isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeA):
             lower = -self.davg[:, 0] / self.dstd[:, 0]
             upper = ((1 / min_nbor_dist) * sw - self.davg[:, 0]) / self.dstd[:, 0]
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeT):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeT):
             var = np.square(sw / (min_nbor_dist * self.dstd[:, 1:4]))
             lower = np.min(-var, axis=1)
             upper = np.max(var, axis=1)
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeR):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeR):
             lower = -self.davg[:, 0] / self.dstd[:, 0]
             upper = ((1 / min_nbor_dist) * sw - self.davg[:, 0]) / self.dstd[:, 0]
         else:
             raise RuntimeError("Unsupported descriptor")
         log.info("training data with lower boundary: " + str(lower))
         log.info("training data with upper boundary: " + str(upper))
         # returns element-wise lower and upper
@@ -737,49 +741,49 @@
             vv = uu * uu * uu * (-6 * uu * uu + 15 * uu - 10) + 1
         else:
             vv = 0
         return vv
 
     def _get_layer_size(self):
         layer_size = 0
-        if isinstance(self.descrpt, deepmd.descriptor.DescrptSeAtten) or isinstance(
-            self.descrpt, deepmd.descriptor.DescrptSeAEbdV2
+        if isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeAtten) or isinstance(
+            self.descrpt, deepmd.tf.descriptor.DescrptSeAEbdV2
         ):
             layer_size = len(self.embedding_net_nodes) // 2
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeA):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeA):
             layer_size = len(self.embedding_net_nodes) // (
                 (self.ntypes * self.ntypes - len(self.exclude_types)) * 2
             )
             if self.type_one_side:
                 layer_size = len(self.embedding_net_nodes) // (
                     (self.ntypes - self._n_all_excluded) * 2
                 )
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeT):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeT):
             layer_size = len(self.embedding_net_nodes) // int(
                 comb(self.ntypes + 1, 2) * 2
             )
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeR):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeR):
             layer_size = len(self.embedding_net_nodes) // (
                 (self.ntypes * self.ntypes - len(self.exclude_types)) * 2
             )
             if self.type_one_side:
                 layer_size = len(self.embedding_net_nodes) // (
                     (self.ntypes - self._n_all_excluded) * 2
                 )
         else:
             raise RuntimeError("Unsupported descriptor")
         return layer_size
 
     @property
-    @lru_cache()
+    @lru_cache
     def _n_all_excluded(self) -> int:
         """Then number of types excluding all types."""
         return sum(int(self._all_excluded(ii)) for ii in range(0, self.ntypes))
 
-    @lru_cache()
+    @lru_cache
     def _all_excluded(self, ii: int) -> bool:
         """Check if type ii excluds all types.
 
         Parameters
         ----------
         ii : int
             type index
@@ -789,25 +793,25 @@
         bool
             if type ii excluds all types
         """
         return all((ii, type_i) in self.exclude_types for type_i in range(self.ntypes))
 
     def _get_table_size(self):
         table_size = 0
-        if isinstance(self.descrpt, deepmd.descriptor.DescrptSeAtten) or isinstance(
-            self.descrpt, deepmd.descriptor.DescrptSeAEbdV2
+        if isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeAtten) or isinstance(
+            self.descrpt, deepmd.tf.descriptor.DescrptSeAEbdV2
         ):
             table_size = 1
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeA):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeA):
             table_size = self.ntypes * self.ntypes
             if self.type_one_side:
                 table_size = self.ntypes
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeT):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeT):
             table_size = int(comb(self.ntypes + 1, 2))
-        elif isinstance(self.descrpt, deepmd.descriptor.DescrptSeR):
+        elif isinstance(self.descrpt, deepmd.tf.descriptor.DescrptSeR):
             table_size = self.ntypes * self.ntypes
             if self.type_one_side:
                 table_size = self.ntypes
         else:
             raise RuntimeError("Unsupported descriptor")
         return table_size
```

### Comparing `deepmd_kit-2.2.9/deepmd/utils/type_embed.py` & `deepmd_kit-3.0.0a0/deepmd/tf/utils/type_embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 from typing import (
     List,
     Optional,
     Union,
 )
 
-from deepmd.common import (
+from deepmd.tf.common import (
     get_activation_func,
     get_precision,
 )
-from deepmd.env import (
+from deepmd.tf.env import (
     tf,
 )
-from deepmd.nvnmd.utils.config import (
+from deepmd.tf.nvnmd.utils.config import (
     nvnmd_cfg,
 )
-from deepmd.utils.graph import (
+from deepmd.tf.utils.graph import (
     get_type_embedding_net_variables_from_graph_def,
 )
-from deepmd.utils.network import (
+from deepmd.tf.utils.network import (
     embedding_net,
 )
 
 
 def embed_atom_type(
     ntypes: int,
     natoms: tf.Tensor,
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/common.py` & `deepmd_kit-3.0.0a0/deepmd/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
+import glob
 import json
+import os
+import platform
+import shutil
 import warnings
+from hashlib import (
+    sha1,
+)
 from pathlib import (
     Path,
 )
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
@@ -18,18 +25,18 @@
     from typing import Literal  # python >=3.8
 except ImportError:
     from typing_extensions import Literal  # type: ignore
 
 import numpy as np
 import yaml
 
-from deepmd_utils.env import (
+from deepmd.env import (
     GLOBAL_NP_FLOAT_PRECISION,
 )
-from deepmd_utils.utils.path import (
+from deepmd.utils.path import (
     DPPath,
 )
 
 __all__ = [
     "data_requirement",
     "add_data_requirement",
     "select_idx_map",
@@ -67,14 +74,15 @@
     atomic: bool = False,
     must: bool = False,
     high_prec: bool = False,
     type_sel: Optional[bool] = None,
     repeat: int = 1,
     default: float = 0.0,
     dtype: Optional[np.dtype] = None,
+    output_natoms_for_type_sel: bool = False,
 ):
     """Specify data requirements for training.
 
     Parameters
     ----------
     key : str
         type of data stored in corresponding `*.npy` file e.g. `forces` or `energy`
@@ -92,24 +100,27 @@
         select only certain type of atoms, by default None
     repeat : int, optional
         if specify repaeat data `repeat` times, by default 1
     default : float, optional, default=0.
         default value of data
     dtype : np.dtype, optional
         the dtype of data, overwrites `high_prec` if provided
+    output_natoms_for_type_sel : bool, optional
+        if True and type_sel is True, the atomic dimension will be natoms instead of nsel
     """
     data_requirement[key] = {
         "ndof": ndof,
         "atomic": atomic,
         "must": must,
         "high_prec": high_prec,
         "type_sel": type_sel,
         "repeat": repeat,
         "default": default,
         "dtype": dtype,
+        "output_natoms_for_type_sel": output_natoms_for_type_sel,
     }
 
 
 def select_idx_map(atom_types: np.ndarray, select_types: np.ndarray) -> np.ndarray:
     """Build map of indices for element supplied element types from all atoms list.
 
     Parameters
@@ -264,7 +275,66 @@
         return np.float16
     elif precision == "float32":
         return np.float32
     elif precision == "float64":
         return np.float64
     else:
         raise RuntimeError(f"{precision} is not a valid precision")
+
+
+def symlink_prefix_files(old_prefix: str, new_prefix: str):
+    """Create symlinks from old checkpoint prefix to new one.
+
+    On Windows this function will copy files instead of creating symlinks.
+
+    Parameters
+    ----------
+    old_prefix : str
+        old checkpoint prefix, all files with this prefix will be symlinked
+    new_prefix : str
+        new checkpoint prefix
+    """
+    original_files = glob.glob(old_prefix + ".*")
+    for ori_ff in original_files:
+        new_ff = new_prefix + ori_ff[len(old_prefix) :]
+        try:
+            # remove old one
+            os.remove(new_ff)
+        except OSError:
+            pass
+        if platform.system() != "Windows":
+            # by default one does not have access to create symlink on Windows
+            os.symlink(os.path.relpath(ori_ff, os.path.dirname(new_ff)), new_ff)
+        else:
+            shutil.copyfile(ori_ff, new_ff)
+
+
+def get_hash(obj) -> str:
+    """Get hash of object.
+
+    Parameters
+    ----------
+    obj
+        object to hash
+    """
+    return sha1(json.dumps(obj).encode("utf-8")).hexdigest()
+
+
+def j_get_type(data: dict, class_name: str = "object") -> str:
+    """Get the type from the data.
+
+    Parameters
+    ----------
+    data : dict
+        the data
+    class_name : str, optional
+        the name of the class for error message, by default "object"
+
+    Returns
+    -------
+    str
+        the type
+    """
+    try:
+        return data["type"]
+    except KeyError as e:
+        raise KeyError(f"the type of the {class_name} should be set by `type`") from e
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/entrypoints/doc.py` & `deepmd_kit-3.0.0a0/deepmd/entrypoints/doc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Module that prints train input arguments docstrings."""
 
-from deepmd_utils.utils.argcheck import (
+from deepmd.utils.argcheck import (
     gen_doc,
     gen_json,
 )
 
 __all__ = ["doc_train_input"]
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/entrypoints/gui.py` & `deepmd_kit-3.0.0a0/deepmd/entrypoints/gui.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd_utils/loggers/loggers.py` & `deepmd_kit-3.0.0a0/deepmd/loggers/loggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,22 @@
 
 # logger formater
 FFORMATTER = logging.Formatter(
     "[%(asctime)s] %(app_name)s %(levelname)-7s %(name)-45s %(message)s"
 )
 CFORMATTER = logging.Formatter(
     #    "%(app_name)s %(levelname)-7s |-> %(name)-45s %(message)s"
-    "%(app_name)s %(levelname)-7s %(message)s"
+    "[%(asctime)s] %(app_name)s %(levelname)-7s %(message)s"
 )
 FFORMATTER_MPI = logging.Formatter(
     "[%(asctime)s] %(app_name)s rank:%(rank)-2s %(levelname)-7s %(name)-45s %(message)s"
 )
 CFORMATTER_MPI = logging.Formatter(
     #    "%(app_name)s rank:%(rank)-2s %(levelname)-7s |-> %(name)-45s %(message)s"
-    "%(app_name)s rank:%(rank)-2s %(levelname)-7s %(message)s"
+    "[%(asctime)s] %(app_name)s rank:%(rank)-2s %(levelname)-7s %(message)s"
 )
 
 
 class _AppFilter(logging.Filter):
     """Add field `app_name` to log messages."""
 
     def filter(self, record):
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/main.py` & `deepmd_kit-3.0.0a0/deepmd/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,32 @@
 """The entry points for DeePMD-kit.
 
 If only printing the help message, this module does not call
 the main DeePMD-kit module to avoid the slow import of TensorFlow.
 """
 import argparse
 import logging
+import os
 import textwrap
+from collections import (
+    defaultdict,
+)
 from typing import (
+    Dict,
     List,
     Optional,
+    Type,
+)
+
+from deepmd.backend.backend import (
+    Backend,
 )
 
 try:
-    from deepmd_utils._version import version as __version__
+    from deepmd._version import version as __version__
 except ImportError:
     __version__ = "unknown"
 
 
 def get_ll(log_level: str) -> int:
     """Convert string to python logging level.
 
@@ -41,27 +51,81 @@
 
 class RawTextArgumentDefaultsHelpFormatter(
     argparse.RawTextHelpFormatter, argparse.ArgumentDefaultsHelpFormatter
 ):
     """This formatter is used to print multile-line help message with default value."""
 
 
+BACKENDS: Dict[str, Type[Backend]] = Backend.get_backends_by_feature(
+    Backend.Feature.ENTRY_POINT
+)
+BACKEND_TABLE: Dict[str, str] = {kk: vv.name.lower() for kk, vv in BACKENDS.items()}
+
+
+class BackendOption(argparse.Action):
+    """Map backend alias to unique name."""
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        setattr(namespace, self.dest, BACKEND_TABLE[values])
+
+
 def main_parser() -> argparse.ArgumentParser:
     """DeePMD-Kit commandline options argument parser.
 
     Returns
     -------
     argparse.ArgumentParser
         main parser of DeePMD-kit
     """
     parser = argparse.ArgumentParser(
         description="DeePMD-kit: A deep learning package for many-body potential energy"
         " representation and molecular dynamics",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+        formatter_class=RawTextArgumentDefaultsHelpFormatter,
+        epilog=textwrap.dedent(
+            """\
+        Use --tf or --pt to choose the backend:
+            dp --tf train input.json
+            dp --pt train input.json
+        """
+        ),
     )
+
+    # default backend is TF for compatibility
+    default_backend = os.environ.get("DP_BACKEND", "tensorflow").lower()
+    if default_backend not in BACKEND_TABLE.keys():
+        raise ValueError(
+            f"Unknown backend {default_backend}. "
+            "Please set DP_BACKEND to either tensorflow or pytorch."
+        )
+
+    parser_backend = parser.add_mutually_exclusive_group()
+    parser_backend.add_argument(
+        "-b",
+        "--backend",
+        choices=list(BACKEND_TABLE.keys()),
+        action=BackendOption,
+        default=default_backend,
+        help=(
+            "The backend of the model. Default can be set by environment variable "
+            "DP_BACKEND."
+        ),
+    )
+
+    BACKEND_ALIAS: Dict[str, List[str]] = defaultdict(list)
+    for alias, backend in BACKEND_TABLE.items():
+        BACKEND_ALIAS[backend].append(alias)
+    for backend, alias in BACKEND_ALIAS.items():
+        parser_backend.add_argument(
+            *[f"--{aa}" for aa in alias],
+            action="store_const",
+            dest="backend",
+            const=backend,
+            help=f"Alias for --backend {backend}",
+        )
+
     subparsers = parser.add_subparsers(title="Valid subcommands", dest="command")
 
     # * logging options parser *********************************************************
     # with use of the parent argument this options will be added to every parser
     parser_log = argparse.ArgumentParser(
         add_help=False, formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
@@ -94,15 +158,17 @@
         help="Set the manner of logging when running with MPI. 'master' logs only on "
         "main process, 'collect' broadcasts logs from workers to master and 'workers' "
         "means each process will output its own log",
     )
 
     # * transfer script ****************************************************************
     parser_transfer = subparsers.add_parser(
-        "transfer", parents=[parser_log], help="pass parameters to another model"
+        "transfer",
+        parents=[parser_log],
+        help="(Supported backend: TensorFlow) pass parameters to another model",
     )
     parser_transfer.add_argument(
         "-r",
         "--raw-model",
         default="raw_frozen_model.pb",
         type=str,
         help="the model receiving parameters",
@@ -177,14 +243,26 @@
         help="The output file of the parameters used in training.",
     )
     parser_train.add_argument(
         "--skip-neighbor-stat",
         action="store_true",
         help="Skip calculating neighbor statistics. Sel checking, automatic sel, and model compression will be disabled.",
     )
+    parser_train.add_argument(
+        # -m has been used by mpi-log
+        "--model-branch",
+        type=str,
+        default="",
+        help="(Supported backend: PyTorch) Model branch chosen for fine-tuning if multi-task. If not specified, it will re-init the fitting net.",
+    )
+    parser_train.add_argument(
+        "--force-load",
+        action="store_true",
+        help="(Supported backend: PyTorch) Force load from ckpt, other missing tensors will init from scratch",
+    )
 
     # * freeze script ******************************************************************
     parser_frz = subparsers.add_parser(
         "freeze",
         parents=[parser_log],
         help="freeze the model",
         formatter_class=RawTextArgumentDefaultsHelpFormatter,
@@ -195,44 +273,51 @@
             dp freeze -o graph.pb
         """
         ),
     )
     parser_frz.add_argument(
         "-c",
         "--checkpoint-folder",
+        "--checkpoint",
         type=str,
         default=".",
-        help="path to checkpoint folder",
+        help="Path to checkpoint, either a folder containing checkpoint or the checkpoint prefix",
     )
     parser_frz.add_argument(
         "-o",
         "--output",
         type=str,
-        default="frozen_model.pb",
-        help="name of graph, will output to the checkpoint folder",
+        default="frozen_model",
+        help="Filename (prefix) of the output model file. TensorFlow backend: suffix is .pb; PyTorch backend: suffix is .pth",
     )
     parser_frz.add_argument(
         "-n",
         "--node-names",
         type=str,
         default=None,
-        help="the frozen nodes, if not set, determined from the model type",
+        help="(Supported backend: TensorFlow) the frozen nodes, if not set, determined from the model type",
     )
     parser_frz.add_argument(
         "-w",
         "--nvnmd-weight",
         type=str,
         default=None,
-        help="the name of weight file (.npy), if set, save the model's weight into the file",
+        help="(Supported backend: TensorFlow) the name of weight file (.npy), if set, save the model's weight into the file",
     )
     parser_frz.add_argument(
         "--united-model",
         action="store_true",
         default=False,
-        help="When in multi-task mode, freeze all nodes into one united model",
+        help="(Supported backend: TensorFlow) When in multi-task mode, freeze all nodes into one united model",
+    )
+    parser_frz.add_argument(
+        "--head",
+        default=None,
+        type=str,
+        help="(Supported backend: PyTorch) Task head to freeze if in multi-task mode.",
     )
 
     # * test script ********************************************************************
     parser_tst = subparsers.add_parser(
         "test",
         parents=[parser_log],
         help="test the model",
@@ -243,17 +328,17 @@
             dp test -m graph.pb -s /path/to/system -n 30
         """
         ),
     )
     parser_tst.add_argument(
         "-m",
         "--model",
-        default="frozen_model.pb",
+        default="frozen_model",
         type=str,
-        help="Frozen model file to import",
+        help="Frozen model file (prefix) to import. TensorFlow backend: suffix is .pb; PyTorch backend: suffix is .pth.",
     )
     parser_tst_subgroup = parser_tst.add_mutually_exclusive_group()
     parser_tst_subgroup.add_argument(
         "-s",
         "--system",
         default=".",
         type=str,
@@ -263,25 +348,33 @@
         "-f",
         "--datafile",
         default=None,
         type=str,
         help="The path to file of test list.",
     )
     parser_tst.add_argument(
-        "-S", "--set-prefix", default="set", type=str, help="The set prefix"
+        "-S",
+        "--set-prefix",
+        default="set",
+        type=str,
+        help="(Supported backend: TensorFlow) The set prefix",
     )
     parser_tst.add_argument(
         "-n",
         "--numb-test",
         default=0,
         type=int,
         help="The number of data for test. 0 means all data.",
     )
     parser_tst.add_argument(
-        "-r", "--rand-seed", type=int, default=None, help="The random seed"
+        "-r",
+        "--rand-seed",
+        type=int,
+        default=None,
+        help="(Supported backend: TensorFlow) The random seed",
     )
     parser_tst.add_argument(
         "--shuffle-test", action="store_true", default=False, help="Shuffle test data"
     )
     parser_tst.add_argument(
         "-d",
         "--detail-file",
@@ -290,29 +383,41 @@
         help="The prefix to files where details of energy, force and virial accuracy/accuracy per atom will be written",
     )
     parser_tst.add_argument(
         "-a",
         "--atomic",
         action="store_true",
         default=False,
-        help="Test the accuracy of atomic label, i.e. energy / tensor (dipole, polar)",
+        help="(Supported backend: TensorFlow) Test the accuracy of atomic label, i.e. energy / tensor (dipole, polar)",
+    )
+    parser_tst.add_argument(
+        "-i",
+        "--input_script",
+        type=str,
+        help="(Supported backend: PyTorch) The input script of the model",
+    )
+    parser_tst.add_argument(
+        "--head",
+        default=None,
+        type=str,
+        help="(Supported backend: PyTorch) Task head to test if in multi-task mode.",
     )
 
     # * compress model *****************************************************************
     # Compress a model, which including tabulating the embedding-net.
     # The table is composed of fifth-order polynomial coefficients and is assembled
     # from two sub-tables. The first table takes the step(parameter) as it's uniform
     # step, while the second table takes 10 * step as it\s uniform step
     #  The range of the first table is automatically detected by deepmd-kit, while the
     # second table ranges from the first table's upper boundary(upper) to the
     # extrapolate(parameter) * upper.
     parser_compress = subparsers.add_parser(
         "compress",
         parents=[parser_log, parser_mpi_log],
-        help="compress a model",
+        help="(Supported backend: TensorFlow) compress a model",
         formatter_class=RawTextArgumentDefaultsHelpFormatter,
         epilog=textwrap.dedent(
             """\
         examples:
             dp compress
             dp compress -i graph.pb -o compressed.pb
         """
@@ -405,18 +510,18 @@
             dp model-devi -m graph.000.pb graph.001.pb graph.002.pb graph.003.pb -s ./data -o model_devi.out
         """
         ),
     )
     parser_model_devi.add_argument(
         "-m",
         "--models",
-        default=["graph.000.pb", "graph.001.pb", "graph.002.pb", "graph.003.pb"],
+        default=["graph.000", "graph.001", "graph.002", "graph.003"],
         nargs="+",
         type=str,
-        help="Frozen models file to import",
+        help="Frozen models file (prefix) to import. TensorFlow backend: suffix is .pb; PyTorch backend: suffix is .pth.",
     )
     parser_model_devi.add_argument(
         "-s",
         "--system",
         default=".",
         type=str,
         help="The system directory. Recursively detect systems in this directory.",
@@ -461,15 +566,15 @@
         help="Calculate the relative model deviation of virial. The level parameter for computing the relative model deviation of the virial should be given.",
     )
 
     # * convert models
     parser_transform = subparsers.add_parser(
         "convert-from",
         parents=[parser_log],
-        help="convert lower model version to supported version",
+        help="(Supported backend: TensorFlow) convert lower model version to supported version",
         formatter_class=RawTextArgumentDefaultsHelpFormatter,
         epilog=textwrap.dedent(
             """\
         examples:
             dp convert-from -i graph.pb -o graph_new.pb
             dp convert-from auto -i graph.pb -o graph_new.pb
             dp convert-from 1.0 -i graph.pb -o graph_new.pb
@@ -531,14 +636,15 @@
         "--type-map",
         type=str,
         nargs="+",
         required=True,
         help="type map",
     )
     parser_neighbor_stat.add_argument(
+        "--mixed-type",
         "--one-type",
         action="store_true",
         default=False,
         help="treat all types as a single type. Used with se_atten descriptor.",
     )
 
     # --version
@@ -546,15 +652,15 @@
         "--version", action="version", version="DeePMD-kit v%s" % __version__
     )
 
     # * train nvnmd script ******************************************************************
     parser_train_nvnmd = subparsers.add_parser(
         "train-nvnmd",
         parents=[parser_log],
-        help="train nvnmd model",
+        help="(Supported backend: TensorFlow) train nvnmd model",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         epilog=textwrap.dedent(
             """\
         examples:
             dp train-nvnmd input_cnn.json -s s1
             dp train-nvnmd input_qnn.json -s s2
             dp train-nvnmd input_cnn.json -s s1 --restart model.ckpt
@@ -611,14 +717,31 @@
         "--bind_all",
         action="store_true",
         help=(
             "Serve on all public interfaces. This will expose your DP-GUI instance "
             "to the network on both IPv4 and IPv6 (where available)."
         ),
     )
+
+    # convert_backend
+    parser_convert_backend = subparsers.add_parser(
+        "convert-backend",
+        parents=[parser_log],
+        help="Convert model to another backend.",
+        formatter_class=RawTextArgumentDefaultsHelpFormatter,
+        epilog=textwrap.dedent(
+            """\
+        examples:
+            dp convert-backend model.pb model.pth
+            dp convert-backend model.pb model.dp
+        """
+        ),
+    )
+    parser_convert_backend.add_argument("INPUT", help="The input model file.")
+    parser_convert_backend.add_argument("OUTPUT", help="The output model file.")
     return parser
 
 
 def parse_args(args: Optional[List[str]] = None) -> argparse.Namespace:
     """Parse arguments and convert argument strings to objects.
 
     Parameters
@@ -647,10 +770,36 @@
 
     Raises
     ------
     RuntimeError
         if no command was input
     """
     args = parse_args()
-    from deepmd.entrypoints.main import main as deepmd_main
+
+    if args.backend not in BACKEND_TABLE:
+        raise ValueError(f"Unknown backend {args.backend}")
+
+    if args.command in (
+        "test",
+        "doc-train-input",
+        "model-devi",
+        "neighbor-stat",
+        "gui",
+        "convert-backend",
+    ):
+        # common entrypoints
+        from deepmd.entrypoints.main import main as deepmd_main
+    elif args.command in (
+        "train",
+        "freeze",
+        "transfer",
+        "compress",
+        "convert-from",
+        "train-nvnmd",
+    ):
+        deepmd_main = BACKENDS[args.backend]().entry_point_hook
+    elif args.command is None:
+        pass
+    else:
+        raise RuntimeError(f"unknown command {args.command}")
 
     deepmd_main(args)
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/model_format/env_mat.py` & `deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/env_mat.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import (
     Optional,
     Union,
 )
 
 import numpy as np
 
-from .common import (
+from deepmd.dpmodel import (
     NativeOP,
 )
 
 
 def compute_smooth_weight(
     distance: np.ndarray,
     rmin: float,
@@ -26,14 +26,15 @@
 
 
 def _make_env_mat(
     nlist,
     coord,
     rcut: float,
     ruct_smth: float,
+    radial_only: bool = False,
 ):
     """Make smooth environment matrix."""
     nf, nloc, nnei = nlist.shape
     # nf x nall x 3
     coord = coord.reshape(nf, -1, 3)
     mask = nlist >= 0
     nlist = nlist * mask
@@ -49,16 +50,20 @@
     # nf x nloc x nnei
     length = np.linalg.norm(diff, axis=-1, keepdims=True)
     # for index 0 nloc atom
     length = length + ~np.expand_dims(mask, -1)
     t0 = 1 / length
     t1 = diff / length**2
     weight = compute_smooth_weight(length, ruct_smth, rcut)
-    env_mat_se_a = np.concatenate([t0, t1], axis=-1) * weight * np.expand_dims(mask, -1)
-    return env_mat_se_a, diff * np.expand_dims(mask, -1), weight
+    weight = weight * np.expand_dims(mask, -1)
+    if radial_only:
+        env_mat = t0 * weight
+    else:
+        env_mat = np.concatenate([t0, t1], axis=-1) * weight
+    return env_mat, diff * np.expand_dims(mask, -1), weight
 
 
 class EnvMat(NativeOP):
     def __init__(
         self,
         rcut,
         rcut_smth,
@@ -69,52 +74,56 @@
     def call(
         self,
         coord_ext: np.ndarray,
         atype_ext: np.ndarray,
         nlist: np.ndarray,
         davg: Optional[np.ndarray] = None,
         dstd: Optional[np.ndarray] = None,
+        radial_only: bool = False,
     ) -> Union[np.ndarray, np.ndarray]:
         """Compute the environment matrix.
 
         Parameters
         ----------
         nlist
             The neighbor list. shape: nf x nloc x nnei
         coord_ext
             The extended coordinates of atoms. shape: nf x (nallx3)
         atype_ext
             The extended aotm types. shape: nf x nall
         davg
-            The data avg. shape: nt x nnei x 4
+            The data avg. shape: nt x nnei x (4 or 1)
         dstd
-            The inverse of data std. shape: nt x nnei x 4
+            The inverse of data std. shape: nt x nnei x (4 or 1)
+        radial_only
+            Whether to only compute radial part of the environment matrix.
+            If True, the output will be of shape nf x nloc x nnei x 1.
+            Otherwise, the output will be of shape nf x nloc x nnei x 4.
+            Default: False.
 
         Returns
         -------
         env_mat
-            The environment matrix. shape: nf x nloc x nnei x 4
+            The environment matrix. shape: nf x nloc x nnei x (4 or 1)
         switch
             The value of switch function. shape: nf x nloc x nnei
         """
-        em, sw = self._call(nlist, coord_ext)
+        em, sw = self._call(nlist, coord_ext, radial_only)
         nf, nloc, nnei = nlist.shape
         atype = atype_ext[:, :nloc]
         if davg is not None:
             em -= davg[atype]
         if dstd is not None:
             em /= dstd[atype]
         return em, sw
 
-    def _call(
-        self,
-        nlist,
-        coord_ext,
-    ):
-        em, diff, ww = _make_env_mat(nlist, coord_ext, self.rcut, self.rcut_smth)
+    def _call(self, nlist, coord_ext, radial_only):
+        em, diff, ww = _make_env_mat(
+            nlist, coord_ext, self.rcut, self.rcut_smth, radial_only
+        )
         return em, ww
 
     def serialize(
         self,
     ) -> dict:
         return {
             "rcut": self.rcut,
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/model_format/network.py` & `deepmd_kit-3.0.0a0/deepmd/dpmodel/utils/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,38 @@
 """Native DP model format for multiple backends.
 
 See issue #2982 for more information.
 """
 import copy
 import itertools
 import json
+from datetime import (
+    datetime,
+)
 from typing import (
     ClassVar,
     Dict,
     List,
     Optional,
     Union,
 )
 
 import h5py
 import numpy as np
 
+from deepmd.utils.version import (
+    check_version_compatibility,
+)
+
 try:
-    from deepmd_utils._version import version as __version__
+    from deepmd._version import version as __version__
 except ImportError:
     __version__ = "unknown"
 
-from .common import (
+from deepmd.dpmodel import (
     DEFAULT_PRECISION,
     PRECISION_DICT,
     NativeOP,
 )
 
 
 def traverse_model_dict(model_obj, callback: callable, is_variable: bool = False):
@@ -50,14 +57,16 @@
         for kk, vv in model_obj.items():
             model_obj[kk] = traverse_model_dict(
                 vv, callback, is_variable=is_variable or kk == "@variables"
             )
     elif isinstance(model_obj, list):
         for ii, vv in enumerate(model_obj):
             model_obj[ii] = traverse_model_dict(vv, callback, is_variable=is_variable)
+    elif model_obj is None:
+        return model_obj
     elif is_variable:
         model_obj = callback(model_obj)
     return model_obj
 
 
 class Counter:
     """A callable counter.
@@ -75,44 +84,40 @@
         self.count = -1
 
     def __call__(self):
         self.count += 1
         return self.count
 
 
-def save_dp_model(filename: str, model_dict: dict, extra_info: Optional[dict] = None):
+# TODO: should be moved to otherwhere...
+def save_dp_model(filename: str, model_dict: dict) -> None:
     """Save a DP model to a file in the native format.
 
     Parameters
     ----------
     filename : str
         The filename to save to.
     model_dict : dict
         The model dict to save.
-    extra_info : dict, optional
-        Extra meta information to save.
     """
     model_dict = model_dict.copy()
     variable_counter = Counter()
-    if extra_info is not None:
-        extra_info = extra_info.copy()
-    else:
-        extra_info = {}
     with h5py.File(filename, "w") as f:
         model_dict = traverse_model_dict(
             model_dict,
             lambda x: f.create_dataset(
                 f"variable_{variable_counter():04d}", data=x
             ).name,
         )
         save_dict = {
-            "model": model_dict,
             "software": "deepmd-kit",
             "version": __version__,
-            **extra_info,
+            # use UTC+0 time
+            "time": str(datetime.utcnow()),
+            **model_dict,
         }
         f.attrs["json"] = json.dumps(save_dict, separators=(",", ":"))
 
 
 def load_dp_model(filename: str) -> dict:
     """Load a DP model from a file in the native format.
 
@@ -157,14 +162,16 @@
         use_timestep: bool = False,
         activation_function: Optional[str] = None,
         resnet: bool = False,
         precision: str = DEFAULT_PRECISION,
     ) -> None:
         prec = PRECISION_DICT[precision.lower()]
         self.precision = precision
+        # only use_timestep when skip connection is established.
+        use_timestep = use_timestep and (num_out == num_in or num_out == num_in * 2)
         rng = np.random.default_rng()
         self.w = rng.normal(size=(num_in, num_out)).astype(prec)
         self.b = rng.normal(size=(num_out,)).astype(prec) if bias else None
         self.idt = rng.normal(size=(num_out,)).astype(prec) if use_timestep else None
         self.activation_function = (
             activation_function if activation_function is not None else "none"
         )
@@ -182,32 +189,37 @@
         """
         data = {
             "w": self.w,
             "b": self.b,
             "idt": self.idt,
         }
         return {
+            "@class": "Layer",
+            "@version": 1,
             "bias": self.b is not None,
             "use_timestep": self.idt is not None,
             "activation_function": self.activation_function,
             "resnet": self.resnet,
-            "precision": self.precision,
+            # make deterministic
+            "precision": np.dtype(PRECISION_DICT[self.precision]).name,
             "@variables": data,
         }
 
     @classmethod
     def deserialize(cls, data: dict) -> "NativeLayer":
         """Deserialize the layer from a dict.
 
         Parameters
         ----------
         data : dict
             The dict to deserialize from.
         """
         data = copy.deepcopy(data)
+        check_version_compatibility(data.pop("@version", 1), 1, 1)
+        data.pop("@class", None)
         variables = data.pop("@variables")
         assert variables["w"] is not None and len(variables["w"].shape) == 2
         num_in, num_out = variables["w"].shape
         obj = cls(
             num_in,
             num_out,
             **data,
@@ -341,25 +353,32 @@
             """Serialize the network to a dict.
 
             Returns
             -------
             dict
                 The serialized network.
             """
-            return {"layers": [layer.serialize() for layer in self.layers]}
+            return {
+                "@class": "NN",
+                "@version": 1,
+                "layers": [layer.serialize() for layer in self.layers],
+            }
 
         @classmethod
         def deserialize(cls, data: dict) -> "NN":
             """Deserialize the network from a dict.
 
             Parameters
             ----------
             data : dict
                 The dict to deserialize from.
             """
+            data = data.copy()
+            check_version_compatibility(data.pop("@version", 1), 1, 1)
+            data.pop("@class", None)
             return cls(data["layers"])
 
         def __getitem__(self, key):
             assert isinstance(key, int)
             return self.layers[key]
 
         def __setitem__(self, key, value):
@@ -388,14 +407,23 @@
             np.ndarray
                 The output.
             """
             for layer in self.layers:
                 x = layer(x)
             return x
 
+        def clear(self):
+            """Clear the network parameters to zero."""
+            for layer in self.layers:
+                layer.w.fill(0.0)
+                if layer.b is not None:
+                    layer.b.fill(0.0)
+                if layer.idt is not None:
+                    layer.idt.fill(0.0)
+
     return NN
 
 
 NativeNet = make_multilayer_network(NativeLayer, NativeOP)
 
 
 def make_embedding_network(T_Network, T_NetworkLayer):
@@ -454,32 +482,37 @@
 
             Returns
             -------
             dict
                 The serialized network.
             """
             return {
+                "@class": "EmbeddingNetwork",
+                "@version": 1,
                 "in_dim": self.in_dim,
                 "neuron": self.neuron.copy(),
                 "activation_function": self.activation_function,
                 "resnet_dt": self.resnet_dt,
-                "precision": self.precision,
+                # make deterministic
+                "precision": np.dtype(PRECISION_DICT[self.precision]).name,
                 "layers": [layer.serialize() for layer in self.layers],
             }
 
         @classmethod
         def deserialize(cls, data: dict) -> "EmbeddingNet":
             """Deserialize the network from a dict.
 
             Parameters
             ----------
             data : dict
                 The dict to deserialize from.
             """
             data = copy.deepcopy(data)
+            check_version_compatibility(data.pop("@version", 1), 1, 1)
+            data.pop("@class", None)
             layers = data.pop("layers")
             obj = cls(**data)
             super(EN, obj).__init__(layers)
             return obj
 
     return EN
 
@@ -548,14 +581,16 @@
 
             Returns
             -------
             dict
                 The serialized network.
             """
             return {
+                "@class": "FittingNetwork",
+                "@version": 1,
                 "in_dim": self.in_dim,
                 "out_dim": self.out_dim,
                 "neuron": self.neuron.copy(),
                 "activation_function": self.activation_function,
                 "resnet_dt": self.resnet_dt,
                 "precision": self.precision,
                 "bias_out": self.bias_out,
@@ -568,14 +603,16 @@
 
             Parameters
             ----------
             data : dict
                 The dict to deserialize from.
             """
             data = copy.deepcopy(data)
+            check_version_compatibility(data.pop("@version", 1), 1, 1)
+            data.pop("@class", None)
             layers = data.pop("layers")
             obj = cls(**data)
             T_Network.__init__(obj, layers)
             return obj
 
     return FN
 
@@ -670,14 +707,16 @@
         -------
         dict
             The serialized networks.
         """
         network_type_map_inv = {v: k for k, v in self.NETWORK_TYPE_MAP.items()}
         network_type_name = network_type_map_inv[self.network_type]
         return {
+            "@class": "NetworkCollection",
+            "@version": 1,
             "ndim": self.ndim,
             "ntypes": self.ntypes,
             "network_type": network_type_name,
             "networks": [nn.serialize() for nn in self._networks],
         }
 
     @classmethod
@@ -685,8 +724,11 @@
         """Deserialize the networks from a dict.
 
         Parameters
         ----------
         data : dict
             The dict to deserialize from.
         """
+        data = data.copy()
+        check_version_compatibility(data.pop("@version", 1), 1, 1)
+        data.pop("@class", None)
         return cls(**data)
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/argcheck.py` & `deepmd_kit-3.0.0a0/deepmd/utils/argcheck.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,49 @@
 from dargs import (
     Argument,
     ArgumentEncoder,
     Variant,
     dargs,
 )
 
-from deepmd.common import (
-    ACTIVATION_FN_DICT,
-    PRECISION_DICT,
-)
-from deepmd_utils.utils.argcheck_nvnmd import (
+from deepmd.utils.argcheck_nvnmd import (
     nvnmd_args,
 )
-from deepmd_utils.utils.plugin import (
+from deepmd.utils.plugin import (
     Plugin,
 )
 
 log = logging.getLogger(__name__)
 
 
+# TODO: import from a module outside tf/pt
+ACTIVATION_FN_DICT = {
+    "relu": None,
+    "relu6": None,
+    "softplus": None,
+    "sigmoid": None,
+    "tanh": None,
+    "gelu": None,
+    "gelu_tf": None,
+    "None": None,
+    "none": None,
+}
+# TODO: import from a module outside tf/pt
+PRECISION_DICT = {
+    "default": None,
+    "float16": None,
+    "float32": None,
+    "float64": None,
+    "bfloat16": None,
+}
+
+doc_only_tf_supported = "(Supported Backend: TensorFlow) "
+doc_only_pt_supported = "(Supported Backend: PyTorch) "
+
+
 def list_to_doc(xx):
     items = []
     for ii in xx:
         if len(items) == 0:
             items.append(f'"{ii}"')
         else:
             items.append(f', "{ii}"')
@@ -87,15 +108,15 @@
 
 
 class ArgsPlugin:
     def __init__(self) -> None:
         self.__plugin = Plugin()
 
     def register(
-        self, name: str, alias: Optional[List[str]] = None
+        self, name: str, alias: Optional[List[str]] = None, doc: str = ""
     ) -> Callable[[], List[Argument]]:
         """Register a descriptor argument plugin.
 
         Parameters
         ----------
         name : str
             the name of a descriptor
@@ -113,15 +134,15 @@
         >>> @some_plugin.register("some_descrpt")
             def descrpt_some_descrpt_args():
                 return []
         """
         # convert alias to hashed item
         if isinstance(alias, list):
             alias = tuple(alias)
-        return self.__plugin.register((name, alias))
+        return self.__plugin.register((name, alias, doc))
 
     def get_all_argument(self, exclude_hybrid: bool = False) -> List[Argument]:
         """Get all arguments.
 
         Parameters
         ----------
         exclude_hybrid : bool
@@ -129,27 +150,27 @@
 
         Returns
         -------
         List[Argument]
             all arguments
         """
         arguments = []
-        for (name, alias), metd in self.__plugin.plugins.items():
+        for (name, alias, doc), metd in self.__plugin.plugins.items():
             if exclude_hybrid and name == "hybrid":
                 continue
             arguments.append(
-                Argument(name=name, dtype=dict, sub_fields=metd(), alias=alias)
+                Argument(name=name, dtype=dict, sub_fields=metd(), alias=alias, doc=doc)
             )
         return arguments
 
 
 descrpt_args_plugin = ArgsPlugin()
 
 
-@descrpt_args_plugin.register("loc_frame")
+@descrpt_args_plugin.register("loc_frame", doc=doc_only_tf_supported)
 def descrpt_local_frame_args():
     doc_sel_a = "A list of integers. The length of the list should be the same as the number of atom types in the system. `sel_a[i]` gives the selected number of type-i neighbors. The full relative coordinates of the neighbors are used by the descriptor."
     doc_sel_r = "A list of integers. The length of the list should be the same as the number of atom types in the system. `sel_r[i]` gives the selected number of type-i neighbors. Only relative distance of the neighbors are used by the descriptor. sel_a[i] + sel_r[i] is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius."
     doc_rcut = "The cut-off radius. The default value is 6.0"
     doc_axis_rule = "A list of integers. The length should be 6 times of the number of types. \n\n\
 - axis_rule[i*6+0]: class of the atom defining the first axis of type-i atom. 0 for neighbors with full coordinates and 1 for neighbors only with relative distance.\n\n\
 - axis_rule[i*6+1]: type of the atom defining the first axis of type-i atom.\n\n\
@@ -222,15 +243,17 @@
         ),
         Argument(
             "set_davg_zero", bool, optional=True, default=False, doc=doc_set_davg_zero
         ),
     ]
 
 
-@descrpt_args_plugin.register("se_e3", alias=["se_at", "se_a_3be", "se_t"])
+@descrpt_args_plugin.register(
+    "se_e3", alias=["se_at", "se_a_3be", "se_t"], doc=doc_only_tf_supported
+)
 def descrpt_se_t_args():
     doc_sel = 'This parameter set the number of selected neighbors for each type of atom. It can be:\n\n\
     - `List[int]`. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. `sel[i]` is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius. It is noted that the total sel value must be less than 4096 in a GPU environment.\n\n\
     - `str`. Can be "auto:factor" or "auto". "factor" is a float number larger than 1. This option will automatically determine the `sel`. In detail it counts the maximal number of neighbors with in the cutoff radius for each type of neighbor, then multiply the maximum by the "factor". Finally the number is wraped up to 4 divisible. The option "auto" is equivalent to "auto:1.1".'
     doc_rcut = "The cut-off radius."
     doc_rcut_smth = "Where to start smoothing. For example the 1/r term is smoothed from `rcut` to `rcut_smth`"
     doc_neuron = "Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built."
@@ -261,15 +284,15 @@
         Argument("seed", [int, None], optional=True, doc=doc_seed),
         Argument(
             "set_davg_zero", bool, optional=True, default=False, doc=doc_set_davg_zero
         ),
     ]
 
 
-@descrpt_args_plugin.register("se_a_tpe", alias=["se_a_ebd"])
+@descrpt_args_plugin.register("se_a_tpe", alias=["se_a_ebd"], doc=doc_only_tf_supported)
 def descrpt_se_a_tpe_args():
     doc_type_nchanl = "number of channels for type embedding"
     doc_type_nlayer = "number of hidden layers of type embedding net"
     doc_numb_aparam = "dimension of atomic parameter. if set to a value > 0, the atomic parameters are embedded."
 
     return [
         *descrpt_se_a_args(),
@@ -354,20 +377,33 @@
     - `List[int]`. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. Only the summation of `sel[i]` matters, and it is recommended to be less than 200.\
     - `str`. Can be "auto:factor" or "auto". "factor" is a float number larger than 1. This option will automatically determine the `sel`. In detail it counts the maximal number of neighbors with in the cutoff radius for each type of neighbor, then multiply the maximum by the "factor". Finally the number is wraped up to 4 divisible. The option "auto" is equivalent to "auto:1.1".'
     doc_rcut = "The cut-off radius."
     doc_rcut_smth = "Where to start smoothing. For example the 1/r term is smoothed from `rcut` to `rcut_smth`"
     doc_neuron = "Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built."
     doc_axis_neuron = "Size of the submatrix of G (embedding matrix)."
     doc_activation_function = f'The activation function in the embedding net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())} Note that "gelu" denotes the custom operator version, and "gelu_tf" denotes the TF standard version. If you set "None" or "none" here, no activation function will be used.'
-    doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
-    doc_type_one_side = r"If true, the embedding network parameters vary by types of neighbor atoms only, so there will be $N_\text{types}$ sets of embedding network parameters. Otherwise, the embedding network parameters vary by types of centric atoms and types of neighbor atoms, so there will be $N_\text{types}^2$ sets of embedding network parameters."
-    doc_precision = f"The precision of the embedding net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())} Default follows the interface precision."
-    doc_trainable = "If the parameters in the embedding net is trainable"
+    doc_resnet_dt = (
+        doc_only_tf_supported + 'Whether to use a "Timestep" in the skip connection'
+    )
+    doc_type_one_side = (
+        doc_only_tf_supported
+        + r"If true, the embedding network parameters vary by types of neighbor atoms only, so there will be $N_\text{types}$ sets of embedding network parameters. Otherwise, the embedding network parameters vary by types of centric atoms and types of neighbor atoms, so there will be $N_\text{types}^2$ sets of embedding network parameters."
+    )
+    doc_precision = (
+        doc_only_tf_supported
+        + f"The precision of the embedding net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())} Default follows the interface precision."
+    )
+    doc_trainable = (
+        doc_only_tf_supported + "If the parameters in the embedding net is trainable"
+    )
     doc_seed = "Random seed for parameter initialization"
-    doc_exclude_types = "The excluded pairs of types which have no interaction with each other. For example, `[[0, 1]]` means no interaction between type 0 and type 1."
+    doc_exclude_types = (
+        doc_only_tf_supported
+        + "The excluded pairs of types which have no interaction with each other. For example, `[[0, 1]]` means no interaction between type 0 and type 1."
+    )
     doc_attn = "The length of hidden vectors in attention layers"
     doc_attn_layer = "The number of attention layers. Note that model compression of `se_atten` is only enabled when attn_layer==0 and stripped_type_embedding is True"
     doc_attn_dotr = "Whether to do dot product with the normalized relative coordinates"
     doc_attn_mask = "Whether to do mask on the diagonal in the attention matrix"
 
     return [
         Argument(
@@ -410,60 +446,411 @@
         Argument("attn", int, optional=True, default=128, doc=doc_attn),
         Argument("attn_layer", int, optional=True, default=2, doc=doc_attn_layer),
         Argument("attn_dotr", bool, optional=True, default=True, doc=doc_attn_dotr),
         Argument("attn_mask", bool, optional=True, default=False, doc=doc_attn_mask),
     ]
 
 
-@descrpt_args_plugin.register("se_atten")
+@descrpt_args_plugin.register("se_atten", alias=["dpa1"])
 def descrpt_se_atten_args():
     doc_stripped_type_embedding = "Whether to strip the type embedding into a separated embedding network. Setting it to `False` will fall back to the previous version of `se_atten` which is non-compressible."
     doc_smooth_type_embdding = "When using stripped type embedding, whether to dot smooth factor on the network output of type embedding to keep the network smooth, instead of setting `set_davg_zero` to be True."
     doc_set_davg_zero = "Set the normalization average to zero. This option should be set when `se_atten` descriptor or `atom_ener` in the energy fitting is used"
+    doc_tebd_dim = "The dimension of atom type embedding."
+    doc_temperature = "The scaling factor of normalization in calculations of attention weights, which is used to scale the matmul(Q, K)."
+    doc_scaling_factor = (
+        "The scaling factor of normalization in calculations of attention weights, which is used to scale the matmul(Q, K). "
+        "If `temperature` is None, the scaling of attention weights is (N_hidden_dim * scaling_factor)**0.5. "
+        "Else, the scaling of attention weights is setting to `temperature`."
+    )
+    doc_normalize = (
+        "Whether to normalize the hidden vectors during attention calculation."
+    )
+    doc_concat_output_tebd = (
+        "Whether to concat type embedding at the output of the descriptor."
+    )
+    doc_deprecated = "This feature will be removed in a future release."
 
     return [
         *descrpt_se_atten_common_args(),
         Argument(
             "stripped_type_embedding",
             bool,
             optional=True,
             default=False,
-            doc=doc_stripped_type_embedding,
+            doc=doc_only_tf_supported + doc_stripped_type_embedding,
         ),
         Argument(
             "smooth_type_embdding",
             bool,
             optional=True,
             default=False,
-            doc=doc_smooth_type_embdding,
+            doc=doc_only_tf_supported + doc_smooth_type_embdding,
         ),
         Argument(
             "set_davg_zero", bool, optional=True, default=True, doc=doc_set_davg_zero
         ),
+        # pt only
+        Argument(
+            "tebd_dim",
+            int,
+            optional=True,
+            default=8,
+            doc=doc_only_pt_supported + doc_tebd_dim,
+        ),
+        Argument(
+            "tebd_input_mode",
+            str,
+            optional=True,
+            default="concat",
+            doc=doc_only_pt_supported + doc_deprecated,
+        ),
+        Argument(
+            "post_ln",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_only_pt_supported + doc_deprecated,
+        ),
+        Argument(
+            "ffn",
+            bool,
+            optional=True,
+            default=False,
+            doc=doc_only_pt_supported + doc_deprecated,
+        ),
+        Argument(
+            "ffn_embed_dim",
+            int,
+            optional=True,
+            default=1024,
+            doc=doc_only_pt_supported + doc_deprecated,
+        ),
+        Argument(
+            "scaling_factor",
+            float,
+            optional=True,
+            default=1.0,
+            doc=doc_only_pt_supported + doc_scaling_factor,
+        ),
+        Argument(
+            "head_num",
+            int,
+            optional=True,
+            default=1,
+            doc=doc_only_pt_supported + doc_deprecated,
+        ),
+        Argument(
+            "normalize",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_only_pt_supported + doc_normalize,
+        ),
+        Argument(
+            "temperature",
+            float,
+            optional=True,
+            doc=doc_only_pt_supported + doc_temperature,
+        ),
+        Argument(
+            "return_rot",
+            bool,
+            optional=True,
+            default=False,
+            doc=doc_only_pt_supported + doc_deprecated,
+        ),
+        Argument(
+            "concat_output_tebd",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_only_pt_supported + doc_concat_output_tebd,
+        ),
     ]
 
 
-@descrpt_args_plugin.register("se_atten_v2")
+@descrpt_args_plugin.register("se_atten_v2", doc=doc_only_tf_supported)
 def descrpt_se_atten_v2_args():
     doc_set_davg_zero = "Set the normalization average to zero. This option should be set when `se_atten` descriptor or `atom_ener` in the energy fitting is used"
 
     return [
         *descrpt_se_atten_common_args(),
         Argument(
             "set_davg_zero", bool, optional=True, default=False, doc=doc_set_davg_zero
         ),
     ]
 
 
-@descrpt_args_plugin.register("se_a_ebd_v2", alias=["se_a_tpe_v2"])
+@descrpt_args_plugin.register("dpa2", doc=doc_only_pt_supported)
+def descrpt_dpa2_args():
+    # Generate by GitHub Copilot
+    doc_repinit_rcut = "The cut-off radius of the repinit block"
+    doc_repinit_rcut_smth = "From this position the inverse distance smoothly decays to 0 at the cut-off. Use in the repinit block."
+    doc_repinit_nsel = "Maximally possible number of neighbors for repinit block."
+    doc_repformer_rcut = "The cut-off radius of the repformer block"
+    doc_repformer_rcut_smth = "From this position the inverse distance smoothly decays to 0 at the cut-off. Use in the repformer block."
+    doc_repformer_nsel = "Maximally possible number of neighbors for repformer block."
+    doc_tebd_dim = "The dimension of atom type embedding"
+    doc_concat_output_tebd = (
+        "Whether to concat type embedding at the output of the descriptor."
+    )
+    doc_repinit_neuron = "repinit block: the number of neurons in the embedding net."
+    doc_repinit_axis_neuron = (
+        "repinit block: the number of dimension of split in the symmetrization op."
+    )
+    doc_repinit_activation = (
+        "repinit block: the activation function in the embedding net"
+    )
+    doc_repformer_nlayers = "repformers block: the number of repformer layers"
+    doc_repformer_g1_dim = "repformers block: the dimension of single-atom rep"
+    doc_repformer_g2_dim = "repformers block: the dimension of invariant pair-atom rep"
+    doc_repformer_axis_dim = (
+        "repformers block: the number of dimension of split in the symmetrization ops."
+    )
+    doc_repformer_do_bn_mode = "repformers block: do batch norm in the repformer layers"
+    doc_repformer_bn_momentum = "repformers block: moment in the batch normalization"
+    doc_repformer_update_g1_has_conv = (
+        "repformers block: update the g1 rep with convolution term"
+    )
+    doc_repformer_update_g1_has_drrd = (
+        "repformers block: update the g1 rep with the drrd term"
+    )
+    doc_repformer_update_g1_has_grrg = (
+        "repformers block: update the g1 rep with the grrg term"
+    )
+    doc_repformer_update_g1_has_attn = (
+        "repformers block: update the g1 rep with the localized self-attention"
+    )
+    doc_repformer_update_g2_has_g1g1 = (
+        "repformers block: update the g2 rep with the g1xg1 term"
+    )
+    doc_repformer_update_g2_has_attn = (
+        "repformers block: update the g2 rep with the gated self-attention"
+    )
+    doc_repformer_update_h2 = "repformers block: update the h2 rep"
+    doc_repformer_attn1_hidden = (
+        "repformers block: the hidden dimension of localized self-attention"
+    )
+    doc_repformer_attn1_nhead = (
+        "repformers block: the number of heads in localized self-attention"
+    )
+    doc_repformer_attn2_hidden = (
+        "repformers block: the hidden dimension of gated self-attention"
+    )
+    doc_repformer_attn2_nhead = (
+        "repformers block: the number of heads in gated self-attention"
+    )
+    doc_repformer_attn2_has_gate = (
+        "repformers block: has gate in the gated self-attention"
+    )
+    doc_repformer_activation = "repformers block: the activation function in the MLPs."
+    doc_repformer_update_style = "repformers block: style of update a rep. can be res_avg or res_incr. res_avg updates a rep `u` with: u = 1/\\sqrt{n+1} (u + u_1 + u_2 + ... + u_n) res_incr updates a rep `u` with: u = u + 1/\\sqrt{n} (u_1 + u_2 + ... + u_n)"
+    doc_repformer_set_davg_zero = "repformers block: set the avg to zero in statistics"
+    doc_repformer_add_type_ebd_to_seq = (
+        "repformers block: concatenate the type embedding at the output"
+    )
+    return [
+        Argument("repinit_rcut", float, doc=doc_repinit_rcut),
+        Argument("repinit_rcut_smth", float, doc=doc_repinit_rcut_smth),
+        Argument("repinit_nsel", int, doc=doc_repinit_nsel),
+        Argument("repformer_rcut", float, doc=doc_repformer_rcut),
+        Argument("repformer_rcut_smth", float, doc=doc_repformer_rcut_smth),
+        Argument("repformer_nsel", int, doc=doc_repformer_nsel),
+        Argument("tebd_dim", int, optional=True, default=8, doc=doc_tebd_dim),
+        Argument(
+            "concat_output_tebd",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_concat_output_tebd,
+        ),
+        Argument(
+            "repinit_neuron",
+            list,
+            optional=True,
+            default=[25, 50, 100],
+            doc=doc_repinit_neuron,
+        ),
+        Argument(
+            "repinit_axis_neuron",
+            int,
+            optional=True,
+            default=16,
+            doc=doc_repinit_axis_neuron,
+        ),
+        Argument("repinit_set_davg_zero", bool, optional=True, default=True),
+        Argument(
+            "repinit_activation",
+            str,
+            optional=True,
+            default="tanh",
+            doc=doc_repinit_activation,
+        ),
+        Argument(
+            "repformer_nlayers",
+            int,
+            optional=True,
+            default=3,
+            doc=doc_repformer_nlayers,
+        ),
+        Argument(
+            "repformer_g1_dim",
+            int,
+            optional=True,
+            default=128,
+            doc=doc_repformer_g1_dim,
+        ),
+        Argument(
+            "repformer_g2_dim", int, optional=True, default=16, doc=doc_repformer_g2_dim
+        ),
+        Argument(
+            "repformer_axis_dim",
+            int,
+            optional=True,
+            default=4,
+            doc=doc_repformer_axis_dim,
+        ),
+        Argument(
+            "repformer_do_bn_mode",
+            str,
+            optional=True,
+            default="no",
+            doc=doc_repformer_do_bn_mode,
+        ),
+        Argument(
+            "repformer_bn_momentum",
+            float,
+            optional=True,
+            default=0.1,
+            doc=doc_repformer_bn_momentum,
+        ),
+        Argument(
+            "repformer_update_g1_has_conv",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_repformer_update_g1_has_conv,
+        ),
+        Argument(
+            "repformer_update_g1_has_drrd",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_repformer_update_g1_has_drrd,
+        ),
+        Argument(
+            "repformer_update_g1_has_grrg",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_repformer_update_g1_has_grrg,
+        ),
+        Argument(
+            "repformer_update_g1_has_attn",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_repformer_update_g1_has_attn,
+        ),
+        Argument(
+            "repformer_update_g2_has_g1g1",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_repformer_update_g2_has_g1g1,
+        ),
+        Argument(
+            "repformer_update_g2_has_attn",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_repformer_update_g2_has_attn,
+        ),
+        Argument(
+            "repformer_update_h2",
+            bool,
+            optional=True,
+            default=False,
+            doc=doc_repformer_update_h2,
+        ),
+        Argument(
+            "repformer_attn1_hidden",
+            int,
+            optional=True,
+            default=64,
+            doc=doc_repformer_attn1_hidden,
+        ),
+        Argument(
+            "repformer_attn1_nhead",
+            int,
+            optional=True,
+            default=4,
+            doc=doc_repformer_attn1_nhead,
+        ),
+        Argument(
+            "repformer_attn2_hidden",
+            int,
+            optional=True,
+            default=16,
+            doc=doc_repformer_attn2_hidden,
+        ),
+        Argument(
+            "repformer_attn2_nhead",
+            int,
+            optional=True,
+            default=4,
+            doc=doc_repformer_attn2_nhead,
+        ),
+        Argument(
+            "repformer_attn2_has_gate",
+            bool,
+            optional=True,
+            default=False,
+            doc=doc_repformer_attn2_has_gate,
+        ),
+        Argument(
+            "repformer_activation",
+            str,
+            optional=True,
+            default="tanh",
+            doc=doc_repformer_activation,
+        ),
+        Argument(
+            "repformer_update_style",
+            str,
+            optional=True,
+            default="res_avg",
+            doc=doc_repformer_update_style,
+        ),
+        Argument(
+            "repformer_set_davg_zero",
+            bool,
+            optional=True,
+            default=True,
+            doc=doc_repformer_set_davg_zero,
+        ),
+        Argument(
+            "repformer_add_type_ebd_to_seq",
+            bool,
+            optional=True,
+            default=False,
+            doc=doc_repformer_add_type_ebd_to_seq,
+        ),
+    ]
+
+
+@descrpt_args_plugin.register(
+    "se_a_ebd_v2", alias=["se_a_tpe_v2"], doc=doc_only_tf_supported
+)
 def descrpt_se_a_ebd_v2_args():
     return descrpt_se_a_args()
 
 
-@descrpt_args_plugin.register("se_a_mask")
+@descrpt_args_plugin.register("se_a_mask", doc=doc_only_tf_supported)
 def descrpt_se_a_mask_args():
     doc_sel = 'This parameter sets the number of selected neighbors for each type of atom. It can be:\n\n\
     - `List[int]`. The length of the list should be the same as the number of atom types in the system. `sel[i]` gives the selected number of type-i neighbors. `sel[i]` is recommended to be larger than the maximally possible number of type-i neighbors in the cut-off radius. It is noted that the total sel value must be less than 4096 in a GPU environment.\n\n\
     - `str`. Can be "auto:factor" or "auto". "factor" is a float number larger than 1. This option will automatically determine the `sel`. In detail it counts the maximal number of neighbors with in the cutoff radius for each type of neighbor, then multiply the maximum by the "factor". Finally the number is wraped up to 4 divisible. The option "auto" is equivalent to "auto:1.1".'
 
     doc_neuron = "Number of neurons in each hidden layers of the embedding net. When two layers are of the same size or one layer is twice as large as the previous layer, a skip connection is built."
     doc_axis_neuron = "Size of the submatrix of G (embedding matrix)."
@@ -547,17 +934,17 @@
 def fitting_ener():
     doc_numb_fparam = "The dimension of the frame parameter. If set to >0, file `fparam.npy` should be included to provided the input fparams."
     doc_numb_aparam = "The dimension of the atomic parameter. If set to >0, file `aparam.npy` should be included to provided the input aparams."
     doc_neuron = "The number of neurons in each hidden layers of the fitting net. When two hidden layers are of the same size, a skip connection is built."
     doc_activation_function = f'The activation function in the fitting net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())} Note that "gelu" denotes the custom operator version, and "gelu_tf" denotes the TF standard version. If you set "None" or "none" here, no activation function will be used.'
     doc_precision = f"The precision of the fitting net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())} Default follows the interface precision."
     doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
-    doc_trainable = "Whether the parameters in the fitting net are trainable. This option can be\n\n\
+    doc_trainable = f"Whether the parameters in the fitting net are trainable. This option can be\n\n\
 - bool: True if all parameters of the fitting net are trainable, False otherwise.\n\n\
-- list of bool: Specifies if each layer is trainable. Since the fitting net is composed by hidden layers followed by a output layer, the length of this list should be equal to len(`neuron`)+1."
+- list of bool{doc_only_tf_supported}: Specifies if each layer is trainable. Since the fitting net is composed by hidden layers followed by a output layer, the length of this list should be equal to len(`neuron`)+1."
     doc_rcond = "The condition number used to determine the inital energy shift for each type of atoms. See `rcond` in :py:meth:`numpy.linalg.lstsq` for more details."
     doc_seed = "Random seed for parameter initialization of the fitting net"
     doc_atom_ener = "Specify the atomic energy in vacuum for each type"
     doc_layer_name = (
         "The name of the each layer. The length of this list should be equal to n_neuron + 1. "
         "If two layers, either in the same fitting or different fittings, "
         "have the same name, they will share the same neural network parameters. "
@@ -615,15 +1002,15 @@
             optional=True,
             default=False,
             doc=doc_use_aparam_as_mask,
         ),
     ]
 
 
-@fitting_args_plugin.register("dos")
+@fitting_args_plugin.register("dos", doc=doc_only_tf_supported)
 def fitting_dos():
     doc_numb_fparam = "The dimension of the frame parameter. If set to >0, file `fparam.npy` should be included to provided the input fparams."
     doc_numb_aparam = "The dimension of the atomic parameter. If set to >0, file `aparam.npy` should be included to provided the input aparams."
     doc_neuron = "The number of neurons in each hidden layers of the fitting net. When two hidden layers are of the same size, a skip connection is built."
     doc_activation_function = f'The activation function in the fitting net. Supported activation functions are {list_to_doc(ACTIVATION_FN_DICT.keys())} Note that "gelu" denotes the custom operator version, and "gelu_tf" denotes the TF standard version. If you set "None" or "none" here, no activation function will be used.'
     doc_precision = f"The precision of the fitting net parameters, supported options are {list_to_doc(PRECISION_DICT.keys())} Default follows the interface precision."
     doc_resnet_dt = 'Whether to use a "Timestep" in the skip connection'
@@ -706,15 +1093,15 @@
         # Argument("diag_shift", [list,float], optional = True, default = 0.0, doc = doc_diag_shift),
         Argument("shift_diag", bool, optional=True, default=True, doc=doc_shift_diag),
         Argument(
             "sel_type",
             [List[int], int, None],
             optional=True,
             alias=["pol_type"],
-            doc=doc_sel_type,
+            doc=doc_sel_type + doc_only_tf_supported,
         ),
         Argument("seed", [int, None], optional=True, doc=doc_seed),
     ]
 
 
 # def fitting_global_polar():
 #    return fitting_polar()
@@ -747,15 +1134,15 @@
         Argument("resnet_dt", bool, optional=True, default=True, doc=doc_resnet_dt),
         Argument("precision", str, optional=True, default="default", doc=doc_precision),
         Argument(
             "sel_type",
             [List[int], int, None],
             optional=True,
             alias=["dipole_type"],
-            doc=doc_sel_type,
+            doc=doc_sel_type + doc_only_tf_supported,
         ),
         Argument("seed", [int, None], optional=True, doc=doc_seed),
     ]
 
 
 #   YWolfeee: Delete global polar mode, merge it into polar mode and use loss setting to support.
 def fitting_variant_type_args():
@@ -844,14 +1231,17 @@
     doc_use_srtab = "The table for the short-range pairwise interaction added on top of DP. The table is a text data file with (N_t + 1) * N_t / 2 + 1 columes. The first colume is the distance between atoms. The second to the last columes are energies for pairs of certain types. For example we have two atom types, 0 and 1. The columes from 2nd to 4th are for 0-0, 0-1 and 1-1 correspondingly."
     doc_smin_alpha = "The short-range tabulated interaction will be swithed according to the distance of the nearest neighbor. This distance is calculated by softmin. This parameter is the decaying parameter in the softmin. It is only required when `use_srtab` is provided."
     doc_sw_rmin = "The lower boundary of the interpolation between short-range tabulated interaction and DP. It is only required when `use_srtab` is provided."
     doc_sw_rmax = "The upper boundary of the interpolation between short-range tabulated interaction and DP. It is only required when `use_srtab` is provided."
     doc_srtab_add_bias = "Whether add energy bias from the statistics of the data to short-range tabulated atomic energy. It only takes effect when `use_srtab` is provided."
     doc_compress_config = "Model compression configurations"
     doc_spin = "The settings for systems with spin."
+    doc_atom_exclude_types = "Exclude the atomic contribution of the listed atom types"
+    doc_pair_exclude_types = "The atom pairs of the listed types are not treated to be neighbors, i.e. they do not see each other."
+
     hybrid_models = []
     if not exclude_hybrid:
         hybrid_models.extend(
             [
                 pairwise_dprc(),
                 linear_ener_model_args(),
             ]
@@ -878,48 +1268,76 @@
             Argument(
                 "data_bias_nsample",
                 int,
                 optional=True,
                 default=10,
                 doc=doc_data_bias_nsample,
             ),
-            Argument("use_srtab", str, optional=True, doc=doc_use_srtab),
-            Argument("smin_alpha", float, optional=True, doc=doc_smin_alpha),
-            Argument("sw_rmin", float, optional=True, doc=doc_sw_rmin),
-            Argument("sw_rmax", float, optional=True, doc=doc_sw_rmax),
+            Argument(
+                "use_srtab",
+                str,
+                optional=True,
+                doc=doc_only_tf_supported + doc_use_srtab,
+            ),
+            Argument(
+                "smin_alpha",
+                float,
+                optional=True,
+                doc=doc_only_tf_supported + doc_smin_alpha,
+            ),
+            Argument(
+                "sw_rmin", float, optional=True, doc=doc_only_tf_supported + doc_sw_rmin
+            ),
+            Argument(
+                "sw_rmax", float, optional=True, doc=doc_only_tf_supported + doc_sw_rmax
+            ),
+            Argument(
+                "pair_exclude_types",
+                list,
+                optional=True,
+                default=[],
+                doc=doc_only_pt_supported + doc_pair_exclude_types,
+            ),
+            Argument(
+                "atom_exclude_types",
+                list,
+                optional=True,
+                default=[],
+                doc=doc_only_pt_supported + doc_atom_exclude_types,
+            ),
             Argument(
                 "srtab_add_bias",
                 bool,
                 optional=True,
                 default=True,
-                doc=doc_srtab_add_bias,
+                doc=doc_only_tf_supported + doc_srtab_add_bias,
             ),
             Argument(
                 "type_embedding",
                 dict,
                 type_embedding_args(),
                 [],
                 optional=True,
-                doc=doc_type_embedding,
+                doc=doc_only_tf_supported + doc_type_embedding,
             ),
             Argument(
                 "modifier",
                 dict,
                 [],
                 [modifier_variant_type_args()],
                 optional=True,
-                doc=doc_modifier,
+                doc=doc_only_tf_supported + doc_modifier,
             ),
             Argument(
                 "compress",
                 dict,
                 [],
                 [model_compression_type_args()],
                 optional=True,
-                doc=doc_compress_config,
+                doc=doc_only_tf_supported + doc_compress_config,
                 fold_subdoc=True,
             ),
             Argument("spin", dict, spin_args(), [], optional=True, doc=doc_spin),
         ],
         [
             Variant(
                 "type",
@@ -975,15 +1393,15 @@
                 [],
                 [descrpt_variant_type_args()],
                 doc=doc_descrpt,
                 fold_subdoc=True,
             ),
             Argument("fitting_net_dict", dict, doc=doc_fitting_net_dict),
         ],
-        doc="Multiple-task model.",
+        doc=doc_only_tf_supported + "Multiple-task model.",
     )
     return ca
 
 
 def pairwise_dprc() -> Argument:
     qm_model_args = model_args(exclude_hybrid=True)
     qm_model_args.name = "qm_model"
@@ -994,26 +1412,28 @@
     ca = Argument(
         "pairwise_dprc",
         dict,
         [
             qm_model_args,
             qmmm_model_args,
         ],
+        doc=doc_only_tf_supported,
     )
     return ca
 
 
 def frozen_model_args() -> Argument:
     doc_model_file = "Path to the frozen model file."
     ca = Argument(
         "frozen",
         dict,
         [
             Argument("model_file", str, optional=False, doc=doc_model_file),
         ],
+        doc=doc_only_tf_supported,
     )
     return ca
 
 
 def pairtab_model_args() -> Argument:
     doc_tab_file = "Path to the tabulation file."
     doc_rcut = "The cut-off radius."
@@ -1025,15 +1445,15 @@
         "pairtab",
         dict,
         [
             Argument("tab_file", str, optional=False, doc=doc_tab_file),
             Argument("rcut", float, optional=False, doc=doc_rcut),
             Argument("sel", [int, List[int], str], optional=False, doc=doc_sel),
         ],
-        doc="Pairwise tabulation energy model.",
+        doc=doc_only_tf_supported + "Pairwise tabulation energy model.",
     )
     return ca
 
 
 def linear_ener_model_args() -> Argument:
     doc_weights = (
         "If the type is list of float, a list of weights for each model. "
@@ -1054,14 +1474,15 @@
             Argument(
                 "weights",
                 [list, str],
                 optional=False,
                 doc=doc_weights,
             ),
         ],
+        doc=doc_only_tf_supported,
     )
     return ca
 
 
 #  --- Learning rate configurations: --- #
 def learning_rate_exp():
     doc_start_lr = "The learning rate at the start of the training."
@@ -1368,15 +1789,15 @@
             optional=True,
             default=False,
             doc=doc_enable_atom_ener_coeff,
         ),
     ]
 
 
-@loss_args_plugin.register("dos")
+@loss_args_plugin.register("dos", doc=doc_only_tf_supported)
 def loss_dos():
     doc_start_pref_dos = start_pref("Density of State (DOS)")
     doc_limit_pref_dos = limit_pref("Density of State (DOS)")
     doc_start_pref_cdf = start_pref(
         "Cumulative Distribution Function (cumulative intergral of DOS)"
     )
     doc_limit_pref_cdf = limit_pref(
@@ -1443,15 +1864,15 @@
             default=0.00,
             doc=doc_limit_pref_acdf,
         ),
     ]
 
 
 # YWolfeee: Modified to support tensor type of loss args.
-@loss_args_plugin.register("tensor")
+@loss_args_plugin.register("tensor", doc=doc_only_tf_supported)
 def loss_tensor():
     # doc_global_weight = "The prefactor of the weight of global loss. It should be larger than or equal to 0. If only `pref` is provided or both are not provided, training will be global mode, i.e. the shape of 'polarizability.npy` or `dipole.npy` should be #frams x [9 or 3]."
     # doc_local_weight =  "The prefactor of the weight of atomic loss. It should be larger than or equal to 0. If only `pref_atomic` is provided, training will be atomic mode, i.e. the shape of `polarizability.npy` or `dipole.npy` should be #frames x ([9 or 3] x #selected atoms). If both `pref` and `pref_atomic` are provided, training will be combined mode, and atomic label should be provided as well."
     doc_global_weight = "The prefactor of the weight of global loss. It should be larger than or equal to 0. If controls the weight of loss corresponding to global label, i.e. 'polarizability.npy` or `dipole.npy`, whose shape should be #frames x [9 or 3]. If it's larger than 0.0, this npy should be included."
     doc_local_weight = "The prefactor of the weight of atomic loss. It should be larger than or equal to 0. If controls the weight of loss corresponding to atomic label, i.e. `atomic_polarizability.npy` or `atomic_dipole.npy`, whose shape should be #frames x ([9 or 3] x #selected atoms). If it's larger than 0.0, this npy should be included. Both `pref` and `pref_atomic` should be provided, and either can be set to 0.0."
     return [
         Argument(
@@ -1681,15 +2102,15 @@
     doc_disp_freq = "The frequency of printing learning curve."
     doc_save_freq = "The frequency of saving check point."
     doc_save_ckpt = "The path prefix of saving check point files."
     doc_disp_training = "Displaying verbose information during training."
     doc_time_training = "Timing durining training."
     doc_profiling = "Profiling during training."
     doc_profiling_file = "Output file for profiling."
-    doc_enable_profiler = "Enable TensorFlow Profiler (available in TensorFlow 2.3) to analyze performance. The log will be saved to `tensorboard_log_dir`."
+    doc_enable_profiler = "Enable TensorFlow Profiler (available in TensorFlow 2.3) or PyTorch Profiler to analyze performance. The log will be saved to `tensorboard_log_dir`."
     doc_tensorboard = "Enable tensorboard"
     doc_tensorboard_log_dir = "The log directory of tensorboard outputs"
     doc_tensorboard_freq = "The frequency of writing tensorboard events."
     doc_data_dict = (
         "The dictionary of multi DataSystems in multi-task mode. "
         "Each data_dict[fitting_key], with user-defined name `fitting_key` in `model/fitting_net_dict`, "
         "contains training data and optional validation data definitions."
@@ -1697,14 +2118,31 @@
     doc_fitting_weight = (
         "Each fitting_weight[fitting_key], with user-defined name `fitting_key` in `model/fitting_net_dict`, "
         "is the training weight of fitting net `fitting_key`. "
         "Fitting nets with higher weights will be selected with higher probabilities to be trained in one step. "
         "Weights will be normalized and minus ones will be ignored. "
         "If not set, each fitting net will be equally selected when training."
     )
+    doc_warmup_steps = (
+        "The number of steps for learning rate warmup. During warmup, "
+        "the learning rate begins at zero and progressively increases linearly to `start_lr`, "
+        "rather than starting directly from `start_lr`"
+    )
+    doc_gradient_max_norm = (
+        "Clips the gradient norm to a maximum value. "
+        "If the gradient norm exceeds this value, it will be clipped to this limit. "
+        "No gradient clipping will occur if set to 0."
+    )
+    doc_stat_file = (
+        "The file path for saving the data statistics results. "
+        "If set, the results will be saved and directly loaded during the next training session, "
+        "avoiding the need to recalculate the statistics"
+    )
+    doc_opt_type = "The type of optimizer to use."
+    doc_kf_blocksize = "The blocksize for the Kalman filter."
 
     arg_training_data = training_data_args()
     arg_validation_data = validation_data_args()
     mixed_precision_data = mixed_precision_args()
 
     args = [
         arg_training_data,
@@ -1724,21 +2162,27 @@
         ),
         Argument(
             "disp_training", bool, optional=True, default=True, doc=doc_disp_training
         ),
         Argument(
             "time_training", bool, optional=True, default=True, doc=doc_time_training
         ),
-        Argument("profiling", bool, optional=True, default=False, doc=doc_profiling),
+        Argument(
+            "profiling",
+            bool,
+            optional=True,
+            default=False,
+            doc=doc_only_tf_supported + doc_profiling,
+        ),
         Argument(
             "profiling_file",
             str,
             optional=True,
             default="timeline.json",
-            doc=doc_profiling_file,
+            doc=doc_only_tf_supported + doc_profiling_file,
         ),
         Argument(
             "enable_profiler",
             bool,
             optional=True,
             default=False,
             doc=doc_enable_profiler,
@@ -1754,18 +2198,58 @@
             doc=doc_tensorboard_log_dir,
         ),
         Argument(
             "tensorboard_freq", int, optional=True, default=1, doc=doc_tensorboard_freq
         ),
         Argument("data_dict", dict, optional=True, doc=doc_data_dict),
         Argument("fitting_weight", dict, optional=True, doc=doc_fitting_weight),
+        Argument(
+            "warmup_steps",
+            int,
+            optional=True,
+            doc=doc_only_pt_supported + doc_warmup_steps,
+        ),
+        Argument(
+            "gradient_max_norm",
+            float,
+            optional=True,
+            doc=doc_only_pt_supported + doc_gradient_max_norm,
+        ),
+        Argument(
+            "stat_file", str, optional=True, doc=doc_only_pt_supported + doc_stat_file
+        ),
+    ]
+    variants = [
+        Variant(
+            "opt_type",
+            choices=[
+                Argument("Adam", dict, [], [], optional=True),
+                Argument(
+                    "LKF",
+                    dict,
+                    [
+                        Argument(
+                            "kf_blocksize",
+                            int,
+                            optional=True,
+                            doc=doc_only_pt_supported + doc_kf_blocksize,
+                        ),
+                    ],
+                    [],
+                    optional=True,
+                ),
+            ],
+            optional=True,
+            default_tag="Adam",
+            doc=doc_only_pt_supported + doc_opt_type,
+        )
     ]
 
     doc_training = "The training options."
-    return Argument("training", dict, args, [], doc=doc_training)
+    return Argument("training", dict, args, variants, doc=doc_training)
 
 
 def make_index(keys):
     ret = []
     for ii in keys:
         ret.append(make_link(ii, ii))
     return ", ".join(ret)
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/argcheck_nvnmd.py` & `deepmd_kit-3.0.0a0/deepmd/utils/argcheck_nvnmd.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/batch_size.py` & `deepmd_kit-3.0.0a0/deepmd/utils/batch_size.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import (
     Callable,
     Tuple,
 )
 
 import numpy as np
 
-from deepmd_utils.utils.errors import (
+from deepmd.utils.errors import (
     OutOfMemoryError,
 )
 
 log = logging.getLogger(__name__)
 
 
 class AutoBatchSize(ABC):
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/compat.py` & `deepmd_kit-3.0.0a0/deepmd/utils/compat.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/data.py` & `deepmd_kit-3.0.0a0/deepmd/utils/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 
 # SPDX-License-Identifier: LGPL-3.0-or-later
+import bisect
 import logging
 from typing import (
     List,
     Optional,
 )
 
 import numpy as np
 
-from deepmd_utils.env import (
+from deepmd.env import (
     GLOBAL_ENER_FLOAT_PRECISION,
     GLOBAL_NP_FLOAT_PRECISION,
 )
-from deepmd_utils.utils import random as dp_random
-from deepmd_utils.utils.path import (
+from deepmd.utils import random as dp_random
+from deepmd.utils.path import (
     DPPath,
 )
 
 log = logging.getLogger(__name__)
 
 
 class DeepmdData:
@@ -125,26 +126,32 @@
         self.add("numb_copy", 1, must=False, default=1, dtype=int)
         # set counters
         self.set_count = 0
         self.iterator = 0
         self.shuffle_test = shuffle_test
         # set modifier
         self.modifier = modifier
+        # calculate prefix sum for get_item method
+        frames_list = [self._get_nframes(item) for item in self.dirs]
+        self.nframes = np.sum(frames_list)
+        # The prefix sum stores the range of indices contained in each directory, which is needed by get_item method
+        self.prefix_sum = np.cumsum(frames_list).tolist()
 
     def add(
         self,
         key: str,
         ndof: int,
         atomic: bool = False,
         must: bool = False,
         high_prec: bool = False,
         type_sel: Optional[List[int]] = None,
         repeat: int = 1,
         default: float = 0.0,
         dtype: Optional[np.dtype] = None,
+        output_natoms_for_type_sel: bool = False,
     ):
         """Add a data item that to be loaded.
 
         Parameters
         ----------
         key
             The key of the item. The corresponding data is stored in `sys_path/set.*/key.npy`
@@ -163,25 +170,28 @@
             Select certain type of atoms
         repeat
             The data will be repeated `repeat` times.
         default : float, default=0.
             default value of data
         dtype : np.dtype, optional
             the dtype of data, overwrites `high_prec` if provided
+        output_natoms_for_type_sel : bool, optional
+            if True and type_sel is True, the atomic dimension will be natoms instead of nsel
         """
         self.data_dict[key] = {
             "ndof": ndof,
             "atomic": atomic,
             "must": must,
             "high_prec": high_prec,
             "type_sel": type_sel,
             "repeat": repeat,
             "reduce": None,
             "default": default,
             "dtype": dtype,
+            "output_natoms_for_type_sel": output_natoms_for_type_sel,
         }
         return self
 
     def reduce(self, key_out: str, key_in: str):
         """Generate a new item from the reduction of another atom.
 
         Parameters
@@ -245,14 +255,29 @@
         if tmpe.ndim == 1:
             tmpe = tmpe.reshape([1, -1])
         if tmpe.shape[0] < test_size:
             return self.test_dir, tmpe.shape[0]
         else:
             return None
 
+    def get_item_torch(self, index: int) -> dict:
+        """Get a single frame data . The frame is picked from the data system by index. The index is coded across all the sets.
+
+        Parameters
+        ----------
+        index
+            index of the frame
+        """
+        i = bisect.bisect_right(self.prefix_sum, index)
+        frames = self._load_set(self.dirs[i])
+        frame = self._get_subdata(frames, index - self.prefix_sum[i])
+        frame = self.reformat_data_torch(frame)
+        frame["fid"] = index
+        return frame
+
     def get_batch(self, batch_size: int) -> dict:
         """Get a batch of data with `batch_size` frames. The frames are randomly picked from the data system.
 
         Parameters
         ----------
         batch_size
             size of the batch
@@ -436,14 +461,47 @@
                 and "find_" not in kk
             ):
                 ret[kk] = data[kk][idx]
             else:
                 ret[kk] = data[kk]
         return ret, idx
 
+    def _get_nframes(self, set_name: DPPath):
+        # get nframes
+        if not isinstance(set_name, DPPath):
+            set_name = DPPath(set_name)
+        path = set_name / "coord.npy"
+        if self.data_dict["coord"]["high_prec"]:
+            coord = path.load_numpy().astype(GLOBAL_ENER_FLOAT_PRECISION)
+        else:
+            coord = path.load_numpy().astype(GLOBAL_NP_FLOAT_PRECISION)
+        if coord.ndim == 1:
+            coord = coord.reshape([1, -1])
+        nframes = coord.shape[0]
+        return nframes
+
+    def reformat_data_torch(self, data):
+        """Modify the data format for the requirements of Torch backend.
+
+        Parameters
+        ----------
+        data
+            original data
+        """
+        for kk in self.data_dict.keys():
+            if "find_" in kk:
+                pass
+            else:
+                if self.data_dict[kk]["atomic"]:
+                    data[kk] = data[kk].reshape(-1, self.data_dict[kk]["ndof"])
+        data["atype"] = data["type"]
+        if not self.pbc:
+            data["box"] = None
+        return data
+
     def _load_set(self, set_name: DPPath):
         # get nframes
         if not isinstance(set_name, DPPath):
             set_name = DPPath(set_name)
         path = set_name / "coord.npy"
         if self.data_dict["coord"]["high_prec"]:
             coord = path.load_numpy().astype(GLOBAL_ENER_FLOAT_PRECISION)
@@ -465,14 +523,17 @@
                     atomic=self.data_dict[kk]["atomic"],
                     high_prec=self.data_dict[kk]["high_prec"],
                     must=self.data_dict[kk]["must"],
                     type_sel=self.data_dict[kk]["type_sel"],
                     repeat=self.data_dict[kk]["repeat"],
                     default=self.data_dict[kk]["default"],
                     dtype=self.data_dict[kk]["dtype"],
+                    output_natoms_for_type_sel=self.data_dict[kk][
+                        "output_natoms_for_type_sel"
+                    ],
                 )
         for kk in self.data_dict.keys():
             if self.data_dict[kk]["reduce"] is not None:
                 k_in = self.data_dict[kk]["reduce"]
                 ndof = self.data_dict[kk]["ndof"]
                 data["find_" + kk] = data["find_" + k_in]
                 tmp_in = data[k_in].astype(GLOBAL_ENER_FLOAT_PRECISION)
@@ -531,53 +592,93 @@
         atomic=False,
         must=True,
         repeat=1,
         high_prec=False,
         type_sel=None,
         default: float = 0.0,
         dtype: Optional[np.dtype] = None,
+        output_natoms_for_type_sel: bool = False,
     ):
         if atomic:
             natoms = self.natoms
             idx_map = self.idx_map
             # if type_sel, then revise natoms and idx_map
             if type_sel is not None:
-                natoms = 0
+                natoms_sel = 0
                 for jj in type_sel:
-                    natoms += np.sum(self.atom_type == jj)
-                idx_map = self._idx_map_sel(self.atom_type, type_sel)
+                    natoms_sel += np.sum(self.atom_type == jj)
+                idx_map_sel = self._idx_map_sel(self.atom_type, type_sel)
+            else:
+                natoms_sel = natoms
+                idx_map_sel = idx_map
             ndof = ndof_ * natoms
         else:
             ndof = ndof_
+            natoms_sel = 0
+            idx_map_sel = None
         if dtype is not None:
             pass
         elif high_prec:
             dtype = GLOBAL_ENER_FLOAT_PRECISION
         else:
             dtype = GLOBAL_NP_FLOAT_PRECISION
         path = set_name / (key + ".npy")
         if path.is_file():
             data = path.load_numpy().astype(dtype)
             try:  # YWolfeee: deal with data shape error
                 if atomic:
+                    if type_sel is not None:
+                        # check the data shape is nsel or natoms
+                        if data.size == nframes * natoms_sel * ndof_:
+                            if output_natoms_for_type_sel:
+                                tmp = np.zeros(
+                                    [nframes, natoms, ndof_], dtype=data.dtype
+                                )
+                                sel_mask = np.isin(self.atom_type, type_sel)
+                                tmp[:, sel_mask] = data.reshape(
+                                    [nframes, natoms_sel, ndof_]
+                                )
+                                data = tmp
+                            else:
+                                natoms = natoms_sel
+                                idx_map = idx_map_sel
+                                ndof = ndof_ * natoms
+                        elif data.size == nframes * natoms * ndof_:
+                            if output_natoms_for_type_sel:
+                                pass
+                            else:
+                                sel_mask = np.isin(self.atom_type, type_sel)
+                                data = data[:, sel_mask]
+                                natoms = natoms_sel
+                                idx_map = idx_map_sel
+                                ndof = ndof_ * natoms
+                        else:
+                            raise ValueError(
+                                f"The shape of the data {key} in {set_name}"
+                                f"is {data.shape}, which doesn't match either"
+                                f"({nframes}, {natoms_sel}, {ndof_}) or"
+                                f"({nframes}, {natoms}, {ndof_})"
+                            )
                     data = data.reshape([nframes, natoms, -1])
                     data = data[:, idx_map, :]
                     data = data.reshape([nframes, -1])
                 data = np.reshape(data, [nframes, ndof])
             except ValueError as err_message:
                 explanation = "This error may occur when your label mismatch it's name, i.e. you might store global tensor in `atomic_tensor.npy` or atomic tensor in `tensor.npy`."
                 log.error(str(err_message))
                 log.error(explanation)
-                raise ValueError(str(err_message) + ". " + explanation)
+                raise ValueError(str(err_message) + ". " + explanation) from err_message
             if repeat != 1:
                 data = np.repeat(data, repeat).reshape([nframes, -1])
             return np.float32(1.0), data
         elif must:
             raise RuntimeError("%s not found!" % path)
         else:
+            if type_sel is not None and not output_natoms_for_type_sel:
+                ndof = ndof_ * natoms_sel
             data = np.full([nframes, ndof], default, dtype=dtype)
             if repeat != 1:
                 data = np.repeat(data, repeat).reshape([nframes, -1])
             return np.float32(0.0), data
 
     def _load_type(self, sys_path: DPPath):
         atom_type = (sys_path / "type.raw").load_txt(ndmin=1).astype(np.int32)
@@ -608,7 +709,82 @@
         pbc = True
         if (sys_path / "nopbc").is_file():
             pbc = False
         return pbc
 
     def _check_mode(self, set_path: DPPath):
         return (set_path / "real_atom_types.npy").is_file()
+
+
+class DataRequirementItem:
+    """A class to store the data requirement for data systems.
+
+    Parameters
+    ----------
+    key
+        The key of the item. The corresponding data is stored in `sys_path/set.*/key.npy`
+    ndof
+        The number of dof
+    atomic
+        The item is an atomic property.
+        If False, the size of the data should be nframes x ndof
+        If True, the size of data should be nframes x natoms x ndof
+    must
+        The data file `sys_path/set.*/key.npy` must exist.
+        If must is False and the data file does not exist, the `data_dict[find_key]` is set to 0.0
+    high_prec
+        Load the data and store in float64, otherwise in float32
+    type_sel
+        Select certain type of atoms
+    repeat
+        The data will be repeated `repeat` times.
+    default : float, default=0.
+        default value of data
+    dtype : np.dtype, optional
+        the dtype of data, overwrites `high_prec` if provided
+    output_natoms_for_type_sel : bool, optional
+        if True and type_sel is True, the atomic dimension will be natoms instead of nsel
+    """
+
+    def __init__(
+        self,
+        key: str,
+        ndof: int,
+        atomic: bool = False,
+        must: bool = False,
+        high_prec: bool = False,
+        type_sel: Optional[List[int]] = None,
+        repeat: int = 1,
+        default: float = 0.0,
+        dtype: Optional[np.dtype] = None,
+        output_natoms_for_type_sel: bool = False,
+    ) -> None:
+        self.key = key
+        self.ndof = ndof
+        self.atomic = atomic
+        self.must = must
+        self.high_prec = high_prec
+        self.type_sel = type_sel
+        self.repeat = repeat
+        self.default = default
+        self.dtype = dtype
+        self.output_natoms_for_type_sel = output_natoms_for_type_sel
+        self.dict = self.to_dict()
+
+    def to_dict(self) -> dict:
+        return {
+            "key": self.key,
+            "ndof": self.ndof,
+            "atomic": self.atomic,
+            "must": self.must,
+            "high_prec": self.high_prec,
+            "type_sel": self.type_sel,
+            "repeat": self.repeat,
+            "default": self.default,
+            "dtype": self.dtype,
+            "output_natoms_for_type_sel": self.output_natoms_for_type_sel,
+        }
+
+    def __getitem__(self, key: str):
+        if key not in self.dict:
+            raise KeyError(key)
+        return self.dict[key]
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/model_stat.py` & `deepmd_kit-3.0.0a0/deepmd/utils/model_stat.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/path.py` & `deepmd_kit-3.0.0a0/deepmd/utils/path.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,17 +25,19 @@
 class DPPath(ABC):
     """The path class to data system (DeepmdData).
 
     Parameters
     ----------
     path : str
         path
+    mode : str, optional
+        mode, by default "r"
     """
 
-    def __new__(cls, path: str):
+    def __new__(cls, path: str, mode: str = "r"):
         if cls is DPPath:
             if os.path.isdir(path):
                 return super().__new__(DPOSPath)
             elif os.path.isfile(path.split("#")[0]):
                 # assume h5 if it is not dir
                 # TODO: check if it is a real h5? or just check suffix?
                 return super().__new__(DPH5Path)
@@ -59,14 +61,24 @@
         Returns
         -------
         np.ndarray
             loaded NumPy array
         """
 
     @abstractmethod
+    def save_numpy(self, arr: np.ndarray) -> None:
+        """Save NumPy array.
+
+        Parameters
+        ----------
+        arr : np.ndarray
+            NumPy array
+        """
+
+    @abstractmethod
     def glob(self, pattern: str) -> List["DPPath"]:
         """Search path using the glob pattern.
 
         Parameters
         ----------
         pattern : str
             glob pattern
@@ -118,26 +130,46 @@
 
     def __eq__(self, other) -> bool:
         return str(self) == str(other)
 
     def __hash__(self):
         return hash(str(self))
 
+    @property
+    @abstractmethod
+    def name(self) -> str:
+        """Name of the path."""
+
+    @abstractmethod
+    def mkdir(self, parents: bool = False, exist_ok: bool = False) -> None:
+        """Make directory.
+
+        Parameters
+        ----------
+        parents : bool, optional
+            If true, any missing parents of this directory are created as well.
+        exist_ok : bool, optional
+            If true, no error will be raised if the target directory already exists.
+        """
+
 
 class DPOSPath(DPPath):
     """The OS path class to data system (DeepmdData) for real directories.
 
     Parameters
     ----------
     path : str
         path
+    mode : str, optional
+        mode, by default "r"
     """
 
-    def __init__(self, path: str) -> None:
+    def __init__(self, path: str, mode: str = "r") -> None:
         super().__init__()
+        self.mode = mode
         if isinstance(path, Path):
             self.path = path
         else:
             self.path = Path(path)
 
     def load_numpy(self) -> np.ndarray:
         """Load NumPy array.
@@ -155,14 +187,26 @@
         Returns
         -------
         np.ndarray
             loaded NumPy array
         """
         return np.loadtxt(str(self.path), **kwargs)
 
+    def save_numpy(self, arr: np.ndarray) -> None:
+        """Save NumPy array.
+
+        Parameters
+        ----------
+        arr : np.ndarray
+            NumPy array
+        """
+        if self.mode == "r":
+            raise ValueError("Cannot save to read-only path")
+        np.save(str(self.path), arr)
+
     def glob(self, pattern: str) -> List["DPPath"]:
         """Search path using the glob pattern.
 
         Parameters
         ----------
         pattern : str
             glob pattern
@@ -170,15 +214,15 @@
         Returns
         -------
         List[DPPath]
             list of paths
         """
         # currently DPOSPath will only derivative DPOSPath
         # TODO: discuss if we want to mix DPOSPath and DPH5Path?
-        return [type(self)(p) for p in self.path.glob(pattern)]
+        return [type(self)(p, mode=self.mode) for p in self.path.glob(pattern)]
 
     def rglob(self, pattern: str) -> List["DPPath"]:
         """This is like calling :meth:`DPPath.glob()` with `**/` added in front
         of the given relative pattern.
 
         Parameters
         ----------
@@ -186,117 +230,154 @@
             glob pattern
 
         Returns
         -------
         List[DPPath]
             list of paths
         """
-        return [type(self)(p) for p in self.path.rglob(pattern)]
+        return [type(self)(p, mode=self.mode) for p in self.path.rglob(pattern)]
 
     def is_file(self) -> bool:
         """Check if self is file."""
         return self.path.is_file()
 
     def is_dir(self) -> bool:
         """Check if self is directory."""
         return self.path.is_dir()
 
     def __truediv__(self, key: str) -> "DPPath":
         """Used for / operator."""
-        return type(self)(self.path / key)
+        return type(self)(self.path / key, mode=self.mode)
 
     def __lt__(self, other: "DPOSPath") -> bool:
         """Whether this DPPath is less than other for sorting."""
         return self.path < other.path
 
     def __str__(self) -> str:
         """Represent string."""
         return str(self.path)
 
+    @property
+    def name(self) -> str:
+        """Name of the path."""
+        return self.path.name
+
+    def mkdir(self, parents: bool = False, exist_ok: bool = False) -> None:
+        """Make directory.
+
+        Parameters
+        ----------
+        parents : bool, optional
+            If true, any missing parents of this directory are created as well.
+        exist_ok : bool, optional
+            If true, no error will be raised if the target directory already exists.
+        """
+        if self.mode == "r":
+            raise ValueError("Cannot mkdir to read-only path")
+        self.path.mkdir(parents=parents, exist_ok=exist_ok)
+
 
 class DPH5Path(DPPath):
     """The path class to data system (DeepmdData) for HDF5 files.
 
     Notes
     -----
     OS - HDF5 relationship:
         directory - Group
         file - Dataset
 
     Parameters
     ----------
     path : str
         path
+    mode : str, optional
+        mode, by default "r"
     """
 
-    def __init__(self, path: str) -> None:
+    def __init__(self, path: str, mode: str = "r") -> None:
         super().__init__()
+        self.mode = mode
         # we use "#" to split path
         # so we do not support file names containing #...
         s = path.split("#")
         self.root_path = s[0]
-        self.root = self._load_h5py(s[0])
+        self.root = self._load_h5py(s[0], mode)
         # h5 path: default is the root path
-        self.name = s[1] if len(s) > 1 else "/"
+        self._name = s[1] if len(s) > 1 else "/"
 
     @classmethod
     @lru_cache(None)
-    def _load_h5py(cls, path: str) -> h5py.File:
+    def _load_h5py(cls, path: str, mode: str = "r") -> h5py.File:
         """Load hdf5 file.
 
         Parameters
         ----------
         path : str
             path to hdf5 file
+        mode : str, optional
+            mode, by default 'r'
         """
         # this method has cache to avoid duplicated
         # loading from different DPH5Path
         # However the file will be never closed?
-        return h5py.File(path, "r")
+        return h5py.File(path, mode)
 
     def load_numpy(self) -> np.ndarray:
         """Load NumPy array.
 
         Returns
         -------
         np.ndarray
             loaded NumPy array
         """
-        return self.root[self.name][:]
+        return self.root[self._name][:]
 
     def load_txt(self, dtype: Optional[np.dtype] = None, **kwargs) -> np.ndarray:
         """Load NumPy array from text.
 
         Returns
         -------
         np.ndarray
             loaded NumPy array
         """
         arr = self.load_numpy()
         if dtype:
             arr = arr.astype(dtype)
         return arr
 
+    def save_numpy(self, arr: np.ndarray) -> None:
+        """Save NumPy array.
+
+        Parameters
+        ----------
+        arr : np.ndarray
+            NumPy array
+        """
+        if self._name in self._keys:
+            del self.root[self._name]
+        self.root.create_dataset(self._name, data=arr)
+        self.root.flush()
+
     def glob(self, pattern: str) -> List["DPPath"]:
         """Search path using the glob pattern.
 
         Parameters
         ----------
         pattern : str
             glob pattern
 
         Returns
         -------
         List[DPPath]
             list of paths
         """
         # got paths starts with current path first, which is faster
-        subpaths = [ii for ii in self._keys if ii.startswith(self.name)]
+        subpaths = [ii for ii in self._keys if ii.startswith(self._name)]
         return [
-            type(self)(f"{self.root_path}#{pp}")
+            type(self)(f"{self.root_path}#{pp}", mode=self.mode)
             for pp in globfilter(subpaths, self._connect_path(pattern))
         ]
 
     def rglob(self, pattern: str) -> List["DPPath"]:
         """This is like calling :meth:`DPPath.glob()` with `**/` added in front
         of the given relative pattern.
 
@@ -323,36 +404,62 @@
         """Walk all groups and dataset."""
         l = []
         file.visit(lambda x: l.append("/" + x))
         return l
 
     def is_file(self) -> bool:
         """Check if self is file."""
-        if self.name not in self._keys:
+        if self._name not in self._keys:
             return False
-        return isinstance(self.root[self.name], h5py.Dataset)
+        return isinstance(self.root[self._name], h5py.Dataset)
 
     def is_dir(self) -> bool:
         """Check if self is directory."""
-        if self.name not in self._keys:
+        if self._name == "/":
+            return True
+        if self._name not in self._keys:
             return False
-        return isinstance(self.root[self.name], h5py.Group)
+        return isinstance(self.root[self._name], h5py.Group)
 
     def __truediv__(self, key: str) -> "DPPath":
         """Used for / operator."""
-        return type(self)(f"{self.root_path}#{self._connect_path(key)}")
+        return type(self)(f"{self.root_path}#{self._connect_path(key)}", mode=self.mode)
 
     def _connect_path(self, path: str) -> str:
         """Connect self with path."""
-        if self.name.endswith("/"):
-            return f"{self.name}{path}"
-        return f"{self.name}/{path}"
+        if self._name.endswith("/"):
+            return f"{self._name}{path}"
+        return f"{self._name}/{path}"
 
     def __lt__(self, other: "DPH5Path") -> bool:
         """Whether this DPPath is less than other for sorting."""
         if self.root_path == other.root_path:
-            return self.name < other.name
+            return self._name < other._name
         return self.root_path < other.root_path
 
     def __str__(self) -> str:
         """Returns path of self."""
-        return f"{self.root_path}#{self.name}"
+        return f"{self.root_path}#{self._name}"
+
+    @property
+    def name(self) -> str:
+        """Name of the path."""
+        return self._name.split("/")[-1]
+
+    def mkdir(self, parents: bool = False, exist_ok: bool = False) -> None:
+        """Make directory.
+
+        Parameters
+        ----------
+        parents : bool, optional
+            If true, any missing parents of this directory are created as well.
+        exist_ok : bool, optional
+            If true, no error will be raised if the target directory already exists.
+        """
+        if self._name in self._keys:
+            if not exist_ok:
+                raise FileExistsError(f"{self} already exists")
+            return
+        if parents:
+            self.root.require_group(self._name)
+        else:
+            self.root.create_group(self._name)
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/plugin.py` & `deepmd_kit-3.0.0a0/deepmd/utils/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
 """Base of plugin systems."""
 # copied from https://github.com/deepmodeling/dpdata/blob/a3e76d75de53f6076254de82d18605a010dc3b00/dpdata/plugin.py
 
+import difflib
 from abc import (
     ABCMeta,
 )
 from typing import (
     Callable,
+    Dict,
+    Optional,
+    Type,
 )
 
 
 class Plugin:
     """A class to register and restore plugins.
 
     Attributes
@@ -20,15 +24,15 @@
 
     Examples
     --------
     >>> plugin = Plugin()
     >>> @plugin.register("xx")
         def xxx():
             pass
-    >>> print(plugin.plugins['xx'])
+    >>> print(plugin.plugins["xx"])
     """
 
     def __init__(self):
         self.plugins = {}
 
     def __add__(self, other) -> "Plugin":
         self.plugins.update(other.plugins)
@@ -89,7 +93,69 @@
     pass
 
 
 class PluginVariant(metaclass=VariantABCMeta):
     """A class to remove `type` from input arguments."""
 
     pass
+
+
+def make_plugin_registry(name: Optional[str] = None) -> Type[object]:
+    """Make a plugin registry.
+
+    Parameters
+    ----------
+    name : Optional[str]
+        the name of the registry for the error message, e.g. descriptor, backend, etc.
+
+    Examples
+    --------
+    >>> class BaseClass(make_plugin_registry()):
+            pass
+    """
+    if name is None:
+        name = "class"
+
+    class PR:
+        __plugins = Plugin()
+
+        @staticmethod
+        def register(key: str) -> Callable[[object], object]:
+            """Register a descriptor plugin.
+
+            Parameters
+            ----------
+            key : str
+                the key of a descriptor
+
+            Returns
+            -------
+            callable[[object], object]
+                the registered descriptor
+
+            Examples
+            --------
+            >>> @BaseClass.register("some_class")
+                class SomeClass(BaseClass):
+                    pass
+            """
+            return PR.__plugins.register(key)
+
+        @classmethod
+        def get_class_by_type(cls, class_type: str) -> Type[object]:
+            """Get the class by the plugin type."""
+            if class_type in PR.__plugins.plugins:
+                return PR.__plugins.plugins[class_type]
+            else:
+                # did you mean
+                matches = difflib.get_close_matches(
+                    class_type, PR.__plugins.plugins.keys()
+                )
+                dym_message = f"Did you mean: {matches[0]}?" if matches else ""
+                raise RuntimeError(f"Unknown {name} type: {class_type}. {dym_message}")
+
+        @classmethod
+        def get_plugins(cls) -> Dict[str, Type[object]]:
+            """Get all the registered plugins."""
+            return PR.__plugins.plugins
+
+    return PR
```

### Comparing `deepmd_kit-2.2.9/deepmd_utils/utils/weight_avg.py` & `deepmd_kit-3.0.0a0/deepmd/utils/weight_avg.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/pyproject.toml` & `deepmd_kit-3.0.0a0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
     # dynamic metadata API is still unstable
     # TODO: unpin the upper bound when it is stable
-    "scikit-build-core>=0.5,<0.8,!=0.6.0",
+    "scikit-build-core>=0.5,<0.9,!=0.6.0",
     "packaging",
 ]
 build-backend = "backend.dp_backend"
 backend-path = ["."]
 
 [project]
 name = "deepmd-kit"
@@ -23,41 +23,43 @@
     "Operating System :: Microsoft :: Windows",
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: C",
     "Programming Language :: C++",
     "Programming Language :: Python :: 3 :: Only",
     "Environment :: GPU :: NVIDIA CUDA :: 12 :: 12.2",
     "Intended Audience :: Science/Research",
-    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Environment :: Console",
 ]
 dependencies = [
     'numpy',
     'scipy',
     'pyyaml',
     'dargs >= 0.4.1',
-    'python-hostlist >= 1.21',
     'typing_extensions; python_version < "3.8"',
     'importlib_metadata>=1.4; python_version < "3.8"',
     'h5py',
     'wcmatch',
     'packaging',
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 keywords = ["deepmd"]
 
 [project.entry-points."lammps.plugins"]
-deepmd = "deepmd.lmp:get_op_dir"
+deepmd = "deepmd.tf.lmp:get_op_dir"
 
 [project.entry-points."dpgui"]
-"DeePMD-kit" = "deepmd_utils.utils.argcheck:gen_args"
+"DeePMD-kit" = "deepmd.utils.argcheck:gen_args"
+
+[project.entry-points."dpdata.plugins"]
+deepmd_driver = "deepmd.driver:DPDriver"
 
 [project.urls]
 Homepage = "https://github.com/deepmodeling/deepmd-kit"
 documentation = "https://docs.deepmodeling.com/projects/deepmd"
 repository = "https://github.com/deepmodeling/deepmd-kit"
 
 [tool.setuptools_scm]
@@ -78,15 +80,14 @@
     "/doc",
     "/examples",
     "/data",
     "/.github",
 ]
 wheel.packages = [
     "deepmd",
-    "deepmd_utils",
 ]
 wheel.py-api = "py37"
 build-dir = "build/{wheel_tag}"
 
 [tool.scikit-build.metadata.version]
 provider = "scikit_build_core.metadata.setuptools_scm"
 
@@ -98,15 +99,15 @@
 provider = "backend.dynamic_metadata"
 provider-path = "backend"
 
 [tool.scikit-build.metadata.readme]
 provider = "scikit_build_core.metadata.fancy_pypi_readme"
 
 [[tool.scikit-build.generate]]
-path = "deepmd_utils/_version.py"
+path = "deepmd/_version.py"
 template = '''
 version = "${version}"
 '''
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
@@ -124,43 +125,45 @@
 replacement = '\1="https://github.com/deepmodeling/deepmd-kit/raw/master/\g<2>"'
 
 [tool.cibuildwheel]
 test-command = [
     "python -m deepmd -h",
     "dp -h",
     "dp_ipi",
-    "pytest {project}/source/tests/test_lammps.py"
+    "pytest {project}/source/tests/tf/test_lammps.py"
 ]
 test-extras = ["cpu", "test", "lmp", "ipi"]
 build = ["cp310-*"]
 skip = ["*-win32", "*-manylinux_i686", "*-musllinux*"]
 # TODO: uncomment when CUDA 11 is deprecated
 # manylinux-x86_64-image = "manylinux_2_28"
 manylinux-x86_64-image = "quay.io/pypa/manylinux_2_28_x86_64:2022-11-19-1b19e81"
 manylinux-aarch64-image = "manylinux_2_28"
 
 [tool.cibuildwheel.macos]
-environment = { PIP_PREFER_BINARY="1", DP_LAMMPS_VERSION="stable_2Aug2023_update2", DP_ENABLE_IPI="1" }
+environment = { PIP_PREFER_BINARY="1", DP_LAMMPS_VERSION="stable_2Aug2023_update3", DP_ENABLE_IPI="1" }
 before-all = [
-    # enable MPI for macos-arm64 in the next lammps release for compatibility
-    """if [[ "$CIBW_BUILD" != *macosx_arm64* ]]; then brew install mpich; fi""",
+    """brew install mpich""",
 ]
 repair-wheel-command = """delocate-wheel --require-archs {delocate_archs} -w {dest_dir} -v {wheel} --ignore-missing-dependencies"""
 
 [tool.cibuildwheel.linux]
 repair-wheel-command = "auditwheel repair --exclude libtensorflow_framework.so.2 --exclude libtensorflow_framework.so.1 --exclude libtensorflow_framework.so --exclude _pywrap_tensorflow_internal.so --exclude libtensorflow_cc.so.2 -w {dest_dir} {wheel}"
 environment-pass = [
     "CIBW_BUILD",
     "DP_VARIANT",
     "CUDA_VERSION",
     "DP_PKG_NAME",
+    "SETUPTOOLS_SCM_PRETEND_VERSION_FOR_DEEPMD-KIT-CU11",
 ]
-environment = { PIP_PREFER_BINARY="1", DP_LAMMPS_VERSION="stable_2Aug2023_update2", DP_ENABLE_IPI="1", MPI_HOME="/usr/lib64/mpich", PATH="/usr/lib64/mpich/bin:$PATH" }
+environment = { PIP_PREFER_BINARY="1", DP_LAMMPS_VERSION="stable_2Aug2023_update3", DP_ENABLE_IPI="1", MPI_HOME="/usr/lib64/mpich", PATH="/usr/lib64/mpich/bin:$PATH" }
 before-all = [
     """if [ ! -z "${DP_PKG_NAME}" ]; then sed -i "s/name = \\"deepmd-kit\\"/name = \\"${DP_PKG_NAME}\\"/g" pyproject.toml; fi""",
+    # https://almalinux.org/blog/2023-12-20-almalinux-8-key-update/
+    """rpm --import https://repo.almalinux.org/almalinux/RPM-GPG-KEY-AlmaLinux""",
     """{ if [ "$(uname -m)" = "x86_64" ] ; then yum config-manager --add-repo http://developer.download.nvidia.com/compute/cuda/repos/rhel8/x86_64/cuda-rhel8.repo && yum install -y cuda-nvcc-${CUDA_VERSION/./-} cuda-cudart-devel-${CUDA_VERSION/./-}; fi }""",
     "yum install -y mpich-devel",
 ]
 
 [tool.cibuildwheel.windows]
 environment = { PIP_PREFER_BINARY="1" }
 test-extras = ["cpu"]
@@ -217,23 +220,28 @@
 [tool.pydocstyle]
 ignore = "D413, D416, D203, D107, D213"
 
 [tool.isort]
 profile = "black"
 force_grid_wrap = 1
 
-[tool.ruff]
+[tool.ruff.format]
+docstring-code-format = true
+
+[tool.ruff.lint]
 select = [
     "E", # errors
     "F", # pyflakes
     "D", # pydocstyle
     "UP", # pyupgrade
     "C4", # flake8-comprehensions
     "RUF", # ruff
     "NPY", # numpy
+    "TID251", # banned-api
+    "TID253", # banned-module-level-imports
 ]
 
 ignore = [
     "E501", # line too long
     "F841", # local variable is assigned to but never used
     "E741", # ambiguous variable name
     "E402", # module level import not at top of file
@@ -245,12 +253,39 @@
     "D105", # TODO: missing docstring in magic method
     "D205", # 1 blank line required between summary line and description
     "D401", # TODO: first line should be in imperative mood
     "D404", # TODO: first word of the docstring should not be This
 ]
 ignore-init-module-imports = true
 
-[tool.ruff.pydocstyle]
+exclude = [
+    "source/3rdparty/**",
+]
+
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
+[tool.ruff.lint.flake8-tidy-imports]
+banned-module-level-imports = [
+    "deepmd.tf",
+    "deepmd.pt",
+    "tensorflow",
+    "torch",
+]
+
+[tool.ruff.lint.flake8-tidy-imports.banned-api]
+"torch.testing.assert_allclose".msg = "Use `torch.testing.assert_close()` instead, see https://github.com/pytorch/pytorch/issues/61844."
+
+[tool.ruff.lint.extend-per-file-ignores]
+# Also ignore `E402` in all `__init__.py` files.
+"deepmd/tf/**" = ["TID253"]
+"deepmd/pt/**" = ["TID253"]
+"source/tests/tf/**" = ["TID253"]
+"source/tests/pt/**" = ["TID253"]
+"source/ipi/tests/**" = ["TID253"]
+"source/lmp/tests/**" = ["TID253"]
+
 [tool.pytest.ini_options]
 markers = "run"
+
+[tool.coverage.run]
+plugins = ["source.3rdparty.coverage_plugins.jit_plugin"]
```

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/aarch64/table.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/aarch64/table.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/aarch64/trampoline.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/aarch64/trampoline.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/arm/table.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/arm/table.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/arm/trampoline.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/arm/trampoline.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/common/init.c.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/common/init.c.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/e2k/table.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/e2k/table.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/e2k/trampoline.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/e2k/trampoline.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/i386/table.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/i386/table.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/i386/trampoline.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/i386/trampoline.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips/table.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips/table.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips/trampoline.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips/trampoline.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips64/table.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips64/table.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/mips64/trampoline.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/mips64/trampoline.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/x86_64/table.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/x86_64/table.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/arch/x86_64/trampoline.S.tpl` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/arch/x86_64/trampoline.S.tpl`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/implib/implib-gen.py` & `deepmd_kit-3.0.0a0/source/3rdparty/implib/implib-gen.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/3rdparty/json.hpp` & `deepmd_kit-3.0.0a0/source/3rdparty/json.hpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # new in 3.16: GET_RUNTIME_DEPENDENCIES, target_precompile_headers
 cmake_minimum_required(VERSION 3.16)
 project(DeePMD)
 
+option(ENABLE_TENSORFLOW "Enable TensorFlow interface" OFF)
+option(ENABLE_PYTORCH "Enable PyTorch interface" OFF)
 option(BUILD_TESTING "Build test and enable converage" OFF)
 set(DEEPMD_C_ROOT
     ""
     CACHE PATH "Path to imported DeePMD-kit C library")
 
 if(BUILD_TESTING)
   enable_testing()
@@ -127,29 +129,67 @@
 set(DEEPMD_SOURCE_DIR ${PROJECT_SOURCE_DIR}/..)
 
 # setup tensorflow libraries by python
 if(INSTALL_TENSORFLOW)
   set(USE_TF_PYTHON_LIBS TRUE)
 endif(INSTALL_TENSORFLOW)
 if(USE_TF_PYTHON_LIBS)
+  set(ENABLE_TENSORFLOW TRUE)
   if(NOT "$ENV{CIBUILDWHEEL}" STREQUAL "1")
     find_package(
       Python
       COMPONENTS Interpreter Development
       REQUIRED)
   else()
     set(Python_LIBRARIES ${Python_LIBRARY})
     set(PYTHON_INCLUDE_DIRS ${PYTHON_INCLUDE_DIR})
   endif()
 endif(USE_TF_PYTHON_LIBS)
+if(TENSORFLOW_ROOT)
+  set(ENABLE_TENSORFLOW TRUE)
+endif()
 
 # find tensorflow, I need tf abi info
-if(NOT DEEPMD_C_ROOT)
+if(ENABLE_TENSORFLOW AND NOT DEEPMD_C_ROOT)
   find_package(tensorflow REQUIRED)
 endif()
+if(ENABLE_PYTORCH AND NOT DEEPMD_C_ROOT)
+  find_package(Torch REQUIRED)
+  string(REGEX MATCH "_GLIBCXX_USE_CXX11_ABI=([0-9]+)" CXXABI_PT_MATCH
+               ${TORCH_CXX_FLAGS})
+  if(CXXABI_PT_MATCH)
+    message(STATUS "PyTorch CXX11 ABI: ${CMAKE_MATCH_1}")
+    if(DEFINED OP_CXX_ABI)
+      if(NOT ${CMAKE_MATCH_1} EQUAL ${OP_CXX_ABI})
+        message(
+          FATAL_ERROR
+            "PyTorch CXX11 ABI mismatch TensorFlow: ${CMAKE_MATCH_1} != ${OP_CXX_ABI}"
+        )
+      endif()
+    else()
+      set(OP_CXX_ABI ${CMAKE_MATCH_1})
+      add_definitions(-D_GLIBCXX_USE_CXX11_ABI=${OP_CXX_ABI})
+    endif()
+  endif()
+endif()
+# log enabled backends
+if(NOT DEEPMD_C_ROOT)
+  message(STATUS "Enabled backends:")
+  if(ENABLE_TENSORFLOW)
+    message(STATUS "- TensorFlow")
+  endif()
+  if(ENABLE_PYTORCH)
+    message(STATUS "- PyTorch")
+  endif()
+  if(NOT ENABLE_TENSORFLOW
+     AND NOT ENABLE_PYTORCH
+     AND NOT BUILD_PY_IF)
+    message(FATAL_ERROR "No backend is enabled.")
+  endif()
+endif()
 
 # find threads
 find_package(Threads)
 
 # define build type
 if((NOT DEFINED CMAKE_BUILD_TYPE) OR CMAKE_BUILD_TYPE STREQUAL "")
   set(CMAKE_BUILD_TYPE release)
@@ -230,18 +270,21 @@
     PROPERTIES IMPORTED_LINK_INTERFACE_LANGUAGES "C"
                IMPORTED_LOCATION "${deepmd_c}"
                INTERFACE_INCLUDE_DIRECTORIES "${DEEPMD_INCLUDE_C_DIR}/deepmd")
   # use variable for TF path to set deepmd_c path
   set(TENSORFLOW_ROOT "${DEEPMD_C_ROOT}")
   set(TensorFlow_LIBRARY_PATH "${DEEPMD_C_ROOT}/lib")
   set(TENSORFLOW_INCLUDE_DIRS "${DEEPMD_C_ROOT}/include")
+  set(TORCH_LIBRARIES "${DEEPMD_C_ROOT}/lib/libtorch.so")
 endif()
 
 if(NOT DEEPMD_C_ROOT)
-  add_subdirectory(op/)
+  if(ENABLE_TENSORFLOW)
+    add_subdirectory(op/)
+  endif()
   add_subdirectory(lib/)
 endif()
 if(BUILD_PY_IF)
   add_subdirectory(config/)
   # add_subdirectory (tests/)
 endif(BUILD_PY_IF)
 if(BUILD_CPP_IF)
@@ -250,18 +293,15 @@
     add_subdirectory(api_c/)
   endif()
   if(LAMMPS_VERSION OR NOT BUILD_PY_IF)
     add_subdirectory(lmp/)
   endif()
   if(CMAKE_CXX_COMPILER_VERSION VERSION_GREATER 4.8)
     # add_subdirectory (md/)
-    if(ENABLE_IPI
-       OR NOT BUILD_PY_IF
-       AND NOT DEEPMD_C_ROOT)
-      # ipi has a dependency on libdeepmd
+    if(ENABLE_IPI OR NOT BUILD_PY_IF)
       add_subdirectory(ipi/)
     endif()
     if(NOT BUILD_PY_IF)
       add_subdirectory(gmx/)
     endif()
   endif()
   if(BUILD_NODEJS_IF)
```

### Comparing `deepmd_kit-2.2.9/source/api_c/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/api_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/api_c/include/c_api.h` & `deepmd_kit-3.0.0a0/source/api_c/include/c_api.h`

 * *Files 0% similar despite different names*

```diff
@@ -1130,28 +1130,28 @@
 extern void DP_DeleteDipoleChargeModifier(DP_DipoleChargeModifier* dcm);
 
 /**
  * @brief Evaluate the force and virial correction by using a dipole charge
  *modifier with the neighbor list. (double version)
  * @param[in] dcm The dipole charge modifier to use.
  * @param[in] natoms The number of atoms.
- * @param[in] coord The coordinates of atoms. The array should be of size natoms
+ * @param[in] coord The coordinates of atoms. The array should be of size nall
  *x 3.
- * @param[in] atype The atom types. The array should contain natoms ints.
+ * @param[in] atype The atom types. The array should contain nall ints.
  * @param[in] cell The cell of the region. The array should be of size 9. Pass
  *NULL if pbc is not used.
  * @param[in] pairs The pairs of atoms. The list should contain npairs pairs of
  *ints.
  * @param[in] npairs The number of pairs.
  * @param[in] delef_ The electric field on each atom. The array should be of
- *size nframes x natoms x 3.
+ *size nframes x nloc x 3.
  * @param[in] nghost The number of ghost atoms.
  * @param[in] nlist The neighbor list.
  * @param[out] dfcorr_ Output force correction. The array should be of size
- *natoms x 3.
+ *nall x 3.
  * @param[out] dvcorr_ Output virial correction. The array should be of size 9.
  * @warning The output arrays should be allocated before calling this function.
  *Pass NULL if not required.
  **/
 extern void DP_DipoleChargeModifierComputeNList(DP_DipoleChargeModifier* dcm,
                                                 const int natom,
                                                 const double* coord,
```

### Comparing `deepmd_kit-2.2.9/source/api_c/include/c_api_internal.h` & `deepmd_kit-3.0.0a0/source/api_c/include/c_api_internal.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/api_c/include/deepmd.hpp` & `deepmd_kit-3.0.0a0/source/api_c/include/deepmd.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1961,21 +1961,21 @@
   };
   /**
    * @brief Evaluate the force and virial correction by using this dipole charge
    *modifier.
    * @param[out] dfcorr_ The force correction on each atom.
    * @param[out] dvcorr_ The virial correction.
    * @param[in] dcoord_ The coordinates of atoms. The array should be of size
-   *natoms x 3.
-   * @param[in] datype_ The atom types. The list should contain natoms ints.
+   *nall x 3.
+   * @param[in] datype_ The atom types. The list should contain nall ints.
    * @param[in] dbox The cell of the region. The array should be of size 9.
    * @param[in] pairs The pairs of atoms. The list should contain npairs pairs
    *of ints.
    * @param[in] delef_ The electric field on each atom. The array should be of
-   *size natoms x 3.
+   *size nghost x 3.
    * @param[in] nghost The number of ghost atoms.
    * @param[in] lmp_list The neighbor list.
    **/
   template <typename VALUETYPE>
   void compute(std::vector<VALUETYPE> &dfcorr_,
                std::vector<VALUETYPE> &dvcorr_,
                const std::vector<VALUETYPE> &dcoord_,
```

### Comparing `deepmd_kit-2.2.9/source/api_c/src/c_api.cc` & `deepmd_kit-3.0.0a0/source/api_c/src/c_api.cc`

 * *Files 0% similar despite different names*

```diff
@@ -781,15 +781,15 @@
     cell_.assign(cell, cell + 9);
   }
   // pairs
   std::vector<std::pair<int, int>> pairs_;
   for (int i = 0; i < npairs; i++) {
     pairs_.push_back(std::make_pair(pairs[i * 2], pairs[i * 2 + 1]));
   }
-  std::vector<VALUETYPE> delef_(delef, delef + natoms * 3);
+  std::vector<VALUETYPE> delef_(delef, delef + (natoms - nghost) * 3);
   std::vector<VALUETYPE> df, dv;
 
   DP_REQUIRES_OK(dcm, dcm->dcm.compute(df, dv, coord_, atype_, cell_, pairs_,
                                        delef_, nghost, nlist->nl));
   // copy from C++ vectors to C arrays, if not NULL pointer
   if (dfcorr_) {
     std::copy(df.begin(), df.end(), dfcorr_);
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/api_cc/CMakeLists.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,16 +7,24 @@
 
 set(libname "${LIB_DEEPMD_CC}")
 
 add_library(${libname} SHARED ${LIB_SRC})
 
 # link: libdeepmd libdeepmd_op libtensorflow_cc libtensorflow_framework
 target_link_libraries(${libname} PUBLIC ${LIB_DEEPMD})
-target_link_libraries(${libname} PRIVATE TensorFlow::tensorflow_cc
-                                         TensorFlow::tensorflow_framework)
+if(ENABLE_TENSORFLOW)
+  target_link_libraries(${libname} PRIVATE TensorFlow::tensorflow_cc
+                                           TensorFlow::tensorflow_framework)
+  target_compile_definitions(${libname} PRIVATE BUILD_TENSORFLOW)
+endif()
+if(ENABLE_PYTORCH)
+  target_link_libraries(${libname} PRIVATE "${TORCH_LIBRARIES}")
+  target_compile_definitions(${libname} PRIVATE BUILD_PYTORCH)
+endif()
+
 target_include_directories(
   ${libname}
   PUBLIC $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
          $<BUILD_INTERFACE:${CMAKE_CURRENT_BINARY_DIR}>
          $<INSTALL_INTERFACE:include>)
 target_precompile_headers(${libname} PUBLIC [["common.h"]])
 
@@ -51,7 +59,18 @@
 ${CMAKE_INSTALL_PREFIX}/lib/${CMAKE_SHARED_LIBRARY_PREFIX}${libname}${LOW_PREC_VARIANT}${CMAKE_SHARED_LIBRARY_SUFFIX}   \
 )")
 
   if(CMAKE_TESTING_ENABLED)
     add_subdirectory(tests)
   endif()
 endif(BUILD_PY_IF)
+
+if(BUILD_TESTING)
+  # A compilation test to make sure api_cc can compile without any backend
+  add_library(deepmd_cc_test_no_backend SHARED ${LIB_SRC})
+  target_link_libraries(deepmd_cc_test_no_backend PUBLIC ${LIB_DEEPMD})
+  target_include_directories(
+    deepmd_cc_test_no_backend
+    PUBLIC $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
+           $<BUILD_INTERFACE:${CMAKE_CURRENT_BINARY_DIR}>
+           $<INSTALL_INTERFACE:include>)
+endif()
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/include/AtomMap.h` & `deepmd_kit-3.0.0a0/source/api_cc/include/AtomMap.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/api_cc/include/DataModifier.h` & `deepmd_kit-3.0.0a0/source/api_cc/include/DataModifier.h`

 * *Files 2% similar despite different names*

```diff
@@ -123,21 +123,21 @@
 
   /**
    * @brief Evaluate the force and virial correction by using this dipole charge
    *modifier.
    * @param[out] dfcorr_ The force correction on each atom.
    * @param[out] dvcorr_ The virial correction.
    * @param[in] dcoord_ The coordinates of atoms. The array should be of size
-   *natoms x 3.
-   * @param[in] datype_ The atom types. The list should contain natoms ints.
+   *nall x 3.
+   * @param[in] datype_ The atom types. The list should contain nall ints.
    * @param[in] dbox The cell of the region. The array should be of size 9.
    * @param[in] pairs The pairs of atoms. The list should contain npairs pairs
    *of ints.
    * @param[in] delef_ The electric field on each atom. The array should be of
-   *size natoms x 3.
+   *size nloc x 3.
    * @param[in] nghost The number of ghost atoms.
    * @param[in] lmp_list The neighbor list.
    **/
   template <typename VALUETYPE>
   void compute(std::vector<VALUETYPE>& dfcorr_,
                std::vector<VALUETYPE>& dvcorr_,
                const std::vector<VALUETYPE>& dcoord_,
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/include/DataModifierTF.h` & `deepmd_kit-3.0.0a0/source/api_cc/include/DataModifierTF.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
 #pragma once
 
 #include "DataModifier.h"
 #include "common.h"
+#include "commonTF.h"
 
 namespace deepmd {
 /**
  * @brief Dipole charge modifier.
  **/
 class DipoleChargeModifierTF : public DipoleChargeModifierBase {
  public:
@@ -37,21 +38,21 @@
  private:
   /**
    * @brief Evaluate the force and virial correction by using this dipole charge
    *modifier.
    * @param[out] dfcorr_ The force correction on each atom.
    * @param[out] dvcorr_ The virial correction.
    * @param[in] dcoord_ The coordinates of atoms. The array should be of size
-   *natoms x 3.
-   * @param[in] datype_ The atom types. The list should contain natoms ints.
+   *nall x 3.
+   * @param[in] datype_ The atom types. The list should contain nall ints.
    * @param[in] dbox The cell of the region. The array should be of size 9.
    * @param[in] pairs The pairs of atoms. The list should contain npairs pairs
    *of ints.
    * @param[in] delef_ The electric field on each atom. The array should be of
-   *size natoms x 3.
+   *size nloc x 3.
    * @param[in] nghost The number of ghost atoms.
    * @param[in] lmp_list The neighbor list.
    **/
   template <typename VALUETYPE>
   void compute(std::vector<VALUETYPE>& dfcorr_,
                std::vector<VALUETYPE>& dvcorr_,
                const std::vector<VALUETYPE>& dcoord_,
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/include/DeepPot.h` & `deepmd_kit-3.0.0a0/source/api_cc/include/DeepPot.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/api_cc/include/DeepPotTF.h` & `deepmd_kit-3.0.0a0/source/api_cc/include/DeepPotTF.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
 #pragma once
 
 #include "DeepPot.h"
 #include "common.h"
+#include "commonTF.h"
 #include "neighbor_list.h"
 
 namespace deepmd {
 /**
  * @brief TensorFlow implementation for Deep Potential.
  **/
 class DeepPotTF : public DeepPotBase {
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/include/DeepTensor.h` & `deepmd_kit-3.0.0a0/source/api_cc/include/DeepTensor.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/api_cc/include/DeepTensorTF.h` & `deepmd_kit-3.0.0a0/source/api_cc/include/DeepTensorTF.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
 #pragma once
 
 #include "DeepTensor.h"
 #include "common.h"
+#include "commonTF.h"
 #include "neighbor_list.h"
 
 namespace deepmd {
 /**
  * @brief Deep Tensor.
  **/
 class DeepTensorTF : public DeepTensorBase {
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/include/tf_private.h` & `deepmd_kit-3.0.0a0/source/api_cc/include/tf_private.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/api_cc/src/AtomMap.cc` & `deepmd_kit-3.0.0a0/source/api_cc/src/AtomMap.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/api_cc/src/DataModifier.cc` & `deepmd_kit-3.0.0a0/source/api_cc/src/DataModifier.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
 #include "DataModifier.h"
 
+#ifdef BUILD_TENSORFLOW
 #include "DataModifierTF.h"
+#endif
 #include "common.h"
 
 using namespace deepmd;
 
 DipoleChargeModifier::DipoleChargeModifier() : inited(false) {}
 
 DipoleChargeModifier::DipoleChargeModifier(const std::string& model,
@@ -25,17 +27,20 @@
                  "nothing at the second call of initializer"
               << std::endl;
     return;
   }
   // TODO: To implement detect_backend
   DPBackend backend = deepmd::DPBackend::TensorFlow;
   if (deepmd::DPBackend::TensorFlow == backend) {
-    // TODO: throw errors if TF backend is not built, without mentioning TF
+#ifdef BUILD_TENSORFLOW
     dcm = std::make_shared<deepmd::DipoleChargeModifierTF>(model, gpu_rank,
                                                            name_scope_);
+#else
+    throw deepmd::deepmd_exception("TensorFlow backend is not built");
+#endif
   } else if (deepmd::DPBackend::PyTorch == backend) {
     throw deepmd::deepmd_exception("PyTorch backend is not supported yet");
   } else if (deepmd::DPBackend::Paddle == backend) {
     throw deepmd::deepmd_exception("PaddlePaddle backend is not supported yet");
   } else {
     throw deepmd::deepmd_exception("Unknown file type");
   }
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/src/DataModifierTF.cc` & `deepmd_kit-3.0.0a0/source/api_cc/src/DataModifierTF.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
+#ifdef BUILD_TENSORFLOW
 #include "DataModifierTF.h"
 
 #include "common.h"
 
 using namespace deepmd;
 using namespace tensorflow;
 
@@ -357,7 +358,8 @@
     const std::vector<std::pair<int, int>>& pairs,
     const std::vector<float>& delef_,
     const int nghost,
     const InputNlist& lmp_list) {
   compute(dfcorr_, dvcorr_, dcoord_, datype_, dbox, pairs, delef_, nghost,
           lmp_list);
 }
+#endif  // BUILD_TENSORFLOW
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/src/DeepPot.cc` & `deepmd_kit-3.0.0a0/source/api_cc/src/DeepPot.cc`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 
 #include "common.h"
 // TODO: only include when TF backend is built
 #include <memory>
 #include <stdexcept>
 
 #include "AtomMap.h"
+#ifdef BUILD_TENSORFLOW
 #include "DeepPotTF.h"
+#endif
+#ifdef BUILD_PYTORCH
+#include "DeepPotPT.h"
+#endif
 #include "device.h"
 
 using namespace deepmd;
 
 DeepPot::DeepPot() : inited(false) {}
 
 DeepPot::DeepPot(const std::string& model,
@@ -28,21 +33,34 @@
                    const std::string& file_content) {
   if (inited) {
     std::cerr << "WARNING: deepmd-kit should not be initialized twice, do "
                  "nothing at the second call of initializer"
               << std::endl;
     return;
   }
-  // TODO: To implement detect_backend
-  DPBackend backend = deepmd::DPBackend::TensorFlow;
+  DPBackend backend;
+  if (model.length() >= 4 && model.substr(model.length() - 4) == ".pth") {
+    backend = deepmd::DPBackend::PyTorch;
+  } else if (model.length() >= 3 && model.substr(model.length() - 3) == ".pb") {
+    backend = deepmd::DPBackend::TensorFlow;
+  } else {
+    throw deepmd::deepmd_exception("Unsupported model file format");
+  }
   if (deepmd::DPBackend::TensorFlow == backend) {
-    // TODO: throw errors if TF backend is not built, without mentioning TF
+#ifdef BUILD_TENSORFLOW
     dp = std::make_shared<deepmd::DeepPotTF>(model, gpu_rank, file_content);
+#else
+    throw deepmd::deepmd_exception("TensorFlow backend is not built");
+#endif
   } else if (deepmd::DPBackend::PyTorch == backend) {
-    throw deepmd::deepmd_exception("PyTorch backend is not supported yet");
+#ifdef BUILD_PYTORCH
+    dp = std::make_shared<deepmd::DeepPotPT>(model, gpu_rank, file_content);
+#else
+    throw deepmd::deepmd_exception("PyTorch backend is not built");
+#endif
   } else if (deepmd::DPBackend::Paddle == backend) {
     throw deepmd::deepmd_exception("PaddlePaddle backend is not supported yet");
   } else {
     throw deepmd::deepmd_exception("Unknown file type");
   }
   inited = true;
 }
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/src/DeepPotTF.cc` & `deepmd_kit-3.0.0a0/source/api_cc/src/DeepPotTF.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
+#ifdef BUILD_TENSORFLOW
 #include "DeepPotTF.h"
 
 #include <stdexcept>
 
 #include "AtomMap.h"
 #include "common.h"
 #include "device.h"
@@ -1047,7 +1048,8 @@
                                     const std::vector<int>& atype,
                                     const std::vector<float>& box,
                                     const std::vector<float>& fparam,
                                     const std::vector<float>& aparam) {
   compute_mixed_type(ener, force, virial, atom_energy, atom_virial, nframes,
                      coord, atype, box, fparam, aparam);
 }
+#endif
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/src/DeepTensor.cc` & `deepmd_kit-3.0.0a0/source/api_cc/src/DeepTensor.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
 #include "DeepTensor.h"
 
 #include <memory>
 
+#ifdef BUILD_TENSORFLOW
 #include "DeepTensorTF.h"
+#endif
 #include "common.h"
 
 using namespace deepmd;
 
 DeepTensor::DeepTensor() : inited(false) {}
 
 DeepTensor::DeepTensor(const std::string &model,
@@ -27,16 +29,19 @@
                  "nothing at the second call of initializer"
               << std::endl;
     return;
   }
   // TODO: To implement detect_backend
   DPBackend backend = deepmd::DPBackend::TensorFlow;
   if (deepmd::DPBackend::TensorFlow == backend) {
-    // TODO: throw errors if TF backend is not built, without mentioning TF
+#ifdef BUILD_TENSORFLOW
     dt = std::make_shared<deepmd::DeepTensorTF>(model, gpu_rank, name_scope_);
+#else
+    throw deepmd::deepmd_exception("TensorFlow backend is not built.");
+#endif
   } else if (deepmd::DPBackend::PyTorch == backend) {
     throw deepmd::deepmd_exception("PyTorch backend is not supported yet");
   } else if (deepmd::DPBackend::Paddle == backend) {
     throw deepmd::deepmd_exception("PaddlePaddle backend is not supported yet");
   } else {
     throw deepmd::deepmd_exception("Unknown file type");
   }
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/src/DeepTensorTF.cc` & `deepmd_kit-3.0.0a0/source/api_cc/src/DeepTensorTF.cc`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
+#ifdef BUILD_TENSORFLOW
 #include "DeepTensorTF.h"
 
 using namespace deepmd;
 using namespace tensorflow;
 
 DeepTensorTF::DeepTensorTF() : inited(false), graph_def(new GraphDef()) {}
 
@@ -840,7 +841,8 @@
     compute(global_tensor, coord, atype, box, nghost, inlist);
     force.clear();
     virial.clear();
     atom_tensor.clear();
     atom_virial.clear();
   }
 }
+#endif
```

### Comparing `deepmd_kit-2.2.9/source/api_cc/src/common.cc` & `deepmd_kit-3.0.0a0/source/api_cc/src/common.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
 #include "common.h"
 
 #include <fcntl.h>
 
+#include <cstring>
+#include <fstream>
+#include <sstream>
+#include <string>
+
 #include "AtomMap.h"
 #include "device.h"
 #if defined(_WIN32)
 #if defined(_WIN32_WINNT)
 #undef _WIN32_WINNT
 #endif
 
@@ -16,18 +21,21 @@
 #include <io.h>
 #include <windows.h>
 #define O_RDONLY _O_RDONLY
 #else
 // not windows
 #include <dlfcn.h>
 #endif
+#ifdef BUILD_TENSORFLOW
+#include "commonTF.h"
 #include "google/protobuf/io/zero_copy_stream_impl.h"
 #include "google/protobuf/text_format.h"
 
 using namespace tensorflow;
+#endif
 
 static std::vector<std::string> split(const std::string& input_,
                                       const std::string& delimiter) {
   std::string input = input_;
   size_t pos = 0;
   std::vector<std::string> res;
   while ((pos = input.find(delimiter)) != std::string::npos) {
@@ -281,14 +289,24 @@
       }
       new_jlist.push_back(tmp_jlist);
     }
   }
   ilist = new_ilist;
   jlist = new_jlist;
 }
+void deepmd::NeighborListData::padding() {
+  size_t max_length = 0;
+  for (const auto& row : jlist) {
+    max_length = std::max(max_length, row.size());
+  }
+
+  for (int i = 0; i < jlist.size(); i++) {
+    jlist[i].resize(max_length, -1);
+  }
+}
 
 void deepmd::NeighborListData::make_inlist(InputNlist& inlist) {
   int nloc = ilist.size();
   numneigh.resize(nloc);
   firstneigh.resize(nloc);
   for (int ii = 0; ii < nloc; ++ii) {
     numneigh[ii] = jlist[ii].size();
@@ -296,82 +314,100 @@
   }
   inlist.inum = nloc;
   inlist.ilist = &ilist[0];
   inlist.numneigh = &numneigh[0];
   inlist.firstneigh = &firstneigh[0];
 }
 
+#ifdef BUILD_TENSORFLOW
 void deepmd::check_status(const tensorflow::Status& status) {
   if (!status.ok()) {
     std::cout << status.ToString() << std::endl;
     throw deepmd::tf_exception(status.ToString());
   }
 }
+#endif
 
 void throw_env_not_set_warning(std::string env_name) {
   std::cerr << "DeePMD-kit WARNING: Environmental variable " << env_name
             << " is not set. "
             << "Tune " << env_name << " for the best performance. "
             << "See https://deepmd.rtfd.io/parallelism/ for more information."
             << std::endl;
 }
 
 void deepmd::get_env_nthreads(int& num_intra_nthreads,
                               int& num_inter_nthreads) {
   num_intra_nthreads = 0;
   num_inter_nthreads = 0;
   const char* env_intra_nthreads =
-      std::getenv("TF_INTRA_OP_PARALLELISM_THREADS");
+      std::getenv("DP_INTRA_OP_PARALLELISM_THREADS");
   const char* env_inter_nthreads =
+      std::getenv("DP_INTER_OP_PARALLELISM_THREADS");
+  // backward compatibility
+  const char* env_intra_nthreads_tf =
+      std::getenv("TF_INTRA_OP_PARALLELISM_THREADS");
+  const char* env_inter_nthreads_tf =
       std::getenv("TF_INTER_OP_PARALLELISM_THREADS");
   const char* env_omp_nthreads = std::getenv("OMP_NUM_THREADS");
   if (env_intra_nthreads &&
       std::string(env_intra_nthreads) != std::string("") &&
       atoi(env_intra_nthreads) >= 0) {
     num_intra_nthreads = atoi(env_intra_nthreads);
+  } else if (env_intra_nthreads_tf &&
+             std::string(env_intra_nthreads_tf) != std::string("") &&
+             atoi(env_intra_nthreads_tf) >= 0) {
+    num_intra_nthreads = atoi(env_intra_nthreads_tf);
   } else {
-    throw_env_not_set_warning("TF_INTRA_OP_PARALLELISM_THREADS");
+    throw_env_not_set_warning("DP_INTRA_OP_PARALLELISM_THREADS");
   }
   if (env_inter_nthreads &&
       std::string(env_inter_nthreads) != std::string("") &&
       atoi(env_inter_nthreads) >= 0) {
     num_inter_nthreads = atoi(env_inter_nthreads);
+  } else if (env_inter_nthreads_tf &&
+             std::string(env_inter_nthreads_tf) != std::string("") &&
+             atoi(env_inter_nthreads_tf) >= 0) {
+    num_inter_nthreads = atoi(env_inter_nthreads_tf);
   } else {
-    throw_env_not_set_warning("TF_INTER_OP_PARALLELISM_THREADS");
+    throw_env_not_set_warning("DP_INTER_OP_PARALLELISM_THREADS");
   }
   if (!(env_omp_nthreads && std::string(env_omp_nthreads) != std::string("") &&
         atoi(env_omp_nthreads) >= 0)) {
     throw_env_not_set_warning("OMP_NUM_THREADS");
   }
 }
 
 void deepmd::load_op_library() {
+#ifdef BUILD_TENSORFLOW
   tensorflow::Env* env = tensorflow::Env::Default();
 #if defined(_WIN32)
   std::string dso_path = "deepmd_op.dll";
   void* dso_handle = LoadLibrary(dso_path.c_str());
 #else
   std::string dso_path = "libdeepmd_op.so";
   void* dso_handle = dlopen(dso_path.c_str(), RTLD_NOW | RTLD_LOCAL);
 #endif
   if (!dso_handle) {
     throw deepmd::deepmd_exception(
         dso_path +
         " is not found! You can add the library directory to LD_LIBRARY_PATH");
   }
+#endif
 }
 
 std::string deepmd::name_prefix(const std::string& scope) {
   std::string prefix = "";
   if (scope != "") {
     prefix = scope + "/";
   }
   return prefix;
 }
 
+#ifdef BUILD_TENSORFLOW
 template <typename MODELTYPE, typename VALUETYPE>
 int deepmd::session_input_tensors(
     std::vector<std::pair<std::string, Tensor>>& input_tensors,
     const std::vector<VALUETYPE>& dcoord_,
     const int& ntypes,
     const std::vector<int>& datype_,
     const std::vector<VALUETYPE>& dbox,
@@ -846,14 +882,15 @@
   deepmd::check_status(
       session->Run(std::vector<std::pair<std::string, Tensor>>({}),
                    {name.c_str()}, {}, &output_tensors));
   Tensor output_rc = output_tensors[0];
   // cast enum to int
   return (int)output_rc.dtype();
 }
+#endif
 
 template <typename VT>
 void deepmd::select_map(std::vector<VT>& out,
                         const std::vector<VT>& in,
                         const std::vector<int>& idx_map,
                         const int& stride,
                         const int& nframes,
@@ -936,14 +973,15 @@
       for (int dd = 0; dd < stride; ++dd) {
         *(out + ii * stride + dd) = *(in + from_ii * stride + dd);
       }
     }
   }
 }
 
+#ifdef BUILD_TENSORFLOW
 template int deepmd::session_get_scalar<int>(Session*,
                                              const std::string,
                                              const std::string);
 
 template bool deepmd::session_get_scalar<bool>(Session*,
                                                const std::string,
                                                const std::string);
@@ -985,14 +1023,15 @@
                                                  const std::string,
                                                  const std::string);
 
 template void deepmd::session_get_vector<float>(std::vector<float>&,
                                                 Session*,
                                                 const std::string,
                                                 const std::string);
+#endif
 
 template void deepmd::select_map<float>(std::vector<float>& out,
                                         const std::vector<float>& in,
                                         const std::vector<int>& idx_map,
                                         const int& stride,
                                         const int& nframes,
                                         const int& nall1,
@@ -1014,22 +1053,24 @@
 
 template void deepmd::select_map_inv<float>(
     typename std::vector<float>::iterator out,
     const typename std::vector<float>::const_iterator in,
     const std::vector<int>& idx_map,
     const int& stride);
 
+#ifdef BUILD_TENSORFLOW
 template double deepmd::session_get_scalar<double>(Session*,
                                                    const std::string,
                                                    const std::string);
 
 template void deepmd::session_get_vector<double>(std::vector<double>&,
                                                  Session*,
                                                  const std::string,
                                                  const std::string);
+#endif
 
 template void deepmd::select_map<double>(std::vector<double>& out,
                                          const std::vector<double>& in,
                                          const std::vector<int>& idx_map,
                                          const int& stride,
                                          const int& nframes,
                                          const int& nall1,
@@ -1051,14 +1092,15 @@
 
 template void deepmd::select_map_inv<double>(
     typename std::vector<double>::iterator out,
     const typename std::vector<double>::const_iterator in,
     const std::vector<int>& idx_map,
     const int& stride);
 
+#ifdef BUILD_TENSORFLOW
 template deepmd::STRINGTYPE deepmd::session_get_scalar<deepmd::STRINGTYPE>(
     Session*, const std::string, const std::string);
 
 template void deepmd::session_get_vector<deepmd::STRINGTYPE>(
     std::vector<deepmd::STRINGTYPE>&,
     Session*,
     const std::string,
@@ -1089,32 +1131,47 @@
     const int& stride);
 
 template void deepmd::select_map_inv<deepmd::STRINGTYPE>(
     typename std::vector<deepmd::STRINGTYPE>::iterator out,
     const typename std::vector<deepmd::STRINGTYPE>::const_iterator in,
     const std::vector<int>& idx_map,
     const int& stride);
+#endif
 
 void deepmd::read_file_to_string(std::string model, std::string& file_content) {
-  deepmd::check_status(tensorflow::ReadFileToString(tensorflow::Env::Default(),
-                                                    model, &file_content));
+  // generated by GitHub Copilot
+  std::ifstream file(model);
+  if (file.is_open()) {
+    std::stringstream buffer;
+    buffer << file.rdbuf();
+    file_content = buffer.str();
+    file.close();
+  } else {
+    throw deepmd::deepmd_exception("Failed to open file: " + model);
+  }
 }
 
 void deepmd::convert_pbtxt_to_pb(std::string fn_pb_txt, std::string fn_pb) {
+#ifdef BUILD_TENSORFLOW
   int fd = open(fn_pb_txt.c_str(), O_RDONLY);
   tensorflow::protobuf::io::ZeroCopyInputStream* input =
       new tensorflow::protobuf::io::FileInputStream(fd);
   tensorflow::GraphDef graph_def;
   tensorflow::protobuf::TextFormat::Parse(input, &graph_def);
   delete input;
   std::fstream output(fn_pb,
                       std::ios::out | std::ios::trunc | std::ios::binary);
   graph_def.SerializeToOstream(&output);
+#else
+  throw deepmd::deepmd_exception(
+      "convert_pbtxt_to_pb: TensorFlow backend is not enabled.");
+#endif
 }
 
+#ifdef BUILD_TENSORFLOW
 template int deepmd::session_input_tensors<double, double>(
     std::vector<std::pair<std::string, tensorflow::Tensor>>& input_tensors,
     const std::vector<double>& dcoord_,
     const int& ntypes,
     const std::vector<int>& datype_,
     const std::vector<double>& dbox,
     const double& cell_size,
@@ -1268,14 +1325,15 @@
     const std::vector<float>& dbox,
     const double& cell_size,
     const std::vector<float>& fparam_,
     const std::vector<float>& aparam_,
     const deepmd::AtomMap& atommap,
     const std::string scope,
     const bool aparam_nall);
+#endif
 
 void deepmd::print_summary(const std::string& pre) {
   int num_intra_nthreads, num_inter_nthreads;
   deepmd::get_env_nthreads(num_intra_nthreads, num_inter_nthreads);
   std::cout << pre << "installed to:       " + global_install_prefix << "\n";
   std::cout << pre << "source:             " + global_git_summ << "\n";
   std::cout << pre << "source branch:      " + global_git_branch << "\n";
@@ -1288,16 +1346,21 @@
 #elif defined(TENSORFLOW_USE_ROCM)
   std::cout << pre << "build variant:      rocm"
             << "\n";
 #else
   std::cout << pre << "build variant:      cpu"
             << "\n";
 #endif
+#ifdef BUILD_TENSORFLOW
   std::cout << pre << "build with tf inc:  " + global_tf_include_dir << "\n";
   std::cout << pre << "build with tf lib:  " + global_tf_lib << "\n";
+#endif
+#ifdef BUILD_PYTORCH
+  std::cout << pre << "build with pt lib:  " + global_pt_lib << "\n";
+#endif
   std::cout << pre
             << "set tf intra_op_parallelism_threads: " << num_intra_nthreads
             << "\n";
   std::cout << pre
             << "set tf inter_op_parallelism_threads: " << num_inter_nthreads
             << std::endl;
 }
```

### Comparing `deepmd_kit-2.2.9/source/cmake/Findtensorflow.cmake` & `deepmd_kit-3.0.0a0/source/cmake/Findtensorflow.cmake`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/cmake/Findxdrfile.cmake` & `deepmd_kit-3.0.0a0/source/cmake/Findxdrfile.cmake`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/cmake/cmake_lammps.cmake.in` & `deepmd_kit-3.0.0a0/source/cmake/cmake_lammps.cmake.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/cmake/cmake_uninstall.cmake.in` & `deepmd_kit-3.0.0a0/source/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/cmake/googletest.cmake.in` & `deepmd_kit-3.0.0a0/source/cmake/googletest.cmake.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/gmx/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/gmx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/gmx/dp_gmx_patch` & `deepmd_kit-3.0.0a0/source/gmx/dp_gmx_patch`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/gmx/include/gmx_plugin.h` & `deepmd_kit-3.0.0a0/source/gmx/include/gmx_plugin.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/gmx/patches/2020.2/CMakeLists.txt.patch.in` & `deepmd_kit-3.0.0a0/source/gmx/patches/2020.2/CMakeLists.txt.patch.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/gmx/patches/2020.2/src/gromacs/mdlib/forcerec.cpp.patch` & `deepmd_kit-3.0.0a0/source/gmx/patches/2020.2/src/gromacs/mdlib/forcerec.cpp.patch`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/gmx/patches/2020.2/src/gromacs/mdlib/sim_util.cpp.patch` & `deepmd_kit-3.0.0a0/source/gmx/patches/2020.2/src/gromacs/mdlib/sim_util.cpp.patch`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/gmx/src/gmx_plugin.cpp` & `deepmd_kit-3.0.0a0/source/gmx/src/gmx_plugin.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/install/build_cc.sh` & `deepmd_kit-3.0.0a0/source/install/build_cc.sh`

 * *Files 8% similar despite different names*

```diff
@@ -16,13 +16,19 @@
 NPROC=$(nproc --all)
 
 #------------------
 
 BUILD_TMP_DIR=${SCRIPT_PATH}/../build
 mkdir -p ${BUILD_TMP_DIR}
 cd ${BUILD_TMP_DIR}
-cmake -DCMAKE_INSTALL_PREFIX=${INSTALL_PREFIX} -DUSE_TF_PYTHON_LIBS=TRUE ${CUDA_ARGS} -DLAMMPS_VERSION=stable_2Aug2023_update2 ..
+cmake -D ENABLE_TENSORFLOW=ON \
+	-D ENABLE_PYTORCH=ON \
+	-D CMAKE_INSTALL_PREFIX=${INSTALL_PREFIX} \
+	-D USE_TF_PYTHON_LIBS=TRUE \
+	${CUDA_ARGS} \
+	-D LAMMPS_VERSION=stable_2Aug2023_update3 \
+	..
 cmake --build . -j${NPROC}
 cmake --install .
 
 #------------------
 echo "Congratulations! DeePMD-kit has been installed at ${INSTALL_PREFIX}"
```

### Comparing `deepmd_kit-2.2.9/source/install/build_from_c.sh` & `deepmd_kit-3.0.0a0/source/install/build_from_c.sh`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 NPROC=$(nproc --all)
 
 #------------------
 
 BUILD_TMP_DIR=${SCRIPT_PATH}/../build
 mkdir -p ${BUILD_TMP_DIR}
 cd ${BUILD_TMP_DIR}
-cmake -DCMAKE_INSTALL_PREFIX=${INSTALL_PREFIX} -DDEEPMD_C_ROOT=${DEEPMD_C_ROOT} -DLAMMPS_VERSION=stable_2Aug2023_update2 ..
+cmake -DCMAKE_INSTALL_PREFIX=${INSTALL_PREFIX} -DDEEPMD_C_ROOT=${DEEPMD_C_ROOT} -DLAMMPS_VERSION=stable_2Aug2023_update3 ..
 cmake --build . -j${NPROC}
 cmake --install .
 cmake --build . --target=lammps
 
 #------------------
 echo "Congratulations! DeePMD-kit has been installed at ${INSTALL_PREFIX}"
```

### Comparing `deepmd_kit-2.2.9/source/install/build_lammps.sh` & `deepmd_kit-3.0.0a0/source/install/build_lammps.sh`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #------------------
 
 BUILD_TMP_DIR=${SCRIPT_PATH}/../build_lammps
 mkdir -p ${BUILD_TMP_DIR}
 cd ${BUILD_TMP_DIR}
 # download LAMMMPS
-LAMMPS_VERSION=stable_2Aug2023_update2
+LAMMPS_VERSION=stable_2Aug2023_update3
 if [ ! -d "lammps-${LAMMPS_VERSION}" ]; then
 	curl -L -o lammps.tar.gz https://github.com/lammps/lammps/archive/refs/tags/${LAMMPS_VERSION}.tar.gz
 	tar vxzf lammps.tar.gz
 fi
 
 cd ${BUILD_TMP_DIR}/lammps-${LAMMPS_VERSION}
 mkdir -p ${BUILD_TMP_DIR}/lammps-${LAMMPS_VERSION}/build
```

### Comparing `deepmd_kit-2.2.9/source/install/build_tf.py` & `deepmd_kit-3.0.0a0/source/install/build_tf.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,15 @@
     Yields
     ------
     None
 
     Examples
     --------
     >>> with set_directory("some_path"):
-    ...    do_something()
+    ...     do_something()
     """
     cwd = Path().absolute()
     path.mkdir(exist_ok=True, parents=True)
     try:
         os.chdir(path)
         yield
     finally:
@@ -419,22 +419,22 @@
 
 
 class BuildBazelisk(Build):
     def __init__(self, version="1.11.0") -> None:
         self.version = version
 
     @property
-    @lru_cache()
+    @lru_cache
     def resources(self) -> Dict[str, OnlineResource]:
         return {
             "bazelisk": RESOURCES["bazelisk-" + self.version],
         }
 
     @property
-    @lru_cache()
+    @lru_cache
     def dependencies(self) -> Dict[str, Build]:
         return {}
 
     def build(self):
         bazel_res = self.resources["bazelisk"]
         bin_dst = self.prefix / "bin"
         bin_dst.mkdir(exist_ok=True)
@@ -445,20 +445,20 @@
         return (PREFIX / "bin" / "bazelisk").exists()
 
 
 class BuildNumpy(Build):
     """Build NumPy."""
 
     @property
-    @lru_cache()
+    @lru_cache
     def resources(self) -> Dict[str, OnlineResource]:
         return {}
 
     @property
-    @lru_cache()
+    @lru_cache
     def dependencies(self) -> Dict[str, Build]:
         return {}
 
     @property
     def built(self) -> bool:
         return importlib.util.find_spec("numpy") is not None
 
@@ -477,20 +477,20 @@
             raise RuntimeError("Please manually install numpy!") from e
 
 
 class BuildCUDA(Build):
     """Find CUDA."""
 
     @property
-    @lru_cache()
+    @lru_cache
     def resources(self) -> Dict[str, OnlineResource]:
         return {}
 
     @property
-    @lru_cache()
+    @lru_cache
     def dependencies(self) -> Dict[str, Build]:
         return {}
 
     def build(self):
         raise RuntimeError(
             "NVCC is not found. Please manually install CUDA"
             "Toolkit and cuDNN!\n"
@@ -532,15 +532,15 @@
                     return line.split()[-1]
         raise RuntimeError(
             "cuDNN version is not found!\n"
             "Download from: https://developer.nvidia.com/rdp/cudnn-archive"
         )
 
     @property
-    @lru_cache()
+    @lru_cache
     def cuda_compute_capabilities(self):
         """Get cuda compute capabilities."""
         cuda_version = tuple(map(int, self.cuda_version.split(".")))
         if (10, 0, 0) <= cuda_version < (11, 0, 0):
             return "sm_35,sm_50,sm_60,sm_62,sm_70,sm_72,sm_75,compute_75"
         elif (11, 0, 0) <= cuda_version < (11, 1, 0):
             return "sm_35,sm_50,sm_60,sm_62,sm_70,sm_72,sm_75,sm_80,compute_80"
@@ -550,20 +550,20 @@
             raise RuntimeError("Unsupported CUDA version")
 
 
 class BuildROCM(Build):
     """Find ROCm."""
 
     @property
-    @lru_cache()
+    @lru_cache
     def resources(self) -> Dict[str, OnlineResource]:
         return {}
 
     @property
-    @lru_cache()
+    @lru_cache
     def dependencies(self) -> Dict[str, Build]:
         return {}
 
     def build(self):
         raise RuntimeError("ROCm is not found!")
 
     @property
@@ -595,22 +595,22 @@
     ) -> None:
         self.version = version
         self.enable_mkl = enable_mkl
         self.enable_cuda = enable_cuda
         self.enable_rocm = enable_rocm
 
     @property
-    @lru_cache()
+    @lru_cache
     def resources(self) -> Dict[str, OnlineResource]:
         return {
             "tensorflow": RESOURCES["tensorflow-" + self.version],
         }
 
     @property
-    @lru_cache()
+    @lru_cache
     def dependencies(self) -> Dict[str, Build]:
         optional_dep = {}
         if self.enable_cuda:
             optional_dep["cuda"] = BuildCUDA()
         if self.enable_rocm:
             optional_dep["rocm"] = BuildROCM()
         return {
```

### Comparing `deepmd_kit-2.2.9/source/install/docker/Dockerfile` & `deepmd_kit-3.0.0a0/source/install/docker/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 ARG VARIANT=""
 ARG CUDA_VERSION="12"
 RUN python -m venv /opt/deepmd-kit
 # Make sure we use the virtualenv
 ENV PATH="/opt/deepmd-kit/bin:$PATH"
 # Install package
 COPY dist /dist
-RUN pip install "$(ls /dist/deepmd_kit${VARIANT}-*manylinux*_x86_64.whl)[gpu,cu${CUDA_VERSION},lmp,ipi]" \
+RUN if [ "${CUDA_VERSION}" = 11 ]; then pip install torch --index-url https://download.pytorch.org/whl/cu118; fi \
+    && pip install "$(ls /dist/deepmd_kit${VARIANT}-*manylinux*_x86_64.whl)[gpu,cu${CUDA_VERSION},lmp,ipi,torch]" \
     && dp -h \
     && lmp -h \
     && dp_ipi \
     && python -m deepmd -h
 
 FROM python:3.11 AS build-image
 COPY --from=compile-image /opt/deepmd-kit /opt/deepmd-kit
```

### Comparing `deepmd_kit-2.2.9/source/install/docker_test_package_c.sh` & `deepmd_kit-3.0.0a0/source/install/docker_test_package_c.sh`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/install/install_tf.sh` & `deepmd_kit-3.0.0a0/source/install/install_tf.sh`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/install/package_c.sh` & `deepmd_kit-3.0.0a0/source/install/package_c.sh`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/ipi/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/ipi/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 target_include_directories(${libipiname} PUBLIC ${MD_INCLUDE_PATH})
 
 set(DRIVER_SOURCE_FILES driver.cc)
 add_executable(${ipiname} ${DRIVER_SOURCE_FILES})
 # link: libdeepmd_cc
 if(DP_USING_C_API)
   # SimulationRegion.h
-  target_link_libraries(${ipiname} PRIVATE ${LIB_DEEPMD_C} ${LIB_DEEPMD})
+  target_link_libraries(${ipiname} PRIVATE ${LIB_DEEPMD_C})
   target_precompile_headers(${ipiname} PRIVATE [["deepmd.hpp"]])
   remove_definitions(-D_GLIBCXX_USE_CXX11_ABI=${OP_CXX_ABI})
 else()
   target_link_libraries(${ipiname} PRIVATE ${LIB_DEEPMD_CC})
   target_compile_definitions(${ipiname} PRIVATE "DP_USE_CXX_API")
 endif()
 target_link_libraries(${ipiname} PRIVATE ${libipiname})
```

### Comparing `deepmd_kit-2.2.9/source/ipi/driver.cc` & `deepmd_kit-3.0.0a0/source/ipi/driver.cc`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #ifdef DP_USE_CXX_API
 #include "DeepPot.h"
 namespace deepmd_compat = deepmd;
 #else
 #include "deepmd.hpp"
 namespace deepmd_compat = deepmd::hpp;
 #endif
-#include "SimulationRegion.h"
 #include "XyzFileManager.h"
 #include "json.hpp"
 #include "sockets.h"
 using json = nlohmann::json;
 
 // using namespace std;
 
@@ -45,33 +44,14 @@
     end--;
   }
   // Write new null terminator
   *(end + 1) = 0;
   return str;
 }
 
-void normalize_coord(std::vector<double> &coord,
-                     const SimulationRegion<double> &region) {
-  int natoms = coord.size() / 3;
-
-  for (int ii = 0; ii < natoms; ++ii) {
-    double inter[3];
-    region.phys2Inter(inter, &coord[3 * ii]);
-    for (int dd = 0; dd < 3; ++dd) {
-      inter[dd] -= int(floor(inter[dd]));
-      if (inter[dd] < 0) {
-        inter[dd] += 1.;
-      } else if (inter[dd] >= 1) {
-        inter[dd] -= 1.;
-      }
-    }
-    region.inter2Phys(&coord[3 * ii], inter);
-  }
-}
-
 int main(int argc, char *argv[]) {
   if (argc == 1) {
     std::cerr << "usage " << std::endl;
     std::cerr << argv[0] << " input_script " << std::endl;
     return 0;
   }
 
@@ -118,15 +98,14 @@
   std::vector<double> dforce;
   std::vector<double> dforce_tmp;
   std::vector<double> dvirial(9, 0);
   std::vector<double> dcoord;
   std::vector<double> dcoord_tmp;
   std::vector<int> dtype = cvt.get_type();
   std::vector<double> dbox(9, 0);
-  SimulationRegion<double> region;
   double *msg_buff = NULL;
   double ener;
   double virial[9];
   char msg_needinit[] = "NEEDINIT    ";
   char msg_havedata[] = "HAVEDATA    ";
   char msg_ready[] = "READY       ";
   char msg_forceready[] = "FORCEREADY  ";
@@ -175,15 +154,14 @@
 
       // get box
       readbuffer_(&socket, (char *)(cell_h), 9 * sizeof(double));
       readbuffer_(&socket, (char *)(cell_ih), 9 * sizeof(double));
       for (int dd = 0; dd < 9; ++dd) {
         dbox[dd] = cell_h[(dd % 3) * 3 + (dd / 3)] * cvt_len;
       }
-      region.reinitBox(&dbox[0]);
 
       // get number of atoms
       readbuffer_(&socket, (char *)(&cbuf), sizeof(int32_t));
       if (natoms < 0) {
         natoms = cbuf;
         if (b_verb) {
           std::cout << "# get number of atoms in system: " << natoms
@@ -199,15 +177,14 @@
 
       // get coord
       readbuffer_(&socket, (char *)(msg_buff), natoms * 3 * sizeof(double));
       for (int ii = 0; ii < natoms * 3; ++ii) {
         dcoord_tmp[ii] = msg_buff[ii] * cvt_len;
       }
       cvt.forward(dcoord, dcoord_tmp, 3);
-      normalize_coord(dcoord, region);
 
       // nnp over writes ener, force and virial
       nnp_inter.compute(dener, dforce_tmp, dvirial, dcoord, dtype, dbox);
       cvt.backward(dforce, dforce_tmp, 3);
       hasdata = true;
     } else if (header_str == "GETFORCE") {
       ener = dener * icvt_ener;
```

### Comparing `deepmd_kit-2.2.9/source/ipi/include/Convert.h` & `deepmd_kit-3.0.0a0/source/ipi/include/Convert.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/ipi/include/StringSplit.h` & `deepmd_kit-3.0.0a0/source/ipi/include/StringSplit.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/ipi/include/sockets.h` & `deepmd_kit-3.0.0a0/source/ipi/include/sockets.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/ipi/src/Convert.cc` & `deepmd_kit-3.0.0a0/source/ipi/src/Convert.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/ipi/src/XyzFileManager.cc` & `deepmd_kit-3.0.0a0/source/ipi/src/XyzFileManager.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/ipi/src/sockets.c` & `deepmd_kit-3.0.0a0/source/ipi/src/sockets.c`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/ipi/tests/test_driver.py` & `deepmd_kit-3.0.0a0/deepmd/pt/model/network/mlp.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,223 +1,223 @@
 # SPDX-License-Identifier: LGPL-3.0-or-later
-import json
-import os
-import sys
-import unittest
-from pathlib import (
-    Path,
+from typing import (
+    ClassVar,
+    Dict,
+    Optional,
 )
 
 import numpy as np
-from ase import (
-    Atoms,
+import torch
+import torch.nn as nn
+
+from deepmd.pt.utils import (
+    env,
+)
+
+device = env.DEVICE
+
+from deepmd.dpmodel.utils import (
+    NativeLayer,
 )
-from ase.calculators.calculator import (
-    FileIOCalculator,
+from deepmd.dpmodel.utils import NetworkCollection as DPNetworkCollection
+from deepmd.dpmodel.utils import (
+    make_embedding_network,
+    make_fitting_network,
+    make_multilayer_network,
 )
-from ase.calculators.socketio import (
-    SocketIOCalculator,
+from deepmd.pt.utils.env import (
+    DEFAULT_PRECISION,
+    PRECISION_DICT,
+)
+from deepmd.pt.utils.utils import (
+    ActivationFn,
 )
 
-from deepmd.utils.convert import (
-    convert_pbtxt_to_pb,
-)
-
-tests_path = Path(__file__).parent.parent.parent / "tests"
-default_places = 6
-
-
-class DPiPICalculator(FileIOCalculator):
-    def __init__(self, model: str, use_unix: bool = True, **kwargs):
-        self.xyz_file = "test_ipi.xyz"
-        self.config_file = "config.json"
-        config = {
-            "verbose": False,
-            "use_unix": use_unix,
-            "port": 31415,
-            "host": "localhost",
-            "graph_file": model,
-            "coord_file": self.xyz_file,
-            "atom_type": {
-                "O": 0,
-                "H": 1,
-            },
-        }
-        with open(self.config_file, "w") as f:
-            json.dump(config, f)
-        command = "dp_ipi " + self.config_file
-        FileIOCalculator.__init__(
-            self, command=command, label=self.config_file, **kwargs
+try:
+    from deepmd._version import version as __version__
+except ImportError:
+    __version__ = "unknown"
+
+
+def empty_t(shape, precision):
+    return torch.empty(shape, dtype=precision, device=device)
+
+
+class MLPLayer(nn.Module):
+    def __init__(
+        self,
+        num_in,
+        num_out,
+        bias: bool = True,
+        use_timestep: bool = False,
+        activation_function: Optional[str] = None,
+        resnet: bool = False,
+        bavg: float = 0.0,
+        stddev: float = 1.0,
+        precision: str = DEFAULT_PRECISION,
+    ):
+        super().__init__()
+        # only use_timestep when skip connection is established.
+        self.use_timestep = use_timestep and (
+            num_out == num_in or num_out == num_in * 2
+        )
+        self.activate_name = activation_function
+        self.activate = ActivationFn(self.activate_name)
+        self.precision = precision
+        self.prec = PRECISION_DICT[self.precision]
+        self.matrix = nn.Parameter(data=empty_t((num_in, num_out), self.prec))
+        nn.init.normal_(self.matrix.data, std=stddev / np.sqrt(num_out + num_in))
+        if bias:
+            self.bias = nn.Parameter(
+                data=empty_t([num_out], self.prec),
+            )
+            nn.init.normal_(self.bias.data, mean=bavg, std=stddev)
+        else:
+            self.bias = None
+        if self.use_timestep:
+            self.idt = nn.Parameter(data=empty_t([num_out], self.prec))
+            nn.init.normal_(self.idt.data, mean=0.1, std=0.001)
+        else:
+            self.idt = None
+        self.resnet = resnet
+
+    def check_type_consistency(self):
+        precision = self.precision
+
+        def check_var(var):
+            if var is not None:
+                # assertion "float64" == "double" would fail
+                assert PRECISION_DICT[var.dtype.name] is PRECISION_DICT[precision]
+
+        check_var(self.w)
+        check_var(self.b)
+        check_var(self.idt)
+
+    def dim_in(self) -> int:
+        return self.matrix.shape[0]
+
+    def dim_out(self) -> int:
+        return self.matrix.shape[1]
+
+    def forward(
+        self,
+        xx: torch.Tensor,
+    ) -> torch.Tensor:
+        """One MLP layer used by DP model.
+
+        Parameters
+        ----------
+        xx : torch.Tensor
+            The input.
+
+        Returns
+        -------
+        yy: torch.Tensor
+            The output.
+        """
+        ori_prec = xx.dtype
+        xx = xx.to(self.prec)
+        yy = (
+            torch.matmul(xx, self.matrix) + self.bias
+            if self.bias is not None
+            else torch.matmul(xx, self.matrix)
+        )
+        yy = self.activate(yy).clone()
+        yy = yy * self.idt if self.idt is not None else yy
+        if self.resnet:
+            if xx.shape[-1] == yy.shape[-1]:
+                yy += xx
+            elif 2 * xx.shape[-1] == yy.shape[-1]:
+                yy += torch.concat([xx, xx], dim=-1)
+            else:
+                yy = yy
+        yy = yy.to(ori_prec)
+        return yy
+
+    def serialize(self) -> dict:
+        """Serialize the layer to a dict.
+
+        Returns
+        -------
+        dict
+            The serialized layer.
+        """
+        nl = NativeLayer(
+            self.matrix.shape[0],
+            self.matrix.shape[1],
+            bias=self.bias is not None,
+            use_timestep=self.idt is not None,
+            activation_function=self.activate_name,
+            resnet=self.resnet,
+            precision=self.precision,
+        )
+        nl.w, nl.b, nl.idt = (
+            self.matrix.detach().cpu().numpy(),
+            self.bias.detach().cpu().numpy() if self.bias is not None else None,
+            self.idt.detach().cpu().numpy() if self.idt is not None else None,
         )
+        return nl.serialize()
 
-    def write_input(self, atoms, **kwargs):
-        atoms.write(self.xyz_file, format="xyz")
+    @classmethod
+    def deserialize(cls, data: dict) -> "MLPLayer":
+        """Deserialize the layer from a dict.
 
+        Parameters
+        ----------
+        data : dict
+            The dict to deserialize from.
+        """
+        nl = NativeLayer.deserialize(data)
+        obj = cls(
+            nl["matrix"].shape[0],
+            nl["matrix"].shape[1],
+            bias=nl["bias"] is not None,
+            use_timestep=nl["idt"] is not None,
+            activation_function=nl["activation_function"],
+            resnet=nl["resnet"],
+            precision=nl["precision"],
+        )
+        prec = PRECISION_DICT[obj.precision]
+
+        def check_load_param(ss):
+            return (
+                nn.Parameter(data=torch.tensor(nl[ss], dtype=prec, device=device))
+                if nl[ss] is not None
+                else None
+            )
 
-class TestDeepPotALargeBoxNoPBC(unittest.TestCase):
-    # copy from test_deeppot_a.py
-    @classmethod
-    def setUpClass(cls):
-        cls.model_file = "deeppot.pb"
-        convert_pbtxt_to_pb(
-            str(tests_path / os.path.join("infer", "deeppot.pbtxt")), "deeppot.pb"
-        )
+        obj.matrix = check_load_param("matrix")
+        obj.bias = check_load_param("bias")
+        obj.idt = check_load_param("idt")
+        return obj
 
-    def setUp(self):
-        self.coords = np.array(
-            [
-                12.83,
-                2.56,
-                2.18,
-                12.09,
-                2.87,
-                2.74,
-                00.25,
-                3.32,
-                1.68,
-                3.36,
-                3.00,
-                1.81,
-                3.51,
-                2.51,
-                2.60,
-                4.27,
-                3.22,
-                1.56,
-            ]
-        )
-        self.atype = [0, 1, 1, 0, 1, 1]
-        self.box = np.array([19.0, 0.0, 0.0, 0.0, 13.0, 0.0, 0.0, 0.0, 13.0])
-        self.expected_e = np.array(
-            [
-                -9.255934839310273787e01,
-                -1.863253376736990106e02,
-                -1.857237299341402945e02,
-                -9.279308539717486326e01,
-                -1.863708105823244239e02,
-                -1.863635196514972563e02,
-            ]
-        )
-        self.expected_f = np.array(
-            [
-                -2.161037360255332107e00,
-                9.052994347015581589e-01,
-                1.635379623977007979e00,
-                2.161037360255332107e00,
-                -9.052994347015581589e-01,
-                -1.635379623977007979e00,
-                -1.167128117249453811e-02,
-                1.371975700096064992e-03,
-                -1.575265180249604477e-03,
-                6.226508593971802341e-01,
-                -1.816734122009256991e-01,
-                3.561766019664774907e-01,
-                -1.406075393906316626e-02,
-                3.789140061530929526e-01,
-                -6.018777878642909140e-01,
-                -5.969188242856223736e-01,
-                -1.986125696522633155e-01,
-                2.472764510780630642e-01,
-            ]
-        )
-        self.expected_v = np.array(
-            [
-                -7.042445481792056761e-01,
-                2.950213647777754078e-01,
-                5.329418202437231633e-01,
-                2.950213647777752968e-01,
-                -1.235900311906896754e-01,
-                -2.232594111831812944e-01,
-                5.329418202437232743e-01,
-                -2.232594111831813499e-01,
-                -4.033073234276823849e-01,
-                -8.949230984097404917e-01,
-                3.749002169013777030e-01,
-                6.772391014992630298e-01,
-                3.749002169013777586e-01,
-                -1.570527935667933583e-01,
-                -2.837082722496912512e-01,
-                6.772391014992631408e-01,
-                -2.837082722496912512e-01,
-                -5.125052659994422388e-01,
-                4.858210330291591605e-02,
-                -6.902596153269104431e-03,
-                6.682612642430500391e-03,
-                -5.612247004554610057e-03,
-                9.767795567660207592e-04,
-                -9.773758942738038254e-04,
-                5.638322117219018645e-03,
-                -9.483806049779926932e-04,
-                8.493873281881353637e-04,
-                -2.941738570564985666e-01,
-                -4.482529909499673171e-02,
-                4.091569840186781021e-02,
-                -4.509020615859140463e-02,
-                -1.013919988807244071e-01,
-                1.551440772665269030e-01,
-                4.181857726606644232e-02,
-                1.547200233064863484e-01,
-                -2.398213304685777592e-01,
-                -3.218625798524068354e-02,
-                -1.012438450438508421e-02,
-                1.271639330380921855e-02,
-                3.072814938490859779e-03,
-                -9.556241797915024372e-02,
-                1.512251983492413077e-01,
-                -8.277872384009607454e-03,
-                1.505412040827929787e-01,
-                -2.386150620881526407e-01,
-                -2.312295470054945568e-01,
-                -6.631490213524345034e-02,
-                7.932427266386249398e-02,
-                -8.053754366323923053e-02,
-                -3.294595881137418747e-02,
-                4.342495071150231922e-02,
-                1.004599500126941436e-01,
-                4.450400364869536163e-02,
-                -5.951077548033092968e-02,
-            ]
-        )
 
-    @classmethod
-    def tearDownClass(cls):
-        os.remove("deeppot.pb")
-        cls.dp = None
-
-    def test_ase_unix(self):
-        with SocketIOCalculator(
-            DPiPICalculator(self.model_file), log=sys.stdout, unixsocket="localhost"
-        ) as calc:
-            water = Atoms(
-                "OHHOHH",
-                positions=self.coords.reshape((-1, 3)),
-                cell=self.box.reshape((3, 3)),
-                calculator=calc,
-            )
-        ee = water.get_potential_energy()
-        ff = water.get_forces()
-        nframes = 1
-        np.testing.assert_almost_equal(
-            ff.ravel(), self.expected_f.ravel(), default_places
-        )
-        expected_se = np.sum(self.expected_e.reshape([nframes, -1]), axis=1)
-        np.testing.assert_almost_equal(ee.ravel(), expected_se.ravel(), default_places)
+MLP_ = make_multilayer_network(MLPLayer, nn.Module)
 
-    def test_ase_nounix(self):
-        with SocketIOCalculator(
-            DPiPICalculator(self.model_file, use_unix=False),
-            log=sys.stdout,
-        ) as calc:
-            water = Atoms(
-                "OHHOHH",
-                positions=self.coords.reshape((-1, 3)),
-                cell=self.box.reshape((3, 3)),
-                calculator=calc,
-            )
-        ee = water.get_potential_energy()
-        ff = water.get_forces()
-        nframes = 1
-        np.testing.assert_almost_equal(
-            ff.ravel(), self.expected_f.ravel(), default_places
-        )
-        expected_se = np.sum(self.expected_e.reshape([nframes, -1]), axis=1)
-        np.testing.assert_almost_equal(ee.ravel(), expected_se.ravel(), default_places)
+
+class MLP(MLP_):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.layers = torch.nn.ModuleList(self.layers)
+
+    forward = MLP_.call
+
+
+EmbeddingNet = make_embedding_network(MLP, MLPLayer)
+
+FittingNet = make_fitting_network(EmbeddingNet, MLP, MLPLayer)
+
+
+class NetworkCollection(DPNetworkCollection, nn.Module):
+    """PyTorch implementation of NetworkCollection."""
+
+    NETWORK_TYPE_MAP: ClassVar[Dict[str, type]] = {
+        "network": MLP,
+        "embedding_network": EmbeddingNet,
+        "fitting_network": FittingNet,
+    }
+
+    def __init__(self, *args, **kwargs):
+        # init both two base classes
+        DPNetworkCollection.__init__(self, *args, **kwargs)
+        nn.Module.__init__(self)
+        self.networks = self._networks = torch.nn.ModuleList(self._networks)
```

### Comparing `deepmd_kit-2.2.9/source/lib/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/ComputeDescriptor.h` & `deepmd_kit-3.0.0a0/source/lib/include/ComputeDescriptor.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/DeviceFunctor.h` & `deepmd_kit-3.0.0a0/source/lib/include/DeviceFunctor.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/SimulationRegion.h` & `deepmd_kit-3.0.0a0/source/lib/include/SimulationRegion.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/SimulationRegion_Impl.h` & `deepmd_kit-3.0.0a0/source/lib/include/SimulationRegion_Impl.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/coord.h` & `deepmd_kit-3.0.0a0/source/lib/include/coord.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/env_mat.h` & `deepmd_kit-3.0.0a0/source/lib/include/env_mat.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/env_mat_nvnmd.h` & `deepmd_kit-3.0.0a0/source/lib/include/env_mat_nvnmd.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/errors.h` & `deepmd_kit-3.0.0a0/source/lib/include/errors.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/ewald.h` & `deepmd_kit-3.0.0a0/source/lib/include/ewald.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/fmt_nlist.h` & `deepmd_kit-3.0.0a0/source/lib/include/fmt_nlist.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/gelu.h` & `deepmd_kit-3.0.0a0/source/lib/include/gelu.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/gpu_cuda.h` & `deepmd_kit-3.0.0a0/source/lib/include/gpu_cuda.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/gpu_rocm.h` & `deepmd_kit-3.0.0a0/source/lib/include/gpu_rocm.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/neighbor_list.h` & `deepmd_kit-3.0.0a0/source/lib/include/neighbor_list.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/neighbor_stat.h` & `deepmd_kit-3.0.0a0/source/lib/include/neighbor_stat.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/pair_tab.h` & `deepmd_kit-3.0.0a0/source/lib/include/pair_tab.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/pairwise.h` & `deepmd_kit-3.0.0a0/source/lib/include/pairwise.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/prod_env_mat.h` & `deepmd_kit-3.0.0a0/source/lib/include/prod_env_mat.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/prod_env_mat_nvnmd.h` & `deepmd_kit-3.0.0a0/source/lib/include/prod_env_mat_nvnmd.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/prod_force.h` & `deepmd_kit-3.0.0a0/source/lib/include/prod_force.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/prod_force_grad.h` & `deepmd_kit-3.0.0a0/source/lib/include/prod_force_grad.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/prod_virial.h` & `deepmd_kit-3.0.0a0/source/lib/include/prod_virial.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/prod_virial_grad.h` & `deepmd_kit-3.0.0a0/source/lib/include/prod_virial_grad.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/region.cuh` & `deepmd_kit-3.0.0a0/source/lib/include/region.cuh`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/region.h` & `deepmd_kit-3.0.0a0/source/lib/include/region.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/soft_min_switch_virial.h` & `deepmd_kit-3.0.0a0/source/lib/include/soft_min_switch_virial.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/switcher.h` & `deepmd_kit-3.0.0a0/source/lib/include/switcher.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/tabulate.h` & `deepmd_kit-3.0.0a0/source/lib/include/tabulate.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/include/utilities.h` & `deepmd_kit-3.0.0a0/source/lib/include/utilities.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/coord.cc` & `deepmd_kit-3.0.0a0/source/lib/src/coord.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/env_mat.cc` & `deepmd_kit-3.0.0a0/source/lib/src/env_mat.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/env_mat_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/lib/src/env_mat_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/ewald.cc` & `deepmd_kit-3.0.0a0/source/lib/src/ewald.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/fmt_nlist.cc` & `deepmd_kit-3.0.0a0/source/lib/src/fmt_nlist.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gelu.cc` & `deepmd_kit-3.0.0a0/source/lib/src/gelu.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,18 @@
   set(GPU_LIB_NAME deepmd_op_cuda)
 
   if(NOT DEFINED CMAKE_CUDA_ARCHITECTURES)
     set(CMAKE_CUDA_ARCHITECTURES all)
   endif()
   enable_language(CUDA)
   set(CMAKE_CUDA_STANDARD 11)
-  add_compile_definitions(
-    "$<$<COMPILE_LANGUAGE:CUDA>:_GLIBCXX_USE_CXX11_ABI=${OP_CXX_ABI}>")
+  if(DEFINED OP_CXX_ABI)
+    add_compile_definitions(
+      "$<$<COMPILE_LANGUAGE:CUDA>:_GLIBCXX_USE_CXX11_ABI=${OP_CXX_ABI}>")
+  endif()
 
   find_package(CUDAToolkit REQUIRED)
 
   # take dynamic open cudart library replace of static one so it's not required
   # when using CPUs
   add_subdirectory(cudart)
```

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/coord.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/coord.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/cudart/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/cudart/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/cudart/cudart_stub.cc` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/cudart/cudart_stub.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/gelu.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/gelu.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/neighbor_list.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/neighbor_list.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/neighbor_stat.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/neighbor_stat.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/prod_env_mat.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_env_mat.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/prod_force.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_force.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/prod_force_grad.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_force_grad.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/prod_virial.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_virial.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/prod_virial_grad.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/prod_virial_grad.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/region.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/region.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/gpu/tabulate.cu` & `deepmd_kit-3.0.0a0/source/lib/src/gpu/tabulate.cu`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/map_aparam.cc` & `deepmd_kit-3.0.0a0/source/lib/src/map_aparam.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/neighbor_list.cc` & `deepmd_kit-3.0.0a0/source/lib/src/neighbor_list.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/pair_tab.cc` & `deepmd_kit-3.0.0a0/source/lib/src/pair_tab.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/pairwise.cc` & `deepmd_kit-3.0.0a0/source/lib/src/pairwise.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/prod_env_mat.cc` & `deepmd_kit-3.0.0a0/source/lib/src/prod_env_mat.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/prod_env_mat_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/lib/src/prod_env_mat_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/prod_force.cc` & `deepmd_kit-3.0.0a0/source/lib/src/prod_force.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/prod_force_grad.cc` & `deepmd_kit-3.0.0a0/source/lib/src/prod_force_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/prod_virial.cc` & `deepmd_kit-3.0.0a0/source/lib/src/prod_virial.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/prod_virial_grad.cc` & `deepmd_kit-3.0.0a0/source/lib/src/prod_virial_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/region.cc` & `deepmd_kit-3.0.0a0/source/lib/src/region.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/soft_min_switch.cc` & `deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/soft_min_switch_force.cc` & `deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch_force.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/soft_min_switch_force_grad.cc` & `deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch_force_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/soft_min_switch_virial.cc` & `deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch_virial.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/soft_min_switch_virial_grad.cc` & `deepmd_kit-3.0.0a0/source/lib/src/soft_min_switch_virial_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lib/src/tabulate.cc` & `deepmd_kit-3.0.0a0/source/lib/src/tabulate.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/lmp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/Install.sh` & `deepmd_kit-3.0.0a0/source/lmp/Install.sh`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/builtin.cmake` & `deepmd_kit-3.0.0a0/source/lmp/builtin.cmake`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/compute_deeptensor_atom.cpp` & `deepmd_kit-3.0.0a0/source/lmp/compute_deeptensor_atom.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/compute_deeptensor_atom.h` & `deepmd_kit-3.0.0a0/source/lmp/compute_deeptensor_atom.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/deepmd_version.h.in` & `deepmd_kit-3.0.0a0/source/lmp/deepmd_version.h.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/env.sh.in` & `deepmd_kit-3.0.0a0/source/lmp/env.sh.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/env_c.sh.in` & `deepmd_kit-3.0.0a0/source/lmp/env_c.sh.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/env_py.sh.in` & `deepmd_kit-3.0.0a0/source/lmp/env_py.sh.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/env_py_c.sh.in` & `deepmd_kit-3.0.0a0/source/lmp/env_py_c.sh.in`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/fix_dplr.cpp` & `deepmd_kit-3.0.0a0/source/lmp/fix_dplr.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -309,19 +309,14 @@
 
 void FixDPLR::setup(int vflag) {
   // if (strstr(update->integrate_style,"verlet"))
   post_force(vflag);
   // else {
   //   error->all(FLERR, "respa is not supported by this fix");
   // }
-  if (vflag) {
-    v_setup(vflag);
-  } else {
-    evflag = 0;
-  }
 }
 
 /* ---------------------------------------------------------------------- */
 
 void FixDPLR::min_setup(int vflag) { setup(vflag); }
 
 /* ---------------------------------------------------------------------- */
@@ -523,14 +518,15 @@
     int idx0 = valid_pairs[ii].first;
     int idx1 = valid_pairs[ii].second;
     assert(idx0 < sel_fwd.size());  // && sel_fwd[idx0] < sort_fwd_map.size());
     // Yixiao: the sort map is no longer needed
     // int res_idx = sort_fwd_map[sel_fwd[idx0]];
     int res_idx = sel_fwd[idx0];
     // int ret_idx = dpl_bwd[res_idx];
+    atom->image[idx1] = atom->image[idx0];
     for (int dd = 0; dd < 3; ++dd) {
       x[idx1][dd] =
           x[idx0][dd] + tensor[res_idx * 3 + dd] * dist_unit_cvt_factor;
       // res_buff[idx1 * odim + dd] = tensor[res_idx * odim + dd];
       dipole_recd[idx0 * 3 + dd] =
           tensor[res_idx * 3 + dd] * dist_unit_cvt_factor;
     }
```

### Comparing `deepmd_kit-2.2.9/source/lmp/fix_dplr.h` & `deepmd_kit-3.0.0a0/source/lmp/fix_dplr.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/pair_deepmd.cpp` & `deepmd_kit-3.0.0a0/source/lmp/pair_deepmd.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/pair_deepmd.h` & `deepmd_kit-3.0.0a0/source/lmp/pair_deepmd.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/plugin/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/lmp/plugin/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/plugin/deepmdplugin.cpp` & `deepmd_kit-3.0.0a0/source/lmp/plugin/deepmdplugin.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/pppm_dplr.cpp` & `deepmd_kit-3.0.0a0/source/lmp/pppm_dplr.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/lmp/pppm_dplr.h` & `deepmd_kit-3.0.0a0/source/lmp/pppm_dplr.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/md/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/AdWeight.h` & `deepmd_kit-3.0.0a0/source/md/include/AdWeight.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/Convert.h` & `deepmd_kit-3.0.0a0/source/md/include/Convert.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/CosSwitch.h` & `deepmd_kit-3.0.0a0/source/md/include/CosSwitch.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/GroFileManager.h` & `deepmd_kit-3.0.0a0/source/md/include/GroFileManager.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/HarmonicAngle.h` & `deepmd_kit-3.0.0a0/source/md/include/HarmonicAngle.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/HarmonicBond.h` & `deepmd_kit-3.0.0a0/source/md/include/HarmonicBond.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/Integrator.h` & `deepmd_kit-3.0.0a0/source/md/include/Integrator.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/Interpolation.h` & `deepmd_kit-3.0.0a0/source/md/include/Interpolation.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/LJInter.h` & `deepmd_kit-3.0.0a0/source/md/include/LJInter.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/LJTab.h` & `deepmd_kit-3.0.0a0/source/md/include/LJTab.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/MaxShift.h` & `deepmd_kit-3.0.0a0/source/md/include/MaxShift.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/Poly.h` & `deepmd_kit-3.0.0a0/source/md/include/Poly.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/Statistics.h` & `deepmd_kit-3.0.0a0/source/md/include/Statistics.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/TF.h` & `deepmd_kit-3.0.0a0/source/md/include/TF.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/TableFileLoader.h` & `deepmd_kit-3.0.0a0/source/md/include/TableFileLoader.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/Tabulated.h` & `deepmd_kit-3.0.0a0/source/md/include/Tabulated.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/Trajectory.h` & `deepmd_kit-3.0.0a0/source/md/include/Trajectory.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/UnitManager.h` & `deepmd_kit-3.0.0a0/source/md/include/UnitManager.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/XyzFileManager.h` & `deepmd_kit-3.0.0a0/source/md/include/XyzFileManager.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/ZM.h` & `deepmd_kit-3.0.0a0/source/md/include/ZM.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/ZMFunctions.h` & `deepmd_kit-3.0.0a0/source/md/include/ZMFunctions.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/common.h` & `deepmd_kit-3.0.0a0/source/md/include/common.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/include/mymath.h` & `deepmd_kit-3.0.0a0/source/md/include/mymath.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/mdnn.cc` & `deepmd_kit-3.0.0a0/source/md/mdnn.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/AdWeight.cc` & `deepmd_kit-3.0.0a0/source/md/src/AdWeight.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/Convert.cc` & `deepmd_kit-3.0.0a0/source/md/src/Convert.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/Gaussian.cc` & `deepmd_kit-3.0.0a0/source/md/src/Gaussian.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/GroFileManager.cc` & `deepmd_kit-3.0.0a0/source/md/src/GroFileManager.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/HarmonicAngle.cc` & `deepmd_kit-3.0.0a0/source/md/src/HarmonicAngle.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/HarmonicBond.cc` & `deepmd_kit-3.0.0a0/source/md/src/HarmonicBond.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/Integrator.cc` & `deepmd_kit-3.0.0a0/source/md/src/Integrator.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/Interpolation.cpp` & `deepmd_kit-3.0.0a0/source/md/src/Interpolation.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/LJInter.cc` & `deepmd_kit-3.0.0a0/source/md/src/LJInter.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/LJTab.cc` & `deepmd_kit-3.0.0a0/source/md/src/LJTab.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/MaxShift.cc` & `deepmd_kit-3.0.0a0/source/md/src/MaxShift.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/Poly.cpp` & `deepmd_kit-3.0.0a0/source/md/src/Poly.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/RandomGenerator_MT19937.cc` & `deepmd_kit-3.0.0a0/source/md/src/RandomGenerator_MT19937.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/Statistics.cc` & `deepmd_kit-3.0.0a0/source/md/src/Statistics.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/StringSplit.cpp` & `deepmd_kit-3.0.0a0/source/md/src/StringSplit.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/TF.cc` & `deepmd_kit-3.0.0a0/source/md/src/TF.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/TableFileLoader.cpp` & `deepmd_kit-3.0.0a0/source/md/src/TableFileLoader.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/Tabulated.cc` & `deepmd_kit-3.0.0a0/source/md/src/Tabulated.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/Trajectory.cc` & `deepmd_kit-3.0.0a0/source/md/src/Trajectory.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/UnitManager.cc` & `deepmd_kit-3.0.0a0/source/md/src/UnitManager.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/XyzFileManager.cc` & `deepmd_kit-3.0.0a0/source/md/src/XyzFileManager.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/ZM.cc` & `deepmd_kit-3.0.0a0/source/md/src/ZM.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/md/src/ZMFunctions.cpp` & `deepmd_kit-3.0.0a0/source/md/src/ZMFunctions.cpp`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/nodejs/.gitignore` & `deepmd_kit-3.0.0a0/source/nodejs/.gitignore`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/nodejs/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/nodejs/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/nodejs/README.md` & `deepmd_kit-3.0.0a0/source/nodejs/README.md`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/nodejs/package.json` & `deepmd_kit-3.0.0a0/source/nodejs/package.json`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/nodejs/prepublish.py` & `deepmd_kit-3.0.0a0/source/nodejs/prepublish.py`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/nodejs/tests/test_deeppot.js` & `deepmd_kit-3.0.0a0/source/nodejs/tests/test_deeppot.js`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/nodejs/yarn.lock` & `deepmd_kit-3.0.0a0/source/nodejs/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -303,17 +303,17 @@
 
 inherits@2, inherits@^2.0.3:
   version "2.0.4"
   resolved "https://registry.yarnpkg.com/inherits/-/inherits-2.0.4.tgz#0fa2c64f932917c3433a0ded55363aae37416b7c"
   integrity sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==
 
 ip@^2.0.0:
-  version "2.0.0"
-  resolved "https://registry.yarnpkg.com/ip/-/ip-2.0.0.tgz#4cf4ab182fee2314c75ede1276f8c80b479936da"
-  integrity sha512-WKa+XuLG1A1R0UWhl2+1XQSi+fZWMsYKffMZTTYsiZaUD8k2yDAj5atimTUD2TZkyCkNEeYE5NhFZmupOGtjYQ==
+  version "2.0.1"
+  resolved "https://registry.yarnpkg.com/ip/-/ip-2.0.1.tgz#e8f3595d33a3ea66490204234b77636965307105"
+  integrity sha512-lJUL9imLTNi1ZfXT+DU6rBBdbiKGBuay9B6xGSPVjUeQwaH1RIGqef8RZkUtHioLmSNpPR5M4HVKJGm1j8FWVQ==
 
 is-fullwidth-code-point@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/is-fullwidth-code-point/-/is-fullwidth-code-point-3.0.0.tgz#f116f8064fe90b3f7844a38997c0b75051269f1d"
   integrity sha512-zymm5+u+sCsSWyD9qNaejV3DFvhCKclKdizYaJUuHA83RLjb7nSuGnddCHGv0hk+KY7BMAlsWeK4Ueg6EV6XQg==
 
 is-lambda@^1.0.1:
```

### Comparing `deepmd_kit-2.2.9/source/op/CMakeLists.txt` & `deepmd_kit-3.0.0a0/source/op/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/add_flt_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/add_flt_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/copy_flt_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/copy_flt_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/custom_op.cc` & `deepmd_kit-3.0.0a0/source/op/custom_op.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/custom_op.h` & `deepmd_kit-3.0.0a0/source/op/custom_op.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/descrpt.cc` & `deepmd_kit-3.0.0a0/source/op/descrpt.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/descrpt_se_a_ef.cc` & `deepmd_kit-3.0.0a0/source/op/descrpt_se_a_ef.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/descrpt_se_a_ef_para.cc` & `deepmd_kit-3.0.0a0/source/op/descrpt_se_a_ef_para.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/descrpt_se_a_ef_vert.cc` & `deepmd_kit-3.0.0a0/source/op/descrpt_se_a_ef_vert.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/descrpt_se_a_mask.cc` & `deepmd_kit-3.0.0a0/source/op/descrpt_se_a_mask.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/dotmul_flt_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/dotmul_flt_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/ewald_recp.cc` & `deepmd_kit-3.0.0a0/source/op/ewald_recp.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/flt_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/flt_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/gelu_multi_device.cc` & `deepmd_kit-3.0.0a0/source/op/gelu_multi_device.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/map_aparam.cc` & `deepmd_kit-3.0.0a0/source/op/map_aparam.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/map_flt_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/map_flt_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/matmul_fitnet_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/matmul_fitnet_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/matmul_flt2fix_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/matmul_flt2fix_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/matmul_flt_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/matmul_flt_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/mul_flt_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/mul_flt_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/neighbor_stat.cc` & `deepmd_kit-3.0.0a0/source/op/neighbor_stat.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/optimizer/parallel.cc` & `deepmd_kit-3.0.0a0/source/op/optimizer/parallel.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/optimizer/parallel.h` & `deepmd_kit-3.0.0a0/source/op/optimizer/parallel.h`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/pair_tab.cc` & `deepmd_kit-3.0.0a0/source/op/pair_tab.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/pairwise.cc` & `deepmd_kit-3.0.0a0/source/op/pairwise.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_env_mat_multi_device.cc` & `deepmd_kit-3.0.0a0/source/op/prod_env_mat_multi_device.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_env_mat_multi_device_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/prod_env_mat_multi_device_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_force.cc` & `deepmd_kit-3.0.0a0/source/op/prod_force.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_force_grad.cc` & `deepmd_kit-3.0.0a0/source/op/prod_force_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_force_grad_multi_device.cc` & `deepmd_kit-3.0.0a0/source/op/prod_force_grad_multi_device.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_force_multi_device.cc` & `deepmd_kit-3.0.0a0/source/op/prod_force_multi_device.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_force_se_a_grad.cc` & `deepmd_kit-3.0.0a0/source/op/prod_force_se_a_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_force_se_a_mask.cc` & `deepmd_kit-3.0.0a0/source/op/prod_force_se_a_mask.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_force_se_a_mask_grad.cc` & `deepmd_kit-3.0.0a0/source/op/prod_force_se_a_mask_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_force_se_r_grad.cc` & `deepmd_kit-3.0.0a0/source/op/prod_force_se_r_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_virial.cc` & `deepmd_kit-3.0.0a0/source/op/prod_virial.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_virial_grad.cc` & `deepmd_kit-3.0.0a0/source/op/prod_virial_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_virial_grad_multi_device.cc` & `deepmd_kit-3.0.0a0/source/op/prod_virial_grad_multi_device.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_virial_multi_device.cc` & `deepmd_kit-3.0.0a0/source/op/prod_virial_multi_device.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_virial_se_a_grad.cc` & `deepmd_kit-3.0.0a0/source/op/prod_virial_se_a_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/prod_virial_se_r_grad.cc` & `deepmd_kit-3.0.0a0/source/op/prod_virial_se_r_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/quantize_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/quantize_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/soft_min.cc` & `deepmd_kit-3.0.0a0/source/op/soft_min.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/soft_min_force.cc` & `deepmd_kit-3.0.0a0/source/op/soft_min_force.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/soft_min_force_grad.cc` & `deepmd_kit-3.0.0a0/source/op/soft_min_force_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/soft_min_virial.cc` & `deepmd_kit-3.0.0a0/source/op/soft_min_virial.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/soft_min_virial_grad.cc` & `deepmd_kit-3.0.0a0/source/op/soft_min_virial_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/tabulate_multi_device.cc` & `deepmd_kit-3.0.0a0/source/op/tabulate_multi_device.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/tanh4_flt_nvnmd.cc` & `deepmd_kit-3.0.0a0/source/op/tanh4_flt_nvnmd.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/op/unaggregated_grad.cc` & `deepmd_kit-3.0.0a0/source/op/unaggregated_grad.cc`

 * *Files identical despite different names*

### Comparing `deepmd_kit-2.2.9/source/swig/deepmd.i` & `deepmd_kit-3.0.0a0/source/swig/deepmd.i`

 * *Files identical despite different names*

