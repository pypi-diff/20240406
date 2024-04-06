# Comparing `tmp/hwi-3.0.0.tar.gz` & `tmp/hwi-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hwi-3.0.0.tar", max compression
+gzip compressed data, was "hwi-3.0.0rc1.tar", max compression
```

## Comparing `hwi-3.0.0.tar` & `hwi-3.0.0rc1.tar`

### file list

```diff
@@ -1,309 +1,309 @@
--rw-r--r--   0        0        0     1068 2021-03-12 18:18:18.568731 hwi-3.0.0/LICENSE
--rw-r--r--   0        0        0     3410 2024-01-17 18:53:31.437873 hwi-3.0.0/README.md
--rwxr-xr-x   0        0        0      175 2021-03-12 18:18:18.585398 hwi-3.0.0/hwi-qt.py
--rwxr-xr-x   0        0        0      210 2021-03-12 18:18:18.585398 hwi-3.0.0/hwi.py
--rw-r--r--   0        0        0       22 2024-04-06 16:56:36.330614 hwi-3.0.0/hwilib/__init__.py
--rw-r--r--   0        0        0     4442 2023-08-16 21:25:52.309774 hwi-3.0.0/hwilib/_base58.py
--rw-r--r--   0        0        0     5720 2021-12-20 17:20:33.201156 hwi-3.0.0/hwilib/_bech32.py
--rw-r--r--   0        0        0    16325 2024-04-01 21:00:33.209488 hwi-3.0.0/hwilib/_cli.py
--rw-r--r--   0        0        0    22665 2024-04-01 21:00:33.209488 hwi-3.0.0/hwilib/_gui.py
--rw-r--r--   0        0        0     4193 2022-03-15 13:41:28.603552 hwi-3.0.0/hwilib/_script.py
--rw-r--r--   0        0        0     6526 2021-03-12 18:18:18.585398 hwi-3.0.0/hwilib/_serialize.py
--rw-r--r--   0        0        0    23930 2024-04-01 21:00:33.209488 hwi-3.0.0/hwilib/commands.py
--rw-r--r--   0        0        0     2242 2023-07-22 03:20:43.415813 hwi-3.0.0/hwilib/common.py
--rw-r--r--   0        0        0    22613 2023-11-14 21:48:56.313976 hwi-3.0.0/hwilib/descriptor.py
--rw-r--r--   0        0        0      121 2021-11-24 18:14:09.145516 hwi-3.0.0/hwilib/devices/__init__.py
--rw-r--r--   0        0        0      257 2024-01-19 21:50:50.608490 hwi-3.0.0/hwilib/devices/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      210 2024-01-18 19:00:59.113475 hwi-3.0.0/hwilib/devices/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    43235 2024-01-19 21:50:51.325214 hwi-3.0.0/hwilib/devices/__pycache__/bitbox02.cpython-311.pyc
--rw-r--r--   0        0        0    22561 2024-01-19 21:50:51.025190 hwi-3.0.0/hwilib/devices/__pycache__/coldcard.cpython-311.pyc
--rw-r--r--   0        0        0    38977 2024-01-19 21:50:51.015189 hwi-3.0.0/hwilib/devices/__pycache__/digitalbitbox.cpython-311.pyc
--rw-r--r--   0        0        0    29159 2024-01-19 21:50:51.708578 hwi-3.0.0/hwilib/devices/__pycache__/jade.cpython-311.pyc
--rw-r--r--   0        0        0    12728 2024-01-19 21:50:50.875178 hwi-3.0.0/hwilib/devices/__pycache__/keepkey.cpython-311.pyc
--rw-r--r--   0        0        0    30444 2024-01-19 21:50:50.855176 hwi-3.0.0/hwilib/devices/__pycache__/ledger.cpython-311.pyc
--rw-r--r--   0        0        0    46188 2024-01-19 21:50:50.635159 hwi-3.0.0/hwilib/devices/__pycache__/trezor.cpython-311.pyc
--rw-r--r--   0        0        0    34980 2024-04-01 21:00:33.209488 hwi-3.0.0/hwilib/devices/bitbox02.py
--rw-r--r--   0        0        0    11432 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/LICENSE
--rw-r--r--   0        0        0      613 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/README.md
--rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/__init__.py
--rw-r--r--   0        0        0      177 2024-01-19 21:50:51.325214 hwi-3.0.0/hwilib/devices/bitbox02_lib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      141 2024-01-18 19:01:04.037196 hwi-3.0.0/hwilib/devices/bitbox02_lib/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    14641 2024-01-19 21:50:51.328548 hwi-3.0.0/hwilib/devices/bitbox02_lib/__pycache__/util.cpython-311.pyc
--rw-r--r--   0        0        0     1642 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__init__.py
--rw-r--r--   0        0        0     1829 2024-01-19 21:50:51.408554 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1157 2024-01-18 19:01:04.237212 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    53197 2024-01-19 21:50:51.411888 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-311.pyc
--rw-r--r--   0        0        0    28620 2024-01-18 19:01:04.243879 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-39.pyc
--rw-r--r--   0        0        0    10987 2024-01-19 21:50:51.448557 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-311.pyc
--rw-r--r--   0        0        0     6612 2024-01-18 19:01:04.247213 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-39.pyc
--rw-r--r--   0        0        0     3118 2024-01-19 21:50:51.445224 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-311.pyc
--rw-r--r--   0        0        0     1931 2024-01-18 19:01:04.243879 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-39.pyc
--rw-r--r--   0        0        0    43441 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/bitbox02.py
--rw-r--r--   0        0        0     7359 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/bootloader.py
--rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/py.typed
--rw-r--r--   0        0        0     2371 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/secp256k1.py
--rw-r--r--   0        0        0     1030 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__init__.py
--rw-r--r--   0        0        0      870 2024-01-19 21:50:51.418555 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      675 2024-01-18 19:01:04.037196 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    39476 2024-01-19 21:50:51.421888 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-311.pyc
--rw-r--r--   0        0        0    24433 2024-01-18 19:01:04.053864 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-39.pyc
--rw-r--r--   0        0        0     2625 2024-01-19 21:50:51.418555 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-311.pyc
--rw-r--r--   0        0        0     2063 2024-01-18 19:01:04.040530 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-39.pyc
--rw-r--r--   0        0        0     7499 2024-01-19 21:50:51.425222 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-311.pyc
--rw-r--r--   0        0        0     4741 2024-01-18 19:01:04.167206 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-39.pyc
--rw-r--r--   0        0        0    27806 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/bitbox_api_protocol.py
--rw-r--r--   0        0        0     1669 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/communication.py
--rw-r--r--   0        0        0     4666 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/devices.py
--rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__init__.py
--rw-r--r--   0        0        0      201 2024-01-19 21:50:51.425222 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      165 2024-01-18 19:01:04.170540 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1622 2024-01-19 21:50:51.441890 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1119 2024-01-18 19:01:04.223877 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     2132 2024-01-19 21:50:51.441890 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1511 2024-01-18 19:01:04.220544 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     2577 2024-01-19 21:50:51.441890 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1866 2024-01-18 19:01:04.220544 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     7901 2024-01-19 21:50:51.441890 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     6623 2024-01-18 19:01:04.223877 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     5318 2024-01-19 21:50:51.445224 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     4351 2024-01-18 19:01:04.227211 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     1794 2024-01-19 21:50:51.438556 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1238 2024-01-18 19:01:04.210543 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     5216 2024-01-19 21:50:51.445224 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     4298 2024-01-18 19:01:04.227211 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     5007 2024-01-19 21:50:51.425222 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     4320 2024-01-18 19:01:04.170540 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     1474 2024-01-19 21:50:51.445224 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1002 2024-01-18 19:01:04.227211 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     1614 2024-01-19 21:50:51.445224 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1112 2024-01-18 19:01:04.230544 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     1616 2024-01-19 21:50:51.445224 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-311.pyc
--rw-r--r--   0        0        0     1143 2024-01-18 19:01:04.230544 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     1460 2024-01-19 21:50:51.445224 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-311.pyc
--rw-r--r--   0        0        0      990 2024-01-18 19:01:04.230544 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-39.pyc
--rw-r--r--   0        0        0     1401 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.py
--rw-r--r--   0        0        0     1638 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.pyi
--rw-r--r--   0        0        0     2102 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.py
--rw-r--r--   0        0        0     3851 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.pyi
--rw-r--r--   0        0        0     2699 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.py
--rw-r--r--   0        0        0     5248 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.pyi
--rw-r--r--   0        0        0    10516 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.py
--rw-r--r--   0        0        0    33375 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.pyi
--rw-r--r--   0        0        0     6703 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.py
--rw-r--r--   0        0        0    18628 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.pyi
--rw-r--r--   0        0        0     1664 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.py
--rw-r--r--   0        0        0     3152 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.pyi
--rw-r--r--   0        0        0     6698 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.py
--rw-r--r--   0        0        0    19589 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.pyi
--rw-r--r--   0        0        0     5757 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.py
--rw-r--r--   0        0        0    13514 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.pyi
--rw-r--r--   0        0        0     1205 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.py
--rw-r--r--   0        0        0     1308 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.pyi
--rw-r--r--   0        0        0     1386 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.py
--rw-r--r--   0        0        0     1541 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.pyi
--rw-r--r--   0        0        0     1444 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.py
--rw-r--r--   0        0        0     1990 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.pyi
--rw-r--r--   0        0        0     1186 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.py
--rw-r--r--   0        0        0     1394 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.pyi
--rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/py.typed
--rw-r--r--   0        0        0      709 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__init__.py
--rw-r--r--   0        0        0      432 2024-01-19 21:50:51.448557 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      346 2024-01-18 19:01:04.233878 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7264 2024-01-19 21:50:51.448557 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-311.pyc
--rw-r--r--   0        0        0     4443 2024-01-18 19:01:04.237212 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-39.pyc
--rw-r--r--   0        0        0     5793 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/u2fhid.py
--rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/py.typed
--rw-r--r--   0        0        0     8035 2023-07-18 15:44:04.532963 hwi-3.0.0/hwilib/devices/bitbox02_lib/util.py
--rw-r--r--   0        0        0      384 2021-03-12 18:18:18.588731 hwi-3.0.0/hwilib/devices/ckcc/README.md
--rw-r--r--   0        0        0       74 2021-03-12 18:18:18.588731 hwi-3.0.0/hwilib/devices/ckcc/__init__.py
--rw-r--r--   0        0        0      248 2024-01-19 21:50:51.025190 hwi-3.0.0/hwilib/devices/ckcc/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      204 2024-01-18 19:01:04.247213 hwi-3.0.0/hwilib/devices/ckcc/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    16309 2024-01-19 21:50:51.025190 hwi-3.0.0/hwilib/devices/ckcc/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     2625 2024-01-19 21:50:51.028524 hwi-3.0.0/hwilib/devices/ckcc/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0    15194 2024-01-19 21:50:51.028524 hwi-3.0.0/hwilib/devices/ckcc/__pycache__/protocol.cpython-311.pyc
--rw-r--r--   0        0        0     4456 2024-01-19 21:50:51.028524 hwi-3.0.0/hwilib/devices/ckcc/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0    13206 2023-07-22 03:20:43.419147 hwi-3.0.0/hwilib/devices/ckcc/client.py
--rw-r--r--   0        0        0     2997 2021-03-12 18:18:18.588731 hwi-3.0.0/hwilib/devices/ckcc/constants.py
--rw-r--r--   0        0        0     9877 2021-03-12 18:18:18.588731 hwi-3.0.0/hwilib/devices/ckcc/protocol.py
--rw-r--r--   0        0        0     1807 2021-03-12 18:18:18.588731 hwi-3.0.0/hwilib/devices/ckcc/sigheader.py
--rw-r--r--   0        0        0     3470 2021-03-12 18:18:18.588731 hwi-3.0.0/hwilib/devices/ckcc/utils.py
--rw-r--r--   0        0        0    14585 2024-04-01 21:00:33.212822 hwi-3.0.0/hwilib/devices/coldcard.py
--rw-r--r--   0        0        0    27404 2024-04-01 21:00:33.212822 hwi-3.0.0/hwilib/devices/digitalbitbox.py
--rw-r--r--   0        0        0    25827 2024-04-01 21:00:33.212822 hwi-3.0.0/hwilib/devices/jade.py
--rw-r--r--   0        0        0      320 2022-10-28 21:25:37.086384 hwi-3.0.0/hwilib/devices/jadepy/README.md
--rw-r--r--   0        0        0       83 2022-10-28 21:25:37.086384 hwi-3.0.0/hwilib/devices/jadepy/__init__.py
--rw-r--r--   0        0        0      308 2024-01-19 21:50:51.708578 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      241 2024-01-18 19:01:04.003860 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    83592 2024-01-19 21:50:51.711912 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade.cpython-311.pyc
--rw-r--r--   0        0        0    67602 2024-01-18 19:01:04.010527 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade.cpython-39.pyc
--rw-r--r--   0        0        0     1422 2024-01-19 21:50:51.718579 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_error.cpython-311.pyc
--rw-r--r--   0        0        0     1037 2024-01-18 19:01:04.010527 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_error.cpython-39.pyc
--rw-r--r--   0        0        0     3617 2024-01-19 21:50:51.721912 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-311.pyc
--rw-r--r--   0        0        0     2051 2024-01-18 19:01:04.010527 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-39.pyc
--rw-r--r--   0        0        0     3412 2024-01-19 21:50:51.728580 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2024-01-30 19:06:23.837885 hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-39.pyc
--rw-r--r--   0        0        0    75800 2023-11-14 21:41:54.054474 hwi-3.0.0/hwilib/devices/jadepy/jade.py
--rw-r--r--   0        0        0      655 2021-11-24 18:14:09.145516 hwi-3.0.0/hwilib/devices/jadepy/jade_error.py
--rw-r--r--   0        0        0     2348 2023-11-14 21:41:54.054474 hwi-3.0.0/hwilib/devices/jadepy/jade_serial.py
--rw-r--r--   0        0        0     1797 2023-11-14 21:41:54.054474 hwi-3.0.0/hwilib/devices/jadepy/jade_tcp.py
--rw-r--r--   0        0        0     9391 2024-04-01 21:00:33.212822 hwi-3.0.0/hwilib/devices/keepkey.py
--rw-r--r--   0        0        0    23345 2024-04-01 21:00:33.212822 hwi-3.0.0/hwilib/devices/ledger.py
--rw-r--r--   0        0        0     1265 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/README.md
--rw-r--r--   0        0        0      327 2022-11-15 21:45:17.006790 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__init__.py
--rw-r--r--   0        0        0      615 2024-01-19 21:50:50.855176 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      488 2024-01-18 19:01:04.290549 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    17244 2024-01-19 21:50:50.865177 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0     9524 2024-01-18 19:01:04.330552 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-39.pyc
--rw-r--r--   0        0        0    12612 2024-01-19 21:50:50.855176 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-311.pyc
--rw-r--r--   0        0        0     9527 2024-01-18 19:01:04.290549 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-39.pyc
--rw-r--r--   0        0        0    21273 2024-01-19 21:50:50.865177 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-311.pyc
--rw-r--r--   0        0        0    13479 2024-01-18 19:01:04.330552 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-39.pyc
--rw-r--r--   0        0        0    17593 2024-01-19 21:50:50.868511 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-311.pyc
--rw-r--r--   0        0        0     8700 2024-01-18 19:01:04.333886 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-39.pyc
--rw-r--r--   0        0        0    10966 2024-01-19 21:50:50.858510 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-311.pyc
--rw-r--r--   0        0        0     6728 2024-01-18 19:01:04.303884 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-39.pyc
--rw-r--r--   0        0        0    13766 2024-01-19 21:50:50.861843 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-311.pyc
--rw-r--r--   0        0        0     8873 2024-01-18 19:01:04.307217 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-39.pyc
--rw-r--r--   0        0        0     8620 2024-01-19 21:50:50.861843 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-311.pyc
--rw-r--r--   0        0        0     5021 2024-01-18 19:01:04.307217 hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-39.pyc
--rw-r--r--   0        0        0      488 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/README.md
--rw-r--r--   0        0        0      855 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__init__.py
--rw-r--r--   0        0        0     1061 2024-01-19 21:50:50.868511 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1016 2024-01-18 19:01:04.333886 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9117 2024-01-19 21:50:50.871844 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-311.pyc
--rw-r--r--   0        0        0     5025 2024-01-18 19:01:04.340553 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-39.pyc
--rw-r--r--   0        0        0     3158 2024-01-19 21:50:50.871844 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-311.pyc
--rw-r--r--   0        0        0     2061 2024-01-18 19:01:04.340553 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-39.pyc
--rw-r--r--   0        0        0    25379 2024-01-19 21:50:50.871844 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-311.pyc
--rw-r--r--   0        0        0    12165 2024-01-18 19:01:04.337220 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-39.pyc
--rw-r--r--   0        0        0     1707 2024-01-19 21:50:50.871844 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-311.pyc
--rw-r--r--   0        0        0     1501 2024-01-18 19:01:04.340553 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-39.pyc
--rw-r--r--   0        0        0     5339 2024-01-19 21:50:50.871844 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-311.pyc
--rw-r--r--   0        0        0     2910 2024-01-18 19:01:04.343887 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-39.pyc
--rw-r--r--   0        0        0     6230 2024-01-19 21:50:50.871844 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-311.pyc
--rw-r--r--   0        0        0     3432 2024-01-18 19:01:04.347220 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-39.pyc
--rw-r--r--   0        0        0     4874 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/bitcoinTransaction.py
--rw-r--r--   0        0        0     2025 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/bitcoinVarint.py
--rw-r--r--   0        0        0    16449 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/btchip.py
--rw-r--r--   0        0        0     1020 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/btchipException.py
--rw-r--r--   0        0        0     2715 2023-08-16 21:27:10.379182 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/btchipHelpers.py
--rw-r--r--   0        0        0     3416 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/btchipUtils.py
--rw-r--r--   0        0        0     3224 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/ledgerWrapper.py
--rw-r--r--   0        0        0    11666 2022-11-15 21:45:17.006790 hwi-3.0.0/hwilib/devices/ledger_bitcoin/client.py
--rw-r--r--   0        0        0     8168 2022-11-15 21:45:17.006790 hwi-3.0.0/hwilib/devices/ledger_bitcoin/client_base.py
--rw-r--r--   0        0        0    12284 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/client_command.py
--rw-r--r--   0        0        0    13915 2022-11-15 21:45:17.006790 hwi-3.0.0/hwilib/devices/ledger_bitcoin/client_legacy.py
--rw-r--r--   0        0        0     6437 2022-11-15 21:45:17.006790 hwi-3.0.0/hwilib/devices/ledger_bitcoin/command_builder.py
--rw-r--r--   0        0        0     8188 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/errors.py
--rw-r--r--   0        0        0      806 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__init__.py
--rw-r--r--   0        0        0      813 2024-01-19 21:50:50.861843 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      622 2024-01-18 19:01:04.310551 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1837 2024-01-19 21:50:50.861843 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-311.pyc
--rw-r--r--   0        0        0     1286 2024-01-18 19:01:04.310551 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-39.pyc
--rw-r--r--   0        0        0     2682 2024-01-19 21:50:50.861843 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     1940 2024-01-18 19:01:04.313884 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0     1251 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/device_exception.py
--rw-r--r--   0        0        0      652 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/errors.py
--rw-r--r--   0        0        0      576 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/README.md
--rw-r--r--   0        0        0      107 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__init__.py
--rw-r--r--   0        0        0      340 2024-01-19 21:50:50.855176 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      280 2024-01-18 19:01:04.290549 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      413 2024-01-19 21:50:50.858510 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/log.cpython-311.pyc
--rw-r--r--   0        0        0      273 2024-01-18 19:01:04.297217 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/log.cpython-39.pyc
--rw-r--r--   0        0        0     9497 2024-01-19 21:50:50.855176 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-311.pyc
--rw-r--r--   0        0        0     6952 2024-01-18 19:01:04.293883 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-39.pyc
--rw-r--r--   0        0        0       36 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__init__.py
--rw-r--r--   0        0        0      244 2024-01-19 21:50:50.858510 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      206 2024-01-18 19:01:04.293883 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1868 2024-01-19 21:50:50.858510 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-311.pyc
--rw-r--r--   0        0        0     1430 2024-01-18 19:01:04.297217 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-39.pyc
--rw-r--r--   0        0        0     7896 2024-01-19 21:50:50.858510 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-311.pyc
--rw-r--r--   0        0        0     4826 2024-01-18 19:01:04.300550 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-39.pyc
--rw-r--r--   0        0        0     5057 2024-01-19 21:50:50.858510 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-311.pyc
--rw-r--r--   0        0        0     3483 2024-01-18 19:01:04.297217 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-39.pyc
--rw-r--r--   0        0        0      922 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/comm.py
--rw-r--r--   0        0        0     5086 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/hid_device.py
--rw-r--r--   0        0        0     2997 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/tcp_client.py
--rw-r--r--   0        0        0       98 2023-08-16 21:28:50.470303 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/log.py
--rw-r--r--   0        0        0     7019 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/transport.py
--rw-r--r--   0        0        0     8430 2022-02-28 10:20:27.103458 hwi-3.0.0/hwilib/devices/ledger_bitcoin/merkle.py
--rw-r--r--   0        0        0     4547 2022-11-15 21:45:17.006790 hwi-3.0.0/hwilib/devices/ledger_bitcoin/wallet.py
--rw-r--r--   0        0        0    36930 2024-04-01 21:00:33.212822 hwi-3.0.0/hwilib/devices/trezor.py
--rw-r--r--   0        0        0      628 2021-12-22 17:36:23.909185 hwi-3.0.0/hwilib/devices/trezorlib/README.md
--rw-r--r--   0        0        0      704 2021-12-22 17:36:23.909185 hwi-3.0.0/hwilib/devices/trezorlib/__init__.py
--rw-r--r--   0        0        0      197 2024-01-19 21:50:50.635159 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      160 2024-01-18 19:01:04.277215 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    17113 2024-01-19 21:50:50.688496 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/btc.cpython-311.pyc
--rw-r--r--   0        0        0    24116 2024-01-19 21:50:50.638492 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/client.cpython-311.pyc
--rw-r--r--   0        0        0    41480 2024-01-19 21:50:50.661827 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-311.pyc
--rw-r--r--   0        0        0     9639 2024-01-19 21:50:50.691830 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/device.cpython-311.pyc
--rw-r--r--   0        0        0     2651 2024-01-19 21:50:50.641826 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     1688 2024-01-18 19:01:04.280548 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-39.pyc
--rw-r--r--   0        0        0     3505 2024-01-19 21:50:50.658494 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/log.cpython-311.pyc
--rw-r--r--   0        0        0     4282 2024-01-19 21:50:50.641826 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/mapping.cpython-311.pyc
--rw-r--r--   0        0        0    94387 2024-01-19 21:50:50.648493 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/messages.cpython-311.pyc
--rw-r--r--   0        0        0     2474 2024-01-19 21:50:50.655160 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    30470 2024-01-19 21:50:50.651827 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-311.pyc
--rw-r--r--   0        0        0    15554 2024-01-19 21:50:50.658494 hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/tools.cpython-311.pyc
--rw-r--r--   0        0        0    13203 2021-12-22 17:36:23.909185 hwi-3.0.0/hwilib/devices/trezorlib/btc.py
--rw-r--r--   0        0        0    18854 2021-12-22 17:36:23.909185 hwi-3.0.0/hwilib/devices/trezorlib/client.py
--rw-r--r--   0        0        0    25872 2021-12-22 17:36:23.909185 hwi-3.0.0/hwilib/devices/trezorlib/debuglink.py
--rw-r--r--   0        0        0     7081 2021-12-22 17:36:23.909185 hwi-3.0.0/hwilib/devices/trezorlib/device.py
--rw-r--r--   0        0        0     1601 2021-12-22 17:36:23.909185 hwi-3.0.0/hwilib/devices/trezorlib/exceptions.py
--rw-r--r--   0        0        0    16038 2021-12-22 17:36:23.912518 hwi-3.0.0/hwilib/devices/trezorlib/firmware.py
--rw-r--r--   0        0        0     2275 2023-08-16 21:28:50.470303 hwi-3.0.0/hwilib/devices/trezorlib/log.py
--rw-r--r--   0        0        0     3499 2021-12-22 17:36:23.912518 hwi-3.0.0/hwilib/devices/trezorlib/mapping.py
--rw-r--r--   0        0        0    72766 2022-11-10 16:51:27.184728 hwi-3.0.0/hwilib/devices/trezorlib/messages.py
--rw-r--r--   0        0        0     2534 2024-01-17 18:52:53.554894 hwi-3.0.0/hwilib/devices/trezorlib/models.py
--rw-r--r--   0        0        0    20415 2021-12-22 17:36:23.912518 hwi-3.0.0/hwilib/devices/trezorlib/protobuf.py
--rw-r--r--   0        0        0    10087 2021-12-22 17:36:23.912518 hwi-3.0.0/hwilib/devices/trezorlib/tools.py
--rw-r--r--   0        0        0     4913 2021-11-19 17:56:12.722101 hwi-3.0.0/hwilib/devices/trezorlib/transport/__init__.py
--rw-r--r--   0        0        0     7845 2024-01-19 21:50:50.661827 hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4979 2024-01-18 19:01:04.280548 hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     8592 2024-01-19 21:50:50.665161 hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-311.pyc
--rw-r--r--   0        0        0     8878 2024-01-19 21:50:50.665161 hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-311.pyc
--rw-r--r--   0        0        0     8134 2024-01-19 21:50:50.671828 hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-311.pyc
--rw-r--r--   0        0        0     8656 2024-01-19 21:50:50.675162 hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-311.pyc
--rw-r--r--   0        0        0     5374 2021-11-19 17:56:12.722101 hwi-3.0.0/hwilib/devices/trezorlib/transport/hid.py
--rw-r--r--   0        0        0     5372 2021-03-12 18:18:18.592065 hwi-3.0.0/hwilib/devices/trezorlib/transport/protocol.py
--rw-r--r--   0        0        0     4881 2021-11-19 17:56:12.722101 hwi-3.0.0/hwilib/devices/trezorlib/transport/udp.py
--rw-r--r--   0        0        0     5315 2021-11-19 17:56:12.722101 hwi-3.0.0/hwilib/devices/trezorlib/transport/webusb.py
--rw-r--r--   0        0        0     7048 2021-03-12 18:18:18.592065 hwi-3.0.0/hwilib/errors.py
--rw-r--r--   0        0        0     9167 2022-12-08 02:29:17.216573 hwi-3.0.0/hwilib/hwwclient.py
--rw-r--r--   0        0        0    14015 2022-05-23 15:49:56.363380 hwi-3.0.0/hwilib/key.py
--rw-r--r--   0        0        0    46452 2022-02-09 23:43:14.298584 hwi-3.0.0/hwilib/psbt.py
--rw-r--r--   0        0        0        0 2021-03-12 18:18:18.592065 hwi-3.0.0/hwilib/py.typed
--rw-r--r--   0        0        0     9191 2022-06-15 16:50:33.542133 hwi-3.0.0/hwilib/tx.py
--rw-r--r--   0        0        0     1756 2022-05-18 21:55:00.930698 hwi-3.0.0/hwilib/udev/20-hw1.rules
--rw-r--r--   0        0        0      310 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/udev/51-coinkite.rules
--rw-r--r--   0        0        0      119 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/udev/51-hid-digitalbitbox.rules
--rw-r--r--   0        0        0      980 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/udev/51-trezor.rules
--rw-r--r--   0        0        0      769 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/udev/51-usb-keepkey.rules
--rw-r--r--   0        0        0      142 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/udev/52-hid-digitalbitbox.rules
--rw-r--r--   0        0        0      125 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/udev/53-hid-bitbox02.rules
--rw-r--r--   0        0        0      147 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/udev/54-hid-bitbox02.rules
--rw-r--r--   0        0        0      340 2022-02-01 17:28:57.968878 hwi-3.0.0/hwilib/udev/55-usb-jade.rules
--rw-r--r--   0        0        0     1158 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/udev/README.md
--rw-r--r--   0        0        0     3416 2021-05-27 16:48:25.993035 hwi-3.0.0/hwilib/udevinstaller.py
--rw-r--r--   0        0        0     2687 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/ui/bitbox02pairing.ui
--rw-r--r--   0        0        0     5380 2023-07-26 16:14:31.195563 hwi-3.0.0/hwilib/ui/displayaddressdialog.ui
--rw-r--r--   0        0        0     6167 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/ui/getkeypooloptionsdialog.ui
--rw-r--r--   0        0        0     2872 2022-11-17 18:05:36.906293 hwi-3.0.0/hwilib/ui/getxpubdialog.ui
--rw-r--r--   0        0        0      196 2021-03-12 18:18:18.595398 hwi-3.0.0/hwilib/ui/hwiqt.pyproject
--rw-r--r--   0        0        0     7628 2022-11-17 18:05:36.906293 hwi-3.0.0/hwilib/ui/mainwindow.ui
--rw-r--r--   0        0        0     4431 2022-11-17 18:05:36.906293 hwi-3.0.0/hwilib/ui/sendpindialog.ui
--rw-r--r--   0        0        0     2117 2022-11-17 18:05:36.906293 hwi-3.0.0/hwilib/ui/setpassphrasedialog.ui
--rw-r--r--   0        0        0     4378 2022-11-17 18:05:36.906293 hwi-3.0.0/hwilib/ui/signmessagedialog.ui
--rw-r--r--   0        0        0     6092 2023-07-22 03:30:06.522930 hwi-3.0.0/hwilib/ui/signpsbtdialog.ui
--rw-r--r--   0        0        0     2545 2024-04-06 16:58:56.488025 hwi-3.0.0/hwilib/ui/ui_bitbox02pairing.py
--rw-r--r--   0        0        0     5425 2024-04-06 16:58:56.541363 hwi-3.0.0/hwilib/ui/ui_displayaddressdialog.py
--rw-r--r--   0        0        0     5724 2024-04-06 16:58:56.591366 hwi-3.0.0/hwilib/ui/ui_getkeypooloptionsdialog.py
--rw-r--r--   0        0        0     3151 2024-04-06 16:58:56.641370 hwi-3.0.0/hwilib/ui/ui_getxpubdialog.py
--rw-r--r--   0        0        0     8994 2024-04-06 16:58:56.691374 hwi-3.0.0/hwilib/ui/ui_mainwindow.py
--rw-r--r--   0        0        0     4729 2024-04-06 16:58:56.744711 hwi-3.0.0/hwilib/ui/ui_sendpindialog.py
--rw-r--r--   0        0        0     2057 2024-04-06 16:58:56.794715 hwi-3.0.0/hwilib/ui/ui_setpassphrasedialog.py
--rw-r--r--   0        0        0     4017 2024-04-06 16:58:56.844719 hwi-3.0.0/hwilib/ui/ui_signmessagedialog.py
--rw-r--r--   0        0        0     5419 2024-04-06 16:58:56.894723 hwi-3.0.0/hwilib/ui/ui_signpsbtdialog.py
--rw-r--r--   0        0        0     1277 2024-04-06 16:56:44.374568 hwi-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     5409 1970-01-01 00:00:00.000000 hwi-3.0.0/setup.py
--rw-r--r--   0        0        0     4722 1970-01-01 00:00:00.000000 hwi-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2021-03-12 18:18:18.568731 hwi-3.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3410 2024-01-17 18:53:31.437873 hwi-3.0.0rc1/README.md
+-rwxr-xr-x   0        0        0      175 2021-03-12 18:18:18.585398 hwi-3.0.0rc1/hwi-qt.py
+-rwxr-xr-x   0        0        0      210 2021-03-12 18:18:18.585398 hwi-3.0.0rc1/hwi.py
+-rw-r--r--   0        0        0       27 2024-04-01 21:01:04.688649 hwi-3.0.0rc1/hwilib/__init__.py
+-rw-r--r--   0        0        0     4442 2023-08-16 21:25:52.309774 hwi-3.0.0rc1/hwilib/_base58.py
+-rw-r--r--   0        0        0     5720 2021-12-20 17:20:33.201156 hwi-3.0.0rc1/hwilib/_bech32.py
+-rw-r--r--   0        0        0    16325 2024-04-01 21:00:33.209488 hwi-3.0.0rc1/hwilib/_cli.py
+-rw-r--r--   0        0        0    22665 2024-04-01 21:00:33.209488 hwi-3.0.0rc1/hwilib/_gui.py
+-rw-r--r--   0        0        0     4193 2022-03-15 13:41:28.603552 hwi-3.0.0rc1/hwilib/_script.py
+-rw-r--r--   0        0        0     6526 2021-03-12 18:18:18.585398 hwi-3.0.0rc1/hwilib/_serialize.py
+-rw-r--r--   0        0        0    23930 2024-04-01 21:00:33.209488 hwi-3.0.0rc1/hwilib/commands.py
+-rw-r--r--   0        0        0     2242 2023-07-22 03:20:43.415813 hwi-3.0.0rc1/hwilib/common.py
+-rw-r--r--   0        0        0    22613 2023-11-14 21:48:56.313976 hwi-3.0.0rc1/hwilib/descriptor.py
+-rw-r--r--   0        0        0      121 2021-11-24 18:14:09.145516 hwi-3.0.0rc1/hwilib/devices/__init__.py
+-rw-r--r--   0        0        0      257 2024-01-19 21:50:50.608490 hwi-3.0.0rc1/hwilib/devices/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      210 2024-01-18 19:00:59.113475 hwi-3.0.0rc1/hwilib/devices/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    43235 2024-01-19 21:50:51.325214 hwi-3.0.0rc1/hwilib/devices/__pycache__/bitbox02.cpython-311.pyc
+-rw-r--r--   0        0        0    22561 2024-01-19 21:50:51.025190 hwi-3.0.0rc1/hwilib/devices/__pycache__/coldcard.cpython-311.pyc
+-rw-r--r--   0        0        0    38977 2024-01-19 21:50:51.015189 hwi-3.0.0rc1/hwilib/devices/__pycache__/digitalbitbox.cpython-311.pyc
+-rw-r--r--   0        0        0    29159 2024-01-19 21:50:51.708578 hwi-3.0.0rc1/hwilib/devices/__pycache__/jade.cpython-311.pyc
+-rw-r--r--   0        0        0    12728 2024-01-19 21:50:50.875178 hwi-3.0.0rc1/hwilib/devices/__pycache__/keepkey.cpython-311.pyc
+-rw-r--r--   0        0        0    30444 2024-01-19 21:50:50.855176 hwi-3.0.0rc1/hwilib/devices/__pycache__/ledger.cpython-311.pyc
+-rw-r--r--   0        0        0    46188 2024-01-19 21:50:50.635159 hwi-3.0.0rc1/hwilib/devices/__pycache__/trezor.cpython-311.pyc
+-rw-r--r--   0        0        0    34980 2024-04-01 21:00:33.209488 hwi-3.0.0rc1/hwilib/devices/bitbox02.py
+-rw-r--r--   0        0        0    11432 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/LICENSE
+-rw-r--r--   0        0        0      613 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/__init__.py
+-rw-r--r--   0        0        0      177 2024-01-19 21:50:51.325214 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      141 2024-01-18 19:01:04.037196 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    14641 2024-01-19 21:50:51.328548 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0     1642 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__init__.py
+-rw-r--r--   0        0        0     1829 2024-01-19 21:50:51.408554 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1157 2024-01-18 19:01:04.237212 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    53197 2024-01-19 21:50:51.411888 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-311.pyc
+-rw-r--r--   0        0        0    28620 2024-01-18 19:01:04.243879 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-39.pyc
+-rw-r--r--   0        0        0    10987 2024-01-19 21:50:51.448557 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-311.pyc
+-rw-r--r--   0        0        0     6612 2024-01-18 19:01:04.247213 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-39.pyc
+-rw-r--r--   0        0        0     3118 2024-01-19 21:50:51.445224 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-311.pyc
+-rw-r--r--   0        0        0     1931 2024-01-18 19:01:04.243879 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-39.pyc
+-rw-r--r--   0        0        0    43441 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/bitbox02.py
+-rw-r--r--   0        0        0     7359 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/bootloader.py
+-rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/py.typed
+-rw-r--r--   0        0        0     2371 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/secp256k1.py
+-rw-r--r--   0        0        0     1030 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__init__.py
+-rw-r--r--   0        0        0      870 2024-01-19 21:50:51.418555 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      675 2024-01-18 19:01:04.037196 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    39476 2024-01-19 21:50:51.421888 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-311.pyc
+-rw-r--r--   0        0        0    24433 2024-01-18 19:01:04.053864 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-39.pyc
+-rw-r--r--   0        0        0     2625 2024-01-19 21:50:51.418555 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-311.pyc
+-rw-r--r--   0        0        0     2063 2024-01-18 19:01:04.040530 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-39.pyc
+-rw-r--r--   0        0        0     7499 2024-01-19 21:50:51.425222 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-311.pyc
+-rw-r--r--   0        0        0     4741 2024-01-18 19:01:04.167206 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-39.pyc
+-rw-r--r--   0        0        0    27806 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/bitbox_api_protocol.py
+-rw-r--r--   0        0        0     1669 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/communication.py
+-rw-r--r--   0        0        0     4666 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/devices.py
+-rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__init__.py
+-rw-r--r--   0        0        0      201 2024-01-19 21:50:51.425222 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      165 2024-01-18 19:01:04.170540 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1622 2024-01-19 21:50:51.441890 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     1119 2024-01-18 19:01:04.223877 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     2132 2024-01-19 21:50:51.441890 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     1511 2024-01-18 19:01:04.220544 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     2577 2024-01-19 21:50:51.441890 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     1866 2024-01-18 19:01:04.220544 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     7901 2024-01-19 21:50:51.441890 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     6623 2024-01-18 19:01:04.223877 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     5318 2024-01-19 21:50:51.445224 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     4351 2024-01-18 19:01:04.227211 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1794 2024-01-19 21:50:51.438556 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     1238 2024-01-18 19:01:04.210543 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     5216 2024-01-19 21:50:51.445224 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     4298 2024-01-18 19:01:04.227211 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     5007 2024-01-19 21:50:51.425222 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     4320 2024-01-18 19:01:04.170540 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1474 2024-01-19 21:50:51.445224 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     1002 2024-01-18 19:01:04.227211 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1614 2024-01-19 21:50:51.445224 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     1112 2024-01-18 19:01:04.230544 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1616 2024-01-19 21:50:51.445224 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0     1143 2024-01-18 19:01:04.230544 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1460 2024-01-19 21:50:51.445224 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-311.pyc
+-rw-r--r--   0        0        0      990 2024-01-18 19:01:04.230544 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-39.pyc
+-rw-r--r--   0        0        0     1401 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.py
+-rw-r--r--   0        0        0     1638 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.pyi
+-rw-r--r--   0        0        0     2102 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.py
+-rw-r--r--   0        0        0     3851 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.pyi
+-rw-r--r--   0        0        0     2699 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.py
+-rw-r--r--   0        0        0     5248 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.pyi
+-rw-r--r--   0        0        0    10516 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.py
+-rw-r--r--   0        0        0    33375 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.pyi
+-rw-r--r--   0        0        0     6703 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.py
+-rw-r--r--   0        0        0    18628 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.pyi
+-rw-r--r--   0        0        0     1664 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.py
+-rw-r--r--   0        0        0     3152 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.pyi
+-rw-r--r--   0        0        0     6698 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.py
+-rw-r--r--   0        0        0    19589 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.pyi
+-rw-r--r--   0        0        0     5757 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.py
+-rw-r--r--   0        0        0    13514 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.pyi
+-rw-r--r--   0        0        0     1205 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.py
+-rw-r--r--   0        0        0     1308 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.pyi
+-rw-r--r--   0        0        0     1386 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.py
+-rw-r--r--   0        0        0     1541 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.pyi
+-rw-r--r--   0        0        0     1444 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.py
+-rw-r--r--   0        0        0     1990 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.pyi
+-rw-r--r--   0        0        0     1186 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.py
+-rw-r--r--   0        0        0     1394 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.pyi
+-rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/py.typed
+-rw-r--r--   0        0        0      709 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/__init__.py
+-rw-r--r--   0        0        0      432 2024-01-19 21:50:51.448557 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      346 2024-01-18 19:01:04.233878 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7264 2024-01-19 21:50:51.448557 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-311.pyc
+-rw-r--r--   0        0        0     4443 2024-01-18 19:01:04.237212 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-39.pyc
+-rw-r--r--   0        0        0     5793 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/u2fhid.py
+-rw-r--r--   0        0        0        0 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/py.typed
+-rw-r--r--   0        0        0     8035 2023-07-18 15:44:04.532963 hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/util.py
+-rw-r--r--   0        0        0      384 2021-03-12 18:18:18.588731 hwi-3.0.0rc1/hwilib/devices/ckcc/README.md
+-rw-r--r--   0        0        0       74 2021-03-12 18:18:18.588731 hwi-3.0.0rc1/hwilib/devices/ckcc/__init__.py
+-rw-r--r--   0        0        0      248 2024-01-19 21:50:51.025190 hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      204 2024-01-18 19:01:04.247213 hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    16309 2024-01-19 21:50:51.025190 hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     2625 2024-01-19 21:50:51.028524 hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0        0        0    15194 2024-01-19 21:50:51.028524 hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/protocol.cpython-311.pyc
+-rw-r--r--   0        0        0     4456 2024-01-19 21:50:51.028524 hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0    13206 2023-07-22 03:20:43.419147 hwi-3.0.0rc1/hwilib/devices/ckcc/client.py
+-rw-r--r--   0        0        0     2997 2021-03-12 18:18:18.588731 hwi-3.0.0rc1/hwilib/devices/ckcc/constants.py
+-rw-r--r--   0        0        0     9877 2021-03-12 18:18:18.588731 hwi-3.0.0rc1/hwilib/devices/ckcc/protocol.py
+-rw-r--r--   0        0        0     1807 2021-03-12 18:18:18.588731 hwi-3.0.0rc1/hwilib/devices/ckcc/sigheader.py
+-rw-r--r--   0        0        0     3470 2021-03-12 18:18:18.588731 hwi-3.0.0rc1/hwilib/devices/ckcc/utils.py
+-rw-r--r--   0        0        0    14585 2024-04-01 21:00:33.212822 hwi-3.0.0rc1/hwilib/devices/coldcard.py
+-rw-r--r--   0        0        0    27404 2024-04-01 21:00:33.212822 hwi-3.0.0rc1/hwilib/devices/digitalbitbox.py
+-rw-r--r--   0        0        0    25827 2024-04-01 21:00:33.212822 hwi-3.0.0rc1/hwilib/devices/jade.py
+-rw-r--r--   0        0        0      320 2022-10-28 21:25:37.086384 hwi-3.0.0rc1/hwilib/devices/jadepy/README.md
+-rw-r--r--   0        0        0       83 2022-10-28 21:25:37.086384 hwi-3.0.0rc1/hwilib/devices/jadepy/__init__.py
+-rw-r--r--   0        0        0      308 2024-01-19 21:50:51.708578 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      241 2024-01-18 19:01:04.003860 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    83592 2024-01-19 21:50:51.711912 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade.cpython-311.pyc
+-rw-r--r--   0        0        0    67602 2024-01-18 19:01:04.010527 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade.cpython-39.pyc
+-rw-r--r--   0        0        0     1422 2024-01-19 21:50:51.718579 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_error.cpython-311.pyc
+-rw-r--r--   0        0        0     1037 2024-01-18 19:01:04.010527 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_error.cpython-39.pyc
+-rw-r--r--   0        0        0     3617 2024-01-19 21:50:51.721912 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-311.pyc
+-rw-r--r--   0        0        0     2051 2024-01-18 19:01:04.010527 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-39.pyc
+-rw-r--r--   0        0        0     3412 2024-01-19 21:50:51.728580 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2024-01-30 19:06:23.837885 hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-39.pyc
+-rw-r--r--   0        0        0    75800 2023-11-14 21:41:54.054474 hwi-3.0.0rc1/hwilib/devices/jadepy/jade.py
+-rw-r--r--   0        0        0      655 2021-11-24 18:14:09.145516 hwi-3.0.0rc1/hwilib/devices/jadepy/jade_error.py
+-rw-r--r--   0        0        0     2348 2023-11-14 21:41:54.054474 hwi-3.0.0rc1/hwilib/devices/jadepy/jade_serial.py
+-rw-r--r--   0        0        0     1797 2023-11-14 21:41:54.054474 hwi-3.0.0rc1/hwilib/devices/jadepy/jade_tcp.py
+-rw-r--r--   0        0        0     9391 2024-04-01 21:00:33.212822 hwi-3.0.0rc1/hwilib/devices/keepkey.py
+-rw-r--r--   0        0        0    23345 2024-04-01 21:00:33.212822 hwi-3.0.0rc1/hwilib/devices/ledger.py
+-rw-r--r--   0        0        0     1265 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/README.md
+-rw-r--r--   0        0        0      327 2022-11-15 21:45:17.006790 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__init__.py
+-rw-r--r--   0        0        0      615 2024-01-19 21:50:50.855176 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      488 2024-01-18 19:01:04.290549 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    17244 2024-01-19 21:50:50.865177 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0     9524 2024-01-18 19:01:04.330552 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-39.pyc
+-rw-r--r--   0        0        0    12612 2024-01-19 21:50:50.855176 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-311.pyc
+-rw-r--r--   0        0        0     9527 2024-01-18 19:01:04.290549 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-39.pyc
+-rw-r--r--   0        0        0    21273 2024-01-19 21:50:50.865177 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-311.pyc
+-rw-r--r--   0        0        0    13479 2024-01-18 19:01:04.330552 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-39.pyc
+-rw-r--r--   0        0        0    17593 2024-01-19 21:50:50.868511 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-311.pyc
+-rw-r--r--   0        0        0     8700 2024-01-18 19:01:04.333886 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-39.pyc
+-rw-r--r--   0        0        0    10966 2024-01-19 21:50:50.858510 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-311.pyc
+-rw-r--r--   0        0        0     6728 2024-01-18 19:01:04.303884 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-39.pyc
+-rw-r--r--   0        0        0    13766 2024-01-19 21:50:50.861843 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-311.pyc
+-rw-r--r--   0        0        0     8873 2024-01-18 19:01:04.307217 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-39.pyc
+-rw-r--r--   0        0        0     8620 2024-01-19 21:50:50.861843 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-311.pyc
+-rw-r--r--   0        0        0     5021 2024-01-18 19:01:04.307217 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-39.pyc
+-rw-r--r--   0        0        0      488 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/README.md
+-rw-r--r--   0        0        0      855 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__init__.py
+-rw-r--r--   0        0        0     1061 2024-01-19 21:50:50.868511 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1016 2024-01-18 19:01:04.333886 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9117 2024-01-19 21:50:50.871844 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-311.pyc
+-rw-r--r--   0        0        0     5025 2024-01-18 19:01:04.340553 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-39.pyc
+-rw-r--r--   0        0        0     3158 2024-01-19 21:50:50.871844 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-311.pyc
+-rw-r--r--   0        0        0     2061 2024-01-18 19:01:04.340553 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-39.pyc
+-rw-r--r--   0        0        0    25379 2024-01-19 21:50:50.871844 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-311.pyc
+-rw-r--r--   0        0        0    12165 2024-01-18 19:01:04.337220 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-39.pyc
+-rw-r--r--   0        0        0     1707 2024-01-19 21:50:50.871844 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-311.pyc
+-rw-r--r--   0        0        0     1501 2024-01-18 19:01:04.340553 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-39.pyc
+-rw-r--r--   0        0        0     5339 2024-01-19 21:50:50.871844 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-311.pyc
+-rw-r--r--   0        0        0     2910 2024-01-18 19:01:04.343887 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-39.pyc
+-rw-r--r--   0        0        0     6230 2024-01-19 21:50:50.871844 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-311.pyc
+-rw-r--r--   0        0        0     3432 2024-01-18 19:01:04.347220 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-39.pyc
+-rw-r--r--   0        0        0     4874 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/bitcoinTransaction.py
+-rw-r--r--   0        0        0     2025 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/bitcoinVarint.py
+-rw-r--r--   0        0        0    16449 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/btchip.py
+-rw-r--r--   0        0        0     1020 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/btchipException.py
+-rw-r--r--   0        0        0     2715 2023-08-16 21:27:10.379182 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/btchipHelpers.py
+-rw-r--r--   0        0        0     3416 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/btchipUtils.py
+-rw-r--r--   0        0        0     3224 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/ledgerWrapper.py
+-rw-r--r--   0        0        0    11666 2022-11-15 21:45:17.006790 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/client.py
+-rw-r--r--   0        0        0     8168 2022-11-15 21:45:17.006790 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/client_base.py
+-rw-r--r--   0        0        0    12284 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/client_command.py
+-rw-r--r--   0        0        0    13915 2022-11-15 21:45:17.006790 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/client_legacy.py
+-rw-r--r--   0        0        0     6437 2022-11-15 21:45:17.006790 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/command_builder.py
+-rw-r--r--   0        0        0     8188 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/errors.py
+-rw-r--r--   0        0        0      806 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__init__.py
+-rw-r--r--   0        0        0      813 2024-01-19 21:50:50.861843 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      622 2024-01-18 19:01:04.310551 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1837 2024-01-19 21:50:50.861843 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-311.pyc
+-rw-r--r--   0        0        0     1286 2024-01-18 19:01:04.310551 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-39.pyc
+-rw-r--r--   0        0        0     2682 2024-01-19 21:50:50.861843 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     1940 2024-01-18 19:01:04.313884 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-39.pyc
+-rw-r--r--   0        0        0     1251 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/device_exception.py
+-rw-r--r--   0        0        0      652 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/errors.py
+-rw-r--r--   0        0        0      576 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/README.md
+-rw-r--r--   0        0        0      107 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__init__.py
+-rw-r--r--   0        0        0      340 2024-01-19 21:50:50.855176 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      280 2024-01-18 19:01:04.290549 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      413 2024-01-19 21:50:50.858510 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/log.cpython-311.pyc
+-rw-r--r--   0        0        0      273 2024-01-18 19:01:04.297217 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0     9497 2024-01-19 21:50:50.855176 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-311.pyc
+-rw-r--r--   0        0        0     6952 2024-01-18 19:01:04.293883 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-39.pyc
+-rw-r--r--   0        0        0       36 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__init__.py
+-rw-r--r--   0        0        0      244 2024-01-19 21:50:50.858510 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      206 2024-01-18 19:01:04.293883 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1868 2024-01-19 21:50:50.858510 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-311.pyc
+-rw-r--r--   0        0        0     1430 2024-01-18 19:01:04.297217 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-39.pyc
+-rw-r--r--   0        0        0     7896 2024-01-19 21:50:50.858510 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-311.pyc
+-rw-r--r--   0        0        0     4826 2024-01-18 19:01:04.300550 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-39.pyc
+-rw-r--r--   0        0        0     5057 2024-01-19 21:50:50.858510 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-311.pyc
+-rw-r--r--   0        0        0     3483 2024-01-18 19:01:04.297217 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-39.pyc
+-rw-r--r--   0        0        0      922 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/comm.py
+-rw-r--r--   0        0        0     5086 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/hid_device.py
+-rw-r--r--   0        0        0     2997 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/tcp_client.py
+-rw-r--r--   0        0        0       98 2023-08-16 21:28:50.470303 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/log.py
+-rw-r--r--   0        0        0     7019 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/transport.py
+-rw-r--r--   0        0        0     8430 2022-02-28 10:20:27.103458 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/merkle.py
+-rw-r--r--   0        0        0     4547 2022-11-15 21:45:17.006790 hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/wallet.py
+-rw-r--r--   0        0        0    36930 2024-04-01 21:00:33.212822 hwi-3.0.0rc1/hwilib/devices/trezor.py
+-rw-r--r--   0        0        0      628 2021-12-22 17:36:23.909185 hwi-3.0.0rc1/hwilib/devices/trezorlib/README.md
+-rw-r--r--   0        0        0      704 2021-12-22 17:36:23.909185 hwi-3.0.0rc1/hwilib/devices/trezorlib/__init__.py
+-rw-r--r--   0        0        0      197 2024-01-19 21:50:50.635159 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      160 2024-01-18 19:01:04.277215 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    17113 2024-01-19 21:50:50.688496 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/btc.cpython-311.pyc
+-rw-r--r--   0        0        0    24116 2024-01-19 21:50:50.638492 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/client.cpython-311.pyc
+-rw-r--r--   0        0        0    41480 2024-01-19 21:50:50.661827 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-311.pyc
+-rw-r--r--   0        0        0     9639 2024-01-19 21:50:50.691830 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/device.cpython-311.pyc
+-rw-r--r--   0        0        0     2651 2024-01-19 21:50:50.641826 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     1688 2024-01-18 19:01:04.280548 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0        0        0     3505 2024-01-19 21:50:50.658494 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/log.cpython-311.pyc
+-rw-r--r--   0        0        0     4282 2024-01-19 21:50:50.641826 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/mapping.cpython-311.pyc
+-rw-r--r--   0        0        0    94387 2024-01-19 21:50:50.648493 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/messages.cpython-311.pyc
+-rw-r--r--   0        0        0     2474 2024-01-19 21:50:50.655160 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0    30470 2024-01-19 21:50:50.651827 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-311.pyc
+-rw-r--r--   0        0        0    15554 2024-01-19 21:50:50.658494 hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/tools.cpython-311.pyc
+-rw-r--r--   0        0        0    13203 2021-12-22 17:36:23.909185 hwi-3.0.0rc1/hwilib/devices/trezorlib/btc.py
+-rw-r--r--   0        0        0    18854 2021-12-22 17:36:23.909185 hwi-3.0.0rc1/hwilib/devices/trezorlib/client.py
+-rw-r--r--   0        0        0    25872 2021-12-22 17:36:23.909185 hwi-3.0.0rc1/hwilib/devices/trezorlib/debuglink.py
+-rw-r--r--   0        0        0     7081 2021-12-22 17:36:23.909185 hwi-3.0.0rc1/hwilib/devices/trezorlib/device.py
+-rw-r--r--   0        0        0     1601 2021-12-22 17:36:23.909185 hwi-3.0.0rc1/hwilib/devices/trezorlib/exceptions.py
+-rw-r--r--   0        0        0    16038 2021-12-22 17:36:23.912518 hwi-3.0.0rc1/hwilib/devices/trezorlib/firmware.py
+-rw-r--r--   0        0        0     2275 2023-08-16 21:28:50.470303 hwi-3.0.0rc1/hwilib/devices/trezorlib/log.py
+-rw-r--r--   0        0        0     3499 2021-12-22 17:36:23.912518 hwi-3.0.0rc1/hwilib/devices/trezorlib/mapping.py
+-rw-r--r--   0        0        0    72766 2022-11-10 16:51:27.184728 hwi-3.0.0rc1/hwilib/devices/trezorlib/messages.py
+-rw-r--r--   0        0        0     2534 2024-01-17 18:52:53.554894 hwi-3.0.0rc1/hwilib/devices/trezorlib/models.py
+-rw-r--r--   0        0        0    20415 2021-12-22 17:36:23.912518 hwi-3.0.0rc1/hwilib/devices/trezorlib/protobuf.py
+-rw-r--r--   0        0        0    10087 2021-12-22 17:36:23.912518 hwi-3.0.0rc1/hwilib/devices/trezorlib/tools.py
+-rw-r--r--   0        0        0     4913 2021-11-19 17:56:12.722101 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__init__.py
+-rw-r--r--   0        0        0     7845 2024-01-19 21:50:50.661827 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4979 2024-01-18 19:01:04.280548 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8592 2024-01-19 21:50:50.665161 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-311.pyc
+-rw-r--r--   0        0        0     8878 2024-01-19 21:50:50.665161 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-311.pyc
+-rw-r--r--   0        0        0     8134 2024-01-19 21:50:50.671828 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-311.pyc
+-rw-r--r--   0        0        0     8656 2024-01-19 21:50:50.675162 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-311.pyc
+-rw-r--r--   0        0        0     5374 2021-11-19 17:56:12.722101 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/hid.py
+-rw-r--r--   0        0        0     5372 2021-03-12 18:18:18.592065 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/protocol.py
+-rw-r--r--   0        0        0     4881 2021-11-19 17:56:12.722101 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/udp.py
+-rw-r--r--   0        0        0     5315 2021-11-19 17:56:12.722101 hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/webusb.py
+-rw-r--r--   0        0        0     7048 2021-03-12 18:18:18.592065 hwi-3.0.0rc1/hwilib/errors.py
+-rw-r--r--   0        0        0     9167 2022-12-08 02:29:17.216573 hwi-3.0.0rc1/hwilib/hwwclient.py
+-rw-r--r--   0        0        0    14015 2022-05-23 15:49:56.363380 hwi-3.0.0rc1/hwilib/key.py
+-rw-r--r--   0        0        0    46452 2022-02-09 23:43:14.298584 hwi-3.0.0rc1/hwilib/psbt.py
+-rw-r--r--   0        0        0        0 2021-03-12 18:18:18.592065 hwi-3.0.0rc1/hwilib/py.typed
+-rw-r--r--   0        0        0     9191 2022-06-15 16:50:33.542133 hwi-3.0.0rc1/hwilib/tx.py
+-rw-r--r--   0        0        0     1756 2022-05-18 21:55:00.930698 hwi-3.0.0rc1/hwilib/udev/20-hw1.rules
+-rw-r--r--   0        0        0      310 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/udev/51-coinkite.rules
+-rw-r--r--   0        0        0      119 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/udev/51-hid-digitalbitbox.rules
+-rw-r--r--   0        0        0      980 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/udev/51-trezor.rules
+-rw-r--r--   0        0        0      769 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/udev/51-usb-keepkey.rules
+-rw-r--r--   0        0        0      142 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/udev/52-hid-digitalbitbox.rules
+-rw-r--r--   0        0        0      125 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/udev/53-hid-bitbox02.rules
+-rw-r--r--   0        0        0      147 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/udev/54-hid-bitbox02.rules
+-rw-r--r--   0        0        0      340 2022-02-01 17:28:57.968878 hwi-3.0.0rc1/hwilib/udev/55-usb-jade.rules
+-rw-r--r--   0        0        0     1158 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/udev/README.md
+-rw-r--r--   0        0        0     3416 2021-05-27 16:48:25.993035 hwi-3.0.0rc1/hwilib/udevinstaller.py
+-rw-r--r--   0        0        0     2687 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/ui/bitbox02pairing.ui
+-rw-r--r--   0        0        0     5380 2023-07-26 16:14:31.195563 hwi-3.0.0rc1/hwilib/ui/displayaddressdialog.ui
+-rw-r--r--   0        0        0     6167 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/ui/getkeypooloptionsdialog.ui
+-rw-r--r--   0        0        0     2872 2022-11-17 18:05:36.906293 hwi-3.0.0rc1/hwilib/ui/getxpubdialog.ui
+-rw-r--r--   0        0        0      196 2021-03-12 18:18:18.595398 hwi-3.0.0rc1/hwilib/ui/hwiqt.pyproject
+-rw-r--r--   0        0        0     7628 2022-11-17 18:05:36.906293 hwi-3.0.0rc1/hwilib/ui/mainwindow.ui
+-rw-r--r--   0        0        0     4431 2022-11-17 18:05:36.906293 hwi-3.0.0rc1/hwilib/ui/sendpindialog.ui
+-rw-r--r--   0        0        0     2117 2022-11-17 18:05:36.906293 hwi-3.0.0rc1/hwilib/ui/setpassphrasedialog.ui
+-rw-r--r--   0        0        0     4378 2022-11-17 18:05:36.906293 hwi-3.0.0rc1/hwilib/ui/signmessagedialog.ui
+-rw-r--r--   0        0        0     6092 2023-07-22 03:30:06.522930 hwi-3.0.0rc1/hwilib/ui/signpsbtdialog.ui
+-rw-r--r--   0        0        0     2604 2024-04-01 21:11:44.362655 hwi-3.0.0rc1/hwilib/ui/ui_bitbox02pairing.py
+-rw-r--r--   0        0        0     5548 2024-04-01 21:11:46.706174 hwi-3.0.0rc1/hwilib/ui/ui_displayaddressdialog.py
+-rw-r--r--   0        0        0     5827 2024-04-01 21:11:49.033026 hwi-3.0.0rc1/hwilib/ui/ui_getkeypooloptionsdialog.py
+-rw-r--r--   0        0        0     3229 2024-04-01 21:11:51.359876 hwi-3.0.0rc1/hwilib/ui/ui_getxpubdialog.py
+-rw-r--r--   0        0        0     9189 2024-04-01 21:11:53.760067 hwi-3.0.0rc1/hwilib/ui/ui_mainwindow.py
+-rw-r--r--   0        0        0     4845 2024-04-01 21:11:56.266932 hwi-3.0.0rc1/hwilib/ui/ui_sendpindialog.py
+-rw-r--r--   0        0        0     2107 2024-04-01 21:11:58.723793 hwi-3.0.0rc1/hwilib/ui/ui_setpassphrasedialog.py
+-rw-r--r--   0        0        0     4113 2024-04-01 21:12:01.130650 hwi-3.0.0rc1/hwilib/ui/ui_signmessagedialog.py
+-rw-r--r--   0        0        0     5552 2024-04-01 21:12:03.667518 hwi-3.0.0rc1/hwilib/ui/ui_signpsbtdialog.py
+-rw-r--r--   0        0        0     1282 2024-04-01 21:00:57.781435 hwi-3.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5412 1970-01-01 00:00:00.000000 hwi-3.0.0rc1/setup.py
+-rw-r--r--   0        0        0     4725 1970-01-01 00:00:00.000000 hwi-3.0.0rc1/PKG-INFO
```

### Comparing `hwi-3.0.0/LICENSE` & `hwi-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/README.md` & `hwi-3.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/_base58.py` & `hwi-3.0.0rc1/hwilib/_base58.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/_bech32.py` & `hwi-3.0.0rc1/hwilib/_bech32.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/_cli.py` & `hwi-3.0.0rc1/hwilib/_cli.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/_gui.py` & `hwi-3.0.0rc1/hwilib/_gui.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/_script.py` & `hwi-3.0.0rc1/hwilib/_script.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/_serialize.py` & `hwi-3.0.0rc1/hwilib/_serialize.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/commands.py` & `hwi-3.0.0rc1/hwilib/commands.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/common.py` & `hwi-3.0.0rc1/hwilib/common.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/descriptor.py` & `hwi-3.0.0rc1/hwilib/descriptor.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/__pycache__/bitbox02.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/__pycache__/bitbox02.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/__pycache__/coldcard.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/__pycache__/coldcard.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/__pycache__/digitalbitbox.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/__pycache__/digitalbitbox.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/__pycache__/jade.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/__pycache__/jade.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/__pycache__/keepkey.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/__pycache__/keepkey.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/__pycache__/ledger.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/__pycache__/ledger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/__pycache__/trezor.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/__pycache__/trezor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/LICENSE` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/LICENSE`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/README.md` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/README.md`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/__pycache__/util.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__init__.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bitbox02.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/bootloader.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/__pycache__/secp256k1.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/bitbox02.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/bitbox02.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/bootloader.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/bootloader.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/bitbox02/secp256k1.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/bitbox02/secp256k1.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__init__.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/bitbox_api_protocol.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/communication.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/__pycache__/devices.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/bitbox_api_protocol.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/bitbox_api_protocol.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/communication.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/communication.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/devices.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/devices.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/antiklepto_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/backup_commands_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/bitbox02_system_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/btc_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/cardano_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/common_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/eth_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/hww_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/keystore_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/mnemonic_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/perform_attestation_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/__pycache__/system_pb2.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/antiklepto_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/backup_commands_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/bitbox02_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/btc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/cardano_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/eth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/hww_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/keystore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/mnemonic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/perform_attestation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.pyi` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/generated/system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__init__.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/__pycache__/u2fhid.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/communication/u2fhid/u2fhid.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/communication/u2fhid/u2fhid.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/bitbox02_lib/util.py` & `hwi-3.0.0rc1/hwilib/devices/bitbox02_lib/util.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/__pycache__/client.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/__pycache__/constants.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/__pycache__/protocol.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/protocol.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/__pycache__/utils.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ckcc/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/client.py` & `hwi-3.0.0rc1/hwilib/devices/ckcc/client.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/constants.py` & `hwi-3.0.0rc1/hwilib/devices/ckcc/constants.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/protocol.py` & `hwi-3.0.0rc1/hwilib/devices/ckcc/protocol.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/sigheader.py` & `hwi-3.0.0rc1/hwilib/devices/ckcc/sigheader.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ckcc/utils.py` & `hwi-3.0.0rc1/hwilib/devices/ckcc/utils.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/coldcard.py` & `hwi-3.0.0rc1/hwilib/devices/coldcard.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/digitalbitbox.py` & `hwi-3.0.0rc1/hwilib/devices/digitalbitbox.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jade.py` & `hwi-3.0.0rc1/hwilib/devices/jade.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_error.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_error.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_error.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_error.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_serial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/jadepy/__pycache__/jade_tcp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/jade.py` & `hwi-3.0.0rc1/hwilib/devices/jadepy/jade.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/jade_error.py` & `hwi-3.0.0rc1/hwilib/devices/jadepy/jade_error.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/jade_serial.py` & `hwi-3.0.0rc1/hwilib/devices/jadepy/jade_serial.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/jadepy/jade_tcp.py` & `hwi-3.0.0rc1/hwilib/devices/jadepy/jade_tcp.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/keepkey.py` & `hwi-3.0.0rc1/hwilib/devices/keepkey.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger.py` & `hwi-3.0.0rc1/hwilib/devices/ledger.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/README.md` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/README.md`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/__init__.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_command.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/client_legacy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/command_builder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/merkle.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/__pycache__/wallet.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__init__.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinTransaction.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/bitcoinVarint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchip.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipException.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipHelpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/__pycache__/btchipUtils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/bitcoinTransaction.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/bitcoinTransaction.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/bitcoinVarint.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/bitcoinVarint.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/btchip.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/btchip.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/btchipException.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/btchipException.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/btchipHelpers.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/btchipHelpers.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/btchipUtils.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/btchipUtils.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/btchip/ledgerWrapper.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/btchip/ledgerWrapper.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/client.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/client.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/client_base.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/client_base.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/client_command.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/client_command.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/client_legacy.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/client_legacy.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/command_builder.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/command_builder.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/errors.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/errors.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__init__.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/device_exception.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/__pycache__/errors.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/device_exception.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/device_exception.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/exception/errors.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/exception/errors.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/README.md` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/README.md`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/__pycache__/transport.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/comm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/hid_device.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/__pycache__/tcp_client.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/comm.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/comm.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/hid_device.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/hid_device.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/tcp_client.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/interfaces/tcp_client.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/ledgercomm/transport.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/ledgercomm/transport.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/merkle.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/merkle.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/ledger_bitcoin/wallet.py` & `hwi-3.0.0rc1/hwilib/devices/ledger_bitcoin/wallet.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezor.py` & `hwi-3.0.0rc1/hwilib/devices/trezor.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/README.md` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/README.md`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__init__.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/btc.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/btc.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/client.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/debuglink.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/device.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/device.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/exceptions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/log.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/log.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/mapping.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/mapping.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/messages.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/messages.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/models.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/protobuf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/__pycache__/tools.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/__pycache__/tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/btc.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/btc.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/client.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/client.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/debuglink.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/debuglink.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/device.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/device.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/exceptions.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/firmware.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/firmware.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/log.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/log.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/mapping.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/mapping.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/messages.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/messages.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/models.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/models.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/protobuf.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/protobuf.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/tools.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/tools.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/__init__.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-39.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/hid.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/protocol.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/udp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-311.pyc` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/__pycache__/webusb.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/hid.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/hid.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/protocol.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/protocol.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/udp.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/udp.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/devices/trezorlib/transport/webusb.py` & `hwi-3.0.0rc1/hwilib/devices/trezorlib/transport/webusb.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/errors.py` & `hwi-3.0.0rc1/hwilib/errors.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/hwwclient.py` & `hwi-3.0.0rc1/hwilib/hwwclient.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/key.py` & `hwi-3.0.0rc1/hwilib/key.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/psbt.py` & `hwi-3.0.0rc1/hwilib/psbt.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/tx.py` & `hwi-3.0.0rc1/hwilib/tx.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/udev/20-hw1.rules` & `hwi-3.0.0rc1/hwilib/udev/20-hw1.rules`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/udev/51-trezor.rules` & `hwi-3.0.0rc1/hwilib/udev/51-trezor.rules`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/udev/51-usb-keepkey.rules` & `hwi-3.0.0rc1/hwilib/udev/51-usb-keepkey.rules`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/udev/README.md` & `hwi-3.0.0rc1/hwilib/udev/README.md`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/udevinstaller.py` & `hwi-3.0.0rc1/hwilib/udevinstaller.py`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/bitbox02pairing.ui` & `hwi-3.0.0rc1/hwilib/ui/bitbox02pairing.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/displayaddressdialog.ui` & `hwi-3.0.0rc1/hwilib/ui/displayaddressdialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/getkeypooloptionsdialog.ui` & `hwi-3.0.0rc1/hwilib/ui/getkeypooloptionsdialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/getxpubdialog.ui` & `hwi-3.0.0rc1/hwilib/ui/getxpubdialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/mainwindow.ui` & `hwi-3.0.0rc1/hwilib/ui/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/sendpindialog.ui` & `hwi-3.0.0rc1/hwilib/ui/sendpindialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/setpassphrasedialog.ui` & `hwi-3.0.0rc1/hwilib/ui/setpassphrasedialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/signmessagedialog.ui` & `hwi-3.0.0rc1/hwilib/ui/signmessagedialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/signpsbtdialog.ui` & `hwi-3.0.0rc1/hwilib/ui/signpsbtdialog.ui`

 * *Files identical despite different names*

### Comparing `hwi-3.0.0/hwilib/ui/ui_bitbox02pairing.py` & `hwi-3.0.0rc1/hwilib/ui/ui_bitbox02pairing.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'bitbox02pairing.ui'
-##
-## Created by: Qt User Interface Compiler version 5.15.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
-
-
-class Ui_BitBox02PairingDialog(object):
-    def setupUi(self, BitBox02PairingDialog):
-        if not BitBox02PairingDialog.objectName():
-            BitBox02PairingDialog.setObjectName(u"BitBox02PairingDialog")
-        BitBox02PairingDialog.setWindowModality(Qt.WindowModal)
-        BitBox02PairingDialog.resize(400, 209)
-        self.buttonBox = QDialogButtonBox(BitBox02PairingDialog)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setGeometry(QRect(30, 160, 341, 32))
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.No|QDialogButtonBox.Yes)
-        self.pairingCode = QLabel(BitBox02PairingDialog)
-        self.pairingCode.setObjectName(u"pairingCode")
-        self.pairingCode.setGeometry(QRect(20, 80, 331, 61))
-        font = QFont()
-        font.setFamily(u"DejaVu Sans Mono")
-        font.setPointSize(15)
-        font.setBold(True)
-        font.setWeight(75)
-        self.pairingCode.setFont(font)
-        self.pairingCode.setTextFormat(Qt.RichText)
-        self.pairingCode.setAlignment(Qt.AlignCenter)
-        self.label_2 = QLabel(BitBox02PairingDialog)
-        self.label_2.setObjectName(u"label_2")
-        self.label_2.setGeometry(QRect(20, 10, 351, 61))
-        font1 = QFont()
-        font1.setPointSize(11)
-        self.label_2.setFont(font1)
-        self.label_2.setTextFormat(Qt.PlainText)
-
-        self.retranslateUi(BitBox02PairingDialog)
-        self.buttonBox.accepted.connect(BitBox02PairingDialog.accept)
-        self.buttonBox.rejected.connect(BitBox02PairingDialog.reject)
-
-        QMetaObject.connectSlotsByName(BitBox02PairingDialog)
-    # setupUi
-
-    def retranslateUi(self, BitBox02PairingDialog):
-        BitBox02PairingDialog.setWindowTitle(QCoreApplication.translate("BitBox02PairingDialog", u"Dialog", None))
-        self.pairingCode.setText("")
-        self.label_2.setText(QCoreApplication.translate("BitBox02PairingDialog", u"Please verify the pairing code matches what is\n"
-"shown on your BitBox02.", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'bitbox02pairing.ui'
+##
+## Created by: Qt User Interface Compiler version 5.15.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide2.QtCore import *
+from PySide2.QtGui import *
+from PySide2.QtWidgets import *
+
+
+class Ui_BitBox02PairingDialog(object):
+    def setupUi(self, BitBox02PairingDialog):
+        if not BitBox02PairingDialog.objectName():
+            BitBox02PairingDialog.setObjectName(u"BitBox02PairingDialog")
+        BitBox02PairingDialog.setWindowModality(Qt.WindowModal)
+        BitBox02PairingDialog.resize(400, 209)
+        self.buttonBox = QDialogButtonBox(BitBox02PairingDialog)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setGeometry(QRect(30, 160, 341, 32))
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.No|QDialogButtonBox.Yes)
+        self.pairingCode = QLabel(BitBox02PairingDialog)
+        self.pairingCode.setObjectName(u"pairingCode")
+        self.pairingCode.setGeometry(QRect(20, 80, 331, 61))
+        font = QFont()
+        font.setFamily(u"DejaVu Sans Mono")
+        font.setPointSize(15)
+        font.setBold(True)
+        font.setWeight(75)
+        self.pairingCode.setFont(font)
+        self.pairingCode.setTextFormat(Qt.RichText)
+        self.pairingCode.setAlignment(Qt.AlignCenter)
+        self.label_2 = QLabel(BitBox02PairingDialog)
+        self.label_2.setObjectName(u"label_2")
+        self.label_2.setGeometry(QRect(20, 10, 351, 61))
+        font1 = QFont()
+        font1.setPointSize(11)
+        self.label_2.setFont(font1)
+        self.label_2.setTextFormat(Qt.PlainText)
+
+        self.retranslateUi(BitBox02PairingDialog)
+        self.buttonBox.accepted.connect(BitBox02PairingDialog.accept)
+        self.buttonBox.rejected.connect(BitBox02PairingDialog.reject)
+
+        QMetaObject.connectSlotsByName(BitBox02PairingDialog)
+    # setupUi
+
+    def retranslateUi(self, BitBox02PairingDialog):
+        BitBox02PairingDialog.setWindowTitle(QCoreApplication.translate("BitBox02PairingDialog", u"Dialog", None))
+        self.pairingCode.setText("")
+        self.label_2.setText(QCoreApplication.translate("BitBox02PairingDialog", u"Please verify the pairing code matches what is\n"
+"shown on your BitBox02.", None))
+    # retranslateUi
+
```

### Comparing `hwi-3.0.0/hwilib/ui/ui_displayaddressdialog.py` & `hwi-3.0.0rc1/hwilib/ui/ui_displayaddressdialog.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'displayaddressdialog.ui'
-##
-## Created by: Qt User Interface Compiler version 5.15.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
-
-
-class Ui_DisplayAddressDialog(object):
-    def setupUi(self, DisplayAddressDialog):
-        if not DisplayAddressDialog.objectName():
-            DisplayAddressDialog.setObjectName(u"DisplayAddressDialog")
-        DisplayAddressDialog.resize(500, 200)
-        self.gridLayout = QGridLayout(DisplayAddressDialog)
-        self.gridLayout.setSpacing(10)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.gridLayout.setContentsMargins(10, 10, 10, 10)
-        self.type_groupbox = QGroupBox(DisplayAddressDialog)
-        self.type_groupbox.setObjectName(u"type_groupbox")
-        sizePolicy = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Minimum)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.type_groupbox.sizePolicy().hasHeightForWidth())
-        self.type_groupbox.setSizePolicy(sizePolicy)
-        self.type_groupbox.setMinimumSize(QSize(300, 50))
-        self.type_groupbox.setMaximumSize(QSize(500, 50))
-        self.horizontalLayout_2 = QHBoxLayout(self.type_groupbox)
-        self.horizontalLayout_2.setSpacing(5)
-        self.horizontalLayout_2.setObjectName(u"horizontalLayout_2")
-        self.sh_wpkh_radio = QRadioButton(self.type_groupbox)
-        self.sh_wpkh_radio.setObjectName(u"sh_wpkh_radio")
-        self.sh_wpkh_radio.setChecked(True)
-
-        self.horizontalLayout_2.addWidget(self.sh_wpkh_radio)
-
-        self.wpkh_radio = QRadioButton(self.type_groupbox)
-        self.wpkh_radio.setObjectName(u"wpkh_radio")
-
-        self.horizontalLayout_2.addWidget(self.wpkh_radio)
-
-        self.pkh_radio = QRadioButton(self.type_groupbox)
-        self.pkh_radio.setObjectName(u"pkh_radio")
-
-        self.horizontalLayout_2.addWidget(self.pkh_radio)
-
-
-        self.gridLayout.addWidget(self.type_groupbox, 1, 0, 1, 2)
-
-        self.label_2 = QLabel(DisplayAddressDialog)
-        self.label_2.setObjectName(u"label_2")
-
-        self.gridLayout.addWidget(self.label_2, 2, 0, 1, 1)
-
-        self.address_lineedit = QLineEdit(DisplayAddressDialog)
-        self.address_lineedit.setObjectName(u"address_lineedit")
-        self.address_lineedit.setMinimumSize(QSize(100, 30))
-        self.address_lineedit.setReadOnly(True)
-
-        self.gridLayout.addWidget(self.address_lineedit, 2, 1, 1, 2)
-
-        self.path_lineedit = QLineEdit(DisplayAddressDialog)
-        self.path_lineedit.setObjectName(u"path_lineedit")
-        self.path_lineedit.setMinimumSize(QSize(200, 30))
-
-        self.gridLayout.addWidget(self.path_lineedit, 0, 1, 1, 2)
-
-        self.go_button = QPushButton(DisplayAddressDialog)
-        self.go_button.setObjectName(u"go_button")
-        sizePolicy1 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
-        sizePolicy1.setHorizontalStretch(0)
-        sizePolicy1.setVerticalStretch(0)
-        sizePolicy1.setHeightForWidth(self.go_button.sizePolicy().hasHeightForWidth())
-        self.go_button.setSizePolicy(sizePolicy1)
-        self.go_button.setMinimumSize(QSize(40, 40))
-        self.go_button.setMaximumSize(QSize(50, 40))
-        self.go_button.setAutoDefault(False)
-
-        self.gridLayout.addWidget(self.go_button, 1, 2, 1, 1, Qt.AlignHCenter)
-
-        self.buttonBox = QDialogButtonBox(DisplayAddressDialog)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setMinimumSize(QSize(0, 25))
-        self.buttonBox.setMaximumSize(QSize(80, 25))
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Close)
-
-        self.gridLayout.addWidget(self.buttonBox, 3, 2, 1, 1)
-
-        self.label = QLabel(DisplayAddressDialog)
-        self.label.setObjectName(u"label")
-        self.label.setMaximumSize(QSize(100, 16777215))
-
-        self.gridLayout.addWidget(self.label, 0, 0, 1, 1)
-
-
-        self.retranslateUi(DisplayAddressDialog)
-        self.buttonBox.accepted.connect(DisplayAddressDialog.accept)
-        self.buttonBox.rejected.connect(DisplayAddressDialog.reject)
-
-        self.go_button.setDefault(True)
-
-
-        QMetaObject.connectSlotsByName(DisplayAddressDialog)
-    # setupUi
-
-    def retranslateUi(self, DisplayAddressDialog):
-        DisplayAddressDialog.setWindowTitle(QCoreApplication.translate("DisplayAddressDialog", u"Dialog", None))
-        self.type_groupbox.setTitle("")
-        self.sh_wpkh_radio.setText(QCoreApplication.translate("DisplayAddressDialog", u"P2SH-P2WPKH", None))
-        self.wpkh_radio.setText(QCoreApplication.translate("DisplayAddressDialog", u"P2WPKH", None))
-        self.pkh_radio.setText(QCoreApplication.translate("DisplayAddressDialog", u"P2PKH", None))
-        self.label_2.setText(QCoreApplication.translate("DisplayAddressDialog", u"Address", None))
-        self.go_button.setText(QCoreApplication.translate("DisplayAddressDialog", u"Go", None))
-        self.label.setText(QCoreApplication.translate("DisplayAddressDialog", u"Derivation Path", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'displayaddressdialog.ui'
+##
+## Created by: Qt User Interface Compiler version 5.15.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide2.QtCore import *
+from PySide2.QtGui import *
+from PySide2.QtWidgets import *
+
+
+class Ui_DisplayAddressDialog(object):
+    def setupUi(self, DisplayAddressDialog):
+        if not DisplayAddressDialog.objectName():
+            DisplayAddressDialog.setObjectName(u"DisplayAddressDialog")
+        DisplayAddressDialog.resize(500, 200)
+        self.gridLayout = QGridLayout(DisplayAddressDialog)
+        self.gridLayout.setSpacing(10)
+        self.gridLayout.setObjectName(u"gridLayout")
+        self.gridLayout.setContentsMargins(10, 10, 10, 10)
+        self.type_groupbox = QGroupBox(DisplayAddressDialog)
+        self.type_groupbox.setObjectName(u"type_groupbox")
+        sizePolicy = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Minimum)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.type_groupbox.sizePolicy().hasHeightForWidth())
+        self.type_groupbox.setSizePolicy(sizePolicy)
+        self.type_groupbox.setMinimumSize(QSize(300, 50))
+        self.type_groupbox.setMaximumSize(QSize(500, 50))
+        self.horizontalLayout_2 = QHBoxLayout(self.type_groupbox)
+        self.horizontalLayout_2.setSpacing(5)
+        self.horizontalLayout_2.setObjectName(u"horizontalLayout_2")
+        self.sh_wpkh_radio = QRadioButton(self.type_groupbox)
+        self.sh_wpkh_radio.setObjectName(u"sh_wpkh_radio")
+        self.sh_wpkh_radio.setChecked(True)
+
+        self.horizontalLayout_2.addWidget(self.sh_wpkh_radio)
+
+        self.wpkh_radio = QRadioButton(self.type_groupbox)
+        self.wpkh_radio.setObjectName(u"wpkh_radio")
+
+        self.horizontalLayout_2.addWidget(self.wpkh_radio)
+
+        self.pkh_radio = QRadioButton(self.type_groupbox)
+        self.pkh_radio.setObjectName(u"pkh_radio")
+
+        self.horizontalLayout_2.addWidget(self.pkh_radio)
+
+
+        self.gridLayout.addWidget(self.type_groupbox, 1, 0, 1, 2)
+
+        self.label_2 = QLabel(DisplayAddressDialog)
+        self.label_2.setObjectName(u"label_2")
+
+        self.gridLayout.addWidget(self.label_2, 2, 0, 1, 1)
+
+        self.address_lineedit = QLineEdit(DisplayAddressDialog)
+        self.address_lineedit.setObjectName(u"address_lineedit")
+        self.address_lineedit.setMinimumSize(QSize(100, 30))
+        self.address_lineedit.setReadOnly(True)
+
+        self.gridLayout.addWidget(self.address_lineedit, 2, 1, 1, 2)
+
+        self.path_lineedit = QLineEdit(DisplayAddressDialog)
+        self.path_lineedit.setObjectName(u"path_lineedit")
+        self.path_lineedit.setMinimumSize(QSize(200, 30))
+
+        self.gridLayout.addWidget(self.path_lineedit, 0, 1, 1, 2)
+
+        self.go_button = QPushButton(DisplayAddressDialog)
+        self.go_button.setObjectName(u"go_button")
+        sizePolicy1 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
+        sizePolicy1.setHorizontalStretch(0)
+        sizePolicy1.setVerticalStretch(0)
+        sizePolicy1.setHeightForWidth(self.go_button.sizePolicy().hasHeightForWidth())
+        self.go_button.setSizePolicy(sizePolicy1)
+        self.go_button.setMinimumSize(QSize(40, 40))
+        self.go_button.setMaximumSize(QSize(50, 40))
+        self.go_button.setAutoDefault(False)
+
+        self.gridLayout.addWidget(self.go_button, 1, 2, 1, 1, Qt.AlignHCenter)
+
+        self.buttonBox = QDialogButtonBox(DisplayAddressDialog)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setMinimumSize(QSize(0, 25))
+        self.buttonBox.setMaximumSize(QSize(80, 25))
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Close)
+
+        self.gridLayout.addWidget(self.buttonBox, 3, 2, 1, 1)
+
+        self.label = QLabel(DisplayAddressDialog)
+        self.label.setObjectName(u"label")
+        self.label.setMaximumSize(QSize(100, 16777215))
+
+        self.gridLayout.addWidget(self.label, 0, 0, 1, 1)
+
+
+        self.retranslateUi(DisplayAddressDialog)
+        self.buttonBox.accepted.connect(DisplayAddressDialog.accept)
+        self.buttonBox.rejected.connect(DisplayAddressDialog.reject)
+
+        self.go_button.setDefault(True)
+
+
+        QMetaObject.connectSlotsByName(DisplayAddressDialog)
+    # setupUi
+
+    def retranslateUi(self, DisplayAddressDialog):
+        DisplayAddressDialog.setWindowTitle(QCoreApplication.translate("DisplayAddressDialog", u"Dialog", None))
+        self.type_groupbox.setTitle("")
+        self.sh_wpkh_radio.setText(QCoreApplication.translate("DisplayAddressDialog", u"P2SH-P2WPKH", None))
+        self.wpkh_radio.setText(QCoreApplication.translate("DisplayAddressDialog", u"P2WPKH", None))
+        self.pkh_radio.setText(QCoreApplication.translate("DisplayAddressDialog", u"P2PKH", None))
+        self.label_2.setText(QCoreApplication.translate("DisplayAddressDialog", u"Address", None))
+        self.go_button.setText(QCoreApplication.translate("DisplayAddressDialog", u"Go", None))
+        self.label.setText(QCoreApplication.translate("DisplayAddressDialog", u"Derivation Path", None))
+    # retranslateUi
+
```

### Comparing `hwi-3.0.0/hwilib/ui/ui_getkeypooloptionsdialog.py` & `hwi-3.0.0rc1/hwilib/ui/ui_getkeypooloptionsdialog.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'getkeypooloptionsdialog.ui'
-##
-## Created by: Qt User Interface Compiler version 5.15.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
-
-
-class Ui_GetKeypoolOptionsDialog(object):
-    def setupUi(self, GetKeypoolOptionsDialog):
-        if not GetKeypoolOptionsDialog.objectName():
-            GetKeypoolOptionsDialog.setObjectName(u"GetKeypoolOptionsDialog")
-        GetKeypoolOptionsDialog.resize(440, 224)
-        self.buttonBox = QDialogButtonBox(GetKeypoolOptionsDialog)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setGeometry(QRect(80, 180, 341, 32))
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
-        self.label = QLabel(GetKeypoolOptionsDialog)
-        self.label.setObjectName(u"label")
-        self.label.setGeometry(QRect(20, 20, 41, 18))
-        self.label_2 = QLabel(GetKeypoolOptionsDialog)
-        self.label_2.setObjectName(u"label_2")
-        self.label_2.setGeometry(QRect(20, 60, 31, 18))
-        self.start_spinbox = QSpinBox(GetKeypoolOptionsDialog)
-        self.start_spinbox.setObjectName(u"start_spinbox")
-        self.start_spinbox.setGeometry(QRect(80, 10, 161, 32))
-        self.start_spinbox.setMaximum(2147483647)
-        self.end_spinbox = QSpinBox(GetKeypoolOptionsDialog)
-        self.end_spinbox.setObjectName(u"end_spinbox")
-        self.end_spinbox.setGeometry(QRect(80, 50, 161, 32))
-        self.end_spinbox.setMaximum(2147483647)
-        self.end_spinbox.setValue(1000)
-        self.internal_checkbox = QCheckBox(GetKeypoolOptionsDialog)
-        self.internal_checkbox.setObjectName(u"internal_checkbox")
-        self.internal_checkbox.setGeometry(QRect(280, 10, 88, 22))
-        self.keypool_checkbox = QCheckBox(GetKeypoolOptionsDialog)
-        self.keypool_checkbox.setObjectName(u"keypool_checkbox")
-        self.keypool_checkbox.setGeometry(QRect(280, 40, 88, 22))
-        self.keypool_checkbox.setChecked(True)
-        self.groupBox = QGroupBox(GetKeypoolOptionsDialog)
-        self.groupBox.setObjectName(u"groupBox")
-        self.groupBox.setGeometry(QRect(280, 70, 141, 101))
-        self.sh_wpkh_radio = QRadioButton(self.groupBox)
-        self.sh_wpkh_radio.setObjectName(u"sh_wpkh_radio")
-        self.sh_wpkh_radio.setGeometry(QRect(10, 10, 121, 22))
-        self.sh_wpkh_radio.setChecked(True)
-        self.wpkh_radio = QRadioButton(self.groupBox)
-        self.wpkh_radio.setObjectName(u"wpkh_radio")
-        self.wpkh_radio.setGeometry(QRect(10, 40, 105, 22))
-        self.pkh_radio = QRadioButton(self.groupBox)
-        self.pkh_radio.setObjectName(u"pkh_radio")
-        self.pkh_radio.setGeometry(QRect(10, 70, 105, 22))
-        self.groupBox_2 = QGroupBox(GetKeypoolOptionsDialog)
-        self.groupBox_2.setObjectName(u"groupBox_2")
-        self.groupBox_2.setGeometry(QRect(10, 90, 231, 91))
-        self.account_spinbox = QSpinBox(self.groupBox_2)
-        self.account_spinbox.setObjectName(u"account_spinbox")
-        self.account_spinbox.setGeometry(QRect(100, 10, 111, 32))
-        self.account_spinbox.setMaximum(2147483647)
-        self.account_spinbox.setValue(0)
-        self.account_radio = QRadioButton(self.groupBox_2)
-        self.account_radio.setObjectName(u"account_radio")
-        self.account_radio.setGeometry(QRect(10, 10, 81, 22))
-        self.account_radio.setChecked(True)
-        self.path_radio = QRadioButton(self.groupBox_2)
-        self.path_radio.setObjectName(u"path_radio")
-        self.path_radio.setGeometry(QRect(10, 50, 61, 22))
-        self.path_lineedit = QLineEdit(self.groupBox_2)
-        self.path_lineedit.setObjectName(u"path_lineedit")
-        self.path_lineedit.setEnabled(False)
-        self.path_lineedit.setGeometry(QRect(80, 50, 141, 32))
-
-        self.retranslateUi(GetKeypoolOptionsDialog)
-        self.buttonBox.accepted.connect(GetKeypoolOptionsDialog.accept)
-        self.buttonBox.rejected.connect(GetKeypoolOptionsDialog.reject)
-
-        QMetaObject.connectSlotsByName(GetKeypoolOptionsDialog)
-    # setupUi
-
-    def retranslateUi(self, GetKeypoolOptionsDialog):
-        GetKeypoolOptionsDialog.setWindowTitle(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Dialog", None))
-        self.label.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Start", None))
-        self.label_2.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"End", None))
-        self.internal_checkbox.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Internal", None))
-        self.keypool_checkbox.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"keypool", None))
-        self.groupBox.setTitle("")
-        self.sh_wpkh_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"P2SH-P2WPKH", None))
-        self.wpkh_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"P2WPKH", None))
-        self.pkh_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"P2PKH", None))
-        self.groupBox_2.setTitle("")
-        self.account_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Account", None))
-        self.path_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Path", None))
-        self.path_lineedit.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"m/0'/0'/*", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'getkeypooloptionsdialog.ui'
+##
+## Created by: Qt User Interface Compiler version 5.15.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide2.QtCore import *
+from PySide2.QtGui import *
+from PySide2.QtWidgets import *
+
+
+class Ui_GetKeypoolOptionsDialog(object):
+    def setupUi(self, GetKeypoolOptionsDialog):
+        if not GetKeypoolOptionsDialog.objectName():
+            GetKeypoolOptionsDialog.setObjectName(u"GetKeypoolOptionsDialog")
+        GetKeypoolOptionsDialog.resize(440, 224)
+        self.buttonBox = QDialogButtonBox(GetKeypoolOptionsDialog)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setGeometry(QRect(80, 180, 341, 32))
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
+        self.label = QLabel(GetKeypoolOptionsDialog)
+        self.label.setObjectName(u"label")
+        self.label.setGeometry(QRect(20, 20, 41, 18))
+        self.label_2 = QLabel(GetKeypoolOptionsDialog)
+        self.label_2.setObjectName(u"label_2")
+        self.label_2.setGeometry(QRect(20, 60, 31, 18))
+        self.start_spinbox = QSpinBox(GetKeypoolOptionsDialog)
+        self.start_spinbox.setObjectName(u"start_spinbox")
+        self.start_spinbox.setGeometry(QRect(80, 10, 161, 32))
+        self.start_spinbox.setMaximum(2147483647)
+        self.end_spinbox = QSpinBox(GetKeypoolOptionsDialog)
+        self.end_spinbox.setObjectName(u"end_spinbox")
+        self.end_spinbox.setGeometry(QRect(80, 50, 161, 32))
+        self.end_spinbox.setMaximum(2147483647)
+        self.end_spinbox.setValue(1000)
+        self.internal_checkbox = QCheckBox(GetKeypoolOptionsDialog)
+        self.internal_checkbox.setObjectName(u"internal_checkbox")
+        self.internal_checkbox.setGeometry(QRect(280, 10, 88, 22))
+        self.keypool_checkbox = QCheckBox(GetKeypoolOptionsDialog)
+        self.keypool_checkbox.setObjectName(u"keypool_checkbox")
+        self.keypool_checkbox.setGeometry(QRect(280, 40, 88, 22))
+        self.keypool_checkbox.setChecked(True)
+        self.groupBox = QGroupBox(GetKeypoolOptionsDialog)
+        self.groupBox.setObjectName(u"groupBox")
+        self.groupBox.setGeometry(QRect(280, 70, 141, 101))
+        self.sh_wpkh_radio = QRadioButton(self.groupBox)
+        self.sh_wpkh_radio.setObjectName(u"sh_wpkh_radio")
+        self.sh_wpkh_radio.setGeometry(QRect(10, 10, 121, 22))
+        self.sh_wpkh_radio.setChecked(True)
+        self.wpkh_radio = QRadioButton(self.groupBox)
+        self.wpkh_radio.setObjectName(u"wpkh_radio")
+        self.wpkh_radio.setGeometry(QRect(10, 40, 105, 22))
+        self.pkh_radio = QRadioButton(self.groupBox)
+        self.pkh_radio.setObjectName(u"pkh_radio")
+        self.pkh_radio.setGeometry(QRect(10, 70, 105, 22))
+        self.groupBox_2 = QGroupBox(GetKeypoolOptionsDialog)
+        self.groupBox_2.setObjectName(u"groupBox_2")
+        self.groupBox_2.setGeometry(QRect(10, 90, 231, 91))
+        self.account_spinbox = QSpinBox(self.groupBox_2)
+        self.account_spinbox.setObjectName(u"account_spinbox")
+        self.account_spinbox.setGeometry(QRect(100, 10, 111, 32))
+        self.account_spinbox.setMaximum(2147483647)
+        self.account_spinbox.setValue(0)
+        self.account_radio = QRadioButton(self.groupBox_2)
+        self.account_radio.setObjectName(u"account_radio")
+        self.account_radio.setGeometry(QRect(10, 10, 81, 22))
+        self.account_radio.setChecked(True)
+        self.path_radio = QRadioButton(self.groupBox_2)
+        self.path_radio.setObjectName(u"path_radio")
+        self.path_radio.setGeometry(QRect(10, 50, 61, 22))
+        self.path_lineedit = QLineEdit(self.groupBox_2)
+        self.path_lineedit.setObjectName(u"path_lineedit")
+        self.path_lineedit.setEnabled(False)
+        self.path_lineedit.setGeometry(QRect(80, 50, 141, 32))
+
+        self.retranslateUi(GetKeypoolOptionsDialog)
+        self.buttonBox.accepted.connect(GetKeypoolOptionsDialog.accept)
+        self.buttonBox.rejected.connect(GetKeypoolOptionsDialog.reject)
+
+        QMetaObject.connectSlotsByName(GetKeypoolOptionsDialog)
+    # setupUi
+
+    def retranslateUi(self, GetKeypoolOptionsDialog):
+        GetKeypoolOptionsDialog.setWindowTitle(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Dialog", None))
+        self.label.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Start", None))
+        self.label_2.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"End", None))
+        self.internal_checkbox.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Internal", None))
+        self.keypool_checkbox.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"keypool", None))
+        self.groupBox.setTitle("")
+        self.sh_wpkh_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"P2SH-P2WPKH", None))
+        self.wpkh_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"P2WPKH", None))
+        self.pkh_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"P2PKH", None))
+        self.groupBox_2.setTitle("")
+        self.account_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Account", None))
+        self.path_radio.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"Path", None))
+        self.path_lineedit.setText(QCoreApplication.translate("GetKeypoolOptionsDialog", u"m/0'/0'/*", None))
+    # retranslateUi
+
```

### Comparing `hwi-3.0.0/hwilib/ui/ui_getxpubdialog.py` & `hwi-3.0.0rc1/hwilib/ui/ui_getxpubdialog.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'getxpubdialog.ui'
-##
-## Created by: Qt User Interface Compiler version 5.15.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
-
-
-class Ui_GetXpubDialog(object):
-    def setupUi(self, GetXpubDialog):
-        if not GetXpubDialog.objectName():
-            GetXpubDialog.setObjectName(u"GetXpubDialog")
-        GetXpubDialog.resize(1050, 125)
-        self.gridLayout = QGridLayout(GetXpubDialog)
-        self.gridLayout.setSpacing(10)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.gridLayout.setContentsMargins(10, 10, 10, 10)
-        self.buttonBox = QDialogButtonBox(GetXpubDialog)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setMaximumSize(QSize(200, 16777215))
-        self.buttonBox.setFocusPolicy(Qt.NoFocus)
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Close)
-
-        self.gridLayout.addWidget(self.buttonBox, 2, 2, 1, 1)
-
-        self.path_label = QLabel(GetXpubDialog)
-        self.path_label.setObjectName(u"path_label")
-
-        self.gridLayout.addWidget(self.path_label, 0, 0, 1, 1)
-
-        self.xpub_textedit = QTextEdit(GetXpubDialog)
-        self.xpub_textedit.setObjectName(u"xpub_textedit")
-        self.xpub_textedit.setMinimumSize(QSize(0, 30))
-        self.xpub_textedit.setMaximumSize(QSize(16777215, 30))
-        self.xpub_textedit.setLineWrapMode(QTextEdit.NoWrap)
-        self.xpub_textedit.setReadOnly(True)
-
-        self.gridLayout.addWidget(self.xpub_textedit, 1, 1, 1, 2)
-
-        self.path_lineedit = QLineEdit(GetXpubDialog)
-        self.path_lineedit.setObjectName(u"path_lineedit")
-        self.path_lineedit.setMinimumSize(QSize(200, 30))
-
-        self.gridLayout.addWidget(self.path_lineedit, 0, 1, 1, 1)
-
-        self.getxpub_button = QPushButton(GetXpubDialog)
-        self.getxpub_button.setObjectName(u"getxpub_button")
-        self.getxpub_button.setMaximumSize(QSize(200, 16777215))
-
-        self.gridLayout.addWidget(self.getxpub_button, 0, 2, 1, 1)
-
-        self.xpub_label = QLabel(GetXpubDialog)
-        self.xpub_label.setObjectName(u"xpub_label")
-        self.xpub_label.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.xpub_label, 1, 0, 1, 1)
-
-
-        self.retranslateUi(GetXpubDialog)
-
-        QMetaObject.connectSlotsByName(GetXpubDialog)
-    # setupUi
-
-    def retranslateUi(self, GetXpubDialog):
-        GetXpubDialog.setWindowTitle(QCoreApplication.translate("GetXpubDialog", u"Dialog", None))
-        self.path_label.setText(QCoreApplication.translate("GetXpubDialog", u"Derivation Path", None))
-        self.getxpub_button.setText(QCoreApplication.translate("GetXpubDialog", u"Get xpub", None))
-        self.xpub_label.setText(QCoreApplication.translate("GetXpubDialog", u"xpub", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'getxpubdialog.ui'
+##
+## Created by: Qt User Interface Compiler version 5.15.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide2.QtCore import *
+from PySide2.QtGui import *
+from PySide2.QtWidgets import *
+
+
+class Ui_GetXpubDialog(object):
+    def setupUi(self, GetXpubDialog):
+        if not GetXpubDialog.objectName():
+            GetXpubDialog.setObjectName(u"GetXpubDialog")
+        GetXpubDialog.resize(1050, 125)
+        self.gridLayout = QGridLayout(GetXpubDialog)
+        self.gridLayout.setSpacing(10)
+        self.gridLayout.setObjectName(u"gridLayout")
+        self.gridLayout.setContentsMargins(10, 10, 10, 10)
+        self.buttonBox = QDialogButtonBox(GetXpubDialog)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setMaximumSize(QSize(200, 16777215))
+        self.buttonBox.setFocusPolicy(Qt.NoFocus)
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Close)
+
+        self.gridLayout.addWidget(self.buttonBox, 2, 2, 1, 1)
+
+        self.path_label = QLabel(GetXpubDialog)
+        self.path_label.setObjectName(u"path_label")
+
+        self.gridLayout.addWidget(self.path_label, 0, 0, 1, 1)
+
+        self.xpub_textedit = QTextEdit(GetXpubDialog)
+        self.xpub_textedit.setObjectName(u"xpub_textedit")
+        self.xpub_textedit.setMinimumSize(QSize(0, 30))
+        self.xpub_textedit.setMaximumSize(QSize(16777215, 30))
+        self.xpub_textedit.setLineWrapMode(QTextEdit.NoWrap)
+        self.xpub_textedit.setReadOnly(True)
+
+        self.gridLayout.addWidget(self.xpub_textedit, 1, 1, 1, 2)
+
+        self.path_lineedit = QLineEdit(GetXpubDialog)
+        self.path_lineedit.setObjectName(u"path_lineedit")
+        self.path_lineedit.setMinimumSize(QSize(200, 30))
+
+        self.gridLayout.addWidget(self.path_lineedit, 0, 1, 1, 1)
+
+        self.getxpub_button = QPushButton(GetXpubDialog)
+        self.getxpub_button.setObjectName(u"getxpub_button")
+        self.getxpub_button.setMaximumSize(QSize(200, 16777215))
+
+        self.gridLayout.addWidget(self.getxpub_button, 0, 2, 1, 1)
+
+        self.xpub_label = QLabel(GetXpubDialog)
+        self.xpub_label.setObjectName(u"xpub_label")
+        self.xpub_label.setAlignment(Qt.AlignCenter)
+
+        self.gridLayout.addWidget(self.xpub_label, 1, 0, 1, 1)
+
+
+        self.retranslateUi(GetXpubDialog)
+
+        QMetaObject.connectSlotsByName(GetXpubDialog)
+    # setupUi
+
+    def retranslateUi(self, GetXpubDialog):
+        GetXpubDialog.setWindowTitle(QCoreApplication.translate("GetXpubDialog", u"Dialog", None))
+        self.path_label.setText(QCoreApplication.translate("GetXpubDialog", u"Derivation Path", None))
+        self.getxpub_button.setText(QCoreApplication.translate("GetXpubDialog", u"Get xpub", None))
+        self.xpub_label.setText(QCoreApplication.translate("GetXpubDialog", u"xpub", None))
+    # retranslateUi
+
```

### Comparing `hwi-3.0.0/hwilib/ui/ui_mainwindow.py` & `hwi-3.0.0rc1/hwilib/ui/ui_mainwindow.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'mainwindow.ui'
-##
-## Created by: Qt User Interface Compiler version 5.15.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
-
-
-class Ui_MainWindow(object):
-    def setupUi(self, MainWindow):
-        if not MainWindow.objectName():
-            MainWindow.setObjectName(u"MainWindow")
-        MainWindow.resize(650, 400)
-        self.centralwidget = QWidget(MainWindow)
-        self.centralwidget.setObjectName(u"centralwidget")
-        self.verticalLayout = QVBoxLayout(self.centralwidget)
-        self.verticalLayout.setObjectName(u"verticalLayout")
-        self.horizontalLayout = QHBoxLayout()
-        self.horizontalLayout.setObjectName(u"horizontalLayout")
-        self.label = QLabel(self.centralwidget)
-        self.label.setObjectName(u"label")
-        sizePolicy = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.label.sizePolicy().hasHeightForWidth())
-        self.label.setSizePolicy(sizePolicy)
-        self.label.setMinimumSize(QSize(130, 20))
-        self.label.setMaximumSize(QSize(200, 20))
-        self.label.setAlignment(Qt.AlignRight|Qt.AlignTrailing|Qt.AlignVCenter)
-
-        self.horizontalLayout.addWidget(self.label)
-
-        self.enumerate_combobox = QComboBox(self.centralwidget)
-        self.enumerate_combobox.setObjectName(u"enumerate_combobox")
-        sizePolicy1 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Fixed)
-        sizePolicy1.setHorizontalStretch(0)
-        sizePolicy1.setVerticalStretch(0)
-        sizePolicy1.setHeightForWidth(self.enumerate_combobox.sizePolicy().hasHeightForWidth())
-        self.enumerate_combobox.setSizePolicy(sizePolicy1)
-        self.enumerate_combobox.setMinimumSize(QSize(0, 0))
-
-        self.horizontalLayout.addWidget(self.enumerate_combobox)
-
-        self.enumerate_refresh_button = QPushButton(self.centralwidget)
-        self.enumerate_refresh_button.setObjectName(u"enumerate_refresh_button")
-        sizePolicy2 = QSizePolicy(QSizePolicy.Maximum, QSizePolicy.Fixed)
-        sizePolicy2.setHorizontalStretch(0)
-        sizePolicy2.setVerticalStretch(0)
-        sizePolicy2.setHeightForWidth(self.enumerate_refresh_button.sizePolicy().hasHeightForWidth())
-        self.enumerate_refresh_button.setSizePolicy(sizePolicy2)
-        self.enumerate_refresh_button.setMaximumSize(QSize(100, 30))
-
-        self.horizontalLayout.addWidget(self.enumerate_refresh_button)
-
-
-        self.verticalLayout.addLayout(self.horizontalLayout)
-
-        self.line = QFrame(self.centralwidget)
-        self.line.setObjectName(u"line")
-        self.line.setFrameShape(QFrame.HLine)
-        self.line.setFrameShadow(QFrame.Sunken)
-
-        self.verticalLayout.addWidget(self.line)
-
-        self.gridLayout = QGridLayout()
-        self.gridLayout.setSpacing(10)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.gridLayout.setContentsMargins(10, 10, 10, 10)
-        self.setpass_button = QPushButton(self.centralwidget)
-        self.setpass_button.setObjectName(u"setpass_button")
-
-        self.gridLayout.addWidget(self.setpass_button, 2, 0, 1, 1)
-
-        self.getxpub_button = QPushButton(self.centralwidget)
-        self.getxpub_button.setObjectName(u"getxpub_button")
-        self.getxpub_button.setEnabled(False)
-
-        self.gridLayout.addWidget(self.getxpub_button, 3, 0, 1, 1)
-
-        self.signmsg_button = QPushButton(self.centralwidget)
-        self.signmsg_button.setObjectName(u"signmsg_button")
-        self.signmsg_button.setEnabled(False)
-
-        self.gridLayout.addWidget(self.signmsg_button, 3, 2, 1, 1)
-
-        self.signtx_button = QPushButton(self.centralwidget)
-        self.signtx_button.setObjectName(u"signtx_button")
-        self.signtx_button.setEnabled(False)
-
-        self.gridLayout.addWidget(self.signtx_button, 3, 1, 1, 1)
-
-        self.getkeypool_opts_button = QPushButton(self.centralwidget)
-        self.getkeypool_opts_button.setObjectName(u"getkeypool_opts_button")
-        self.getkeypool_opts_button.setEnabled(False)
-
-        self.gridLayout.addWidget(self.getkeypool_opts_button, 2, 2, 1, 1)
-
-        self.sendpin_button = QPushButton(self.centralwidget)
-        self.sendpin_button.setObjectName(u"sendpin_button")
-        self.sendpin_button.setEnabled(False)
-
-        self.gridLayout.addWidget(self.sendpin_button, 2, 1, 1, 1)
-
-        self.toggle_passphrase_button = QPushButton(self.centralwidget)
-        self.toggle_passphrase_button.setObjectName(u"toggle_passphrase_button")
-        self.toggle_passphrase_button.setEnabled(False)
-
-        self.gridLayout.addWidget(self.toggle_passphrase_button, 4, 1, 1, 1)
-
-        self.display_addr_button = QPushButton(self.centralwidget)
-        self.display_addr_button.setObjectName(u"display_addr_button")
-        self.display_addr_button.setEnabled(False)
-
-        self.gridLayout.addWidget(self.display_addr_button, 4, 0, 1, 1)
-
-        self.actions_label = QLabel(self.centralwidget)
-        self.actions_label.setObjectName(u"actions_label")
-        self.actions_label.setEnabled(True)
-        sizePolicy3 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
-        sizePolicy3.setHorizontalStretch(0)
-        sizePolicy3.setVerticalStretch(0)
-        sizePolicy3.setHeightForWidth(self.actions_label.sizePolicy().hasHeightForWidth())
-        self.actions_label.setSizePolicy(sizePolicy3)
-        self.actions_label.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout.addWidget(self.actions_label, 1, 1, 1, 1)
-
-
-        self.verticalLayout.addLayout(self.gridLayout)
-
-        self.gridLayout_2 = QGridLayout()
-        self.gridLayout_2.setSpacing(10)
-        self.gridLayout_2.setObjectName(u"gridLayout_2")
-        self.gridLayout_2.setContentsMargins(10, 10, 10, 10)
-        self.keypool_label = QLabel(self.centralwidget)
-        self.keypool_label.setObjectName(u"keypool_label")
-        self.keypool_label.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout_2.addWidget(self.keypool_label, 0, 0, 1, 1)
-
-        self.keypool_textedit = QPlainTextEdit(self.centralwidget)
-        self.keypool_textedit.setObjectName(u"keypool_textedit")
-        self.keypool_textedit.setReadOnly(True)
-
-        self.gridLayout_2.addWidget(self.keypool_textedit, 0, 1, 1, 1)
-
-        self.desc_label = QLabel(self.centralwidget)
-        self.desc_label.setObjectName(u"desc_label")
-        self.desc_label.setAlignment(Qt.AlignCenter)
-
-        self.gridLayout_2.addWidget(self.desc_label, 1, 0, 1, 1)
-
-        self.desc_textedit = QPlainTextEdit(self.centralwidget)
-        self.desc_textedit.setObjectName(u"desc_textedit")
-        self.desc_textedit.setReadOnly(True)
-
-        self.gridLayout_2.addWidget(self.desc_textedit, 1, 1, 1, 1)
-
-
-        self.verticalLayout.addLayout(self.gridLayout_2)
-
-        MainWindow.setCentralWidget(self.centralwidget)
-
-        self.retranslateUi(MainWindow)
-
-        QMetaObject.connectSlotsByName(MainWindow)
-    # setupUi
-
-    def retranslateUi(self, MainWindow):
-        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
-        self.label.setText(QCoreApplication.translate("MainWindow", u"Connected devices", None))
-        self.enumerate_refresh_button.setText(QCoreApplication.translate("MainWindow", u"Refresh", None))
-        self.setpass_button.setText(QCoreApplication.translate("MainWindow", u"Set Passphrase", None))
-        self.getxpub_button.setText(QCoreApplication.translate("MainWindow", u"Get an xpub", None))
-        self.signmsg_button.setText(QCoreApplication.translate("MainWindow", u"Sign Message", None))
-        self.signtx_button.setText(QCoreApplication.translate("MainWindow", u"Sign PSBT", None))
-#if QT_CONFIG(tooltip)
-        self.getkeypool_opts_button.setToolTip(QCoreApplication.translate("MainWindow", u"Change the options used for getkeypool", None))
-#endif // QT_CONFIG(tooltip)
-        self.getkeypool_opts_button.setText(QCoreApplication.translate("MainWindow", u"Change getkeypool options", None))
-        self.sendpin_button.setText(QCoreApplication.translate("MainWindow", u"Send Pin", None))
-        self.toggle_passphrase_button.setText(QCoreApplication.translate("MainWindow", u"Toggle Passphrase", None))
-        self.display_addr_button.setText(QCoreApplication.translate("MainWindow", u"Display Address", None))
-        self.actions_label.setText(QCoreApplication.translate("MainWindow", u"Actions", None))
-        self.keypool_label.setText(QCoreApplication.translate("MainWindow", u"Keypool", None))
-        self.desc_label.setText(QCoreApplication.translate("MainWindow", u"Descriptors", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'mainwindow.ui'
+##
+## Created by: Qt User Interface Compiler version 5.15.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide2.QtCore import *
+from PySide2.QtGui import *
+from PySide2.QtWidgets import *
+
+
+class Ui_MainWindow(object):
+    def setupUi(self, MainWindow):
+        if not MainWindow.objectName():
+            MainWindow.setObjectName(u"MainWindow")
+        MainWindow.resize(650, 400)
+        self.centralwidget = QWidget(MainWindow)
+        self.centralwidget.setObjectName(u"centralwidget")
+        self.verticalLayout = QVBoxLayout(self.centralwidget)
+        self.verticalLayout.setObjectName(u"verticalLayout")
+        self.horizontalLayout = QHBoxLayout()
+        self.horizontalLayout.setObjectName(u"horizontalLayout")
+        self.label = QLabel(self.centralwidget)
+        self.label.setObjectName(u"label")
+        sizePolicy = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Preferred)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(0)
+        sizePolicy.setHeightForWidth(self.label.sizePolicy().hasHeightForWidth())
+        self.label.setSizePolicy(sizePolicy)
+        self.label.setMinimumSize(QSize(130, 20))
+        self.label.setMaximumSize(QSize(200, 20))
+        self.label.setAlignment(Qt.AlignRight|Qt.AlignTrailing|Qt.AlignVCenter)
+
+        self.horizontalLayout.addWidget(self.label)
+
+        self.enumerate_combobox = QComboBox(self.centralwidget)
+        self.enumerate_combobox.setObjectName(u"enumerate_combobox")
+        sizePolicy1 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Fixed)
+        sizePolicy1.setHorizontalStretch(0)
+        sizePolicy1.setVerticalStretch(0)
+        sizePolicy1.setHeightForWidth(self.enumerate_combobox.sizePolicy().hasHeightForWidth())
+        self.enumerate_combobox.setSizePolicy(sizePolicy1)
+        self.enumerate_combobox.setMinimumSize(QSize(0, 0))
+
+        self.horizontalLayout.addWidget(self.enumerate_combobox)
+
+        self.enumerate_refresh_button = QPushButton(self.centralwidget)
+        self.enumerate_refresh_button.setObjectName(u"enumerate_refresh_button")
+        sizePolicy2 = QSizePolicy(QSizePolicy.Maximum, QSizePolicy.Fixed)
+        sizePolicy2.setHorizontalStretch(0)
+        sizePolicy2.setVerticalStretch(0)
+        sizePolicy2.setHeightForWidth(self.enumerate_refresh_button.sizePolicy().hasHeightForWidth())
+        self.enumerate_refresh_button.setSizePolicy(sizePolicy2)
+        self.enumerate_refresh_button.setMaximumSize(QSize(100, 30))
+
+        self.horizontalLayout.addWidget(self.enumerate_refresh_button)
+
+
+        self.verticalLayout.addLayout(self.horizontalLayout)
+
+        self.line = QFrame(self.centralwidget)
+        self.line.setObjectName(u"line")
+        self.line.setFrameShape(QFrame.HLine)
+        self.line.setFrameShadow(QFrame.Sunken)
+
+        self.verticalLayout.addWidget(self.line)
+
+        self.gridLayout = QGridLayout()
+        self.gridLayout.setSpacing(10)
+        self.gridLayout.setObjectName(u"gridLayout")
+        self.gridLayout.setContentsMargins(10, 10, 10, 10)
+        self.setpass_button = QPushButton(self.centralwidget)
+        self.setpass_button.setObjectName(u"setpass_button")
+
+        self.gridLayout.addWidget(self.setpass_button, 2, 0, 1, 1)
+
+        self.getxpub_button = QPushButton(self.centralwidget)
+        self.getxpub_button.setObjectName(u"getxpub_button")
+        self.getxpub_button.setEnabled(False)
+
+        self.gridLayout.addWidget(self.getxpub_button, 3, 0, 1, 1)
+
+        self.signmsg_button = QPushButton(self.centralwidget)
+        self.signmsg_button.setObjectName(u"signmsg_button")
+        self.signmsg_button.setEnabled(False)
+
+        self.gridLayout.addWidget(self.signmsg_button, 3, 2, 1, 1)
+
+        self.signtx_button = QPushButton(self.centralwidget)
+        self.signtx_button.setObjectName(u"signtx_button")
+        self.signtx_button.setEnabled(False)
+
+        self.gridLayout.addWidget(self.signtx_button, 3, 1, 1, 1)
+
+        self.getkeypool_opts_button = QPushButton(self.centralwidget)
+        self.getkeypool_opts_button.setObjectName(u"getkeypool_opts_button")
+        self.getkeypool_opts_button.setEnabled(False)
+
+        self.gridLayout.addWidget(self.getkeypool_opts_button, 2, 2, 1, 1)
+
+        self.sendpin_button = QPushButton(self.centralwidget)
+        self.sendpin_button.setObjectName(u"sendpin_button")
+        self.sendpin_button.setEnabled(False)
+
+        self.gridLayout.addWidget(self.sendpin_button, 2, 1, 1, 1)
+
+        self.toggle_passphrase_button = QPushButton(self.centralwidget)
+        self.toggle_passphrase_button.setObjectName(u"toggle_passphrase_button")
+        self.toggle_passphrase_button.setEnabled(False)
+
+        self.gridLayout.addWidget(self.toggle_passphrase_button, 4, 1, 1, 1)
+
+        self.display_addr_button = QPushButton(self.centralwidget)
+        self.display_addr_button.setObjectName(u"display_addr_button")
+        self.display_addr_button.setEnabled(False)
+
+        self.gridLayout.addWidget(self.display_addr_button, 4, 0, 1, 1)
+
+        self.actions_label = QLabel(self.centralwidget)
+        self.actions_label.setObjectName(u"actions_label")
+        self.actions_label.setEnabled(True)
+        sizePolicy3 = QSizePolicy(QSizePolicy.Preferred, QSizePolicy.Maximum)
+        sizePolicy3.setHorizontalStretch(0)
+        sizePolicy3.setVerticalStretch(0)
+        sizePolicy3.setHeightForWidth(self.actions_label.sizePolicy().hasHeightForWidth())
+        self.actions_label.setSizePolicy(sizePolicy3)
+        self.actions_label.setAlignment(Qt.AlignCenter)
+
+        self.gridLayout.addWidget(self.actions_label, 1, 1, 1, 1)
+
+
+        self.verticalLayout.addLayout(self.gridLayout)
+
+        self.gridLayout_2 = QGridLayout()
+        self.gridLayout_2.setSpacing(10)
+        self.gridLayout_2.setObjectName(u"gridLayout_2")
+        self.gridLayout_2.setContentsMargins(10, 10, 10, 10)
+        self.keypool_label = QLabel(self.centralwidget)
+        self.keypool_label.setObjectName(u"keypool_label")
+        self.keypool_label.setAlignment(Qt.AlignCenter)
+
+        self.gridLayout_2.addWidget(self.keypool_label, 0, 0, 1, 1)
+
+        self.keypool_textedit = QPlainTextEdit(self.centralwidget)
+        self.keypool_textedit.setObjectName(u"keypool_textedit")
+        self.keypool_textedit.setReadOnly(True)
+
+        self.gridLayout_2.addWidget(self.keypool_textedit, 0, 1, 1, 1)
+
+        self.desc_label = QLabel(self.centralwidget)
+        self.desc_label.setObjectName(u"desc_label")
+        self.desc_label.setAlignment(Qt.AlignCenter)
+
+        self.gridLayout_2.addWidget(self.desc_label, 1, 0, 1, 1)
+
+        self.desc_textedit = QPlainTextEdit(self.centralwidget)
+        self.desc_textedit.setObjectName(u"desc_textedit")
+        self.desc_textedit.setReadOnly(True)
+
+        self.gridLayout_2.addWidget(self.desc_textedit, 1, 1, 1, 1)
+
+
+        self.verticalLayout.addLayout(self.gridLayout_2)
+
+        MainWindow.setCentralWidget(self.centralwidget)
+
+        self.retranslateUi(MainWindow)
+
+        QMetaObject.connectSlotsByName(MainWindow)
+    # setupUi
+
+    def retranslateUi(self, MainWindow):
+        MainWindow.setWindowTitle(QCoreApplication.translate("MainWindow", u"MainWindow", None))
+        self.label.setText(QCoreApplication.translate("MainWindow", u"Connected devices", None))
+        self.enumerate_refresh_button.setText(QCoreApplication.translate("MainWindow", u"Refresh", None))
+        self.setpass_button.setText(QCoreApplication.translate("MainWindow", u"Set Passphrase", None))
+        self.getxpub_button.setText(QCoreApplication.translate("MainWindow", u"Get an xpub", None))
+        self.signmsg_button.setText(QCoreApplication.translate("MainWindow", u"Sign Message", None))
+        self.signtx_button.setText(QCoreApplication.translate("MainWindow", u"Sign PSBT", None))
+#if QT_CONFIG(tooltip)
+        self.getkeypool_opts_button.setToolTip(QCoreApplication.translate("MainWindow", u"Change the options used for getkeypool", None))
+#endif // QT_CONFIG(tooltip)
+        self.getkeypool_opts_button.setText(QCoreApplication.translate("MainWindow", u"Change getkeypool options", None))
+        self.sendpin_button.setText(QCoreApplication.translate("MainWindow", u"Send Pin", None))
+        self.toggle_passphrase_button.setText(QCoreApplication.translate("MainWindow", u"Toggle Passphrase", None))
+        self.display_addr_button.setText(QCoreApplication.translate("MainWindow", u"Display Address", None))
+        self.actions_label.setText(QCoreApplication.translate("MainWindow", u"Actions", None))
+        self.keypool_label.setText(QCoreApplication.translate("MainWindow", u"Keypool", None))
+        self.desc_label.setText(QCoreApplication.translate("MainWindow", u"Descriptors", None))
+    # retranslateUi
+
```

### Comparing `hwi-3.0.0/hwilib/ui/ui_sendpindialog.py` & `hwi-3.0.0rc1/hwilib/ui/ui_sendpindialog.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'sendpindialog.ui'
-##
-## Created by: Qt User Interface Compiler version 5.15.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
-
-
-class Ui_SendPinDialog(object):
-    def setupUi(self, SendPinDialog):
-        if not SendPinDialog.objectName():
-            SendPinDialog.setObjectName(u"SendPinDialog")
-        SendPinDialog.resize(250, 250)
-        self.verticalLayout = QVBoxLayout(SendPinDialog)
-        self.verticalLayout.setSpacing(10)
-        self.verticalLayout.setObjectName(u"verticalLayout")
-        self.verticalLayout.setContentsMargins(10, 10, 10, 10)
-        self.pin_lineedit = QLineEdit(SendPinDialog)
-        self.pin_lineedit.setObjectName(u"pin_lineedit")
-        sizePolicy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Fixed)
-        sizePolicy.setHorizontalStretch(0)
-        sizePolicy.setVerticalStretch(30)
-        sizePolicy.setHeightForWidth(self.pin_lineedit.sizePolicy().hasHeightForWidth())
-        self.pin_lineedit.setSizePolicy(sizePolicy)
-        self.pin_lineedit.setMinimumSize(QSize(0, 30))
-        self.pin_lineedit.setReadOnly(False)
-
-        self.verticalLayout.addWidget(self.pin_lineedit)
-
-        self.gridLayout = QGridLayout()
-        self.gridLayout.setSpacing(20)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.gridLayout.setContentsMargins(5, 5, 5, 0)
-        self.p7_button = QPushButton(SendPinDialog)
-        self.p7_button.setObjectName(u"p7_button")
-
-        self.gridLayout.addWidget(self.p7_button, 0, 0, 1, 1)
-
-        self.p1_button = QPushButton(SendPinDialog)
-        self.p1_button.setObjectName(u"p1_button")
-
-        self.gridLayout.addWidget(self.p1_button, 2, 0, 1, 1)
-
-        self.p4_button = QPushButton(SendPinDialog)
-        self.p4_button.setObjectName(u"p4_button")
-
-        self.gridLayout.addWidget(self.p4_button, 1, 0, 1, 1)
-
-        self.p9_button = QPushButton(SendPinDialog)
-        self.p9_button.setObjectName(u"p9_button")
-
-        self.gridLayout.addWidget(self.p9_button, 0, 2, 1, 1)
-
-        self.p3_button = QPushButton(SendPinDialog)
-        self.p3_button.setObjectName(u"p3_button")
-
-        self.gridLayout.addWidget(self.p3_button, 2, 2, 1, 1)
-
-        self.p6_button = QPushButton(SendPinDialog)
-        self.p6_button.setObjectName(u"p6_button")
-
-        self.gridLayout.addWidget(self.p6_button, 1, 2, 1, 1)
-
-        self.p2_button = QPushButton(SendPinDialog)
-        self.p2_button.setObjectName(u"p2_button")
-
-        self.gridLayout.addWidget(self.p2_button, 2, 1, 1, 1)
-
-        self.p5_button = QPushButton(SendPinDialog)
-        self.p5_button.setObjectName(u"p5_button")
-
-        self.gridLayout.addWidget(self.p5_button, 1, 1, 1, 1)
-
-        self.p8_button = QPushButton(SendPinDialog)
-        self.p8_button.setObjectName(u"p8_button")
-
-        self.gridLayout.addWidget(self.p8_button, 0, 1, 1, 1)
-
-
-        self.verticalLayout.addLayout(self.gridLayout)
-
-        self.buttonBox = QDialogButtonBox(SendPinDialog)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
-
-        self.verticalLayout.addWidget(self.buttonBox)
-
-
-        self.retranslateUi(SendPinDialog)
-        self.buttonBox.accepted.connect(SendPinDialog.accept)
-        self.buttonBox.rejected.connect(SendPinDialog.reject)
-
-        QMetaObject.connectSlotsByName(SendPinDialog)
-    # setupUi
-
-    def retranslateUi(self, SendPinDialog):
-        SendPinDialog.setWindowTitle(QCoreApplication.translate("SendPinDialog", u"Dialog", None))
-        self.p7_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-        self.p1_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-        self.p4_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-        self.p9_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-        self.p3_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-        self.p6_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-        self.p2_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-        self.p5_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-        self.p8_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'sendpindialog.ui'
+##
+## Created by: Qt User Interface Compiler version 5.15.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide2.QtCore import *
+from PySide2.QtGui import *
+from PySide2.QtWidgets import *
+
+
+class Ui_SendPinDialog(object):
+    def setupUi(self, SendPinDialog):
+        if not SendPinDialog.objectName():
+            SendPinDialog.setObjectName(u"SendPinDialog")
+        SendPinDialog.resize(250, 250)
+        self.verticalLayout = QVBoxLayout(SendPinDialog)
+        self.verticalLayout.setSpacing(10)
+        self.verticalLayout.setObjectName(u"verticalLayout")
+        self.verticalLayout.setContentsMargins(10, 10, 10, 10)
+        self.pin_lineedit = QLineEdit(SendPinDialog)
+        self.pin_lineedit.setObjectName(u"pin_lineedit")
+        sizePolicy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Fixed)
+        sizePolicy.setHorizontalStretch(0)
+        sizePolicy.setVerticalStretch(30)
+        sizePolicy.setHeightForWidth(self.pin_lineedit.sizePolicy().hasHeightForWidth())
+        self.pin_lineedit.setSizePolicy(sizePolicy)
+        self.pin_lineedit.setMinimumSize(QSize(0, 30))
+        self.pin_lineedit.setReadOnly(False)
+
+        self.verticalLayout.addWidget(self.pin_lineedit)
+
+        self.gridLayout = QGridLayout()
+        self.gridLayout.setSpacing(20)
+        self.gridLayout.setObjectName(u"gridLayout")
+        self.gridLayout.setContentsMargins(5, 5, 5, 0)
+        self.p7_button = QPushButton(SendPinDialog)
+        self.p7_button.setObjectName(u"p7_button")
+
+        self.gridLayout.addWidget(self.p7_button, 0, 0, 1, 1)
+
+        self.p1_button = QPushButton(SendPinDialog)
+        self.p1_button.setObjectName(u"p1_button")
+
+        self.gridLayout.addWidget(self.p1_button, 2, 0, 1, 1)
+
+        self.p4_button = QPushButton(SendPinDialog)
+        self.p4_button.setObjectName(u"p4_button")
+
+        self.gridLayout.addWidget(self.p4_button, 1, 0, 1, 1)
+
+        self.p9_button = QPushButton(SendPinDialog)
+        self.p9_button.setObjectName(u"p9_button")
+
+        self.gridLayout.addWidget(self.p9_button, 0, 2, 1, 1)
+
+        self.p3_button = QPushButton(SendPinDialog)
+        self.p3_button.setObjectName(u"p3_button")
+
+        self.gridLayout.addWidget(self.p3_button, 2, 2, 1, 1)
+
+        self.p6_button = QPushButton(SendPinDialog)
+        self.p6_button.setObjectName(u"p6_button")
+
+        self.gridLayout.addWidget(self.p6_button, 1, 2, 1, 1)
+
+        self.p2_button = QPushButton(SendPinDialog)
+        self.p2_button.setObjectName(u"p2_button")
+
+        self.gridLayout.addWidget(self.p2_button, 2, 1, 1, 1)
+
+        self.p5_button = QPushButton(SendPinDialog)
+        self.p5_button.setObjectName(u"p5_button")
+
+        self.gridLayout.addWidget(self.p5_button, 1, 1, 1, 1)
+
+        self.p8_button = QPushButton(SendPinDialog)
+        self.p8_button.setObjectName(u"p8_button")
+
+        self.gridLayout.addWidget(self.p8_button, 0, 1, 1, 1)
+
+
+        self.verticalLayout.addLayout(self.gridLayout)
+
+        self.buttonBox = QDialogButtonBox(SendPinDialog)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
+
+        self.verticalLayout.addWidget(self.buttonBox)
+
+
+        self.retranslateUi(SendPinDialog)
+        self.buttonBox.accepted.connect(SendPinDialog.accept)
+        self.buttonBox.rejected.connect(SendPinDialog.reject)
+
+        QMetaObject.connectSlotsByName(SendPinDialog)
+    # setupUi
+
+    def retranslateUi(self, SendPinDialog):
+        SendPinDialog.setWindowTitle(QCoreApplication.translate("SendPinDialog", u"Dialog", None))
+        self.p7_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+        self.p1_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+        self.p4_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+        self.p9_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+        self.p3_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+        self.p6_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+        self.p2_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+        self.p5_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+        self.p8_button.setText(QCoreApplication.translate("SendPinDialog", u"?", None))
+    # retranslateUi
+
```

### Comparing `hwi-3.0.0/hwilib/ui/ui_setpassphrasedialog.py` & `hwi-3.0.0rc1/hwilib/ui/ui_setpassphrasedialog.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'setpassphrasedialog.ui'
-##
-## Created by: Qt User Interface Compiler version 5.15.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
-
-
-class Ui_SetPassphraseDialog(object):
-    def setupUi(self, SetPassphraseDialog):
-        if not SetPassphraseDialog.objectName():
-            SetPassphraseDialog.setObjectName(u"SetPassphraseDialog")
-        SetPassphraseDialog.resize(400, 100)
-        self.verticalLayout_3 = QVBoxLayout(SetPassphraseDialog)
-        self.verticalLayout_3.setSpacing(10)
-        self.verticalLayout_3.setObjectName(u"verticalLayout_3")
-        self.verticalLayout_3.setContentsMargins(10, 10, 10, 10)
-        self.passphrase_lineedit = QLineEdit(SetPassphraseDialog)
-        self.passphrase_lineedit.setObjectName(u"passphrase_lineedit")
-        self.passphrase_lineedit.setMinimumSize(QSize(0, 30))
-        self.passphrase_lineedit.setClearButtonEnabled(False)
-
-        self.verticalLayout_3.addWidget(self.passphrase_lineedit)
-
-        self.buttonBox = QDialogButtonBox(SetPassphraseDialog)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
-
-        self.verticalLayout_3.addWidget(self.buttonBox)
-
-
-        self.retranslateUi(SetPassphraseDialog)
-        self.buttonBox.accepted.connect(SetPassphraseDialog.accept)
-        self.buttonBox.rejected.connect(SetPassphraseDialog.reject)
-
-        QMetaObject.connectSlotsByName(SetPassphraseDialog)
-    # setupUi
-
-    def retranslateUi(self, SetPassphraseDialog):
-        SetPassphraseDialog.setWindowTitle(QCoreApplication.translate("SetPassphraseDialog", u"Dialog", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'setpassphrasedialog.ui'
+##
+## Created by: Qt User Interface Compiler version 5.15.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide2.QtCore import *
+from PySide2.QtGui import *
+from PySide2.QtWidgets import *
+
+
+class Ui_SetPassphraseDialog(object):
+    def setupUi(self, SetPassphraseDialog):
+        if not SetPassphraseDialog.objectName():
+            SetPassphraseDialog.setObjectName(u"SetPassphraseDialog")
+        SetPassphraseDialog.resize(400, 100)
+        self.verticalLayout_3 = QVBoxLayout(SetPassphraseDialog)
+        self.verticalLayout_3.setSpacing(10)
+        self.verticalLayout_3.setObjectName(u"verticalLayout_3")
+        self.verticalLayout_3.setContentsMargins(10, 10, 10, 10)
+        self.passphrase_lineedit = QLineEdit(SetPassphraseDialog)
+        self.passphrase_lineedit.setObjectName(u"passphrase_lineedit")
+        self.passphrase_lineedit.setMinimumSize(QSize(0, 30))
+        self.passphrase_lineedit.setClearButtonEnabled(False)
+
+        self.verticalLayout_3.addWidget(self.passphrase_lineedit)
+
+        self.buttonBox = QDialogButtonBox(SetPassphraseDialog)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Cancel|QDialogButtonBox.Ok)
+
+        self.verticalLayout_3.addWidget(self.buttonBox)
+
+
+        self.retranslateUi(SetPassphraseDialog)
+        self.buttonBox.accepted.connect(SetPassphraseDialog.accept)
+        self.buttonBox.rejected.connect(SetPassphraseDialog.reject)
+
+        QMetaObject.connectSlotsByName(SetPassphraseDialog)
+    # setupUi
+
+    def retranslateUi(self, SetPassphraseDialog):
+        SetPassphraseDialog.setWindowTitle(QCoreApplication.translate("SetPassphraseDialog", u"Dialog", None))
+    # retranslateUi
+
```

### Comparing `hwi-3.0.0/hwilib/ui/ui_signpsbtdialog.py` & `hwi-3.0.0rc1/hwilib/ui/ui_signpsbtdialog.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-# -*- coding: utf-8 -*-
-
-################################################################################
-## Form generated from reading UI file 'signpsbtdialog.ui'
-##
-## Created by: Qt User Interface Compiler version 5.15.2
-##
-## WARNING! All changes made in this file will be lost when recompiling UI file!
-################################################################################
-
-from PySide2.QtCore import *
-from PySide2.QtGui import *
-from PySide2.QtWidgets import *
-
-
-class Ui_SignPSBTDialog(object):
-    def setupUi(self, SignPSBTDialog):
-        if not SignPSBTDialog.objectName():
-            SignPSBTDialog.setObjectName(u"SignPSBTDialog")
-        SignPSBTDialog.resize(650, 400)
-        self.gridLayout = QGridLayout(SignPSBTDialog)
-        self.gridLayout.setSpacing(10)
-        self.gridLayout.setObjectName(u"gridLayout")
-        self.gridLayout.setContentsMargins(10, 10, 10, 10)
-        self.verticalLayout_2 = QVBoxLayout()
-        self.verticalLayout_2.setObjectName(u"verticalLayout_2")
-        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.verticalLayout_2.addItem(self.verticalSpacer_2)
-
-        self.label = QLabel(SignPSBTDialog)
-        self.label.setObjectName(u"label")
-        self.label.setWordWrap(True)
-
-        self.verticalLayout_2.addWidget(self.label)
-
-        self.import_toolbutton = QToolButton(SignPSBTDialog)
-        self.import_toolbutton.setObjectName(u"import_toolbutton")
-        self.import_toolbutton.setPopupMode(QToolButton.InstantPopup)
-
-        self.verticalLayout_2.addWidget(self.import_toolbutton)
-
-        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.verticalLayout_2.addItem(self.verticalSpacer)
-
-
-        self.gridLayout.addLayout(self.verticalLayout_2, 1, 0, 1, 1)
-
-        self.psbt_in_textedit = QPlainTextEdit(SignPSBTDialog)
-        self.psbt_in_textedit.setObjectName(u"psbt_in_textedit")
-        self.psbt_in_textedit.setMinimumSize(QSize(300, 120))
-
-        self.gridLayout.addWidget(self.psbt_in_textedit, 1, 2, 1, 1)
-
-        self.buttonBox = QDialogButtonBox(SignPSBTDialog)
-        self.buttonBox.setObjectName(u"buttonBox")
-        self.buttonBox.setOrientation(Qt.Horizontal)
-        self.buttonBox.setStandardButtons(QDialogButtonBox.Close)
-
-        self.gridLayout.addWidget(self.buttonBox, 4, 2, 1, 1)
-
-        self.verticalLayout = QVBoxLayout()
-        self.verticalLayout.setObjectName(u"verticalLayout")
-        self.verticalSpacer_3 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.verticalLayout.addItem(self.verticalSpacer_3)
-
-        self.label_2 = QLabel(SignPSBTDialog)
-        self.label_2.setObjectName(u"label_2")
-        self.label_2.setWordWrap(True)
-
-        self.verticalLayout.addWidget(self.label_2)
-
-        self.export_toolbutton = QToolButton(SignPSBTDialog)
-        self.export_toolbutton.setObjectName(u"export_toolbutton")
-        self.export_toolbutton.setPopupMode(QToolButton.InstantPopup)
-
-        self.verticalLayout.addWidget(self.export_toolbutton)
-
-        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
-
-        self.verticalLayout.addItem(self.verticalSpacer_4)
-
-
-        self.gridLayout.addLayout(self.verticalLayout, 3, 0, 1, 1)
-
-        self.psbt_out_textedit = QPlainTextEdit(SignPSBTDialog)
-        self.psbt_out_textedit.setObjectName(u"psbt_out_textedit")
-        self.psbt_out_textedit.setMinimumSize(QSize(300, 120))
-        self.psbt_out_textedit.setTextInteractionFlags(Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
-
-        self.gridLayout.addWidget(self.psbt_out_textedit, 3, 2, 1, 1)
-
-        self.horizontalLayout = QHBoxLayout()
-        self.horizontalLayout.setObjectName(u"horizontalLayout")
-        self.horizontalSpacer = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
-
-        self.horizontalLayout.addItem(self.horizontalSpacer)
-
-        self.sign_psbt_button = QPushButton(SignPSBTDialog)
-        self.sign_psbt_button.setObjectName(u"sign_psbt_button")
-        self.sign_psbt_button.setAutoDefault(False)
-
-        self.horizontalLayout.addWidget(self.sign_psbt_button)
-
-        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
-
-        self.horizontalLayout.addItem(self.horizontalSpacer_2)
-
-
-        self.gridLayout.addLayout(self.horizontalLayout, 2, 2, 1, 1)
-
-
-        self.retranslateUi(SignPSBTDialog)
-        self.buttonBox.accepted.connect(SignPSBTDialog.accept)
-        self.buttonBox.rejected.connect(SignPSBTDialog.reject)
-
-        self.sign_psbt_button.setDefault(True)
-
-
-        QMetaObject.connectSlotsByName(SignPSBTDialog)
-    # setupUi
-
-    def retranslateUi(self, SignPSBTDialog):
-        SignPSBTDialog.setWindowTitle(QCoreApplication.translate("SignPSBTDialog", u"Dialog", None))
-        self.label.setText(QCoreApplication.translate("SignPSBTDialog", u"PSBT To Sign", None))
-        self.import_toolbutton.setText(QCoreApplication.translate("SignPSBTDialog", u"Import PSBT", None))
-        self.label_2.setText(QCoreApplication.translate("SignPSBTDialog", u"PSBT Result", None))
-        self.export_toolbutton.setText(QCoreApplication.translate("SignPSBTDialog", u"Export PSBT", None))
-        self.sign_psbt_button.setText(QCoreApplication.translate("SignPSBTDialog", u"Sign PSBT", None))
-    # retranslateUi
-
+# -*- coding: utf-8 -*-
+
+################################################################################
+## Form generated from reading UI file 'signpsbtdialog.ui'
+##
+## Created by: Qt User Interface Compiler version 5.15.2
+##
+## WARNING! All changes made in this file will be lost when recompiling UI file!
+################################################################################
+
+from PySide2.QtCore import *
+from PySide2.QtGui import *
+from PySide2.QtWidgets import *
+
+
+class Ui_SignPSBTDialog(object):
+    def setupUi(self, SignPSBTDialog):
+        if not SignPSBTDialog.objectName():
+            SignPSBTDialog.setObjectName(u"SignPSBTDialog")
+        SignPSBTDialog.resize(650, 400)
+        self.gridLayout = QGridLayout(SignPSBTDialog)
+        self.gridLayout.setSpacing(10)
+        self.gridLayout.setObjectName(u"gridLayout")
+        self.gridLayout.setContentsMargins(10, 10, 10, 10)
+        self.verticalLayout_2 = QVBoxLayout()
+        self.verticalLayout_2.setObjectName(u"verticalLayout_2")
+        self.verticalSpacer_2 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+
+        self.verticalLayout_2.addItem(self.verticalSpacer_2)
+
+        self.label = QLabel(SignPSBTDialog)
+        self.label.setObjectName(u"label")
+        self.label.setWordWrap(True)
+
+        self.verticalLayout_2.addWidget(self.label)
+
+        self.import_toolbutton = QToolButton(SignPSBTDialog)
+        self.import_toolbutton.setObjectName(u"import_toolbutton")
+        self.import_toolbutton.setPopupMode(QToolButton.InstantPopup)
+
+        self.verticalLayout_2.addWidget(self.import_toolbutton)
+
+        self.verticalSpacer = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+
+        self.verticalLayout_2.addItem(self.verticalSpacer)
+
+
+        self.gridLayout.addLayout(self.verticalLayout_2, 1, 0, 1, 1)
+
+        self.psbt_in_textedit = QPlainTextEdit(SignPSBTDialog)
+        self.psbt_in_textedit.setObjectName(u"psbt_in_textedit")
+        self.psbt_in_textedit.setMinimumSize(QSize(300, 120))
+
+        self.gridLayout.addWidget(self.psbt_in_textedit, 1, 2, 1, 1)
+
+        self.buttonBox = QDialogButtonBox(SignPSBTDialog)
+        self.buttonBox.setObjectName(u"buttonBox")
+        self.buttonBox.setOrientation(Qt.Horizontal)
+        self.buttonBox.setStandardButtons(QDialogButtonBox.Close)
+
+        self.gridLayout.addWidget(self.buttonBox, 4, 2, 1, 1)
+
+        self.verticalLayout = QVBoxLayout()
+        self.verticalLayout.setObjectName(u"verticalLayout")
+        self.verticalSpacer_3 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+
+        self.verticalLayout.addItem(self.verticalSpacer_3)
+
+        self.label_2 = QLabel(SignPSBTDialog)
+        self.label_2.setObjectName(u"label_2")
+        self.label_2.setWordWrap(True)
+
+        self.verticalLayout.addWidget(self.label_2)
+
+        self.export_toolbutton = QToolButton(SignPSBTDialog)
+        self.export_toolbutton.setObjectName(u"export_toolbutton")
+        self.export_toolbutton.setPopupMode(QToolButton.InstantPopup)
+
+        self.verticalLayout.addWidget(self.export_toolbutton)
+
+        self.verticalSpacer_4 = QSpacerItem(20, 40, QSizePolicy.Minimum, QSizePolicy.Expanding)
+
+        self.verticalLayout.addItem(self.verticalSpacer_4)
+
+
+        self.gridLayout.addLayout(self.verticalLayout, 3, 0, 1, 1)
+
+        self.psbt_out_textedit = QPlainTextEdit(SignPSBTDialog)
+        self.psbt_out_textedit.setObjectName(u"psbt_out_textedit")
+        self.psbt_out_textedit.setMinimumSize(QSize(300, 120))
+        self.psbt_out_textedit.setTextInteractionFlags(Qt.TextSelectableByKeyboard|Qt.TextSelectableByMouse)
+
+        self.gridLayout.addWidget(self.psbt_out_textedit, 3, 2, 1, 1)
+
+        self.horizontalLayout = QHBoxLayout()
+        self.horizontalLayout.setObjectName(u"horizontalLayout")
+        self.horizontalSpacer = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        self.horizontalLayout.addItem(self.horizontalSpacer)
+
+        self.sign_psbt_button = QPushButton(SignPSBTDialog)
+        self.sign_psbt_button.setObjectName(u"sign_psbt_button")
+        self.sign_psbt_button.setAutoDefault(False)
+
+        self.horizontalLayout.addWidget(self.sign_psbt_button)
+
+        self.horizontalSpacer_2 = QSpacerItem(40, 20, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        self.horizontalLayout.addItem(self.horizontalSpacer_2)
+
+
+        self.gridLayout.addLayout(self.horizontalLayout, 2, 2, 1, 1)
+
+
+        self.retranslateUi(SignPSBTDialog)
+        self.buttonBox.accepted.connect(SignPSBTDialog.accept)
+        self.buttonBox.rejected.connect(SignPSBTDialog.reject)
+
+        self.sign_psbt_button.setDefault(True)
+
+
+        QMetaObject.connectSlotsByName(SignPSBTDialog)
+    # setupUi
+
+    def retranslateUi(self, SignPSBTDialog):
+        SignPSBTDialog.setWindowTitle(QCoreApplication.translate("SignPSBTDialog", u"Dialog", None))
+        self.label.setText(QCoreApplication.translate("SignPSBTDialog", u"PSBT To Sign", None))
+        self.import_toolbutton.setText(QCoreApplication.translate("SignPSBTDialog", u"Import PSBT", None))
+        self.label_2.setText(QCoreApplication.translate("SignPSBTDialog", u"PSBT Result", None))
+        self.export_toolbutton.setText(QCoreApplication.translate("SignPSBTDialog", u"Export PSBT", None))
+        self.sign_psbt_button.setText(QCoreApplication.translate("SignPSBTDialog", u"Sign PSBT", None))
+    # retranslateUi
+
```

### Comparing `hwi-3.0.0/pyproject.toml` & `hwi-3.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hwi"
-version = "3.0.0"
+version = "3.0.0-rc.1"
 description = "A library for working with Bitcoin hardware wallets"
 authors = ["Ava Chow <me@achow101.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bitcoin-core/HWI"
 homepage = "https://github.com/bitcoin-core/HWI"
 exclude = ["docs/", "test/"]
```

### Comparing `hwi-3.0.0/setup.py` & `hwi-3.0.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
  'qt:python_version < "3.10"': ['pyside2>=5.14.0,<6.0.0']}
 
 entry_points = \
 {'console_scripts': ['hwi = hwilib._cli:main', 'hwi-qt = hwilib._gui:main']}
 
 setup_kwargs = {
     'name': 'hwi',
-    'version': '3.0.0',
+    'version': '3.0.0rc1',
     'description': 'A library for working with Bitcoin hardware wallets',
     'long_description': "# Bitcoin Hardware Wallet Interface\n\n[![Build Status](https://api.cirrus-ci.com/github/bitcoin-core/HWI.svg)](https://cirrus-ci.com/github/bitcoin-core/HWI)\n[![Documentation Status](https://readthedocs.org/projects/hwi/badge/?version=latest)](https://hwi.readthedocs.io/en/latest/?badge=latest)\n\nThe Bitcoin Hardware Wallet Interface is a Python library and command line tool for interacting with hardware wallets.\nIt provides a standard way for software to work with hardware wallets without needing to implement device specific drivers.\nPython software can use the provided library (`hwilib`). Software in other languages can execute the `hwi` tool.\n\nCaveat emptor: Inclusion of a specific hardware wallet vendor does not imply any endorsement of quality or security.\n\n## Prerequisites\n\nPython 3 is required. The libraries and [udev rules](hwilib/udev/README.md) for each device must also be installed. Some libraries will need to be installed\n\nFor Ubuntu/Debian:\n```\nsudo apt install libusb-1.0-0-dev libudev-dev python3-dev\n```\n\nFor Centos:\n```\nsudo yum -y install python3-devel libusbx-devel systemd-devel\n```\n\nFor macOS:\n```\nbrew install libusb\n```\n\n## Install\n\n```\ngit clone https://github.com/bitcoin-core/HWI.git\ncd HWI\npoetry install # or 'pip3 install .' or 'python3 setup.py install'\n```\n\nThis project uses the [Poetry](https://github.com/sdispater/poetry) dependency manager. HWI and its dependencies can be installed via poetry by executing the following in the root source directory:\n\n```\npoetry install\n```\n\nPip can also be used to automatically install HWI and its dependencies using the `setup.py` file (which is usually in sync with `pyproject.toml`):\n\n```\npip3 install .\n```\n\nThe `setup.py` file can be used to install HWI and its dependencies so long as `setuptools` is also installed:\n\n```\npip3 install -U setuptools\npython3 setup.py install\n```\n\n## Dependencies\n\nSee `pyproject.toml` for all dependencies. Dependencies under `[tool.poetry.dependencies]` are user dependencies, and `[tool.poetry.dev-dependencies]` for development based dependencies. These dependencies will be installed with any of the three above installation methods.\n\n## Usage\n\nTo use, first enumerate all devices and find the one that you want to use with\n\n```\n./hwi.py enumerate\n```\n\nOnce the device type and device path are known, issue commands to it like so:\n\n```\n./hwi.py -t <type> -d <path> <command> <command args>\n```\n\nAll output will be in JSON form and sent to `stdout`.\nAdditional information or prompts will be sent to `stderr` and will not necessarily be in JSON.\nThis additional information is for debugging purposes.\n\nTo see a complete list of available commands and global parameters, run\n`./hwi.py --help`.  To see options specific to a particular command,\npass the `--help` parameter after the command name; for example:\n\n```\n./hwi.py getdescriptors --help\n```\n\n## Documentation\n\nDocumentation for HWI can be found on [readthedocs.io](https://hwi.readthedocs.io/).\n\n### Device Support\n\nFor documentation on devices supported and how they are supported, please check the [device support page](https://hwi.readthedocs.io/en/latest/devices/index.html#support-matrix)\n\n### Using with Bitcoin Core\n\nSee [Using Bitcoin Core with Hardware Wallets](https://hwi.readthedocs.io/en/latest/examples/bitcoin-core-usage.html).\n\n## License\n\nThis project is available under the MIT License, Copyright Andrew Chow.\n",
     'author': 'Ava Chow',
     'author_email': 'me@achow101.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bitcoin-core/HWI',
```

### Comparing `hwi-3.0.0/PKG-INFO` & `hwi-3.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwi
-Version: 3.0.0
+Version: 3.0.0rc1
 Summary: A library for working with Bitcoin hardware wallets
 Home-page: https://github.com/bitcoin-core/HWI
 License: MIT
 Author: Ava Chow
 Author-email: me@achow101.com
 Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

