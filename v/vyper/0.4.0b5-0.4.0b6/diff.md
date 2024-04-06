# Comparing `tmp/vyper-0.4.0b5.tar.gz` & `tmp/vyper-0.4.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vyper-0.4.0b5.tar", last modified: Tue Mar 12 15:42:15 2024, max compression
+gzip compressed data, was "vyper-0.4.0b6.tar", last modified: Sat Apr  6 17:26:01 2024, max compression
```

## Comparing `vyper-0.4.0b5.tar` & `vyper-0.4.0b6.tar`

### file list

```diff
@@ -1,574 +1,585 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.398899 vyper-0.4.0b5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.334900 vyper-0.4.0b5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.334900 vyper-0.4.0b5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/ISSUE_TEMPLATE/vip.md
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.334900 vyper-0.4.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/workflows/era-tester.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/workflows/ghcr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-12 15:42:01.000000 vyper-0.4.0b5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-12 15:42:01.000000 vyper-0.4.0b5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-12 15:42:01.000000 vyper-0.4.0b5/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-03-12 15:42:01.000000 vyper-0.4.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-12 15:42:01.000000 vyper-0.4.0b5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-03-12 15:42:15.398899 vyper-0.4.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-03-12 15:42:01.000000 vyper-0.4.0b5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-03-12 15:42:01.000000 vyper-0.4.0b5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.338899 vyper-0.4.0b5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.338899 vyper-0.4.0b5/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (127)    37575 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/built-in-functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/compiler-exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/compiling-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/constants-and-vars.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/control-structures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/deploying-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/event-logging.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/installing-vyper.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/interfaces.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/natspec.rst
--rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/release-notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/scoping-and-declarations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/statements.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/structure-of-a-contract.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/style-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/testing-contracts-brownie.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/testing-contracts-ethtester.rst
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/testing-contracts.rst
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/toctree.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/types.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/versioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-03-12 15:42:01.000000 vyper-0.4.0b5/docs/vyper-by-example.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.338899 vyper-0.4.0b5/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.338899 vyper-0.4.0b5/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/auctions/blind_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/auctions/simple_open_auction.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/crowdfund.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.338899 vyper-0.4.0b5/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/factory/Exchange.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/factory/Factory.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/market_maker/on_chain_market_maker.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/name_registry/name_registry.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/safe_remote_purchase/safe_remote_purchase.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/examples/stock/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/stock/company.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/storage/advanced_storage.vy
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/storage/storage.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/tokens/ERC1155ownable.vy
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/tokens/ERC20.vy
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/tokens/ERC4626.vy
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/tokens/ERC721.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/voting/ballot.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-03-12 15:42:01.000000 vyper-0.4.0b5/examples/wallet/wallet.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-03-12 15:42:01.000000 vyper-0.4.0b5/hooks/build
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-12 15:42:01.000000 vyper-0.4.0b5/make.cmd
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-12 15:42:01.000000 vyper-0.4.0b5/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      239 2024-03-12 15:42:01.000000 vyper-0.4.0b5/quicktest.sh
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-12 15:42:01.000000 vyper-0.4.0b5/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-12 15:42:15.402900 vyper-0.4.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-03-12 15:42:01.000000 vyper-0.4.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16819 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/fixtures/memorymock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.342900 vyper-0.4.0b5/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.326900 vyper-0.4.0b5/tests/functional/builtins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.346900 vyper-0.4.0b5/tests/functional/builtins/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13609 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)    12014 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_addmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)    20337 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_create_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_ecrecover.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_is_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/codegen/test_unsafe_math.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.350900 vyper-0.4.0b5/tests/functional/builtins/folding/
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_addmod_mulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_bitwise.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_floor_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_fold_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_keccak_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/builtins/folding/test_powmod.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.350900 vyper-0.4.0b5/tests/functional/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.350900 vyper-0.4.0b5/tests/functional/codegen/calling_convention/
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_default_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_default_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_erc20_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    59109 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_self_call_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.350900 vyper-0.4.0b5/tests/functional/codegen/environment_variables/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/environment_variables/test_block_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/environment_variables/test_blockhash.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/environment_variables/test_tx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.354900 vyper-0.4.0b5/tests/functional/codegen/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.354900 vyper-0.4.0b5/tests/functional/codegen/features/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_nonreentrant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_private.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_pure.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.354900 vyper-0.4.0b5/tests/functional/codegen/features/iteration/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_break.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_continue.py
--rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_for_in_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_range_in.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_address_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_assert_unreachable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_bytes_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    17466 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_clampers.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_immutable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    15725 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_internal_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    33627 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_logging_bytes_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_logging_from_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_memory_alloc.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_memory_dealloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_reverting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_short_circuiting.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_string_map_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/features/test_transient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.354900 vyper-0.4.0b5/tests/functional/codegen/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/integration/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/integration/test_crowdfund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/integration/test_escrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.358899 vyper-0.4.0b5/tests/functional/codegen/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/modules/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/modules/test_interface_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/modules/test_module_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/modules/test_module_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/modules/test_stateless_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.358899 vyper-0.4.0b5/tests/functional/codegen/storage_variables/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/storage_variables/test_getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/storage_variables/test_setters.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/storage_variables/test_storage_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/test_call_graph_stability.py
--rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/test_selector_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/test_selector_table_stability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.358899 vyper-0.4.0b5/tests/functional/codegen/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.358899 vyper-0.4.0b5/tests/functional/codegen/types/numbers/
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_decimals.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_division.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_exponents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_isqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_modulo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_signed_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_sqrt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_unsigned_ints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_array_indexing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_bytes_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_bytes_zero_padding.py
--rw-r--r--   0 runner    (1001) docker     (127)    49607 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_identifier_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_node_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/codegen/types/test_struct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.358899 vyper-0.4.0b5/tests/functional/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/auctions/
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/auctions/test_blind_auction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/auctions/test_simple_open_auction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/company/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/company/test_company.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/crowdfund/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/crowdfund/test_crowdfund_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/factory/
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/factory/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/market_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/market_maker/test_on_chain_market_maker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/name_registry/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/name_registry/test_name_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/safe_remote_purchase/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/storage/test_advanced_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/storage/test_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/tokens/test_erc1155.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/tokens/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/tokens/test_erc4626.py
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/tokens/test_erc721.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/voting/
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/voting/test_ballot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/examples/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/examples/wallet/test_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.362900 vyper-0.4.0b5/tests/functional/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/grammar/test_grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.370900 vyper-0.4.0b5/tests/functional/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.374899 vyper-0.4.0b5/tests/functional/syntax/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_argument_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_call_violation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_constancy_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_function_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_instantiation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_invalid_payable.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_invalid_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_invalid_type_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_namespace_collision.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_overflow_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_structure_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_syntax_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_undeclared_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.374899 vyper-0.4.0b5/tests/functional/syntax/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/modules/test_deploy_visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/modules/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/modules/test_implements.py
--rw-r--r--   0 runner    (1001) docker     (127)    25198 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/modules/test_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.374899 vyper-0.4.0b5/tests/functional/syntax/names/
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/names/test_event_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/names/test_function_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/names/test_variable_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.374899 vyper-0.4.0b5/tests/functional/syntax/signatures/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/signatures/test_invalid_function_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/signatures/test_method_id_conflicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_abi_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_abi_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_abs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_addmulmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_address_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_ann_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_as_uint256.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_as_wei_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_blockscope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_bool_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_ceil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_chainid.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_code_size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_codehash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_create_with_code_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_dynamic_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_epsilon.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_external_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_extract32.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_floor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_for_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_functions_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_immutables.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_invalids.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_len.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_method_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_minmax.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_minmax_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_msg_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_nested_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_no_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_powmod.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_raw_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_return_tuple.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_self_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_selfdestruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8272 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_ternary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_tuple_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_uint2str.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_unary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/functional/syntax/test_unbalanced_return.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.374899 vyper-0.4.0b5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.374899 vyper-0.4.0b5/tests/unit/abi_types/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/abi_types/test_invalid_abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.374899 vyper-0.4.0b5/tests/unit/ast/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.378899 vyper-0.4.0b5/tests/unit/ast/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_binary.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_compare_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_binop_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_binop_int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_boolop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_subscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_unaryop.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_from_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_get_children.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_get_descendants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/nodes/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/test_annotate_and_optimize_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/test_ast_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/test_metadata_journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/test_natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/ast/test_source_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.330900 vyper-0.4.0b5/tests/unit/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.378899 vyper-0.4.0b5/tests/unit/cli/storage_layout/
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/storage_layout/test_storage_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.378899 vyper-0.4.0b5/tests/unit/cli/vyper_compile/
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/vyper_compile/test_compile_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/vyper_compile/test_parse_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.378899 vyper-0.4.0b5/tests/unit/cli/vyper_json/
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/vyper_json/test_compile_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/vyper_json/test_get_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/vyper_json/test_get_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/vyper_json/test_output_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.378899 vyper-0.4.0b5/tests/unit/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.378899 vyper-0.4.0b5/tests/unit/compiler/asm/
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/asm/test_asm_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.382900 vyper-0.4.0b5/tests/unit/compiler/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/ir/test_calldatacopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/ir/test_compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/ir/test_optimize_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/ir/test_repeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/ir/test_with.py
--rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_bytecode_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_compile_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_default_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_sha3_32.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/test_source_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.382900 vyper-0.4.0b5/tests/unit/compiler/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/venom/test_convert_basicblock_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/venom/test_duplicate_operands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/venom/test_multi_entry_block.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/compiler/venom/test_stack_at_external_return.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.382900 vyper-0.4.0b5/tests/unit/semantics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.382900 vyper-0.4.0b5/tests/unit/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/analysis/test_array_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/analysis/test_cyclic_function_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/analysis/test_for_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/analysis/test_potential_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/test_storage_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.382900 vyper-0.4.0b5/tests/unit/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/types/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/types/test_pure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/types/test_size_in_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/types/test_type_from_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/unit/semantics/types/test_type_from_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-12 15:42:01.000000 vyper-0.4.0b5/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.382900 vyper-0.4.0b5/vyper/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/abi_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.386900 vyper-0.4.0b5/vyper/ast/
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/grammar.lark
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/identifiers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/natspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    44916 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17231 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/pre_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ast/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.386900 vyper-0.4.0b5/vyper/builtins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/_signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    91767 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.386900 vyper-0.4.0b5/vyper/builtins/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/interfaces/IERC165.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/interfaces/IERC20.vyi
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/interfaces/IERC20Detailed.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/interfaces/IERC4626.vyi
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/builtins/interfaces/IERC721.vyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.390900 vyper-0.4.0b5/vyper/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10345 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/cli/vyper_compile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/cli/vyper_ir.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/cli/vyper_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.390900 vyper-0.4.0b5/vyper/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/abi_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    43348 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    30650 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/external_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.390900 vyper-0.4.0b5/vyper/codegen/function_definitions/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/function_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/function_definitions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8137 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/function_definitions/external_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/function_definitions/internal_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/ir_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/jumptable_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/keccak256_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/memory_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/return_.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/self_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/codegen/stmt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.394899 vyper-0.4.0b5/vyper/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/compiler/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/compiler/input_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)    12698 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/compiler/output.py
--rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/compiler/phases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/compiler/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/compiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.394899 vyper-0.4.0b5/vyper/evm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/evm/address_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/evm/opcodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12488 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.394899 vyper-0.4.0b5/vyper/ir/
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45729 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ir/compile_ir.py
--rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ir/optimizer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/ir/s_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.394899 vyper-0.4.0b5/vyper/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.398899 vyper-0.4.0b5/vyper/semantics/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/constant_folding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/data_positions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/global_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/import_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/levenshtein_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    36798 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    34000 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/analysis/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/data_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.398899 vyper-0.4.0b5/vyper/semantics/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/bytestrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    30776 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    16997 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/module.py
--rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/subscriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/semantics/types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.398899 vyper-0.4.0b5/vyper/venom/
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12298 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/basicblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/bb_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    34810 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/ir_node_to_venom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.398899 vyper-0.4.0b5/vyper/venom/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/passes/base_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/passes/constant_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/passes/dft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/passes/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/stack_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/venom/venom_to_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-12 15:42:14.000000 vyper-0.4.0b5/vyper/version.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-12 15:42:12.000000 vyper-0.4.0b5/vyper/vyper_git_commithash.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-12 15:42:01.000000 vyper-0.4.0b5/vyper/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 15:42:15.386900 vyper-0.4.0b5/vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-03-12 15:42:15.000000 vyper-0.4.0b5/vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19859 2024-03-12 15:42:15.000000 vyper-0.4.0b5/vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 15:42:15.000000 vyper-0.4.0b5/vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-12 15:42:15.000000 vyper-0.4.0b5/vyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-12 15:42:15.000000 vyper-0.4.0b5/vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 15:42:15.000000 vyper-0.4.0b5/vyper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.876349 vyper-0.4.0b6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.812349 vyper-0.4.0b6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.812349 vyper-0.4.0b6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/ISSUE_TEMPLATE/vip.md
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.812349 vyper-0.4.0b6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/era-tester.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/ghcr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/release-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-06 17:25:51.000000 vyper-0.4.0b6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-06 17:25:51.000000 vyper-0.4.0b6/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-06 17:25:51.000000 vyper-0.4.0b6/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-06 17:25:51.000000 vyper-0.4.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-06 17:25:51.000000 vyper-0.4.0b6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-06 17:26:01.876349 vyper-0.4.0b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-06 17:25:51.000000 vyper-0.4.0b6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-06 17:25:51.000000 vyper-0.4.0b6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/_templates/versions.html
+-rw-r--r--   0 runner    (1001) docker     (127)    37575 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/built-in-functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/compiler-exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15660 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/compiling-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/constants-and-vars.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13206 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/control-structures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/deploying-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/event-logging.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/installing-vyper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/interfaces.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/natspec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    64067 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/release-notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/scoping-and-declarations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/statements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/structure-of-a-contract.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15593 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/style-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/testing-contracts-brownie.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/testing-contracts-ethtester.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/testing-contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23271 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/types.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    29097 2024-04-06 17:25:51.000000 vyper-0.4.0b6/docs/vyper-by-example.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/auctions/blind_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/auctions/simple_open_auction.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/crowdfund.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/factory/Exchange.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/factory/Factory.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/market_maker/on_chain_market_maker.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/name_registry/name_registry.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/safe_remote_purchase/safe_remote_purchase.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/stock/company.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.816349 vyper-0.4.0b6/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/storage/advanced_storage.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/storage/storage.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    15365 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/tokens/ERC1155ownable.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/tokens/ERC20.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/tokens/ERC4626.vy
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/tokens/ERC721.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/voting/ballot.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-06 17:25:51.000000 vyper-0.4.0b6/examples/wallet/wallet.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      265 2024-04-06 17:25:51.000000 vyper-0.4.0b6/hooks/build
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-06 17:25:51.000000 vyper-0.4.0b6/make.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-06 17:25:51.000000 vyper-0.4.0b6/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      207 2024-04-06 17:25:51.000000 vyper-0.4.0b6/quicktest.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-06 17:25:51.000000 vyper-0.4.0b6/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-06 17:26:01.876349 vyper-0.4.0b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-06 17:25:51.000000 vyper-0.4.0b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19369 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/fixtures/memorymock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.820349 vyper-0.4.0b6/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.804349 vyper-0.4.0b6/tests/functional/builtins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.824349 vyper-0.4.0b6/tests/functional/builtins/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12223 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_addmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20335 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19014 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_create_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4425 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_ecrecover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_is_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16894 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/codegen/test_unsafe_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.824349 vyper-0.4.0b6/tests/functional/builtins/folding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_addmod_mulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_bitwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_floor_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_fold_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_keccak_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/builtins/folding/test_powmod.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.824349 vyper-0.4.0b6/tests/functional/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.824349 vyper-0.4.0b6/tests/functional/codegen/calling_convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_default_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_default_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_erc20_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59109 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_self_call_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.828349 vyper-0.4.0b6/tests/functional/codegen/environment_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/environment_variables/test_block_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/environment_variables/test_blockhash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/environment_variables/test_tx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.828349 vyper-0.4.0b6/tests/functional/codegen/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/features/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     8386 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_nonreentrant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_pure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/features/iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16979 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_for_in_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_range_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_assert_unreachable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_bytes_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16176 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_clampers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15725 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_internal_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33753 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_logging_bytes_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_logging_from_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_memory_alloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_memory_dealloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_reverting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_short_circuiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_string_map_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/features/test_transient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/integration/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/integration/test_crowdfund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/integration/test_escrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_flag_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_interface_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_module_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_module_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8010 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/modules/test_stateless_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.832349 vyper-0.4.0b6/tests/functional/codegen/storage_variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_storage_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/test_call_graph_stability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16003 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14820 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/test_selector_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/test_selector_table_stability.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/codegen/types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/codegen/types/numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_decimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_division.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_exponents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_isqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_modulo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_signed_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_sqrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_unsigned_ints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_array_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_bytes_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_bytes_zero_padding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50078 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_identifier_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_node_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/codegen/types/test_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/auctions/
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/auctions/test_blind_auction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4234 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/auctions/test_simple_open_auction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/company/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/company/test_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/crowdfund/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/crowdfund/test_crowdfund_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/factory/test_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/market_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/market_maker/test_on_chain_market_maker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/name_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/name_registry/test_name_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/safe_remote_purchase/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/storage/test_advanced_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/storage/test_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/tokens/test_erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/tokens/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/tokens/test_erc4626.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/tokens/test_erc721.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/voting/
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/voting/test_ballot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/examples/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/examples/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.836349 vyper-0.4.0b6/tests/functional/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/grammar/test_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_argument_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_call_violation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_constancy_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_function_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_instantiation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_literal_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_payable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_type_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_namespace_collision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_overflow_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_structure_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_syntax_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_type_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_undeclared_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_variable_declaration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/exceptions/test_vyper_exception_pos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/test_deploy_visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/test_implements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25198 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/modules/test_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/names/test_event_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/names/test_function_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/names/test_variable_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/functional/syntax/signatures/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/signatures/test_invalid_function_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/signatures/test_method_id_conflicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_abi_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_abi_encode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_abs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_addmulmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_address_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_ann_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_as_uint256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_as_wei_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_blockscope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_bool_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_chainid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_code_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_codehash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_create_with_code_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_dynamic_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_external_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_extract32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_floor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7848 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_for_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_functions_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_immutables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_invalids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_method_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_minmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_minmax_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_msg_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_nested_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_no_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_powmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_raw_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_return_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_self_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_selfdestruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_tuple_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_uint2str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_unary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/functional/syntax/test_unbalanced_return.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.848349 vyper-0.4.0b6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/abi_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/abi_types/test_invalid_abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/ast/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/ast/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_compare_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_binop_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_binop_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_boolop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_subscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_unaryop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_from_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_get_children.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_get_descendants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/nodes/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_annotate_and_optimize_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68091 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_ast_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_metadata_journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/ast/test_source_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.808349 vyper-0.4.0b6/tests/unit/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/cli/storage_layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/storage_layout/test_storage_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/storage_layout/test_storage_layout_overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.852349 vyper-0.4.0b6/tests/unit/cli/vyper_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_compile/test_compile_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_compile/test_parse_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/cli/vyper_json/
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_compile_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_get_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_output_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/compiler/asm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/asm/test_asm_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/compiler/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_calldatacopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_optimize_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_repeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13843 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/ir/test_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_bytecode_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_compile_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8519 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_sha3_32.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/test_source_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/compiler/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_convert_basicblock_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_dominator_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_duplicate_operands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_liveness_simple_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_multi_entry_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_stack_at_external_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/compiler/venom/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.856349 vyper-0.4.0b6/tests/unit/semantics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/tests/unit/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/analysis/test_array_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/analysis/test_cyclic_function_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/analysis/test_for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/analysis/test_potential_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/test_storage_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/tests/unit/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_pure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_size_in_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_type_from_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/semantics/types/test_type_from_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/unit/utils/test_keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-06 17:25:51.000000 vyper-0.4.0b6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/vyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/abi_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.864349 vyper-0.4.0b6/vyper/ast/
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/natspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45995 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17273 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/pre_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ast/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.864349 vyper-0.4.0b6/vyper/builtins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90791 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.864349 vyper-0.4.0b6/vyper/builtins/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC165.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC20.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC20Detailed.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC4626.vyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/builtins/interfaces/IERC721.vyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.864349 vyper-0.4.0b6/vyper/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10389 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/cli/vyper_compile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/cli/vyper_ir.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15843 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/cli/vyper_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.868349 vyper-0.4.0b6/vyper/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9461 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/abi_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13044 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43348 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30634 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/external_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.868349 vyper-0.4.0b6/vyper/codegen/function_definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/function_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/function_definitions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/function_definitions/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/function_definitions/internal_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23599 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/ir_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/jumptable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/keccak256_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/memory_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21180 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/return_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/self_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/codegen/stmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.868349 vyper-0.4.0b6/vyper/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/input_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/phases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/compiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.868349 vyper-0.4.0b6/vyper/evm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/evm/address_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/evm/opcodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.872349 vyper-0.4.0b6/vyper/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45834 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/compile_ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24821 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/optimizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1076 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/ir/s_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.872349 vyper-0.4.0b6/vyper/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.872349 vyper-0.4.0b6/vyper/semantics/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/constant_folding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/data_positions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/getters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/global_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/import_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/levenshtein_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37194 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23538 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/analysis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/data_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.876349 vyper-0.4.0b6/vyper/semantics/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/bytestrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30776 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17439 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12313 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/subscriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14788 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/semantics/types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17315 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.876349 vyper-0.4.0b6/vyper/venom/
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/basicblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/bb_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/dominators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/ir_node_to_venom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.876349 vyper-0.4.0b6/vyper/venom/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/base_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/constant_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/dft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/make_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/simplify_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/passes/stack_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/stack_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/venom/venom_to_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 17:25:59.000000 vyper-0.4.0b6/vyper/vyper_git_commithash.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-06 17:25:51.000000 vyper-0.4.0b6/vyper/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:26:01.860349 vyper-0.4.0b6/vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20300 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 17:26:01.000000 vyper-0.4.0b6/vyper.egg-info/top_level.txt
```

### Comparing `vyper-0.4.0b5/.github/ISSUE_TEMPLATE/bug.md` & `vyper-0.4.0b6/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/.github/ISSUE_TEMPLATE/vip.md` & `vyper-0.4.0b6/.github/ISSUE_TEMPLATE/vip.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/.github/workflows/build.yml` & `vyper-0.4.0b6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/.github/workflows/codeql.yml` & `vyper-0.4.0b6/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/.github/workflows/era-tester.yml` & `vyper-0.4.0b6/.github/workflows/era-tester.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/.github/workflows/ghcr.yml` & `vyper-0.4.0b6/.github/workflows/ghcr.yml`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/.github/workflows/test.yml` & `vyper-0.4.0b6/.github/workflows/test.yml`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,17 @@
       with:
         python-version: "3.11"
         cache: "pip"
 
     - name: Install Dependencies
       run: pip install .[lint]
 
+    - name: Debug dependencies
+      run: pip freeze
+
     - name: Run Black
       run: black --check -C --force-exclude=vyper/version.py ./vyper ./tests ./setup.py
 
     - name: Run flake8
       run: flake8 ./vyper ./tests ./setup.py
 
     - name: Run isort
@@ -46,55 +49,118 @@
 
       - name: Set up Python 3.11
         uses: actions/setup-python@v5
         with:
           python-version: "3.11"
           cache: "pip"
 
-      - name: Install Tox
-        run: pip install tox
+      - name: Install deps
+        # TODO these should really be in setup.py
+        run: pip install shibuya sphinx sphinx-copybutton
 
-      - name: Run Tox
-        run: TOXENV=docs tox -r
+      - name: Run docs
+        run: sphinx-build -E -b html docs dist/docs -n -q --color
 
   # "Regular"/core tests.
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [["3.11", "311"]]
-        # run in modes: --optimize [gas, none, codesize]
         opt-mode: ["gas", "none", "codesize"]
         debug: [true, false]
-        # run across other python versions.# we don't really need to run all
-        # modes across all python versions - one is enough
+        evm-version: [shanghai]
+        experimental-codegen: [false]
+        memorymock: [false]
+
+        # https://docs.github.com/en/actions/using-jobs/using-a-matrix-for-your-jobs#expanding-or-adding-matrix-configurations
         include:
+          # test default settings with 3.11 across all supported evm versions
+          - python-version: ["3.11", "311"]
+            debug: false
+            opt-mode: gas
+            evm-version: london
+          - python-version: ["3.11", "311"]
+            debug: false
+            opt-mode: gas
+            evm-version: paris
+
+          # redundant rule, for clarity
+          - python-version: ["3.11", "311"]
+            debug: false
+            opt-mode: gas
+            evm-version: shanghai
+
+          - python-version: ["3.11", "311"]
+            debug: false
+            opt-mode: gas
+            evm-version: cancun
+
+          # test experimental pipeline
+          - python-version: ["3.11", "311"]
+            opt-mode: gas
+            debug: false
+            evm-version: shanghai
+            experimental-codegen: true
+          # TODO: test experimental_codegen + -Ocodesize
+
+          # run with `--memorymock`, but only need to do it one configuration
+          # TODO: consider removing the memorymock tests
+          - python-version: ["3.11", "311"]
+            opt-mode: gas
+            debug: false
+            evm-version: shanghai
+            memorymock: true
+
+          # run across other python versions. we don't really need to run all
+          # modes across all python versions - one is enough
           - python-version: ["3.10", "310"]
             opt-mode: gas
             debug: false
+            evm-version: shanghai
+
+          - python-version: ["3.12", "312"]
+            opt-mode: gas
+            debug: false
+            evm-version: shanghai
 
-    name: py${{ matrix.python-version[1] }}-opt-${{ matrix.opt-mode }}${{ matrix.debug && '-debug' || '' }}
+
+    name: py${{ matrix.python-version[1] }}-opt-${{ matrix.opt-mode }}${{ matrix.debug && '-debug' || '' }}${{ matrix.memorymock && '-memorymock' || '' }}${{ matrix.experimental-codegen && '-experimental' || '' }}-${{ matrix.evm-version }}
 
     steps:
     - uses: actions/checkout@v4
       with:
           # need to fetch unshallow so that setuptools_scm can infer the version
           fetch-depth: 0
 
     - name: Set up Python ${{ matrix.python-version[0] }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version[0] }}
         cache: "pip"
 
-    - name: Install Tox
-      run: pip install tox
+    - name: Install dependencies
+      run: pip install .[test]
+
+    - name: Debug dependencies
+      run: pip freeze
 
-    - name: Run Tox
-      run: TOXENV=py${{ matrix.python-version[1] }} tox -r -- --optimize ${{ matrix.opt-mode }} ${{ matrix.debug && '--enable-compiler-debug-mode' || '' }} -r aR tests/
+    - name: Run tests
+      run: |
+        pytest \
+          -m "not fuzzing" \
+          --optimize ${{ matrix.opt-mode }} \
+          --evm-version ${{ matrix.evm-version }} \
+          ${{ matrix.debug && '--enable-compiler-debug-mode' || '' }} \
+          ${{ matrix.memorymock && '--memorymock' || '' }} \
+          ${{ matrix.experimental-codegen && '--experimental-codegen' || '' }} \
+          --cov-branch \
+          --cov-report xml:coverage.xml \
+          --cov=vyper \
+          tests/
 
     - name: Upload Coverage
       uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
 
@@ -114,36 +180,48 @@
   # fuzzing + slow/exhaustive tests (things that are too slow to run in
   # the regular test suite)
   fuzzing:
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        group: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60]
+        # note that every time this is updated, `--splits` needs to be
+        # updated below as well.
+        # python -c "print(list(range(1, 121)))"
+        group: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 44, 45, 46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 74, 75, 76, 77, 78, 79, 80, 81, 82, 83, 84, 85, 86, 87, 88, 89, 90, 91, 92, 93, 94, 95, 96, 97, 98, 99, 100, 101, 102, 103, 104, 105, 106, 107, 108, 109, 110, 111, 112, 113, 114, 115, 116, 117, 118, 119, 120]
 
     steps:
     - uses: actions/checkout@v4
 
     - name: Set up Python 3.11
       uses: actions/setup-python@v5
       with:
         python-version: "3.11"
         cache: "pip"
 
-    - name: Install Tox
-      run: pip install tox
+    - name: Install dependencies
+      run: pip install .[test]
 
     # fetch test durations
     # NOTE: if the tests get poorly distributed, run this and commit the resulting `.test_durations` file to the `vyper-test-durations` repo.
-    # `TOXENV=fuzzing tox -r -- --store-durations -r aR tests/`
+    # `pytest -m "fuzzing" --store-durations -r aR tests/`
     - name: Fetch test-durations
-      run: curl --location "https://raw.githubusercontent.com/vyperlang/vyper-test-durations/5982755ee8459f771f2e8622427c36494646e1dd/test_durations" -o .test_durations
+      run: curl --location "https://raw.githubusercontent.com/vyperlang/vyper-test-durations/master/test_durations" -o .test_durations
 
-    - name: Run Tox
-      run: TOXENV=fuzzing tox -r -- --splits 60 --group ${{ matrix.group }} --splitting-algorithm least_duration -r aR tests/
+    - name: Run tests
+      run: |
+        pytest \
+          -m "fuzzing" \
+          --splits 120 \
+          --group ${{ matrix.group }} \
+          --splitting-algorithm least_duration \
+          --cov-branch \
+          --cov-report xml:coverage.xml \
+          --cov=vyper \
+          tests/
 
     - name: Upload Coverage
       uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
 
@@ -154,34 +232,7 @@
     runs-on: ubuntu-latest
     needs: fuzzing
 
     steps:
       - name: Check slow tests all succeeded
         if: ${{ needs.fuzzing.result != 'success' }}
         run: exit 1
-
-  memory:
-    runs-on: ubuntu-latest
-
-    steps:
-    - uses: actions/checkout@v4
-      with:
-          # need to fetch unshallow so that setuptools_scm can infer the version
-          fetch-depth: 0
-
-    - name: Set up Python 3.11
-      uses: actions/setup-python@v5
-      with:
-        python-version: "3.11"
-        cache: "pip"
-
-    - name: Install Tox
-      run: pip install tox
-
-    - name: Run Tox
-      run: TOXENV=memory tox -r
-
-    - name: Upload Coverage
-      uses: codecov/codecov-action@v4
-      with:
-        token: ${{ secrets.CODECOV_TOKEN }}
-        file: ./coverage.xml
```

### Comparing `vyper-0.4.0b5/.pre-commit-config.yaml` & `vyper-0.4.0b6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.7.1
     hooks:
     -   id: mypy
         additional_dependencies:
           - "types-setuptools"
-        args:  # settings from tox.ini
+        args:  # settings from Makefile
           - --install-types
           - --non-interactive
           - --follow-imports=silent
           - --ignore-missing-imports
           - --implicit-optional
 
 default_language_version:
```

### Comparing `vyper-0.4.0b5/Dockerfile` & `vyper-0.4.0b6/Dockerfile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/LICENSE` & `vyper-0.4.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/Makefile` & `vyper-0.4.0b6/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 
 test:
 	pytest
 
 lint: mypy black flake8 isort
 
 mypy:
-	mypy --install-types --non-interactive --follow-imports=silent --ignore-missing-imports --implicit-optional -p vyper
+	mypy \
+		--disable-error-code "annotation-unchecked" \
+		--follow-imports=silent \
+		--ignore-missing-imports \
+		--implicit-optional \
+		-p vyper
 
 black:
 	black -C -t py311 vyper/ tests/ setup.py --force-exclude=vyper/version.py
 
 flake8: black
 	flake8 vyper/ tests/
```

### Comparing `vyper-0.4.0b5/PKG-INFO` & `vyper-0.4.0b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0b5
+Version: 0.4.0b6
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
-Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/vyperlang/vyper/master/docs/logo.svg?sanitize=true" alt="" width="110">
 
 [![Build Status](https://github.com/vyperlang/vyper/workflows/Test/badge.svg)](https://github.com/vyperlang/vyper/actions/workflows/test.yml)
 [![Documentation Status](https://readthedocs.org/projects/vyper/badge/?version=latest)](http://docs.vyperlang.org/en/latest/?badge=latest "ReadTheDocs")
```

### Comparing `vyper-0.4.0b5/README.md` & `vyper-0.4.0b6/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/SECURITY.md` & `vyper-0.4.0b6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/Makefile` & `vyper-0.4.0b6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/_templates/versions.html` & `vyper-0.4.0b6/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/built-in-functions.rst` & `vyper-0.4.0b6/docs/built-in-functions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/compiler-exceptions.rst` & `vyper-0.4.0b6/docs/compiler-exceptions.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/compiling-a-contract.rst` & `vyper-0.4.0b6/docs/compiling-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/conf.py` & `vyper-0.4.0b6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/constants-and-vars.rst` & `vyper-0.4.0b6/docs/constants-and-vars.rst`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 --------------------------------
 
 ==================== ================ =========================================================
 Name                 Type             Value
 ==================== ================ =========================================================
 ``block.coinbase``   ``address``      Current block miner's address
 ``block.difficulty`` ``uint256``      Current block difficulty
-``block.prevrandao`` ``uint256``      Current randomness beacon provided by the beacon chain
+``block.prevrandao`` ``bytes32``      Current randomness beacon provided by the beacon chain
 ``block.number``     ``uint256``      Current block number
 ``block.prevhash``   ``bytes32``      Equivalent to ``blockhash(block.number - 1)``
 ``block.timestamp``  ``uint256``      Current block epoch timestamp
 ``chain.id``         ``uint256``      Chain ID
 ``msg.data``         ``Bytes``        Message data
 ``msg.gas``          ``uint256``      Remaining gas
 ``msg.sender``       ``address``      Sender of the message (current call)
 ``msg.value``        ``uint256``      Number of wei sent with the message
 ``tx.origin``        ``address``      Sender of the transaction (full call chain)
 ``tx.gasprice``      ``uint256``      Gas price of current transaction in wei
 ==================== ================ =========================================================
 
 .. note::
 
-    ``block.prevrandao`` is an alias for ``block.difficulty``. Since ``block.difficulty`` is considered deprecated according to `EIP-4399 <https://eips.ethereum.org/EIPS/eip-4399>`_ after "The Merge" (Paris hard fork), we recommend using ``block.prevrandao``.
+    ``block.prevrandao`` is an alias for the ``block.difficulty`` opcode. Since ``block.difficulty`` is considered deprecated according to `EIP-4399 <https://eips.ethereum.org/EIPS/eip-4399>`_ after "The Merge" (Paris hard fork), we recommend using ``block.prevrandao``.
 
 .. note::
 
     ``msg.data`` requires the usage of :func:`slice <slice>` to explicitly extract a section of calldata. If the extracted section exceeds the bounds of calldata, this will throw. You can check the size of ``msg.data`` using :func:`len <len>`.
 
 .. _constants-self:
```

### Comparing `vyper-0.4.0b5/docs/contributing.rst` & `vyper-0.4.0b6/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/control-structures.rst` & `vyper-0.4.0b6/docs/control-structures.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/deploying-contracts.rst` & `vyper-0.4.0b6/docs/deploying-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/event-logging.rst` & `vyper-0.4.0b6/docs/event-logging.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/index.rst` & `vyper-0.4.0b6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/installing-vyper.rst` & `vyper-0.4.0b6/docs/installing-vyper.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/interfaces.rst` & `vyper-0.4.0b6/docs/interfaces.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/logo.svg` & `vyper-0.4.0b6/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/make.bat` & `vyper-0.4.0b6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/natspec.rst` & `vyper-0.4.0b6/docs/natspec.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/release-notes.rst` & `vyper-0.4.0b6/docs/release-notes.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/resources.rst` & `vyper-0.4.0b6/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/scoping-and-declarations.rst` & `vyper-0.4.0b6/docs/scoping-and-declarations.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/statements.rst` & `vyper-0.4.0b6/docs/statements.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/structure-of-a-contract.rst` & `vyper-0.4.0b6/docs/structure-of-a-contract.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/style-guide.rst` & `vyper-0.4.0b6/docs/style-guide.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/testing-contracts-brownie.rst` & `vyper-0.4.0b6/docs/testing-contracts-brownie.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/testing-contracts-ethtester.rst` & `vyper-0.4.0b6/docs/testing-contracts-ethtester.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/testing-contracts.rst` & `vyper-0.4.0b6/docs/testing-contracts.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/toctree.rst` & `vyper-0.4.0b6/docs/toctree.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/types.rst` & `vyper-0.4.0b6/docs/types.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/versioning.rst` & `vyper-0.4.0b6/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/docs/vyper-by-example.rst` & `vyper-0.4.0b6/docs/vyper-by-example.rst`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/auctions/blind_auction.vy` & `vyper-0.4.0b6/examples/auctions/blind_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/auctions/simple_open_auction.vy` & `vyper-0.4.0b6/examples/auctions/simple_open_auction.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/crowdfund.vy` & `vyper-0.4.0b6/examples/crowdfund.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/factory/Exchange.vy` & `vyper-0.4.0b6/examples/factory/Exchange.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/factory/Factory.vy` & `vyper-0.4.0b6/examples/factory/Factory.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/market_maker/on_chain_market_maker.vy` & `vyper-0.4.0b6/examples/market_maker/on_chain_market_maker.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/safe_remote_purchase/safe_remote_purchase.vy` & `vyper-0.4.0b6/examples/safe_remote_purchase/safe_remote_purchase.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/stock/company.vy` & `vyper-0.4.0b6/examples/stock/company.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/tokens/ERC1155ownable.vy` & `vyper-0.4.0b6/examples/tokens/ERC1155ownable.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/tokens/ERC20.vy` & `vyper-0.4.0b6/examples/tokens/ERC20.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/tokens/ERC4626.vy` & `vyper-0.4.0b6/examples/tokens/ERC4626.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/tokens/ERC721.vy` & `vyper-0.4.0b6/examples/tokens/ERC721.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/voting/ballot.vy` & `vyper-0.4.0b6/examples/voting/ballot.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/examples/wallet/wallet.vy` & `vyper-0.4.0b6/examples/wallet/wallet.vy`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/make.cmd` & `vyper-0.4.0b6/make.cmd`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/setup.py` & `vyper-0.4.0b6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,43 +4,41 @@
 import re
 import subprocess
 
 from setuptools import setup
 
 extras_require = {
     "test": [
-        "pytest>=6.2.5,<7.0",
-        "pytest-cov>=2.10,<3.0",
+        "pytest>=8.0,<9.0",
+        "pytest-cov>=4.1,<5.0",
         "pytest-instafail>=0.4,<1.0",
-        "pytest-xdist>=2.5,<3.0",
+        "pytest-xdist>=3.0,<3.4",
         "pytest-split>=0.7.0,<1.0",
-        "eth-tester[py-evm]>=0.9.0b1,<0.10",
+        "eth-tester[py-evm]>=0.10.0b4,<0.11",
         "eth_abi>=4.0.0,<5.0.0",
-        "py-evm>=0.7.0a1,<0.8",
+        "py-evm>=0.10.0b4,<0.11",
         "web3==6.0.0",
-        "tox>=3.15,<4.0",
         "lark==1.1.9",
-        "hypothesis[lark]>=5.37.1,<6.0",
-        "eth-stdlib==0.2.6",
+        "hypothesis[lark]>=6.0,<7.0",
+        "eth-stdlib==0.2.7",
+        "setuptools",
+        "hexbytes>=1.2",
     ],
     "lint": [
         "black==23.12.0",
         "flake8==6.1.0",
         "flake8-bugbear==23.12.2",
         "flake8-use-fstring==1.4",
         "isort==5.13.2",
         "mypy==1.5",
     ],
-    "docs": ["recommonmark", "sphinx>=6.0,<7.0", "sphinx_rtd_theme>=1.2,<1.3"],
     "dev": ["ipython", "pre-commit", "pyinstaller", "twine"],
 }
 
-extras_require["dev"] = (
-    extras_require["test"] + extras_require["lint"] + extras_require["docs"] + extras_require["dev"]
-)
+extras_require["dev"] = extras_require["dev"] + extras_require["test"] + extras_require["lint"]
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 # strip local version
 def _local_version(version):
@@ -111,11 +109,12 @@
         ]
     },
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     package_data={"vyper.ast": ["grammar.lark"]},
     data_files=[("", [hash_file_rel_path])],
 )
```

### Comparing `vyper-0.4.0b5/tests/conftest.py` & `vyper-0.4.0b6/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,25 @@
 from eth_utils import setup_DEBUG2_logging
 from eth_utils.toolz import compose
 from hexbytes import HexBytes
 from web3 import Web3
 from web3.contract import Contract
 from web3.providers.eth_tester import EthereumTesterProvider
 
+import vyper.evm.opcodes as evm
 from tests.utils import working_directory
 from vyper import compiler
 from vyper.ast.grammar import parse_vyper_source
 from vyper.codegen.ir_node import IRnode
 from vyper.compiler.input_bundle import FilesystemInputBundle, InputBundle
 from vyper.compiler.settings import OptimizationLevel, Settings, _set_debug_mode
+from vyper.evm.opcodes import version_check
+from vyper.exceptions import EvmVersionException
 from vyper.ir import compile_ir, optimizer
-from vyper.utils import ERC5202_PREFIX
+from vyper.utils import ERC5202_PREFIX, keccak256
 
 # Import the base fixtures
 pytest_plugins = ["tests.fixtures.memorymock"]
 
 ############
 # PATCHING #
 ############
@@ -34,15 +37,15 @@
 
 # disable hypothesis deadline globally
 hypothesis.settings.register_profile("ci", deadline=None)
 hypothesis.settings.load_profile("ci")
 
 
 def set_evm_verbose_logging():
-    logger = logging.getLogger("eth.vm.computation.Computation")
+    logger = logging.getLogger("eth.vm.computation.BaseComputation")
     setup_DEBUG2_logging()
     logger.setLevel("DEBUG2")
 
 
 # Useful options to comment out whilst working:
 # set_evm_verbose_logging()
 #
@@ -54,21 +57,31 @@
     parser.addoption(
         "--optimize",
         choices=["codesize", "gas", "none"],
         default="gas",
         help="change optimization mode",
     )
     parser.addoption("--enable-compiler-debug-mode", action="store_true")
+    parser.addoption("--experimental-codegen", action="store_true")
+
+    parser.addoption(
+        "--evm-version",
+        choices=list(evm.EVM_VERSIONS.keys()),
+        default="shanghai",
+        help="set evm version",
+    )
 
 
 @pytest.fixture(scope="module")
 def output_formats():
     output_formats = compiler.OUTPUT_FORMATS.copy()
     del output_formats["bb"]
     del output_formats["bb_runtime"]
+    del output_formats["cfg"]
+    del output_formats["cfg_runtime"]
     return output_formats
 
 
 @pytest.fixture(scope="module")
 def optimize(pytestconfig):
     flag = pytestconfig.getoption("optimize")
     return OptimizationLevel.from_string(flag)
@@ -77,24 +90,67 @@
 @pytest.fixture(scope="session", autouse=True)
 def debug(pytestconfig):
     debug = pytestconfig.getoption("enable_compiler_debug_mode")
     assert isinstance(debug, bool)
     _set_debug_mode(debug)
 
 
+@pytest.fixture(scope="session")
+def experimental_codegen(pytestconfig):
+    ret = pytestconfig.getoption("experimental_codegen")
+    assert isinstance(ret, bool)
+    return ret
+
+
+@pytest.fixture(autouse=True)
+def check_venom_xfail(request, experimental_codegen):
+    if not experimental_codegen:
+        return
+
+    marker = request.node.get_closest_marker("venom_xfail")
+    if marker is None:
+        return
+
+    # https://github.com/okken/pytest-runtime-xfail?tab=readme-ov-file#alternatives
+    request.node.add_marker(pytest.mark.xfail(strict=True, **marker.kwargs))
+
+
+@pytest.fixture
+def venom_xfail(request, experimental_codegen):
+    def _xfail(*args, **kwargs):
+        if not experimental_codegen:
+            return
+        request.node.add_marker(pytest.mark.xfail(*args, strict=True, **kwargs))
+
+    return _xfail
+
+
+@pytest.fixture(scope="session", autouse=True)
+def evm_version(pytestconfig):
+    # note: we configure the evm version that we emit code for,
+    # but eth-tester is only configured with the latest mainnet
+    # version.
+    evm_version_str = pytestconfig.getoption("evm_version")
+    evm.DEFAULT_EVM_VERSION = evm_version_str
+    # this should get overridden by anchor_evm_version,
+    # but set it anyway
+    evm.active_evm_version = evm.EVM_VERSIONS[evm_version_str]
+
+
 @pytest.fixture
 def chdir_tmp_path(tmp_path):
     # this is useful for when you want imports to have relpaths
     with working_directory(tmp_path):
         yield
 
 
+# CMC 2024-03-01 this doesn't need to be a fixture
 @pytest.fixture
 def keccak():
-    return Web3.keccak
+    return keccak256
 
 
 @pytest.fixture
 def make_file(tmp_path):
     # writes file_contents to file_name, creating it in the
     # tmp_path directory. returns final path.
     def fn(file_name, file_contents):
@@ -297,23 +353,24 @@
     return ir_compiler
 
 
 def _get_contract(
     w3,
     source_code,
     optimize,
+    experimental_codegen,
     output_formats,
     *args,
     override_opt_level=None,
     input_bundle=None,
     **kwargs,
 ):
     settings = Settings()
-    settings.evm_version = kwargs.pop("evm_version", None)
     settings.optimize = override_opt_level or optimize
+    settings.experimental_codegen = experimental_codegen
     out = compiler.compile_code(
         source_code,
         # test that all output formats can get generated
         output_formats=output_formats,
         settings=settings,
         input_bundle=input_bundle,
         show_gas_estimates=True,  # Enable gas estimates for testing
@@ -329,66 +386,82 @@
     tx_info.update(kwargs)
     tx_hash = deploy_transaction.transact(tx_info)
     address = w3.eth.get_transaction_receipt(tx_hash)["contractAddress"]
     return w3.eth.contract(address, abi=abi, bytecode=bytecode, ContractFactoryClass=VyperContract)
 
 
 @pytest.fixture(scope="module")
-def get_contract(w3, optimize, output_formats):
+def get_contract(w3, optimize, experimental_codegen, output_formats):
     def fn(source_code, *args, **kwargs):
-        return _get_contract(w3, source_code, optimize, output_formats, *args, **kwargs)
+        return _get_contract(
+            w3, source_code, optimize, experimental_codegen, output_formats, *args, **kwargs
+        )
 
     return fn
 
 
 @pytest.fixture
-def get_contract_with_gas_estimation(tester, w3, optimize, output_formats):
+def get_contract_with_gas_estimation(tester, w3, optimize, experimental_codegen, output_formats):
     def get_contract_with_gas_estimation(source_code, *args, **kwargs):
-        contract = _get_contract(w3, source_code, optimize, output_formats, *args, **kwargs)
+        contract = _get_contract(
+            w3, source_code, optimize, experimental_codegen, output_formats, *args, **kwargs
+        )
         for abi_ in contract._classic_contract.functions.abi:
             if abi_["type"] == "function":
                 set_decorator_to_contract_function(w3, tester, contract, source_code, abi_["name"])
         return contract
 
     return get_contract_with_gas_estimation
 
 
 @pytest.fixture
-def get_contract_with_gas_estimation_for_constants(w3, optimize, output_formats):
+def get_contract_with_gas_estimation_for_constants(
+    w3, optimize, experimental_codegen, output_formats
+):
     def get_contract_with_gas_estimation_for_constants(source_code, *args, **kwargs):
-        return _get_contract(w3, source_code, optimize, output_formats, *args, **kwargs)
+        return _get_contract(
+            w3, source_code, optimize, experimental_codegen, output_formats, *args, **kwargs
+        )
 
     return get_contract_with_gas_estimation_for_constants
 
 
 @pytest.fixture(scope="module")
-def get_contract_module(optimize, output_formats):
+def get_contract_module(optimize, experimental_codegen, output_formats):
     """
     This fixture is used for Hypothesis tests to ensure that
     the same contract is called over multiple runs of the test.
     """
     custom_genesis = PyEVMBackend._generate_genesis_params(overrides={"gas_limit": 4500000})
     custom_genesis["base_fee_per_gas"] = 0
     backend = PyEVMBackend(genesis_parameters=custom_genesis)
     tester = EthereumTester(backend=backend)
     w3 = Web3(EthereumTesterProvider(tester))
     w3.eth.set_gas_price_strategy(zero_gas_price_strategy)
 
     def get_contract_module(source_code, *args, **kwargs):
-        return _get_contract(w3, source_code, optimize, output_formats, *args, **kwargs)
+        return _get_contract(
+            w3, source_code, optimize, experimental_codegen, output_formats, *args, **kwargs
+        )
 
     return get_contract_module
 
 
 def _deploy_blueprint_for(
-    w3, source_code, optimize, output_formats, initcode_prefix=ERC5202_PREFIX, **kwargs
+    w3,
+    source_code,
+    optimize,
+    experimental_codegen,
+    output_formats,
+    initcode_prefix=ERC5202_PREFIX,
+    **kwargs,
 ):
     settings = Settings()
-    settings.evm_version = kwargs.pop("evm_version", None)
     settings.optimize = optimize
+    settings.experimental_codegen = experimental_codegen
     out = compiler.compile_code(
         source_code,
         output_formats=output_formats,
         settings=settings,
         show_gas_estimates=True,  # Enable gas estimates for testing
     )
     parse_vyper_source(source_code)  # Test grammar.
@@ -416,17 +489,19 @@
             address, abi=abi, bytecode=bytecode, ContractFactoryClass=VyperContract
         )
 
     return w3.eth.contract(address, bytecode=deploy_bytecode), factory
 
 
 @pytest.fixture(scope="module")
-def deploy_blueprint_for(w3, optimize, output_formats):
+def deploy_blueprint_for(w3, optimize, experimental_codegen, output_formats):
     def deploy_blueprint_for(source_code, *args, **kwargs):
-        return _deploy_blueprint_for(w3, source_code, optimize, output_formats, *args, **kwargs)
+        return _deploy_blueprint_for(
+            w3, source_code, optimize, experimental_codegen, output_formats, *args, **kwargs
+        )
 
     return deploy_blueprint_for
 
 
 # TODO: this should not be a fixture.
 # remove me and replace all uses with `with pytest.raises`.
 @pytest.fixture
@@ -503,7 +578,18 @@
             yield excinfo
         tester.revert_to_snapshot(snapshot_id)
         if exc_text:
             # TODO test equality
             assert exc_text in str(excinfo.value), (exc_text, excinfo.value)
 
     return fn
+
+
+def pytest_runtest_call(item):
+    marker = item.get_closest_marker("requires_evm_version")
+    if marker:
+        assert len(marker.args) == 1
+        version = marker.args[0]
+        if not version_check(begin=version):
+            item.add_marker(
+                pytest.mark.xfail(reason="Wrong EVM version", raises=EvmVersionException)
+            )
```

### Comparing `vyper-0.4.0b5/tests/fixtures/memorymock.py` & `vyper-0.4.0b6/tests/fixtures/memorymock.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_abi_decode.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_abi_decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from decimal import Decimal
 
 import pytest
 from eth.codecs import abi
 
-from vyper.exceptions import ArgumentException, StructureException
+from vyper.exceptions import ArgumentException, StackTooDeep, StructureException
 
 TEST_ADDR = "0x" + b"".join(chr(i).encode("utf-8") for i in range(20)).hex()
 
 
 def test_abi_decode_complex(get_contract):
     contract = """
 struct Animal:
@@ -192,14 +192,15 @@
     [[[123, 456, 789], [234, 567]], [[234]], [[567], [912], [345]]],
     [[[]]],
 ]
 
 
 @pytest.mark.parametrize("args", nested_3d_array_args)
 @pytest.mark.parametrize("unwrap_tuple", (True, False))
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_abi_decode_nested_dynarray2(get_contract, args, unwrap_tuple):
     if unwrap_tuple is True:
         encoded = abi.encode("(uint256[][][])", (args,))
         len = 1696
     else:
         encoded = abi.encode("uint256[][][]", args)
         len = 1664
@@ -269,14 +270,15 @@
     """
     c = get_contract(code)
     bs = [1, 2, 3]
     encoded = abi.encode("(uint256[])", (bs,))
     assert c.foo(encoded) == [2**256 - 1, bs]
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_abi_decode_private_nested_dynarray(get_contract):
     code = """
 bytez: DynArray[DynArray[DynArray[uint256, 3], 3], 3]
 
 @internal
 def _foo(bs: Bytes[1696]):
     self.bytez = _abi_decode(bs, DynArray[DynArray[DynArray[uint256, 3], 3], 3])
```

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_abi_encode.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_abi_encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from decimal import Decimal
 
 import pytest
 from eth.codecs import abi
 
+from vyper.exceptions import StackTooDeep
+
 
 # @pytest.mark.parametrize("string", ["a", "abc", "abcde", "potato"])
 def test_abi_encode(get_contract):
     code = """
 struct Animal:
   name: String[5]
   address_: address
@@ -222,14 +224,15 @@
     [[[]], [[123]], [[]]],
     [[[123, 456, 789], [234, 567]], [[234]], [[567], [912], [345]]],
     [[[]]],
 ]
 
 
 @pytest.mark.parametrize("args", nested_3d_array_args)
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_abi_encode_nested_dynarray_2(get_contract, args):
     code = """
 @external
 def abi_encode(
     d: DynArray[DynArray[DynArray[uint256, 3], 3], 3],
     ensure_tuple: bool,
     include_method_id: bool
@@ -326,14 +329,15 @@
     return dont_clobber_me, self.bytez
     """
     c = get_contract(code)
     bs = [1, 2, 3]
     assert c.foo(bs) == [2**256 - 1, abi.encode("(uint256[])", (bs,))]
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_abi_encode_private_nested_dynarray(get_contract):
     code = """
 bytez: Bytes[1696]
 @internal
 def _foo(bs: DynArray[DynArray[DynArray[uint256, 3], 3], 3]):
     self.bytez = _abi_encode(bs)
```

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_addmod.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_addmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_as_wei_value.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_bitwise.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_ceil.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_concat.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_convert.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from vyper.semantics.types import AddressT, BoolT, BytesM_T, BytesT, DecimalT, IntegerT, StringT
 from vyper.semantics.types.shortcuts import BYTES20_T, BYTES32_T, UINT, UINT160_T, UINT256_T
 from vyper.utils import (
     DECIMAL_DIVISOR,
     checksum_encode,
     int_bounds,
     is_checksum_encoded,
+    quantize,
     round_towards_zero,
     unsigned_to_signed,
 )
 
 BASE_TYPES = set(IntegerT.all()) | set(BytesM_T.all()) | {DecimalT(), AddressT(), BoolT()}
 
 TEST_TYPES = BASE_TYPES | {BytesT(32)} | {StringT(32)}
@@ -410,15 +411,15 @@
 
 
 def _vyper_literal(val, typ):
     if isinstance(typ, BytesM_T):
         return "0x" + val.hex()
     if isinstance(typ, DecimalT):
         tmp = val
-        val = val.quantize(DECIMAL_EPSILON)
+        val = quantize(val)
         assert tmp == val
     return str(val)
 
 
 @pytest.mark.parametrize("i_typ,o_typ,val", generate_passing_cases())
 @pytest.mark.fuzzing
 def test_convert_passing(
```

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_create_functions.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_create_functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_ec.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_ec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_ecrecover.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_ecrecover.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_empty.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_empty.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_extract32.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_extract32.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,26 @@
-def test_extract32_extraction(tx_failed, get_contract_with_gas_estimation):
-    extract32_code = """
-y: Bytes[100]
+import pytest
+
+from vyper.evm.opcodes import version_check
+
+
+@pytest.mark.parametrize("location", ["storage", "transient"])
+def test_extract32_extraction(tx_failed, get_contract_with_gas_estimation, location):
+    if location == "transient" and not version_check(begin="cancun"):
+        pytest.skip(
+            "Skipping test as storage_location is 'transient' and EVM version is pre-Cancun"
+        )
+    if location == "storage":
+        decl = "y: Bytes[100]"
+    elif location == "transient":
+        decl = "y: transient(Bytes[100])"
+    else:
+        raise Exception("unreachable")
+    extract32_code = f"""
+{decl}
 @external
 def extrakt32(inp: Bytes[100], index: uint256) -> bytes32:
     return extract32(inp, index)
 
 @external
 def extrakt32_mem(inp: Bytes[100], index: uint256) -> bytes32:
     x: Bytes[100] = inp
@@ -39,16 +55,14 @@
             assert c.extrakt32(S, i) == expected_result
             assert c.extrakt32_mem(S, i) == expected_result
             assert c.extrakt32_storage(i, S) == expected_result
         else:
             with tx_failed():
                 c.extrakt32(S, i)
 
-    print("Passed bytes32 extraction test")
-
 
 def test_extract32_code(tx_failed, get_contract_with_gas_estimation):
     extract32_code = """
 @external
 def foo(inp: Bytes[32]) -> int128:
     return extract32(inp, 0, output_type=int128)
 
@@ -80,9 +94,7 @@
 
     assert c.baz(b"crow" * 8) == b"crow" * 8
     assert c.fop(b"crow" * 8) == b"crow" * 8
     assert c.foq(b"\x00" * 12 + b"3" * 20) == "0x" + "3" * 40
 
     with tx_failed():
         c.foq(b"crow" * 8)
-
-    print("Passed extract32 test")
```

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_floor.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_floor.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_is_contract.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_is_contract.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_keccak256.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_keccak256.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 @external
 def bar() -> bytes32:
     return keccak256("inp")
     """
 
     c = get_contract_with_gas_estimation(hash_code)
     for inp in (b"", b"cow", b"s" * 31, b"\xff" * 32, b"\n" * 33, b"g" * 64, b"h" * 65):
-        assert "0x" + c.foo(inp).hex() == keccak(inp).hex()
+        assert c.foo(inp) == keccak(inp)
 
-    assert "0x" + c.bar().hex() == keccak(b"inp").hex()
-    assert "0x" + c.foob().hex() == keccak(b"inp").hex()
+    assert c.bar() == keccak(b"inp")
+    assert c.foob() == keccak(b"inp")
 
 
 def test_hash_code2(get_contract_with_gas_estimation):
     hash_code2 = """
 @external
 def foo(inp: Bytes[100]) -> bool:
     return keccak256(inp) == keccak256("badminton")
@@ -92,22 +92,22 @@
 BAR: constant(bytes32) = keccak256(FOO)
 @external
 def foo() -> bytes32:
     x: bytes32 = BAR
     return x
     """
     c = get_contract_with_gas_estimation(code)
-    assert "0x" + c.foo().hex() == keccak(hex_to_int(hex_val).to_bytes(32, "big")).hex()
+    assert c.foo() == keccak(hex_to_int(hex_val).to_bytes(32, "big"))
 
 
 def test_hash_constant_string(get_contract_with_gas_estimation, keccak):
     str_val = "0x1234567890123456789012345678901234567890123456789012345678901234"
     code = f"""
 FOO: constant(String[66]) = "{str_val}"
 BAR: constant(bytes32) = keccak256(FOO)
 @external
 def foo() -> bytes32:
     x: bytes32 = BAR
     return x
     """
     c = get_contract_with_gas_estimation(code)
-    assert "0x" + c.foo().hex() == keccak(str_val.encode()).hex()
+    assert c.foo() == keccak(str_val.encode())
```

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_length.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_length.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_method_id.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_minmax.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_minmax_value.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_mulmod.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_raw_call.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_send.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_sha256.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_sha256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_slice.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_slice.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import hypothesis.strategies as st
 import pytest
 from hypothesis import given, settings
 
-from vyper.compiler.settings import OptimizationLevel
+from vyper.compiler import compile_code
+from vyper.compiler.settings import OptimizationLevel, Settings
+from vyper.evm.opcodes import version_check
 from vyper.exceptions import ArgumentException, TypeMismatch
 
 _fun_bytes32_bounds = [(0, 32), (3, 29), (27, 5), (0, 5), (5, 3), (30, 2)]
 
 
 def _generate_bytes(length):
     return bytes(list(range(length)))
@@ -28,23 +30,28 @@
 
 # note: optimization boundaries at 32, 64 and 320 depending on mode
 _draw_1024 = st.integers(min_value=0, max_value=1024)
 _draw_1024_1 = st.integers(min_value=1, max_value=1024)
 _bytes_1024 = st.binary(min_size=0, max_size=1024)
 
 
+def _fail_contract(code, opt_level, exceptions):
+    settings = Settings(optimize=opt_level)
+    with pytest.raises(exceptions):
+        compile_code(code, settings)
+
+
 @pytest.mark.parametrize("use_literal_start", (True, False))
 @pytest.mark.parametrize("use_literal_length", (True, False))
 @pytest.mark.parametrize("opt_level", list(OptimizationLevel))
 @given(start=_draw_1024, length=_draw_1024, length_bound=_draw_1024_1, bytesdata=_bytes_1024)
 @settings(max_examples=100)
 @pytest.mark.fuzzing
 def test_slice_immutable(
     get_contract,
-    assert_compile_failed,
     tx_failed,
     opt_level,
     bytesdata,
     start,
     use_literal_start,
     length,
     use_literal_length,
@@ -72,51 +79,63 @@
 
     if (
         (start + length > length_bound and use_literal_start and use_literal_length)
         or (use_literal_length and length > length_bound)
         or (use_literal_start and start > length_bound)
         or (use_literal_length and length == 0)
     ):
-        assert_compile_failed(lambda: _get_contract(), ArgumentException)
+        _fail_contract(code, opt_level, ArgumentException)
+
     elif start + length > len(bytesdata) or (len(bytesdata) > length_bound):
         # deploy fail
         with tx_failed():
             _get_contract()
     else:
         c = _get_contract()
         assert c.do_splice() == bytesdata[start : start + length]
 
 
-@pytest.mark.parametrize("location", ("storage", "calldata", "memory", "literal", "code"))
+@pytest.mark.parametrize(
+    "location", ["storage", "transient", "calldata", "memory", "literal", "code"]
+)
 @pytest.mark.parametrize("use_literal_start", (True, False))
 @pytest.mark.parametrize("use_literal_length", (True, False))
 @pytest.mark.parametrize("opt_level", list(OptimizationLevel))
 @given(start=_draw_1024, length=_draw_1024, length_bound=_draw_1024_1, bytesdata=_bytes_1024)
 @settings(max_examples=100)
 @pytest.mark.fuzzing
 def test_slice_bytes_fuzz(
     get_contract,
-    assert_compile_failed,
     tx_failed,
     opt_level,
     location,
     bytesdata,
     start,
     use_literal_start,
     length,
     use_literal_length,
     length_bound,
 ):
+    if location == "transient" and not version_check(begin="cancun"):
+        pytest.skip(
+            "Skipping test as storage_location is 'transient' and EVM version is pre-Cancun"
+        )
     preamble = ""
     if location == "memory":
         spliced_code = f"foo: Bytes[{length_bound}] = inp"
         foo = "foo"
     elif location == "storage":
         preamble = f"""
 foo: Bytes[{length_bound}]
+         """
+        spliced_code = "self.foo = inp"
+        foo = "self.foo"
+    elif location == "transient":
+        preamble = f"""
+foo: transient(Bytes[{length_bound}])
         """
         spliced_code = "self.foo = inp"
         foo = "self.foo"
     elif location == "code":
         preamble = f"""
 IMMUTABLE_BYTES: immutable(Bytes[{length_bound}])
 @deploy
@@ -169,32 +188,46 @@
     compile_time_oob = (
         (use_literal_length and (length > input_bound or length == 0))
         or (use_literal_start and start > input_bound)
         or (use_literal_start and use_literal_length and start + length > input_bound)
     )
 
     if compile_time_oob or slice_output_too_large:
-        assert_compile_failed(lambda: _get_contract(), (ArgumentException, TypeMismatch))
+        _fail_contract(code, opt_level, (ArgumentException, TypeMismatch))
+
     elif location == "code" and len(bytesdata) > length_bound:
         # deploy fail
         with tx_failed():
             _get_contract()
     elif end > len(bytesdata) or len(bytesdata) > length_bound:
         c = _get_contract()
         with tx_failed():
             c.do_slice(bytesdata, start, length)
     else:
         c = _get_contract()
         assert c.do_slice(bytesdata, start, length) == bytesdata[start:end], code
 
 
-def test_slice_private(get_contract):
+@pytest.mark.parametrize("location", ["storage", "transient"])
+def test_slice_private(get_contract, location):
+    if location == "transient" and not version_check(begin="cancun"):
+        pytest.skip(
+            "Skipping test as storage_location is 'transient' and EVM version is pre-Cancun"
+        )
+
     # test there are no buffer overruns in the slice function
-    code = """
-bytez: public(String[12])
+    if location == "storage":
+        decl = "bytez: public(String[12])"
+    elif location == "transient":
+        decl = "bytez: public(transient(String[12]))"
+    else:
+        raise Exception("unreachable")
+
+    code = f"""
+{decl}
 
 @internal
 def _slice(start: uint256, length: uint256):
     self.bytez = slice(self.bytez, start, length)
 
 @external
 def foo(x: uint256, y: uint256) -> (uint256, String[12]):
@@ -431,7 +464,70 @@
 @pytest.mark.parametrize("code,result", code_bytes32_calldata_extended)
 def test_slice_bytes32_calldata_extended(get_contract, code, result):
     c = get_contract(code)
     assert (
         c.bar(3, "0x0001020304050607080910111213141516171819202122232425262728293031", 5).hex()
         == result
     )
+
+
+# test cases crafted based on advisory GHSA-9x7f-gwxq-6f2c
+oob_fail_list = [
+    """
+d: public(Bytes[256])
+
+@external
+def do_slice():
+    x : uint256 = max_value(uint256)
+    self.d = b"\x01\x02\x03\x04\x05\x06"
+    assert len(slice(self.d, 1, x)) == max_value(uint256)
+    """,
+    """
+@external
+def do_slice():
+    x: uint256 = max_value(uint256)
+    # y == 0x3232323232323232323232323232323232323232323232323232323232323232
+    y: uint256 = 22704331223003175573249212746801550559464702875615796870481879217237868556850
+    z: uint96 = 1
+    if True:
+        placeholder : uint256[16] = [y, y, y, y, y, y, y, y, y, y, y, y, y, y, y, y]
+    s: String[32] = slice(uint2str(z), 1, x)
+    assert slice(s, 1, 2) == "22"
+    """,
+    """
+x: public(Bytes[64])
+secret: uint256
+
+@deploy
+def __init__():
+    self.x = empty(Bytes[64])
+    self.secret = 42
+
+@external
+def do_slice() -> Bytes[64]:
+    start: uint256 = max_value(uint256) - 63
+    return slice(self.x, start, 64)
+    """,
+    # tests bounds check in adhoc location calldata
+    """
+interface IFace:
+    def choose_value(_x: uint256, _y: uint256, _z: uint256, idx: uint256) -> Bytes[32]: nonpayable
+
+@external
+def choose_value(_x: uint256, _y: uint256, _z: uint256, idx: uint256) -> Bytes[32]:
+    assert idx % 32 == 4
+    return slice(msg.data, idx, 32)
+
+@external
+def do_slice():
+    idx: uint256 = max_value(uint256) - 27
+    ret: uint256 = _abi_decode(extcall IFace(self).choose_value(1, 2, 3, idx), uint256)
+    assert ret == 0
+    """,
+]
+
+
+@pytest.mark.parametrize("bad_code", oob_fail_list)
+def test_slice_buffer_oob_reverts(bad_code, get_contract, tx_failed):
+    c = get_contract(bad_code)
+    with tx_failed():
+        c.do_slice()
```

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_uint2str.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_uint2str.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_unary.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_unary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/codegen/test_unsafe_math.py` & `vyper-0.4.0b6/tests/functional/builtins/codegen/test_unsafe_math.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_abs.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_addmod_mulmod.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_addmod_mulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_bitwise.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_floor_ceil.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_floor_ceil.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_fold_as_wei_value.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_fold_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_keccak_sha.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_keccak_sha.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_len.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_min_max.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_min_max.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/builtins/folding/test_powmod.py` & `vyper-0.4.0b6/tests/functional/builtins/folding/test_powmod.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from hypothesis import given, settings
 from hypothesis import strategies as st
 
 from tests.utils import parse_and_fold
 
-st_uint256 = st.integers(min_value=0, max_value=2**256)
+st_uint256 = st.integers(min_value=0, max_value=(2**256 - 1))
 
 
 @pytest.mark.fuzzing
 @settings(max_examples=100)
 @given(a=st_uint256, b=st_uint256)
 def test_powmod_uint256(get_contract, a, b):
     source = """
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_default_function.py` & `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_default_function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_default_parameters.py` & `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_default_parameters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_erc20_abi.py` & `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_erc20_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_external_contract_calls.py` & `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_external_contract_calls.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     ArgumentException,
     InvalidType,
     StateAccessViolation,
     StructureException,
     UndeclaredDefinition,
     UnknownType,
 )
+from vyper.utils import method_id
 
 
 def test_external_contract_calls(get_contract, get_contract_with_gas_estimation):
     contract_1 = """
 @external
 def foo(arg1: int128) -> int128:
     return arg1
@@ -2492,49 +2493,49 @@
     assert c1.do_stuff(c2.address) == 1
 
 
 TEST_ADDR = b"".join(chr(i).encode("utf-8") for i in range(20)).hex()
 
 
 @pytest.mark.parametrize("typ,val", [("address", TEST_ADDR)])
-def test_calldata_clamp(w3, get_contract, tx_failed, keccak, typ, val):
+def test_calldata_clamp(w3, get_contract, tx_failed, typ, val):
     code = f"""
 @external
 def foo(a: {typ}):
     pass
     """
     c1 = get_contract(code)
-    sig = keccak(f"foo({typ})".encode()).hex()[:10]
+    sig = method_id(f"foo({typ})").hex()
     encoded = abi.encode(f"({typ})", (val,)).hex()
-    data = f"{sig}{encoded}"
+    data = f"0x{sig}{encoded}"
 
     # Static size is short by 1 byte
     malformed = data[:-2]
     with tx_failed():
         w3.eth.send_transaction({"to": c1.address, "data": malformed})
 
     # Static size is exact
     w3.eth.send_transaction({"to": c1.address, "data": data})
 
     # Static size exceeds by 1 byte, ok
     w3.eth.send_transaction({"to": c1.address, "data": data + "ff"})
 
 
 @pytest.mark.parametrize("typ,val", [("address", ([TEST_ADDR] * 3, "vyper"))])
-def test_dynamic_calldata_clamp(w3, get_contract, tx_failed, keccak, typ, val):
+def test_dynamic_calldata_clamp(w3, get_contract, tx_failed, typ, val):
     code = f"""
 @external
 def foo(a: DynArray[{typ}, 3], b: String[5]):
     pass
     """
 
     c1 = get_contract(code)
-    sig = keccak(f"foo({typ}[],string)".encode()).hex()[:10]
+    sig = method_id(f"foo({typ}[],string)").hex()
     encoded = abi.encode(f"({typ}[],string)", val).hex()
-    data = f"{sig}{encoded}"
+    data = f"0x{sig}{encoded}"
 
     # Dynamic size is short by 1 byte
     malformed = data[:264]
     with tx_failed():
         w3.eth.send_transaction({"to": c1.address, "data": malformed})
 
     # Dynamic size is at least minimum (132 bytes * 2 + 2 (for 0x) = 266)
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py` & `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_modifiable_external_contract_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_return.py` & `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/calling_convention/test_self_call_struct.py` & `vyper-0.4.0b6/tests/functional/codegen/calling_convention/test_self_call_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/environment_variables/test_blockhash.py` & `vyper-0.4.0b6/tests/functional/codegen/environment_variables/test_blockhash.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_nonreentrant.py` & `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_nonreentrant.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_payable.py` & `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_private.py` & `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_private.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_public.py` & `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/decorators/test_view.py` & `vyper-0.4.0b6/tests/functional/codegen/features/decorators/test_view.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pytest
+
 from vyper.exceptions import FunctionDeclarationException
 
 
 def test_constant_test(get_contract_with_gas_estimation_for_constants):
     constant_test = """
 @external
 @view
@@ -11,14 +13,28 @@
 
     c = get_contract_with_gas_estimation_for_constants(constant_test)
     assert c.foo() == 5
 
     print("Passed constant function test")
 
 
+@pytest.mark.requires_evm_version("cancun")
+def test_transient_test(get_contract):
+    code = """
+x: transient(uint256)
+
+@external
+@view
+def foo() -> uint256:
+    return self.x
+    """
+    c = get_contract(code)
+    assert c.foo() == 0
+
+
 def test_invalid_constant_and_payable(
     get_contract_with_gas_estimation_for_constants, assert_compile_failed
 ):
     code = """
 @external
 @payable
 @view
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_break.py` & `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_break.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_continue.py` & `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_continue.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_for_in_list.py` & `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_for_in_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_for_range.py` & `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/iteration/test_range_in.py` & `vyper-0.4.0b6/tests/functional/codegen/features/iteration/test_range_in.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_assert.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_assert.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     assert tx_receipt["status"] == 0
     # Checks for gas refund from revert
     assert tx_receipt["gasUsed"] < gas_sent
 
 
 def test_assert_reason(w3, get_contract_with_gas_estimation, tx_failed, memory_mocker):
     code = """
+err: String[32]
+
 @external
 def test(a: int128) -> int128:
     assert a > 1, "larger than one please"
     return 1 + a
 
 @external
 def test2(a: int128, b: int128, extra_reason: String[32]) -> int128:
@@ -39,14 +41,25 @@
     assert a > 1, "a is not large enough"
     assert b == 1, concat("b may only be 1", extra_reason)
     return a + b + c
 
 @external
 def test3(reason_str: String[32]):
     raise reason_str
+
+@external
+def test4(a: int128, reason_str: String[32]) -> int128:
+    self.err = reason_str
+    assert a > 1, self.err
+    return 1 + a
+
+@external
+def test5(reason_str: String[32]):
+    self.err = reason_str
+    raise self.err
     """
     c = get_contract_with_gas_estimation(code)
 
     assert c.test(2) == 3
     with pytest.raises(TransactionFailed) as e_info:
         c.test(0)
 
@@ -62,14 +75,23 @@
     # return correct value
     assert c.test2(5, 1, "") == 17
 
     with pytest.raises(TransactionFailed) as e_info:
         c.test3("An exception")
     assert _fixup_err_str(e_info.value.args[0]) == "An exception"
 
+    assert c.test4(2, "msg") == 3
+    with pytest.raises(TransactionFailed) as e_info:
+        c.test4(0, "larger than one again please")
+    assert _fixup_err_str(e_info.value.args[0]) == "larger than one again please"
+
+    with pytest.raises(TransactionFailed) as e_info:
+        c.test5("A storage exception")
+    assert _fixup_err_str(e_info.value.args[0]) == "A storage exception"
+
 
 invalid_code = [
     """
 @external
 def test(a: int128) -> int128:
     assert a > 1, ""
     return 1 + a
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_assert_unreachable.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_assert_unreachable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_assignment.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_assignment.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_bytes_map_keys.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_bytes_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_clampers.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_clampers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from decimal import Decimal
 
 import pytest
 from eth.codecs import abi
 from eth_utils import keccak
 
-from vyper.evm.opcodes import EVM_VERSIONS
+from vyper.exceptions import StackTooDeep
 from vyper.utils import int_bounds
 
 
 def _make_tx(w3, address, signature, values):
     # helper function to broadcast transactions that fail clamping check
     sig = keccak(signature.encode()).hex()[:8]
     data = "".join(int(i).to_bytes(32, "big", signed=i < 0).hex() for i in values)
@@ -79,34 +79,32 @@
     c = get_contract_with_gas_estimation(clamper_test_code, *[b"cat"])
     assert c.get_foo() == b"cat"
 
     with tx_failed():
         get_contract_with_gas_estimation(clamper_test_code, *[b"cats"])
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("n", list(range(1, 33)))
-def test_bytes_m_clamper_passing(w3, get_contract, n, evm_version):
+def test_bytes_m_clamper_passing(w3, get_contract, n):
     values = [b"\xff" * (i + 1) for i in range(n)]
 
     code = f"""
 @external
 def foo(s: bytes{n}) -> bytes{n}:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     for v in values:
         v = v.ljust(n, b"\x00")
         assert c.foo(v) == v
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("n", list(range(1, 32)))  # bytes32 always passes
-def test_bytes_m_clamper_failing(w3, get_contract, tx_failed, n, evm_version):
+def test_bytes_m_clamper_failing(w3, get_contract, tx_failed, n):
     values = []
     values.append(b"\x00" * n + b"\x80")  # just one bit set
     values.append(b"\xff" * n + b"\x80")  # n*8 + 1 bits set
     values.append(b"\x00" * 31 + b"\x01")  # bytes32
     values.append(b"\xff" * 32)  # bytes32
     values.append(bytes(range(32)))  # 0x00010203..1f
     values.append(bytes(range(1, 33)))  # 0x01020304..a0
@@ -114,198 +112,187 @@
 
     code = f"""
 @external
 def foo(s: bytes{n}) -> bytes{n}:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     for v in values:
         # munge for `_make_tx`
         with tx_failed():
             int_value = int.from_bytes(v, byteorder="big")
             _make_tx(w3, c.address, f"foo(bytes{n})", [int_value])
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("n", list(range(32)))
-def test_sint_clamper_passing(w3, get_contract, n, evm_version):
+def test_sint_clamper_passing(w3, get_contract, n):
     bits = 8 * (n + 1)
     lo, hi = int_bounds(True, bits)
     values = [-1, 0, 1, lo, hi]
     code = f"""
 @external
 def foo(s: int{bits}) -> int{bits}:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     for v in values:
         assert c.foo(v) == v
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("n", list(range(31)))  # int256 does not clamp
-def test_sint_clamper_failing(w3, tx_failed, get_contract, n, evm_version):
+def test_sint_clamper_failing(w3, tx_failed, get_contract, n):
     bits = 8 * (n + 1)
     lo, hi = int_bounds(True, bits)
     values = [-(2**255), 2**255 - 1, lo - 1, hi + 1]
     code = f"""
 @external
 def foo(s: int{bits}) -> int{bits}:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     for v in values:
         with tx_failed():
             _make_tx(w3, c.address, f"foo(int{bits})", [v])
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("value", [True, False])
-def test_bool_clamper_passing(w3, get_contract, value, evm_version):
+def test_bool_clamper_passing(w3, get_contract, value):
     code = """
 @external
 def foo(s: bool) -> bool:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     assert c.foo(value) == value
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("value", [2, 3, 4, 8, 16, 2**256 - 1])
-def test_bool_clamper_failing(w3, tx_failed, get_contract, value, evm_version):
+def test_bool_clamper_failing(w3, tx_failed, get_contract, value):
     code = """
 @external
 def foo(s: bool) -> bool:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     with tx_failed():
         _make_tx(w3, c.address, "foo(bool)", [value])
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("value", [0] + [2**i for i in range(5)])
-def test_flag_clamper_passing(w3, get_contract, value, evm_version):
+def test_flag_clamper_passing(w3, get_contract, value):
     code = """
 flag Roles:
     USER
     STAFF
     ADMIN
     MANAGER
     CEO
 
 @external
 def foo(s: Roles) -> Roles:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     assert c.foo(value) == value
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("value", [2**i for i in range(5, 256)])
-def test_flag_clamper_failing(w3, tx_failed, get_contract, value, evm_version):
+def test_flag_clamper_failing(w3, tx_failed, get_contract, value):
     code = """
 flag Roles:
     USER
     STAFF
     ADMIN
     MANAGER
     CEO
 
 @external
 def foo(s: Roles) -> Roles:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     with tx_failed():
         _make_tx(w3, c.address, "foo(uint256)", [value])
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("n", list(range(32)))
-def test_uint_clamper_passing(w3, get_contract, evm_version, n):
+def test_uint_clamper_passing(w3, get_contract, n):
     bits = 8 * (n + 1)
     values = [0, 1, 2**bits - 1]
     code = f"""
 @external
 def foo(s: uint{bits}) -> uint{bits}:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     for v in values:
         assert c.foo(v) == v
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("n", list(range(31)))  # uint256 has no failing cases
-def test_uint_clamper_failing(w3, tx_failed, get_contract, evm_version, n):
+def test_uint_clamper_failing(w3, tx_failed, get_contract, n):
     bits = 8 * (n + 1)
     values = [-1, -(2**255), 2**bits]
     code = f"""
 @external
 def foo(s: uint{bits}) -> uint{bits}:
     return s
     """
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     for v in values:
         with tx_failed():
             _make_tx(w3, c.address, f"foo(uint{bits})", [v])
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize(
     "value,expected",
     [
         ("0x0000000000000000000000000000000000000000", None),
         (
             "0x0000000000000000000000000000000000000001",
             "0x0000000000000000000000000000000000000001",
         ),
         (
             "0xFFfFfFffFFfffFFfFFfFFFFFffFFFffffFfFFFfF",
             "0xFFfFfFffFFfffFFfFFfFFFFFffFFFffffFfFFFfF",
         ),
     ],
 )
-def test_address_clamper_passing(w3, get_contract, value, expected, evm_version):
+def test_address_clamper_passing(w3, get_contract, value, expected):
     code = """
 @external
 def foo(s: address) -> address:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     assert c.foo(value) == expected
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize("value", [2**160, 2**256 - 1])
-def test_address_clamper_failing(w3, tx_failed, get_contract, value, evm_version):
+def test_address_clamper_failing(w3, tx_failed, get_contract, value):
     code = """
 @external
 def foo(s: address) -> address:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
     with tx_failed():
         _make_tx(w3, c.address, "foo(address)", [value])
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize(
     "value",
     [
         0,
         1,
         -1,
         Decimal(2**167 - 1) / 10**10,
@@ -317,44 +304,43 @@
         "0.9999999999",
         "-0.0000000001",
         "-0.9999999999",
         "18707220957835557353007165858768422651595.9365500927",  # 2**167 - 1e-10
         "-18707220957835557353007165858768422651595.9365500928",  # -2**167
     ],
 )
-def test_decimal_clamper_passing(get_contract, value, evm_version):
+def test_decimal_clamper_passing(get_contract, value):
     code = """
 @external
 def foo(s: decimal) -> decimal:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
 
     assert c.foo(Decimal(value)) == Decimal(value)
 
 
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
 @pytest.mark.parametrize(
     "value",
     [
         2**167,
         -(2**167 + 1),
         187072209578355573530071658587684226515959365500928,  # 2 ** 167
         -187072209578355573530071658587684226515959365500929,  # - (2 ** 127 - 1e-10)
     ],
 )
-def test_decimal_clamper_failing(w3, tx_failed, get_contract, value, evm_version):
+def test_decimal_clamper_failing(w3, tx_failed, get_contract, value):
     code = """
 @external
 def foo(s: decimal) -> decimal:
     return s
     """
 
-    c = get_contract(code, evm_version=evm_version)
+    c = get_contract(code)
 
     with tx_failed():
         _make_tx(w3, c.address, "foo(fixed168x10)", [value])
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
 def test_int128_array_clamper_passing(w3, get_contract, value):
@@ -517,14 +503,15 @@
     data = _make_dynarray_data(32, 10, values)
     signature = "foo(int128[])"
     with tx_failed():
         _make_invalid_dynarray_tx(w3, c.address, signature, data)
 
 
 @pytest.mark.parametrize("value", [0, 1, -1, 2**127 - 1, -(2**127)])
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_multidimension_dynarray_clamper_passing(w3, get_contract, value):
     code = """
 @external
 def foo(
     a: uint256,
     b: DynArray[DynArray[DynArray[DynArray[int128, 5], 6], 7], 8],
     c: uint256
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_comparison.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_comparison.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_conditionals.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_constructor.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_constructor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pytest
 from web3.exceptions import ValidationError
 
+from vyper.exceptions import StackTooDeep
+
 
 def test_init_argument_test(get_contract_with_gas_estimation):
     init_argument_test = """
 moose: int128
 
 @deploy
 def __init__(_moose: int128):
@@ -159,14 +161,15 @@
 def get_foo() -> uint256:
     return self.foo
     """
     c = get_contract_with_gas_estimation(code, *[[[3, 5, 7], [11, 13, 17], [19, 23, 29]]])
     assert c.get_foo() == 39
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_nested_dynamic_array_constructor_arg_2(w3, get_contract_with_gas_estimation):
     code = """
 foo: int128
 
 @deploy
 def __init__(x: DynArray[DynArray[DynArray[int128, 3], 3], 3]):
     self.foo = x[0][1][2] * x[1][1][1] * x[2][1][0] - x[0][0][0] - x[1][1][1] - x[2][2][2]
@@ -204,14 +207,15 @@
 def get_foo() -> DynArray[DynArray[uint256, 3], 3]:
     return self.foo
     """
     c = get_contract_with_gas_estimation(code, *[37, 41, 73])
     assert c.get_foo() == [[37, 41, 73], [37041, 41073, 73037], [146, 123, 148]]
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_initialise_nested_dynamic_array_2(w3, get_contract_with_gas_estimation):
     code = """
 foo: DynArray[DynArray[DynArray[int128, 3], 3], 3]
 
 @deploy
 def __init__(x: int128, y: int128, z: int128):
     self.foo = [
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_immutable.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_immutable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 from vyper.compiler.settings import OptimizationLevel
+from vyper.exceptions import StackTooDeep
 
 
 @pytest.mark.parametrize(
     "typ,value",
     [
         ("uint256", 42),
         ("int256", -(2**200)),
@@ -194,14 +195,15 @@
     values = (100, 42, 23230)
     expected_values = [[100, 42, 23230], [42, 100, 23230], [23230, 42, 100]]
     c = get_contract(code, *values)
     assert c.get_my_list() == expected_values
     assert c.get_idx_two() == expected_values[2][2]
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_nested_dynarray_immutable(get_contract):
     code = """
 my_list: immutable(DynArray[DynArray[DynArray[int128, 3], 3], 3])
 
 @deploy
 def __init__(x: int128, y: int128, z: int128):
     my_list = [
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_init.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_internal_call.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_internal_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_logging.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog()", "utf-8"))
 
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [],
         "anonymous": False,
         "type": "event",
     }
@@ -62,15 +62,15 @@
 
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
     event_id = keccak(bytes("MyLog(bytes)", "utf-8"))
 
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [{"type": "bytes", "name": "arg1", "indexed": True}],
         "anonymous": False,
         "type": "event",
     }
@@ -92,15 +92,15 @@
 
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog(int128,bool,address)", "utf-8"))
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [
             {"type": "int128", "name": "arg1", "indexed": True},
             {"type": "bool", "name": "arg2", "indexed": True},
             {"type": "address", "name": "arg3", "indexed": True},
@@ -168,16 +168,16 @@
     tx_hash1 = c.foo(transact={})
     tx_hash2 = c.bar(transact={})
     receipt1 = tester.get_transaction_receipt(tx_hash1.hex())
     receipt2 = tester.get_transaction_receipt(tx_hash2.hex())
 
     event_id = keccak(bytes("MyLog(int128,address)", "utf-8"))
     # Event id is always the first topic
-    assert receipt1["logs"][0]["topics"][0] == event_id.hex()
-    assert receipt2["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt1["logs"][0]["topics"][0] == "0x" + event_id.hex()
+    assert receipt2["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [
             {"type": "int128", "name": "arg1", "indexed": True},
             {"type": "address", "name": "arg2", "indexed": True},
         ],
@@ -220,15 +220,15 @@
 
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog(int128)", "utf-8"))
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [{"type": "int128", "name": "arg1", "indexed": False}],
         "anonymous": False,
         "type": "event",
     }
@@ -256,15 +256,15 @@
 
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog(int128[2],uint256[3],int128[2][2])", "utf-8"))
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
 
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [
             {"type": "int128[2]", "name": "arg1", "indexed": False},
             {"type": "uint256[3]", "name": "arg2", "indexed": False},
@@ -299,15 +299,15 @@
 
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(b"bar", b"foo", transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog(bytes,bytes,bytes)", "utf-8"))
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [
             {"type": "bytes", "name": "arg1", "indexed": False},
             {"type": "bytes", "name": "arg2", "indexed": True},
             {"type": "bytes", "name": "arg3", "indexed": False},
@@ -337,15 +337,15 @@
 
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(b"hello", transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog(bytes)", "utf-8"))
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "anonymous": False,
         "inputs": [{"indexed": False, "name": "arg1", "type": "bytes"}],
         "name": "MyLog",
         "type": "event",
     }
@@ -366,15 +366,15 @@
 
     c = get_contract(loggy_code)
     tx_hash = c.foo(b"hello", transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog(bytes)", "utf-8"))
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "anonymous": False,
         "inputs": [{"indexed": False, "name": "arg1", "type": "bytes"}],
         "name": "MyLog",
         "type": "event",
     }
@@ -402,15 +402,15 @@
 
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog(int128,bytes,bytes,address,address,uint256)", "utf-8"))
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [
             {"type": "int128", "name": "arg1", "indexed": False},
             {"type": "bytes", "name": "arg2", "indexed": False},
             {"type": "bytes", "name": "arg3", "indexed": False},
@@ -449,15 +449,15 @@
 
     c = get_contract_with_gas_estimation(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     event_id = keccak(bytes("MyLog(int128,bytes)", "utf-8"))
     # Event id is always the first topic
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "anonymous": False,
         "inputs": [
             {"indexed": True, "name": "arg1", "type": "int128"},
             {"indexed": False, "name": "arg2", "type": "bytes"},
         ],
@@ -502,16 +502,16 @@
 
     logs1 = receipt["logs"][0]
     logs2 = receipt["logs"][1]
     event_id1 = keccak(bytes("MyLog(int128,bytes)", "utf-8"))
     event_id2 = keccak(bytes("YourLog(address,(uint256,bytes,(string,fixed168x10)))", "utf-8"))
 
     # Event id is always the first topic
-    assert logs1["topics"][0] == event_id1.hex()
-    assert logs2["topics"][0] == event_id2.hex()
+    assert logs1["topics"][0] == "0x" + event_id1.hex()
+    assert logs2["topics"][0] == "0x" + event_id2.hex()
     # Event abi is created correctly
     assert c._classic_contract.abi[0] == {
         "name": "MyLog",
         "inputs": [
             {"type": "int128", "name": "arg1", "indexed": True},
             {"type": "bytes", "name": "arg2", "indexed": False},
         ],
@@ -1077,15 +1077,15 @@
 
     c = get_contract(loggy_code)
     tx_hash = c.foo(b"bar", 1, "weird", transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     # Event id is always the first topic
     event_id = keccak(b"MyLog(bytes,int128,string)")
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
 
     topic1 = f"0x{keccak256(b'bar').hex()}"
     assert receipt["logs"][0]["topics"][1] == topic1
 
     topic2 = f"0x{abi.encode('int128', 1).hex()}"
     assert receipt["logs"][0]["topics"][2] == topic2
 
@@ -1122,15 +1122,15 @@
 
     c = get_contract(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     # Event id is always the first topic
     event_id = keccak(b"MyLog(bytes,int128,string)")
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
 
     topic1 = f"0x{keccak256(b'potato').hex()}"
     assert receipt["logs"][0]["topics"][1] == topic1
 
     topic2 = f"0x{abi.encode('int128', -777).hex()}"
     assert receipt["logs"][0]["topics"][2] == topic2
 
@@ -1176,15 +1176,15 @@
     c = get_contract(loggy_code)
     c.setter(b"zonk", -2109, "yessir", transact={})
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     # Event id is always the first topic
     event_id = keccak(b"MyLog(bytes,int128,string)")
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
 
     topic1 = f"0x{keccak256(b'zonk').hex()}"
     assert receipt["logs"][0]["topics"][1] == topic1
 
     topic2 = f"0x{abi.encode('int128', -2109).hex()}"
     assert receipt["logs"][0]["topics"][2] == topic2
 
@@ -1218,15 +1218,15 @@
 
     c = get_contract(loggy_code)
     tx_hash = c.foo(transact={})
     receipt = tester.get_transaction_receipt(tx_hash.hex())
 
     # Event id is always the first topic
     event_id = keccak(b"MyLog(bytes,int128,string)")
-    assert receipt["logs"][0]["topics"][0] == event_id.hex()
+    assert receipt["logs"][0]["topics"][0] == "0x" + event_id.hex()
 
     topic1 = f"0x{keccak256(b'wow').hex()}"
     assert receipt["logs"][0]["topics"][1] == topic1
 
     topic2 = f"0x{abi.encode('int128', 666).hex()}"
     assert receipt["logs"][0]["topics"][2] == topic2
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_logging_bytes_extended.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_logging_bytes_extended.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_logging_from_call.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_logging_from_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_memory_dealloc.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_memory_dealloc.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_packing.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_packing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_reverting.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_reverting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_short_circuiting.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_short_circuiting.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_string_map_keys.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_string_map_keys.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/features/test_ternary.py` & `vyper-0.4.0b6/tests/functional/codegen/features/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/integration/test_crowdfund.py` & `vyper-0.4.0b6/tests/functional/codegen/integration/test_crowdfund.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/integration/test_escrow.py` & `vyper-0.4.0b6/tests/functional/codegen/integration/test_escrow.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/modules/test_events.py` & `vyper-0.4.0b6/tests/functional/codegen/modules/test_events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/modules/test_exports.py` & `vyper-0.4.0b6/tests/functional/codegen/modules/test_exports.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import pytest
-
-
 def test_simple_export(make_input_bundle, get_contract):
     lib1 = """
 @external
 def foo() -> uint256:
     return 5
     """
     main = """
@@ -127,17 +124,15 @@
     """
     input_bundle = make_input_bundle({"lib1.vy": lib1, "lib2.vy": lib2})
     c = get_contract(main, input_bundle=input_bundle)
 
     assert c.foo() == 5
 
 
-# not sure if this one should work
-@pytest.mark.xfail(reason="ambiguous spec")
-def test_recursive_export(make_input_bundle, get_contract):
+def test_transitive_export(make_input_bundle, get_contract):
     lib1 = """
 @external
 def foo() -> uint256:
     return 5
     """
     lib2 = """
 import lib1
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/modules/test_interface_imports.py` & `vyper-0.4.0b6/tests/functional/codegen/modules/test_interface_imports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/modules/test_module_constants.py` & `vyper-0.4.0b6/tests/functional/codegen/modules/test_module_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/modules/test_module_variables.py` & `vyper-0.4.0b6/tests/functional/codegen/modules/test_module_variables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/modules/test_stateless_functions.py` & `vyper-0.4.0b6/tests/functional/codegen/modules/test_stateless_functions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/storage_variables/test_getters.py` & `vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/storage_variables/test_setters.py` & `vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_setters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/storage_variables/test_storage_variable.py` & `vyper-0.4.0b6/tests/functional/codegen/storage_variables/test_storage_variable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/test_call_graph_stability.py` & `vyper-0.4.0b6/tests/functional/codegen/test_call_graph_stability.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/test_interfaces.py` & `vyper-0.4.0b6/tests/functional/codegen/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/test_selector_table.py` & `vyper-0.4.0b6/tests/functional/codegen/test_selector_table.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/test_selector_table_stability.py` & `vyper-0.4.0b6/tests/functional/codegen/test_selector_table_stability.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     code = "\n".join(f"@external\ndef {name}():\n  pass" for name in function_names)
 
     output = compile_code(
         code, output_formats=["asm"], settings=Settings(optimize=OptimizationLevel.CODESIZE)
     )
 
     # test that the selector table data is stable across different runs
-    # (tox should provide different PYTHONHASHSEEDs).
+    # (xdist should provide different PYTHONHASHSEEDs).
     expected_asm = """{ DATA _sym_BUCKET_HEADERS b\'\\x0bB\' _sym_bucket_0 b\'\\n\' b\'+\\x8d\' _sym_bucket_1 b\'\\x0c\' b\'\\x00\\x85\' _sym_bucket_2 b\'\\x08\' } { DATA _sym_bucket_1 b\'\\xd8\\xee\\xa1\\xe8\' _sym_external 6 foo6()3639517672 b\'\\x05\' b\'\\xd2\\x9e\\xe0\\xf9\' _sym_external 0 foo0()3533627641 b\'\\x05\' b\'\\x05\\xf1\\xe0_\' _sym_external 2 foo2()99737695 b\'\\x05\' b\'\\x91\\t\\xb4{\' _sym_external 23 foo23()2433332347 b\'\\x05\' b\'np3\\x7f\' _sym_external 11 foo11()1852846975 b\'\\x05\' b\'&\\xf5\\x96\\xf9\' _sym_external 13 foo13()653629177 b\'\\x05\' b\'\\x04ga\\xeb\' _sym_external 14 foo14()73884139 b\'\\x05\' b\'\\x89\\x06\\xad\\xc6\' _sym_external 17 foo17()2298916294 b\'\\x05\' b\'\\xe4%\\xac\\xd1\' _sym_external 4 foo4()3827674321 b\'\\x05\' b\'yj\\x01\\xac\' _sym_external 7 foo7()2036990380 b\'\\x05\' b\'\\xf1\\xe6K\\xe5\' _sym_external 29 foo29()4058401765 b\'\\x05\' b\'\\xd2\\x89X\\xb8\' _sym_external 3 foo3()3532216504 b\'\\x05\' } { DATA _sym_bucket_2 b\'\\x06p\\xffj\' _sym_external 25 foo25()108068714 b\'\\x05\' b\'\\x964\\x99I\' _sym_external 24 foo24()2520029513 b\'\\x05\' b\'s\\x81\\xe7\\xc1\' _sym_external 10 foo10()1937893313 b\'\\x05\' b\'\\x85\\xad\\xc11\' _sym_external 28 foo28()2242756913 b\'\\x05\' b\'\\xfa"\\xb1\\xed\' _sym_external 5 foo5()4196577773 b\'\\x05\' b\'A\\xe7[\\x05\' _sym_external 22 foo22()1105681157 b\'\\x05\' b\'\\xd3\\x89U\\xe8\' _sym_external 1 foo1()3548993000 b\'\\x05\' b\'hL\\xf8\\xf3\' _sym_external 20 foo20()1749874931 b\'\\x05\' } { DATA _sym_bucket_0 b\'\\xee\\xd9\\x1d\\xe3\' _sym_external 9 foo9()4007206371 b\'\\x05\' b\'a\\xbc\\x1ch\' _sym_external 16 foo16()1639717992 b\'\\x05\' b\'\\xd3*\\xa7\\x0c\' _sym_external 21 foo21()3542787852 b\'\\x05\' b\'\\x18iG\\xd9\' _sym_external 19 foo19()409552857 b\'\\x05\' b\'\\n\\xf1\\xf9\\x7f\' _sym_external 18 foo18()183630207 b\'\\x05\' b\')\\xda\\xd7`\' _sym_external 27 foo27()702207840 b\'\\x05\' b\'2\\xf6\\xaa\\xda\' _sym_external 12 foo12()855026394 b\'\\x05\' b\'\\xbe\\xb5\\x05\\xf5\' _sym_external 15 foo15()3199534581 b\'\\x05\' b\'\\xfc\\xa7_\\xe6\' _sym_external 8 foo8()4238827494 b\'\\x05\' b\'\\x1b\\x12C8\' _sym_external 26 foo26()454181688 b\'\\x05\' } }"""  # noqa: E501
     assert expected_asm in output["asm"]
 
 
 def test_sparse_jumptable_stability():
     function_names = [f"foo{i}()" for i in range(30)]
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_constants.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_decimals.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_decimals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,445 +1,439 @@
 00000000: 696d 706f 7274 2077 6172 6e69 6e67 730a  import warnings.
 00000010: 6672 6f6d 2064 6563 696d 616c 2069 6d70  from decimal imp
-00000020: 6f72 7420 524f 554e 445f 444f 574e 2c20  ort ROUND_DOWN, 
-00000030: 4465 6369 6d61 6c2c 2067 6574 636f 6e74  Decimal, getcont
-00000040: 6578 740a 0a69 6d70 6f72 7420 7079 7465  ext..import pyte
-00000050: 7374 0a0a 6672 6f6d 2076 7970 6572 2069  st..from vyper i
-00000060: 6d70 6f72 7420 636f 6d70 696c 655f 636f  mport compile_co
-00000070: 6465 0a66 726f 6d20 7679 7065 722e 6578  de.from vyper.ex
-00000080: 6365 7074 696f 6e73 2069 6d70 6f72 7420  ceptions import 
-00000090: 280a 2020 2020 4465 6369 6d61 6c4f 7665  (.    DecimalOve
-000000a0: 7272 6964 6545 7863 6570 7469 6f6e 2c0a  rrideException,.
-000000b0: 2020 2020 496e 7661 6c69 644f 7065 7261      InvalidOpera
-000000c0: 7469 6f6e 2c0a 2020 2020 4f76 6572 666c  tion,.    Overfl
-000000d0: 6f77 4578 6365 7074 696f 6e2c 0a20 2020  owException,.   
-000000e0: 2054 7970 654d 6973 6d61 7463 682c 0a29   TypeMismatch,.)
-000000f0: 0a66 726f 6d20 7679 7065 722e 7574 696c  .from vyper.util
-00000100: 7320 696d 706f 7274 2044 4543 494d 414c  s import DECIMAL
-00000110: 5f45 5053 494c 4f4e 2c20 5369 7a65 4c69  _EPSILON, SizeLi
-00000120: 6d69 7473 0a0a 0a64 6566 2074 6573 745f  mits...def test_
-00000130: 6465 6369 6d61 6c5f 6f76 6572 7269 6465  decimal_override
-00000140: 2829 3a0a 2020 2020 6765 7463 6f6e 7465  ():.    getconte
-00000150: 7874 2829 2e70 7265 6320 3d20 3738 2020  xt().prec = 78  
-00000160: 2320 7365 7474 696e 6720 7072 6563 2074  # setting prec t
-00000170: 6f20 3738 2069 7320 6f6b 0a0a 2020 2020  o 78 is ok..    
-00000180: 2320 636f 6e73 756d 6572 7320 6f66 2076  # consumers of v
-00000190: 7970 6572 2c20 6576 656e 2061 7320 6120  yper, even as a 
-000001a0: 6c69 6272 6172 792c 2061 7265 206e 6f74  library, are not
-000001b0: 2061 6c6c 6f77 6564 2074 6f20 7265 6475   allowed to redu
-000001c0: 6365 2044 6563 696d 616c 2070 7265 6369  ce Decimal preci
-000001d0: 7369 6f6e 0a20 2020 2077 6974 6820 7079  sion.    with py
-000001e0: 7465 7374 2e72 6169 7365 7328 4465 6369  test.raises(Deci
-000001f0: 6d61 6c4f 7665 7272 6964 6545 7863 6570  malOverrideExcep
-00000200: 7469 6f6e 293a 0a20 2020 2020 2020 2067  tion):.        g
-00000210: 6574 636f 6e74 6578 7428 292e 7072 6563  etcontext().prec
-00000220: 203d 2037 370a 0a20 2020 2077 6974 6820   = 77..    with 
-00000230: 7761 726e 696e 6773 2e63 6174 6368 5f77  warnings.catch_w
-00000240: 6172 6e69 6e67 7328 7265 636f 7264 3d54  arnings(record=T
-00000250: 7275 6529 2061 7320 773a 0a20 2020 2020  rue) as w:.     
-00000260: 2020 2067 6574 636f 6e74 6578 7428 292e     getcontext().
-00000270: 7072 6563 203d 2037 390a 2020 2020 2020  prec = 79.      
-00000280: 2020 2320 6368 6563 6b20 7761 726e 696e    # check warnin
-00000290: 6773 2077 6572 6520 6973 7375 6564 0a20  gs were issued. 
-000002a0: 2020 2020 2020 2061 7373 6572 7420 6c65         assert le
-000002b0: 6e28 7729 203d 3d20 310a 2020 2020 2020  n(w) == 1.      
-000002c0: 2020 6173 7365 7274 2028 0a20 2020 2020    assert (.     
-000002d0: 2020 2020 2020 2073 7472 2877 5b2d 315d         str(w[-1]
-000002e0: 2e6d 6573 7361 6765 2920 3d3d 2022 4368  .message) == "Ch
-000002f0: 616e 6769 6e67 2064 6563 696d 616c 7320  anging decimals 
-00000300: 7072 6563 6973 696f 6e20 636f 756c 6420  precision could 
-00000310: 6861 7665 2075 6e69 6e74 656e 6465 6420  have unintended 
-00000320: 7369 6465 2065 6666 6563 7473 2122 0a20  side effects!". 
-00000330: 2020 2020 2020 2029 0a0a 0a40 7079 7465         )...@pyte
-00000340: 7374 2e6d 6172 6b2e 7061 7261 6d65 7472  st.mark.parametr
-00000350: 697a 6528 226f 7022 2c20 5b22 2f2f 222c  ize("op", ["//",
-00000360: 2022 2a2a 222c 2022 2622 2c20 227c 222c   "**", "&", "|",
-00000370: 2022 5e22 5d29 0a64 6566 2074 6573 745f   "^"]).def test_
-00000380: 696e 7661 6c69 645f 6f70 7328 6f70 293a  invalid_ops(op):
-00000390: 0a20 2020 2063 6f64 6520 3d20 6622 2222  .    code = f"""
-000003a0: 0a40 6578 7465 726e 616c 0a64 6566 2066  .@external.def f
-000003b0: 6f6f 2878 3a20 6465 6369 6d61 6c2c 2079  oo(x: decimal, y
-000003c0: 3a20 6465 6369 6d61 6c29 202d 3e20 6465  : decimal) -> de
-000003d0: 6369 6d61 6c3a 0a20 2020 2072 6574 7572  cimal:.    retur
-000003e0: 6e20 7820 7b6f 707d 2079 0a20 2020 2022  n x {op} y.    "
-000003f0: 2222 0a20 2020 2077 6974 6820 7079 7465  "".    with pyte
-00000400: 7374 2e72 6169 7365 7328 496e 7661 6c69  st.raises(Invali
-00000410: 644f 7065 7261 7469 6f6e 293a 0a20 2020  dOperation):.   
-00000420: 2020 2020 2063 6f6d 7069 6c65 5f63 6f64       compile_cod
-00000430: 6528 636f 6465 290a 0a0a 4070 7974 6573  e(code)...@pytes
-00000440: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00000450: 7a65 2822 6f70 222c 205b 226e 6f74 225d  ze("op", ["not"]
-00000460: 290a 6465 6620 7465 7374 5f69 6e76 616c  ).def test_inval
-00000470: 6964 5f75 6e61 7279 5f6f 7073 286f 7029  id_unary_ops(op)
-00000480: 3a0a 2020 2020 636f 6465 203d 2066 2222  :.    code = f""
-00000490: 220a 4065 7874 6572 6e61 6c0a 6465 6620  ".@external.def 
-000004a0: 666f 6f28 783a 2064 6563 696d 616c 2920  foo(x: decimal) 
-000004b0: 2d3e 2064 6563 696d 616c 3a0a 2020 2020  -> decimal:.    
-000004c0: 7265 7475 726e 207b 6f70 7d20 780a 2020  return {op} x.  
-000004d0: 2020 2222 220a 2020 2020 7769 7468 2070    """.    with p
-000004e0: 7974 6573 742e 7261 6973 6573 2849 6e76  ytest.raises(Inv
-000004f0: 616c 6964 4f70 6572 6174 696f 6e29 3a0a  alidOperation):.
-00000500: 2020 2020 2020 2020 636f 6d70 696c 655f          compile_
-00000510: 636f 6465 2863 6f64 6529 0a0a 0a64 6566  code(code)...def
-00000520: 2071 7561 6e74 697a 6528 783a 2044 6563   quantize(x: Dec
-00000530: 696d 616c 2920 2d3e 2044 6563 696d 616c  imal) -> Decimal
-00000540: 3a0a 2020 2020 7265 7475 726e 2078 2e71  :.    return x.q
-00000550: 7561 6e74 697a 6528 4445 4349 4d41 4c5f  uantize(DECIMAL_
-00000560: 4550 5349 4c4f 4e2c 2072 6f75 6e64 696e  EPSILON, roundin
-00000570: 673d 524f 554e 445f 444f 574e 290a 0a0a  g=ROUND_DOWN)...
-00000580: 6465 6620 7465 7374 5f64 6563 696d 616c  def test_decimal
-00000590: 5f74 6573 7428 6765 745f 636f 6e74 7261  _test(get_contra
-000005a0: 6374 5f77 6974 685f 6761 735f 6573 7469  ct_with_gas_esti
-000005b0: 6d61 7469 6f6e 293a 0a20 2020 2064 6563  mation):.    dec
-000005c0: 696d 616c 5f74 6573 7420 3d20 2222 220a  imal_test = """.
-000005d0: 4065 7874 6572 6e61 6c0a 6465 6620 666f  @external.def fo
-000005e0: 6f28 2920 2d3e 2069 6e74 3235 363a 0a20  o() -> int256:. 
-000005f0: 2020 2072 6574 7572 6e28 666c 6f6f 7228     return(floor(
-00000600: 3939 392e 3029 290a 0a40 6578 7465 726e  999.0))..@extern
-00000610: 616c 0a64 6566 2066 6f70 2829 202d 3e20  al.def fop() -> 
-00000620: 696e 7432 3536 3a0a 2020 2020 7265 7475  int256:.    retu
-00000630: 726e 2866 6c6f 6f72 2833 3333 2e30 202b  rn(floor(333.0 +
-00000640: 2036 3636 2e30 2929 0a0a 4065 7874 6572   666.0))..@exter
-00000650: 6e61 6c0a 6465 6620 666f 7128 2920 2d3e  nal.def foq() ->
-00000660: 2069 6e74 3235 363a 0a20 2020 2072 6574   int256:.    ret
-00000670: 7572 6e28 666c 6f6f 7228 3133 3332 2e31  urn(floor(1332.1
-00000680: 202d 2033 3333 2e31 2929 0a0a 4065 7874   - 333.1))..@ext
-00000690: 6572 6e61 6c0a 6465 6620 6261 7228 2920  ernal.def bar() 
-000006a0: 2d3e 2069 6e74 3235 363a 0a20 2020 2072  -> int256:.    r
-000006b0: 6574 7572 6e28 666c 6f6f 7228 3237 2e30  eturn(floor(27.0
-000006c0: 202a 2033 372e 3029 290a 0a40 6578 7465   * 37.0))..@exte
-000006d0: 726e 616c 0a64 6566 2062 617a 2829 202d  rnal.def baz() -
-000006e0: 3e20 696e 7432 3536 3a0a 2020 2020 783a  > int256:.    x:
-000006f0: 2064 6563 696d 616c 203d 2032 372e 300a   decimal = 27.0.
-00000700: 2020 2020 7265 7475 726e 2866 6c6f 6f72      return(floor
-00000710: 2878 202a 2033 372e 3029 290a 0a40 6578  (x * 37.0))..@ex
-00000720: 7465 726e 616c 0a64 6566 206d 6f6b 2829  ternal.def mok()
-00000730: 202d 3e20 696e 7432 3536 3a0a 2020 2020   -> int256:.    
-00000740: 7265 7475 726e 2866 6c6f 6f72 2839 3939  return(floor(999
-00000750: 3939 392e 3020 2f20 372e 3020 2f20 3131  999.0 / 7.0 / 11
-00000760: 2e30 202f 2031 332e 3029 290a 0a40 6578  .0 / 13.0))..@ex
-00000770: 7465 726e 616c 0a64 6566 206d 6f6c 2829  ternal.def mol()
-00000780: 202d 3e20 696e 7432 3536 3a0a 2020 2020   -> int256:.    
-00000790: 7265 7475 726e 2866 6c6f 6f72 2834 3939  return(floor(499
-000007a0: 2e35 202f 2030 2e35 2929 0a0a 4065 7874  .5 / 0.5))..@ext
-000007b0: 6572 6e61 6c0a 6465 6620 6d6f 6d28 2920  ernal.def mom() 
-000007c0: 2d3e 2069 6e74 3235 363a 0a20 2020 2072  -> int256:.    r
-000007d0: 6574 7572 6e28 666c 6f6f 7228 3134 3938  eturn(floor(1498
-000007e0: 2e35 202f 2031 2e35 2929 0a0a 4065 7874  .5 / 1.5))..@ext
-000007f0: 6572 6e61 6c0a 6465 6620 6d6f 6f28 2920  ernal.def moo() 
-00000800: 2d3e 2069 6e74 3235 363a 0a20 2020 2072  -> int256:.    r
-00000810: 6574 7572 6e28 666c 6f6f 7228 3239 3937  eturn(floor(2997
-00000820: 2e30 202f 2033 2e30 2929 0a0a 4065 7874  .0 / 3.0))..@ext
-00000830: 6572 6e61 6c0a 6465 6620 666f 6f6d 2829  ernal.def foom()
-00000840: 202d 3e20 696e 7432 3536 3a0a 2020 2020   -> int256:.    
-00000850: 7265 7475 726e 2866 6c6f 6f72 2831 3939  return(floor(199
-00000860: 392e 3020 2520 3130 3030 2e30 2929 0a0a  9.0 % 1000.0))..
-00000870: 4065 7874 6572 6e61 6c0a 6465 6620 666f  @external.def fo
-00000880: 6f70 2829 202d 3e20 696e 7432 3536 3a0a  op() -> int256:.
-00000890: 2020 2020 7265 7475 726e 2866 6c6f 6f72      return(floor
-000008a0: 2831 3939 392e 3020 2520 3130 3030 2e30  (1999.0 % 1000.0
-000008b0: 2929 0a20 2020 2022 2222 0a0a 2020 2020  )).    """..    
-000008c0: 6320 3d20 6765 745f 636f 6e74 7261 6374  c = get_contract
-000008d0: 5f77 6974 685f 6761 735f 6573 7469 6d61  _with_gas_estima
-000008e0: 7469 6f6e 2864 6563 696d 616c 5f74 6573  tion(decimal_tes
-000008f0: 7429 0a0a 2020 2020 6173 7365 7274 2063  t)..    assert c
-00000900: 2e66 6f6f 2829 203d 3d20 3939 390a 2020  .foo() == 999.  
-00000910: 2020 6173 7365 7274 2063 2e66 6f70 2829    assert c.fop()
-00000920: 203d 3d20 3939 390a 2020 2020 6173 7365   == 999.    asse
-00000930: 7274 2063 2e66 6f71 2829 203d 3d20 3939  rt c.foq() == 99
-00000940: 390a 2020 2020 6173 7365 7274 2063 2e62  9.    assert c.b
-00000950: 6172 2829 203d 3d20 3939 390a 2020 2020  ar() == 999.    
-00000960: 6173 7365 7274 2063 2e62 617a 2829 203d  assert c.baz() =
-00000970: 3d20 3939 390a 2020 2020 6173 7365 7274  = 999.    assert
-00000980: 2063 2e6d 6f6b 2829 203d 3d20 3939 390a   c.mok() == 999.
-00000990: 2020 2020 6173 7365 7274 2063 2e6d 6f6c      assert c.mol
-000009a0: 2829 203d 3d20 3939 390a 2020 2020 6173  () == 999.    as
-000009b0: 7365 7274 2063 2e6d 6f6d 2829 203d 3d20  sert c.mom() == 
-000009c0: 3939 390a 2020 2020 6173 7365 7274 2063  999.    assert c
-000009d0: 2e6d 6f6f 2829 203d 3d20 3939 390a 2020  .moo() == 999.  
-000009e0: 2020 6173 7365 7274 2063 2e66 6f6f 6d28    assert c.foom(
-000009f0: 2920 3d3d 2039 3939 0a20 2020 2061 7373  ) == 999.    ass
-00000a00: 6572 7420 632e 666f 6f70 2829 203d 3d20  ert c.foop() == 
-00000a10: 3939 390a 0a20 2020 2070 7269 6e74 2822  999..    print("
-00000a20: 5061 7373 6564 2062 6173 6963 2061 6464  Passed basic add
-00000a30: 6974 696f 6e2c 2073 7562 7472 6163 7469  ition, subtracti
-00000a40: 6f6e 2061 6e64 206d 756c 7469 706c 6963  on and multiplic
-00000a50: 6174 696f 6e20 7465 7374 7322 290a 0a0a  ation tests")...
-00000a60: 6465 6620 7465 7374 5f68 6172 6465 725f  def test_harder_
-00000a70: 6465 6369 6d61 6c5f 7465 7374 2867 6574  decimal_test(get
-00000a80: 5f63 6f6e 7472 6163 745f 7769 7468 5f67  _contract_with_g
-00000a90: 6173 5f65 7374 696d 6174 696f 6e29 3a0a  as_estimation):.
-00000aa0: 2020 2020 6861 7264 6572 5f64 6563 696d      harder_decim
-00000ab0: 616c 5f74 6573 7420 3d20 2222 220a 4065  al_test = """.@e
-00000ac0: 7874 6572 6e61 6c0a 6465 6620 7068 6f6f  xternal.def phoo
-00000ad0: 6579 2869 6e70 3a20 6465 6369 6d61 6c29  ey(inp: decimal)
-00000ae0: 202d 3e20 6465 6369 6d61 6c3a 0a20 2020   -> decimal:.   
-00000af0: 2078 3a20 6465 6369 6d61 6c20 3d20 3130   x: decimal = 10
-00000b00: 3030 302e 300a 2020 2020 666f 7220 693a  000.0.    for i:
-00000b10: 2075 696e 7432 3536 2069 6e20 7261 6e67   uint256 in rang
-00000b20: 6528 3429 3a0a 2020 2020 2020 2020 7820  e(4):.        x 
-00000b30: 3d20 7820 2a20 696e 700a 2020 2020 7265  = x * inp.    re
-00000b40: 7475 726e 2078 0a0a 4065 7874 6572 6e61  turn x..@externa
-00000b50: 6c0a 6465 6620 6172 6728 696e 703a 2064  l.def arg(inp: d
-00000b60: 6563 696d 616c 2920 2d3e 2064 6563 696d  ecimal) -> decim
-00000b70: 616c 3a0a 2020 2020 7265 7475 726e 2069  al:.    return i
-00000b80: 6e70 0a0a 4065 7874 6572 6e61 6c0a 6465  np..@external.de
-00000b90: 6620 6761 7267 2829 202d 3e20 6465 6369  f garg() -> deci
-00000ba0: 6d61 6c3a 0a20 2020 2078 3a20 6465 6369  mal:.    x: deci
-00000bb0: 6d61 6c20 3d20 342e 350a 2020 2020 7820  mal = 4.5.    x 
-00000bc0: 2a3d 2031 2e35 0a20 2020 2072 6574 7572  *= 1.5.    retur
-00000bd0: 6e20 780a 0a40 6578 7465 726e 616c 0a64  n x..@external.d
-00000be0: 6566 2068 6172 6728 2920 2d3e 2064 6563  ef harg() -> dec
-00000bf0: 696d 616c 3a0a 2020 2020 783a 2064 6563  imal:.    x: dec
-00000c00: 696d 616c 203d 2034 2e35 0a20 2020 2078  imal = 4.5.    x
-00000c10: 202a 3d20 322e 300a 2020 2020 7265 7475   *= 2.0.    retu
-00000c20: 726e 2078 0a0a 4065 7874 6572 6e61 6c0a  rn x..@external.
-00000c30: 6465 6620 6961 7267 2829 202d 3e20 7569  def iarg() -> ui
-00000c40: 6e74 3235 363a 0a20 2020 2078 3a20 7569  nt256:.    x: ui
-00000c50: 6e74 3235 3620 3d20 6173 5f77 6569 5f76  nt256 = as_wei_v
-00000c60: 616c 7565 2837 2c20 2277 6569 2229 0a20  alue(7, "wei"). 
-00000c70: 2020 2078 202a 3d20 320a 2020 2020 7265     x *= 2.    re
-00000c80: 7475 726e 2078 0a20 2020 2022 2222 0a0a  turn x.    """..
-00000c90: 2020 2020 6320 3d20 6765 745f 636f 6e74      c = get_cont
-00000ca0: 7261 6374 5f77 6974 685f 6761 735f 6573  ract_with_gas_es
-00000cb0: 7469 6d61 7469 6f6e 2868 6172 6465 725f  timation(harder_
-00000cc0: 6465 6369 6d61 6c5f 7465 7374 290a 2020  decimal_test).  
-00000cd0: 2020 6173 7365 7274 2063 2e70 686f 6f65    assert c.phooe
-00000ce0: 7928 4465 6369 6d61 6c28 2231 2e32 2229  y(Decimal("1.2")
-00000cf0: 2920 3d3d 2044 6563 696d 616c 2822 3230  ) == Decimal("20
-00000d00: 3733 362e 3022 290a 2020 2020 6173 7365  736.0").    asse
-00000d10: 7274 2063 2e70 686f 6f65 7928 4465 6369  rt c.phooey(Deci
-00000d20: 6d61 6c28 222d 312e 3222 2929 203d 3d20  mal("-1.2")) == 
-00000d30: 4465 6369 6d61 6c28 2232 3037 3336 2e30  Decimal("20736.0
-00000d40: 2229 0a20 2020 2061 7373 6572 7420 632e  ").    assert c.
-00000d50: 6172 6728 4465 6369 6d61 6c28 222d 332e  arg(Decimal("-3.
-00000d60: 3722 2929 203d 3d20 4465 6369 6d61 6c28  7")) == Decimal(
-00000d70: 222d 332e 3722 290a 2020 2020 6173 7365  "-3.7").    asse
-00000d80: 7274 2063 2e61 7267 2844 6563 696d 616c  rt c.arg(Decimal
-00000d90: 2822 332e 3722 2929 203d 3d20 4465 6369  ("3.7")) == Deci
-00000da0: 6d61 6c28 2233 2e37 2229 0a20 2020 2061  mal("3.7").    a
-00000db0: 7373 6572 7420 632e 6761 7267 2829 203d  ssert c.garg() =
-00000dc0: 3d20 4465 6369 6d61 6c28 2236 2e37 3522  = Decimal("6.75"
-00000dd0: 290a 2020 2020 6173 7365 7274 2063 2e68  ).    assert c.h
-00000de0: 6172 6728 2920 3d3d 2044 6563 696d 616c  arg() == Decimal
-00000df0: 2822 392e 3022 290a 2020 2020 6173 7365  ("9.0").    asse
-00000e00: 7274 2063 2e69 6172 6728 2920 3d3d 2044  rt c.iarg() == D
-00000e10: 6563 696d 616c 2822 3134 2229 0a0a 2020  ecimal("14")..  
-00000e20: 2020 7072 696e 7428 2250 6173 7365 6420    print("Passed 
-00000e30: 6672 6163 7469 6f6e 616c 206d 756c 7469  fractional multi
-00000e40: 706c 6963 6174 696f 6e20 7465 7374 2229  plication test")
-00000e50: 0a0a 0a64 6566 2074 6573 745f 6d75 6c5f  ...def test_mul_
-00000e60: 6f76 6572 666c 6f77 2874 785f 6661 696c  overflow(tx_fail
-00000e70: 6564 2c20 6765 745f 636f 6e74 7261 6374  ed, get_contract
-00000e80: 5f77 6974 685f 6761 735f 6573 7469 6d61  _with_gas_estima
-00000e90: 7469 6f6e 293a 0a20 2020 206d 756c 5f63  tion):.    mul_c
-00000ea0: 6f64 6520 3d20 2222 220a 0a40 6578 7465  ode = """..@exte
-00000eb0: 726e 616c 0a64 6566 205f 6e75 6d5f 6d75  rnal.def _num_mu
-00000ec0: 6c28 783a 2064 6563 696d 616c 2c20 793a  l(x: decimal, y:
-00000ed0: 2064 6563 696d 616c 2920 2d3e 2064 6563   decimal) -> dec
-00000ee0: 696d 616c 3a0a 2020 2020 7265 7475 726e  imal:.    return
-00000ef0: 2078 202a 2079 0a0a 2020 2020 2222 220a   x * y..    """.
-00000f00: 0a20 2020 2063 203d 2067 6574 5f63 6f6e  .    c = get_con
-00000f10: 7472 6163 745f 7769 7468 5f67 6173 5f65  tract_with_gas_e
-00000f20: 7374 696d 6174 696f 6e28 6d75 6c5f 636f  stimation(mul_co
-00000f30: 6465 290a 0a20 2020 2078 203d 2044 6563  de)..    x = Dec
-00000f40: 696d 616c 2822 3835 3037 3035 3931 3733  imal("8507059173
-00000f50: 3032 3334 3631 3538 3635 3834 3336 3531  0234615865843651
-00000f60: 3835 3739 3432 3035 3238 3634 2229 0a20  857942052864"). 
-00000f70: 2020 2079 203d 2044 6563 696d 616c 2822     y = Decimal("
-00000f80: 3133 3631 3132 3934 3637 3638 3337 3533  1361129467683753
-00000f90: 3835 3338 3533 3439 3834 3239 3733 2229  85385349842973")
-00000fa0: 0a0a 2020 2020 7769 7468 2074 785f 6661  ..    with tx_fa
-00000fb0: 696c 6564 2829 3a0a 2020 2020 2020 2020  iled():.        
-00000fc0: 632e 5f6e 756d 5f6d 756c 2878 2c20 7929  c._num_mul(x, y)
-00000fd0: 0a0a 2020 2020 7820 3d20 5369 7a65 4c69  ..    x = SizeLi
-00000fe0: 6d69 7473 2e4d 4158 5f41 5354 5f44 4543  mits.MAX_AST_DEC
-00000ff0: 494d 414c 0a20 2020 2079 203d 2031 202b  IMAL.    y = 1 +
-00001000: 2044 4543 494d 414c 5f45 5053 494c 4f4e   DECIMAL_EPSILON
-00001010: 0a0a 2020 2020 7769 7468 2074 785f 6661  ..    with tx_fa
-00001020: 696c 6564 2829 3a0a 2020 2020 2020 2020  iled():.        
-00001030: 632e 5f6e 756d 5f6d 756c 2878 2c20 7929  c._num_mul(x, y)
-00001040: 0a0a 2020 2020 6173 7365 7274 2063 2e5f  ..    assert c._
-00001050: 6e75 6d5f 6d75 6c28 782c 2044 6563 696d  num_mul(x, Decim
-00001060: 616c 2831 2929 203d 3d20 780a 0a20 2020  al(1)) == x..   
-00001070: 2061 7373 6572 7420 632e 5f6e 756d 5f6d   assert c._num_m
-00001080: 756c 2878 2c20 3120 2d20 4445 4349 4d41  ul(x, 1 - DECIMA
-00001090: 4c5f 4550 5349 4c4f 4e29 203d 3d20 7175  L_EPSILON) == qu
-000010a0: 616e 7469 7a65 2878 202a 2028 3120 2d20  antize(x * (1 - 
-000010b0: 4445 4349 4d41 4c5f 4550 5349 4c4f 4e29  DECIMAL_EPSILON)
-000010c0: 290a 0a20 2020 2078 203d 2053 697a 654c  )..    x = SizeL
-000010d0: 696d 6974 732e 4d49 4e5f 4153 545f 4445  imits.MIN_AST_DE
-000010e0: 4349 4d41 4c0a 2020 2020 6173 7365 7274  CIMAL.    assert
-000010f0: 2063 2e5f 6e75 6d5f 6d75 6c28 782c 2031   c._num_mul(x, 1
-00001100: 202d 2044 4543 494d 414c 5f45 5053 494c   - DECIMAL_EPSIL
-00001110: 4f4e 2920 3d3d 2071 7561 6e74 697a 6528  ON) == quantize(
-00001120: 7820 2a20 2831 202d 2044 4543 494d 414c  x * (1 - DECIMAL
-00001130: 5f45 5053 494c 4f4e 2929 0a0a 0a23 2064  _EPSILON))...# d
-00001140: 6976 6973 696f 6e20 6661 696c 7572 6520  ivision failure 
-00001150: 6d6f 6465 7328 2129 0a64 6566 2074 6573  modes(!).def tes
-00001160: 745f 6469 765f 6f76 6572 666c 6f77 2867  t_div_overflow(g
-00001170: 6574 5f63 6f6e 7472 6163 742c 2074 785f  et_contract, tx_
-00001180: 6661 696c 6564 293a 0a20 2020 2063 6f64  failed):.    cod
-00001190: 6520 3d20 2222 220a 4065 7874 6572 6e61  e = """.@externa
-000011a0: 6c0a 6465 6620 666f 6f28 783a 2064 6563  l.def foo(x: dec
-000011b0: 696d 616c 2c20 793a 2064 6563 696d 616c  imal, y: decimal
-000011c0: 2920 2d3e 2064 6563 696d 616c 3a0a 2020  ) -> decimal:.  
-000011d0: 2020 7265 7475 726e 2078 202f 2079 0a20    return x / y. 
-000011e0: 2020 2022 2222 0a0a 2020 2020 6320 3d20     """..    c = 
-000011f0: 6765 745f 636f 6e74 7261 6374 2863 6f64  get_contract(cod
-00001200: 6529 0a0a 2020 2020 7820 3d20 5369 7a65  e)..    x = Size
-00001210: 4c69 6d69 7473 2e4d 494e 5f41 5354 5f44  Limits.MIN_AST_D
-00001220: 4543 494d 414c 0a20 2020 2079 203d 202d  ECIMAL.    y = -
-00001230: 4445 4349 4d41 4c5f 4550 5349 4c4f 4e0a  DECIMAL_EPSILON.
-00001240: 0a20 2020 2077 6974 6820 7478 5f66 6169  .    with tx_fai
-00001250: 6c65 6428 293a 0a20 2020 2020 2020 2063  led():.        c
-00001260: 2e66 6f6f 2878 2c20 7929 0a20 2020 2077  .foo(x, y).    w
-00001270: 6974 6820 7478 5f66 6169 6c65 6428 293a  ith tx_failed():
-00001280: 0a20 2020 2020 2020 2063 2e66 6f6f 2878  .        c.foo(x
-00001290: 2c20 4465 6369 6d61 6c28 3029 290a 2020  , Decimal(0)).  
-000012a0: 2020 7769 7468 2074 785f 6661 696c 6564    with tx_failed
-000012b0: 2829 3a0a 2020 2020 2020 2020 632e 666f  ():.        c.fo
-000012c0: 6f28 792c 2044 6563 696d 616c 2830 2929  o(y, Decimal(0))
-000012d0: 0a0a 2020 2020 7920 3d20 4465 6369 6d61  ..    y = Decima
-000012e0: 6c28 3129 202d 2044 4543 494d 414c 5f45  l(1) - DECIMAL_E
-000012f0: 5053 494c 4f4e 2020 2320 302e 3939 3939  PSILON  # 0.9999
-00001300: 3939 3939 390a 2020 2020 7769 7468 2074  99999.    with t
-00001310: 785f 6661 696c 6564 2829 3a0a 2020 2020  x_failed():.    
-00001320: 2020 2020 632e 666f 6f28 782c 2079 290a      c.foo(x, y).
-00001330: 0a20 2020 2079 203d 2044 6563 696d 616c  .    y = Decimal
-00001340: 282d 3129 0a20 2020 2077 6974 6820 7478  (-1).    with tx
-00001350: 5f66 6169 6c65 6428 293a 0a20 2020 2020  _failed():.     
-00001360: 2020 2063 2e66 6f6f 2878 2c20 7929 0a0a     c.foo(x, y)..
-00001370: 2020 2020 6173 7365 7274 2063 2e66 6f6f      assert c.foo
-00001380: 2878 2c20 4465 6369 6d61 6c28 3129 2920  (x, Decimal(1)) 
-00001390: 3d3d 2078 0a20 2020 2061 7373 6572 7420  == x.    assert 
-000013a0: 632e 666f 6f28 782c 2031 202b 2044 4543  c.foo(x, 1 + DEC
-000013b0: 494d 414c 5f45 5053 494c 4f4e 2920 3d3d  IMAL_EPSILON) ==
-000013c0: 2071 7561 6e74 697a 6528 7820 2f20 2831   quantize(x / (1
-000013d0: 202b 2044 4543 494d 414c 5f45 5053 494c   + DECIMAL_EPSIL
-000013e0: 4f4e 2929 0a0a 2020 2020 7820 3d20 5369  ON))..    x = Si
-000013f0: 7a65 4c69 6d69 7473 2e4d 4158 5f41 5354  zeLimits.MAX_AST
-00001400: 5f44 4543 494d 414c 0a0a 2020 2020 7769  _DECIMAL..    wi
-00001410: 7468 2074 785f 6661 696c 6564 2829 3a0a  th tx_failed():.
-00001420: 2020 2020 2020 2020 632e 666f 6f28 782c          c.foo(x,
-00001430: 2044 4543 494d 414c 5f45 5053 494c 4f4e   DECIMAL_EPSILON
-00001440: 290a 0a20 2020 2079 203d 2044 6563 696d  )..    y = Decim
-00001450: 616c 2831 2920 2d20 4445 4349 4d41 4c5f  al(1) - DECIMAL_
-00001460: 4550 5349 4c4f 4e0a 2020 2020 7769 7468  EPSILON.    with
-00001470: 2074 785f 6661 696c 6564 2829 3a0a 2020   tx_failed():.  
-00001480: 2020 2020 2020 632e 666f 6f28 782c 2079        c.foo(x, y
-00001490: 290a 0a20 2020 2061 7373 6572 7420 632e  )..    assert c.
-000014a0: 666f 6f28 782c 2044 6563 696d 616c 2831  foo(x, Decimal(1
-000014b0: 2929 203d 3d20 780a 0a20 2020 2061 7373  )) == x..    ass
-000014c0: 6572 7420 632e 666f 6f28 782c 2031 202b  ert c.foo(x, 1 +
-000014d0: 2044 4543 494d 414c 5f45 5053 494c 4f4e   DECIMAL_EPSILON
-000014e0: 2920 3d3d 2071 7561 6e74 697a 6528 7820  ) == quantize(x 
-000014f0: 2f20 2831 202b 2044 4543 494d 414c 5f45  / (1 + DECIMAL_E
-00001500: 5053 494c 4f4e 2929 0a0a 0a64 6566 2074  PSILON))...def t
-00001510: 6573 745f 6465 6369 6d61 6c5f 6d69 6e5f  est_decimal_min_
-00001520: 6d61 785f 6c69 7465 7261 6c73 2874 785f  max_literals(tx_
-00001530: 6661 696c 6564 2c20 6765 745f 636f 6e74  failed, get_cont
-00001540: 7261 6374 5f77 6974 685f 6761 735f 6573  ract_with_gas_es
-00001550: 7469 6d61 7469 6f6e 293a 0a20 2020 2063  timation):.    c
-00001560: 6f64 6520 3d20 2222 220a 4065 7874 6572  ode = """.@exter
-00001570: 6e61 6c0a 6465 6620 6d61 7869 6d75 6d28  nal.def maximum(
-00001580: 293a 0a20 2020 2061 3a20 6465 6369 6d61  ):.    a: decima
-00001590: 6c20 3d20 3138 3730 3732 3230 3935 3738  l = 187072209578
-000015a0: 3335 3535 3733 3533 3030 3731 3635 3835  3555735300716585
-000015b0: 3837 3638 3432 3236 3531 3539 352e 3933  8768422651595.93
-000015c0: 3635 3530 3039 3237 0a40 6578 7465 726e  65500927.@extern
-000015d0: 616c 0a64 6566 206d 696e 696d 756d 2829  al.def minimum()
-000015e0: 3a0a 2020 2020 613a 2064 6563 696d 616c  :.    a: decimal
-000015f0: 203d 202d 3138 3730 3732 3230 3935 3738   = -187072209578
-00001600: 3335 3535 3733 3533 3030 3731 3635 3835  3555735300716585
-00001610: 3837 3638 3432 3236 3531 3539 352e 3933  8768422651595.93
-00001620: 3635 3530 3039 3238 0a20 2020 2022 2222  65500928.    """
-00001630: 0a20 2020 2063 203d 2067 6574 5f63 6f6e  .    c = get_con
-00001640: 7472 6163 745f 7769 7468 5f67 6173 5f65  tract_with_gas_e
-00001650: 7374 696d 6174 696f 6e28 636f 6465 290a  stimation(code).
-00001660: 0a20 2020 2061 7373 6572 7420 632e 6d61  .    assert c.ma
-00001670: 7869 6d75 6d28 2920 3d3d 205b 5d0a 2020  ximum() == [].  
-00001680: 2020 6173 7365 7274 2063 2e6d 696e 696d    assert c.minim
-00001690: 756d 2829 203d 3d20 5b5d 0a0a 0a64 6566  um() == []...def
-000016a0: 2074 6573 745f 7363 6965 6e74 6966 6963   test_scientific
-000016b0: 5f6e 6f74 6174 696f 6e28 6765 745f 636f  _notation(get_co
-000016c0: 6e74 7261 6374 5f77 6974 685f 6761 735f  ntract_with_gas_
-000016d0: 6573 7469 6d61 7469 6f6e 293a 0a20 2020  estimation):.   
-000016e0: 2063 6f64 6520 3d20 2222 220a 4065 7874   code = """.@ext
-000016f0: 6572 6e61 6c0a 6465 6620 666f 6f28 2920  ernal.def foo() 
-00001700: 2d3e 2064 6563 696d 616c 3a0a 2020 2020  -> decimal:.    
-00001710: 7265 7475 726e 2031 652d 3130 0a0a 4065  return 1e-10..@e
-00001720: 7874 6572 6e61 6c0a 6465 6620 6261 7228  xternal.def bar(
-00001730: 6e75 6d3a 2064 6563 696d 616c 2920 2d3e  num: decimal) ->
-00001740: 2064 6563 696d 616c 3a0a 2020 2020 7265   decimal:.    re
-00001750: 7475 726e 206e 756d 202b 202d 3165 3338  turn num + -1e38
-00001760: 0a20 2020 2022 2222 0a20 2020 2063 203d  .    """.    c =
-00001770: 2067 6574 5f63 6f6e 7472 6163 745f 7769   get_contract_wi
-00001780: 7468 5f67 6173 5f65 7374 696d 6174 696f  th_gas_estimatio
-00001790: 6e28 636f 6465 290a 0a20 2020 2061 7373  n(code)..    ass
-000017a0: 6572 7420 632e 666f 6f28 2920 3d3d 2044  ert c.foo() == D
-000017b0: 6563 696d 616c 2822 3165 2d31 3022 2920  ecimal("1e-10") 
-000017c0: 2023 2053 6d61 6c6c 6573 7420 706f 7373   # Smallest poss
-000017d0: 6962 6c65 2064 6563 696d 616c 0a20 2020  ible decimal.   
-000017e0: 2061 7373 6572 7420 632e 6261 7228 4465   assert c.bar(De
-000017f0: 6369 6d61 6c28 2231 6533 3722 2929 203d  cimal("1e37")) =
-00001800: 3d20 4465 6369 6d61 6c28 222d 3965 3337  = Decimal("-9e37
-00001810: 2229 2020 2320 4d61 7468 206c 696e 6573  ")  # Math lines
-00001820: 2075 700a 0a0a 6465 6620 7465 7374 5f65   up...def test_e
-00001830: 7870 6f6e 656e 7473 2829 3a0a 2020 2020  xponents():.    
-00001840: 636f 6465 203d 2022 2222 0a40 6578 7465  code = """.@exte
-00001850: 726e 616c 0a64 6566 2066 6f6f 2829 202d  rnal.def foo() -
-00001860: 3e20 6465 6369 6d61 6c3a 0a20 2020 2072  > decimal:.    r
-00001870: 6574 7572 6e20 322e 3220 2a2a 2032 2e30  eturn 2.2 ** 2.0
-00001880: 0a20 2020 2022 2222 0a0a 2020 2020 7769  .    """..    wi
-00001890: 7468 2070 7974 6573 742e 7261 6973 6573  th pytest.raises
-000018a0: 2854 7970 654d 6973 6d61 7463 6829 3a0a  (TypeMismatch):.
-000018b0: 2020 2020 2020 2020 636f 6d70 696c 655f          compile_
-000018c0: 636f 6465 2863 6f64 6529 0a0a 0a64 6566  code(code)...def
-000018d0: 2074 6573 745f 6465 6369 6d61 6c5f 6e65   test_decimal_ne
-000018e0: 7374 6564 5f69 6e74 6572 6d65 6469 6174  sted_intermediat
-000018f0: 655f 6f76 6572 666c 6f77 2829 3a0a 2020  e_overflow():.  
-00001900: 2020 636f 6465 203d 2022 2222 0a40 6578    code = """.@ex
-00001910: 7465 726e 616c 0a64 6566 2066 6f6f 2829  ternal.def foo()
-00001920: 3a0a 2020 2020 613a 2064 6563 696d 616c  :.    a: decimal
-00001930: 203d 2031 3837 3037 3232 3039 3537 3833   = 1870722095783
-00001940: 3535 3537 3335 3330 3037 3136 3538 3538  5557353007165858
-00001950: 3736 3834 3232 3635 3135 3935 2e39 3336  768422651595.936
-00001960: 3535 3030 3932 3720 2b20 3165 2d31 3020  5500927 + 1e-10 
-00001970: 2d20 3165 2d31 300a 2020 2020 2222 220a  - 1e-10.    """.
-00001980: 2020 2020 7769 7468 2070 7974 6573 742e      with pytest.
-00001990: 7261 6973 6573 284f 7665 7266 6c6f 7745  raises(OverflowE
-000019a0: 7863 6570 7469 6f6e 293a 0a20 2020 2020  xception):.     
-000019b0: 2020 2063 6f6d 7069 6c65 5f63 6f64 6528     compile_code(
-000019c0: 636f 6465 290a 0a0a 6465 6620 7465 7374  code)...def test
-000019d0: 5f72 6570 6c61 6365 5f64 6563 696d 616c  _replace_decimal
-000019e0: 5f6e 6573 7465 645f 696e 7465 726d 6564  _nested_intermed
-000019f0: 6961 7465 5f75 6e64 6572 666c 6f77 2864  iate_underflow(d
-00001a00: 756d 6d79 5f69 6e70 7574 5f62 756e 646c  ummy_input_bundl
-00001a10: 6529 3a0a 2020 2020 636f 6465 203d 2022  e):.    code = "
-00001a20: 2222 0a40 6578 7465 726e 616c 0a64 6566  "".@external.def
-00001a30: 2066 6f6f 2829 3a0a 2020 2020 613a 2064   foo():.    a: d
-00001a40: 6563 696d 616c 203d 202d 3138 3730 3732  ecimal = -187072
-00001a50: 3230 3935 3738 3335 3535 3733 3533 3030  2095783555735300
-00001a60: 3731 3635 3835 3837 3638 3432 3236 3531  7165858768422651
-00001a70: 3539 352e 3933 3635 3530 3039 3238 202d  595.9365500928 -
-00001a80: 2031 652d 3130 202b 2031 652d 3130 0a20   1e-10 + 1e-10. 
-00001a90: 2020 2022 2222 0a20 2020 2077 6974 6820     """.    with 
-00001aa0: 7079 7465 7374 2e72 6169 7365 7328 4f76  pytest.raises(Ov
-00001ab0: 6572 666c 6f77 4578 6365 7074 696f 6e29  erflowException)
-00001ac0: 3a0a 2020 2020 2020 2020 636f 6d70 696c  :.        compil
-00001ad0: 655f 636f 6465 2863 6f64 6529 0a0a 0a64  e_code(code)...d
-00001ae0: 6566 2074 6573 745f 696e 7661 6c69 645f  ef test_invalid_
-00001af0: 666c 6f6f 7264 6976 2829 3a0a 2020 2020  floordiv():.    
-00001b00: 636f 6465 203d 2022 2222 0a40 6578 7465  code = """.@exte
-00001b10: 726e 616c 0a64 6566 2066 6f6f 2829 3a0a  rnal.def foo():.
-00001b20: 2020 2020 613a 2064 6563 696d 616c 203d      a: decimal =
-00001b30: 2035 2e30 202f 2f20 392e 300a 2020 2020   5.0 // 9.0.    
-00001b40: 2222 220a 2020 2020 7769 7468 2070 7974  """.    with pyt
-00001b50: 6573 742e 7261 6973 6573 2849 6e76 616c  est.raises(Inval
-00001b60: 6964 4f70 6572 6174 696f 6e29 2061 7320  idOperation) as 
-00001b70: 653a 0a20 2020 2020 2020 2063 6f6d 7069  e:.        compi
-00001b80: 6c65 5f63 6f64 6528 636f 6465 290a 0a20  le_code(code).. 
-00001b90: 2020 2061 7373 6572 7420 652e 7661 6c75     assert e.valu
-00001ba0: 652e 5f68 696e 7420 3d3d 2022 6469 6420  e._hint == "did 
-00001bb0: 796f 7520 6d65 616e 2060 352e 3020 2f20  you mean `5.0 / 
-00001bc0: 392e 3060 3f22 0a                        9.0`?".
+00000020: 6f72 7420 4465 6369 6d61 6c2c 2067 6574  ort Decimal, get
+00000030: 636f 6e74 6578 740a 0a69 6d70 6f72 7420  context..import 
+00000040: 7079 7465 7374 0a0a 6672 6f6d 2076 7970  pytest..from vyp
+00000050: 6572 2069 6d70 6f72 7420 636f 6d70 696c  er import compil
+00000060: 655f 636f 6465 0a66 726f 6d20 7679 7065  e_code.from vype
+00000070: 722e 6578 6365 7074 696f 6e73 2069 6d70  r.exceptions imp
+00000080: 6f72 7420 280a 2020 2020 4465 6369 6d61  ort (.    Decima
+00000090: 6c4f 7665 7272 6964 6545 7863 6570 7469  lOverrideExcepti
+000000a0: 6f6e 2c0a 2020 2020 496e 7661 6c69 644f  on,.    InvalidO
+000000b0: 7065 7261 7469 6f6e 2c0a 2020 2020 4f76  peration,.    Ov
+000000c0: 6572 666c 6f77 4578 6365 7074 696f 6e2c  erflowException,
+000000d0: 0a20 2020 2054 7970 654d 6973 6d61 7463  .    TypeMismatc
+000000e0: 682c 0a29 0a66 726f 6d20 7679 7065 722e  h,.).from vyper.
+000000f0: 7574 696c 7320 696d 706f 7274 2044 4543  utils import DEC
+00000100: 494d 414c 5f45 5053 494c 4f4e 2c20 5369  IMAL_EPSILON, Si
+00000110: 7a65 4c69 6d69 7473 2c20 7175 616e 7469  zeLimits, quanti
+00000120: 7a65 0a0a 0a64 6566 2074 6573 745f 6465  ze...def test_de
+00000130: 6369 6d61 6c5f 6f76 6572 7269 6465 2829  cimal_override()
+00000140: 3a0a 2020 2020 6765 7463 6f6e 7465 7874  :.    getcontext
+00000150: 2829 2e70 7265 6320 3d20 3738 2020 2320  ().prec = 78  # 
+00000160: 7365 7474 696e 6720 7072 6563 2074 6f20  setting prec to 
+00000170: 3738 2069 7320 6f6b 0a0a 2020 2020 2320  78 is ok..    # 
+00000180: 636f 6e73 756d 6572 7320 6f66 2076 7970  consumers of vyp
+00000190: 6572 2c20 6576 656e 2061 7320 6120 6c69  er, even as a li
+000001a0: 6272 6172 792c 2061 7265 206e 6f74 2061  brary, are not a
+000001b0: 6c6c 6f77 6564 2074 6f20 7265 6475 6365  llowed to reduce
+000001c0: 2044 6563 696d 616c 2070 7265 6369 7369   Decimal precisi
+000001d0: 6f6e 0a20 2020 2077 6974 6820 7079 7465  on.    with pyte
+000001e0: 7374 2e72 6169 7365 7328 4465 6369 6d61  st.raises(Decima
+000001f0: 6c4f 7665 7272 6964 6545 7863 6570 7469  lOverrideExcepti
+00000200: 6f6e 293a 0a20 2020 2020 2020 2067 6574  on):.        get
+00000210: 636f 6e74 6578 7428 292e 7072 6563 203d  context().prec =
+00000220: 2037 370a 0a20 2020 2077 6974 6820 7761   77..    with wa
+00000230: 726e 696e 6773 2e63 6174 6368 5f77 6172  rnings.catch_war
+00000240: 6e69 6e67 7328 7265 636f 7264 3d54 7275  nings(record=Tru
+00000250: 6529 2061 7320 773a 0a20 2020 2020 2020  e) as w:.       
+00000260: 2067 6574 636f 6e74 6578 7428 292e 7072   getcontext().pr
+00000270: 6563 203d 2037 390a 2020 2020 2020 2020  ec = 79.        
+00000280: 2320 6368 6563 6b20 7761 726e 696e 6773  # check warnings
+00000290: 2077 6572 6520 6973 7375 6564 0a20 2020   were issued.   
+000002a0: 2020 2020 2061 7373 6572 7420 6c65 6e28       assert len(
+000002b0: 7729 203d 3d20 310a 2020 2020 2020 2020  w) == 1.        
+000002c0: 6173 7365 7274 2028 0a20 2020 2020 2020  assert (.       
+000002d0: 2020 2020 2073 7472 2877 5b2d 315d 2e6d       str(w[-1].m
+000002e0: 6573 7361 6765 2920 3d3d 2022 4368 616e  essage) == "Chan
+000002f0: 6769 6e67 2064 6563 696d 616c 7320 7072  ging decimals pr
+00000300: 6563 6973 696f 6e20 636f 756c 6420 6861  ecision could ha
+00000310: 7665 2075 6e69 6e74 656e 6465 6420 7369  ve unintended si
+00000320: 6465 2065 6666 6563 7473 2122 0a20 2020  de effects!".   
+00000330: 2020 2020 2029 0a0a 0a40 7079 7465 7374       )...@pytest
+00000340: 2e6d 6172 6b2e 7061 7261 6d65 7472 697a  .mark.parametriz
+00000350: 6528 226f 7022 2c20 5b22 2f2f 222c 2022  e("op", ["//", "
+00000360: 2a2a 222c 2022 2622 2c20 227c 222c 2022  **", "&", "|", "
+00000370: 5e22 5d29 0a64 6566 2074 6573 745f 696e  ^"]).def test_in
+00000380: 7661 6c69 645f 6f70 7328 6f70 293a 0a20  valid_ops(op):. 
+00000390: 2020 2063 6f64 6520 3d20 6622 2222 0a40     code = f""".@
+000003a0: 6578 7465 726e 616c 0a64 6566 2066 6f6f  external.def foo
+000003b0: 2878 3a20 6465 6369 6d61 6c2c 2079 3a20  (x: decimal, y: 
+000003c0: 6465 6369 6d61 6c29 202d 3e20 6465 6369  decimal) -> deci
+000003d0: 6d61 6c3a 0a20 2020 2072 6574 7572 6e20  mal:.    return 
+000003e0: 7820 7b6f 707d 2079 0a20 2020 2022 2222  x {op} y.    """
+000003f0: 0a20 2020 2077 6974 6820 7079 7465 7374  .    with pytest
+00000400: 2e72 6169 7365 7328 496e 7661 6c69 644f  .raises(InvalidO
+00000410: 7065 7261 7469 6f6e 293a 0a20 2020 2020  peration):.     
+00000420: 2020 2063 6f6d 7069 6c65 5f63 6f64 6528     compile_code(
+00000430: 636f 6465 290a 0a0a 4070 7974 6573 742e  code)...@pytest.
+00000440: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
+00000450: 2822 6f70 222c 205b 226e 6f74 225d 290a  ("op", ["not"]).
+00000460: 6465 6620 7465 7374 5f69 6e76 616c 6964  def test_invalid
+00000470: 5f75 6e61 7279 5f6f 7073 286f 7029 3a0a  _unary_ops(op):.
+00000480: 2020 2020 636f 6465 203d 2066 2222 220a      code = f""".
+00000490: 4065 7874 6572 6e61 6c0a 6465 6620 666f  @external.def fo
+000004a0: 6f28 783a 2064 6563 696d 616c 2920 2d3e  o(x: decimal) ->
+000004b0: 2064 6563 696d 616c 3a0a 2020 2020 7265   decimal:.    re
+000004c0: 7475 726e 207b 6f70 7d20 780a 2020 2020  turn {op} x.    
+000004d0: 2222 220a 2020 2020 7769 7468 2070 7974  """.    with pyt
+000004e0: 6573 742e 7261 6973 6573 2849 6e76 616c  est.raises(Inval
+000004f0: 6964 4f70 6572 6174 696f 6e29 3a0a 2020  idOperation):.  
+00000500: 2020 2020 2020 636f 6d70 696c 655f 636f        compile_co
+00000510: 6465 2863 6f64 6529 0a0a 0a64 6566 2074  de(code)...def t
+00000520: 6573 745f 6465 6369 6d61 6c5f 7465 7374  est_decimal_test
+00000530: 2867 6574 5f63 6f6e 7472 6163 745f 7769  (get_contract_wi
+00000540: 7468 5f67 6173 5f65 7374 696d 6174 696f  th_gas_estimatio
+00000550: 6e29 3a0a 2020 2020 6465 6369 6d61 6c5f  n):.    decimal_
+00000560: 7465 7374 203d 2022 2222 0a40 6578 7465  test = """.@exte
+00000570: 726e 616c 0a64 6566 2066 6f6f 2829 202d  rnal.def foo() -
+00000580: 3e20 696e 7432 3536 3a0a 2020 2020 7265  > int256:.    re
+00000590: 7475 726e 2866 6c6f 6f72 2839 3939 2e30  turn(floor(999.0
+000005a0: 2929 0a0a 4065 7874 6572 6e61 6c0a 6465  ))..@external.de
+000005b0: 6620 666f 7028 2920 2d3e 2069 6e74 3235  f fop() -> int25
+000005c0: 363a 0a20 2020 2072 6574 7572 6e28 666c  6:.    return(fl
+000005d0: 6f6f 7228 3333 332e 3020 2b20 3636 362e  oor(333.0 + 666.
+000005e0: 3029 290a 0a40 6578 7465 726e 616c 0a64  0))..@external.d
+000005f0: 6566 2066 6f71 2829 202d 3e20 696e 7432  ef foq() -> int2
+00000600: 3536 3a0a 2020 2020 7265 7475 726e 2866  56:.    return(f
+00000610: 6c6f 6f72 2831 3333 322e 3120 2d20 3333  loor(1332.1 - 33
+00000620: 332e 3129 290a 0a40 6578 7465 726e 616c  3.1))..@external
+00000630: 0a64 6566 2062 6172 2829 202d 3e20 696e  .def bar() -> in
+00000640: 7432 3536 3a0a 2020 2020 7265 7475 726e  t256:.    return
+00000650: 2866 6c6f 6f72 2832 372e 3020 2a20 3337  (floor(27.0 * 37
+00000660: 2e30 2929 0a0a 4065 7874 6572 6e61 6c0a  .0))..@external.
+00000670: 6465 6620 6261 7a28 2920 2d3e 2069 6e74  def baz() -> int
+00000680: 3235 363a 0a20 2020 2078 3a20 6465 6369  256:.    x: deci
+00000690: 6d61 6c20 3d20 3237 2e30 0a20 2020 2072  mal = 27.0.    r
+000006a0: 6574 7572 6e28 666c 6f6f 7228 7820 2a20  eturn(floor(x * 
+000006b0: 3337 2e30 2929 0a0a 4065 7874 6572 6e61  37.0))..@externa
+000006c0: 6c0a 6465 6620 6d6f 6b28 2920 2d3e 2069  l.def mok() -> i
+000006d0: 6e74 3235 363a 0a20 2020 2072 6574 7572  nt256:.    retur
+000006e0: 6e28 666c 6f6f 7228 3939 3939 3939 2e30  n(floor(999999.0
+000006f0: 202f 2037 2e30 202f 2031 312e 3020 2f20   / 7.0 / 11.0 / 
+00000700: 3133 2e30 2929 0a0a 4065 7874 6572 6e61  13.0))..@externa
+00000710: 6c0a 6465 6620 6d6f 6c28 2920 2d3e 2069  l.def mol() -> i
+00000720: 6e74 3235 363a 0a20 2020 2072 6574 7572  nt256:.    retur
+00000730: 6e28 666c 6f6f 7228 3439 392e 3520 2f20  n(floor(499.5 / 
+00000740: 302e 3529 290a 0a40 6578 7465 726e 616c  0.5))..@external
+00000750: 0a64 6566 206d 6f6d 2829 202d 3e20 696e  .def mom() -> in
+00000760: 7432 3536 3a0a 2020 2020 7265 7475 726e  t256:.    return
+00000770: 2866 6c6f 6f72 2831 3439 382e 3520 2f20  (floor(1498.5 / 
+00000780: 312e 3529 290a 0a40 6578 7465 726e 616c  1.5))..@external
+00000790: 0a64 6566 206d 6f6f 2829 202d 3e20 696e  .def moo() -> in
+000007a0: 7432 3536 3a0a 2020 2020 7265 7475 726e  t256:.    return
+000007b0: 2866 6c6f 6f72 2832 3939 372e 3020 2f20  (floor(2997.0 / 
+000007c0: 332e 3029 290a 0a40 6578 7465 726e 616c  3.0))..@external
+000007d0: 0a64 6566 2066 6f6f 6d28 2920 2d3e 2069  .def foom() -> i
+000007e0: 6e74 3235 363a 0a20 2020 2072 6574 7572  nt256:.    retur
+000007f0: 6e28 666c 6f6f 7228 3139 3939 2e30 2025  n(floor(1999.0 %
+00000800: 2031 3030 302e 3029 290a 0a40 6578 7465   1000.0))..@exte
+00000810: 726e 616c 0a64 6566 2066 6f6f 7028 2920  rnal.def foop() 
+00000820: 2d3e 2069 6e74 3235 363a 0a20 2020 2072  -> int256:.    r
+00000830: 6574 7572 6e28 666c 6f6f 7228 3139 3939  eturn(floor(1999
+00000840: 2e30 2025 2031 3030 302e 3029 290a 2020  .0 % 1000.0)).  
+00000850: 2020 2222 220a 0a20 2020 2063 203d 2067    """..    c = g
+00000860: 6574 5f63 6f6e 7472 6163 745f 7769 7468  et_contract_with
+00000870: 5f67 6173 5f65 7374 696d 6174 696f 6e28  _gas_estimation(
+00000880: 6465 6369 6d61 6c5f 7465 7374 290a 0a20  decimal_test).. 
+00000890: 2020 2061 7373 6572 7420 632e 666f 6f28     assert c.foo(
+000008a0: 2920 3d3d 2039 3939 0a20 2020 2061 7373  ) == 999.    ass
+000008b0: 6572 7420 632e 666f 7028 2920 3d3d 2039  ert c.fop() == 9
+000008c0: 3939 0a20 2020 2061 7373 6572 7420 632e  99.    assert c.
+000008d0: 666f 7128 2920 3d3d 2039 3939 0a20 2020  foq() == 999.   
+000008e0: 2061 7373 6572 7420 632e 6261 7228 2920   assert c.bar() 
+000008f0: 3d3d 2039 3939 0a20 2020 2061 7373 6572  == 999.    asser
+00000900: 7420 632e 6261 7a28 2920 3d3d 2039 3939  t c.baz() == 999
+00000910: 0a20 2020 2061 7373 6572 7420 632e 6d6f  .    assert c.mo
+00000920: 6b28 2920 3d3d 2039 3939 0a20 2020 2061  k() == 999.    a
+00000930: 7373 6572 7420 632e 6d6f 6c28 2920 3d3d  ssert c.mol() ==
+00000940: 2039 3939 0a20 2020 2061 7373 6572 7420   999.    assert 
+00000950: 632e 6d6f 6d28 2920 3d3d 2039 3939 0a20  c.mom() == 999. 
+00000960: 2020 2061 7373 6572 7420 632e 6d6f 6f28     assert c.moo(
+00000970: 2920 3d3d 2039 3939 0a20 2020 2061 7373  ) == 999.    ass
+00000980: 6572 7420 632e 666f 6f6d 2829 203d 3d20  ert c.foom() == 
+00000990: 3939 390a 2020 2020 6173 7365 7274 2063  999.    assert c
+000009a0: 2e66 6f6f 7028 2920 3d3d 2039 3939 0a0a  .foop() == 999..
+000009b0: 2020 2020 7072 696e 7428 2250 6173 7365      print("Passe
+000009c0: 6420 6261 7369 6320 6164 6469 7469 6f6e  d basic addition
+000009d0: 2c20 7375 6274 7261 6374 696f 6e20 616e  , subtraction an
+000009e0: 6420 6d75 6c74 6970 6c69 6361 7469 6f6e  d multiplication
+000009f0: 2074 6573 7473 2229 0a0a 0a64 6566 2074   tests")...def t
+00000a00: 6573 745f 6861 7264 6572 5f64 6563 696d  est_harder_decim
+00000a10: 616c 5f74 6573 7428 6765 745f 636f 6e74  al_test(get_cont
+00000a20: 7261 6374 5f77 6974 685f 6761 735f 6573  ract_with_gas_es
+00000a30: 7469 6d61 7469 6f6e 293a 0a20 2020 2068  timation):.    h
+00000a40: 6172 6465 725f 6465 6369 6d61 6c5f 7465  arder_decimal_te
+00000a50: 7374 203d 2022 2222 0a40 6578 7465 726e  st = """.@extern
+00000a60: 616c 0a64 6566 2070 686f 6f65 7928 696e  al.def phooey(in
+00000a70: 703a 2064 6563 696d 616c 2920 2d3e 2064  p: decimal) -> d
+00000a80: 6563 696d 616c 3a0a 2020 2020 783a 2064  ecimal:.    x: d
+00000a90: 6563 696d 616c 203d 2031 3030 3030 2e30  ecimal = 10000.0
+00000aa0: 0a20 2020 2066 6f72 2069 3a20 7569 6e74  .    for i: uint
+00000ab0: 3235 3620 696e 2072 616e 6765 2834 293a  256 in range(4):
+00000ac0: 0a20 2020 2020 2020 2078 203d 2078 202a  .        x = x *
+00000ad0: 2069 6e70 0a20 2020 2072 6574 7572 6e20   inp.    return 
+00000ae0: 780a 0a40 6578 7465 726e 616c 0a64 6566  x..@external.def
+00000af0: 2061 7267 2869 6e70 3a20 6465 6369 6d61   arg(inp: decima
+00000b00: 6c29 202d 3e20 6465 6369 6d61 6c3a 0a20  l) -> decimal:. 
+00000b10: 2020 2072 6574 7572 6e20 696e 700a 0a40     return inp..@
+00000b20: 6578 7465 726e 616c 0a64 6566 2067 6172  external.def gar
+00000b30: 6728 2920 2d3e 2064 6563 696d 616c 3a0a  g() -> decimal:.
+00000b40: 2020 2020 783a 2064 6563 696d 616c 203d      x: decimal =
+00000b50: 2034 2e35 0a20 2020 2078 202a 3d20 312e   4.5.    x *= 1.
+00000b60: 350a 2020 2020 7265 7475 726e 2078 0a0a  5.    return x..
+00000b70: 4065 7874 6572 6e61 6c0a 6465 6620 6861  @external.def ha
+00000b80: 7267 2829 202d 3e20 6465 6369 6d61 6c3a  rg() -> decimal:
+00000b90: 0a20 2020 2078 3a20 6465 6369 6d61 6c20  .    x: decimal 
+00000ba0: 3d20 342e 350a 2020 2020 7820 2a3d 2032  = 4.5.    x *= 2
+00000bb0: 2e30 0a20 2020 2072 6574 7572 6e20 780a  .0.    return x.
+00000bc0: 0a40 6578 7465 726e 616c 0a64 6566 2069  .@external.def i
+00000bd0: 6172 6728 2920 2d3e 2075 696e 7432 3536  arg() -> uint256
+00000be0: 3a0a 2020 2020 783a 2075 696e 7432 3536  :.    x: uint256
+00000bf0: 203d 2061 735f 7765 695f 7661 6c75 6528   = as_wei_value(
+00000c00: 372c 2022 7765 6922 290a 2020 2020 7820  7, "wei").    x 
+00000c10: 2a3d 2032 0a20 2020 2072 6574 7572 6e20  *= 2.    return 
+00000c20: 780a 2020 2020 2222 220a 0a20 2020 2063  x.    """..    c
+00000c30: 203d 2067 6574 5f63 6f6e 7472 6163 745f   = get_contract_
+00000c40: 7769 7468 5f67 6173 5f65 7374 696d 6174  with_gas_estimat
+00000c50: 696f 6e28 6861 7264 6572 5f64 6563 696d  ion(harder_decim
+00000c60: 616c 5f74 6573 7429 0a20 2020 2061 7373  al_test).    ass
+00000c70: 6572 7420 632e 7068 6f6f 6579 2844 6563  ert c.phooey(Dec
+00000c80: 696d 616c 2822 312e 3222 2929 203d 3d20  imal("1.2")) == 
+00000c90: 4465 6369 6d61 6c28 2232 3037 3336 2e30  Decimal("20736.0
+00000ca0: 2229 0a20 2020 2061 7373 6572 7420 632e  ").    assert c.
+00000cb0: 7068 6f6f 6579 2844 6563 696d 616c 2822  phooey(Decimal("
+00000cc0: 2d31 2e32 2229 2920 3d3d 2044 6563 696d  -1.2")) == Decim
+00000cd0: 616c 2822 3230 3733 362e 3022 290a 2020  al("20736.0").  
+00000ce0: 2020 6173 7365 7274 2063 2e61 7267 2844    assert c.arg(D
+00000cf0: 6563 696d 616c 2822 2d33 2e37 2229 2920  ecimal("-3.7")) 
+00000d00: 3d3d 2044 6563 696d 616c 2822 2d33 2e37  == Decimal("-3.7
+00000d10: 2229 0a20 2020 2061 7373 6572 7420 632e  ").    assert c.
+00000d20: 6172 6728 4465 6369 6d61 6c28 2233 2e37  arg(Decimal("3.7
+00000d30: 2229 2920 3d3d 2044 6563 696d 616c 2822  ")) == Decimal("
+00000d40: 332e 3722 290a 2020 2020 6173 7365 7274  3.7").    assert
+00000d50: 2063 2e67 6172 6728 2920 3d3d 2044 6563   c.garg() == Dec
+00000d60: 696d 616c 2822 362e 3735 2229 0a20 2020  imal("6.75").   
+00000d70: 2061 7373 6572 7420 632e 6861 7267 2829   assert c.harg()
+00000d80: 203d 3d20 4465 6369 6d61 6c28 2239 2e30   == Decimal("9.0
+00000d90: 2229 0a20 2020 2061 7373 6572 7420 632e  ").    assert c.
+00000da0: 6961 7267 2829 203d 3d20 4465 6369 6d61  iarg() == Decima
+00000db0: 6c28 2231 3422 290a 0a20 2020 2070 7269  l("14")..    pri
+00000dc0: 6e74 2822 5061 7373 6564 2066 7261 6374  nt("Passed fract
+00000dd0: 696f 6e61 6c20 6d75 6c74 6970 6c69 6361  ional multiplica
+00000de0: 7469 6f6e 2074 6573 7422 290a 0a0a 6465  tion test")...de
+00000df0: 6620 7465 7374 5f6d 756c 5f6f 7665 7266  f test_mul_overf
+00000e00: 6c6f 7728 7478 5f66 6169 6c65 642c 2067  low(tx_failed, g
+00000e10: 6574 5f63 6f6e 7472 6163 745f 7769 7468  et_contract_with
+00000e20: 5f67 6173 5f65 7374 696d 6174 696f 6e29  _gas_estimation)
+00000e30: 3a0a 2020 2020 6d75 6c5f 636f 6465 203d  :.    mul_code =
+00000e40: 2022 2222 0a0a 4065 7874 6572 6e61 6c0a   """..@external.
+00000e50: 6465 6620 5f6e 756d 5f6d 756c 2878 3a20  def _num_mul(x: 
+00000e60: 6465 6369 6d61 6c2c 2079 3a20 6465 6369  decimal, y: deci
+00000e70: 6d61 6c29 202d 3e20 6465 6369 6d61 6c3a  mal) -> decimal:
+00000e80: 0a20 2020 2072 6574 7572 6e20 7820 2a20  .    return x * 
+00000e90: 790a 0a20 2020 2022 2222 0a0a 2020 2020  y..    """..    
+00000ea0: 6320 3d20 6765 745f 636f 6e74 7261 6374  c = get_contract
+00000eb0: 5f77 6974 685f 6761 735f 6573 7469 6d61  _with_gas_estima
+00000ec0: 7469 6f6e 286d 756c 5f63 6f64 6529 0a0a  tion(mul_code)..
+00000ed0: 2020 2020 7820 3d20 4465 6369 6d61 6c28      x = Decimal(
+00000ee0: 2238 3530 3730 3539 3137 3330 3233 3436  "850705917302346
+00000ef0: 3135 3836 3538 3433 3635 3138 3537 3934  1586584365185794
+00000f00: 3230 3532 3836 3422 290a 2020 2020 7920  2052864").    y 
+00000f10: 3d20 4465 6369 6d61 6c28 2231 3336 3131  = Decimal("13611
+00000f20: 3239 3436 3736 3833 3735 3338 3533 3835  2946768375385385
+00000f30: 3334 3938 3432 3937 3322 290a 0a20 2020  349842973")..   
+00000f40: 2077 6974 6820 7478 5f66 6169 6c65 6428   with tx_failed(
+00000f50: 293a 0a20 2020 2020 2020 2063 2e5f 6e75  ):.        c._nu
+00000f60: 6d5f 6d75 6c28 782c 2079 290a 0a20 2020  m_mul(x, y)..   
+00000f70: 2078 203d 2053 697a 654c 696d 6974 732e   x = SizeLimits.
+00000f80: 4d41 585f 4153 545f 4445 4349 4d41 4c0a  MAX_AST_DECIMAL.
+00000f90: 2020 2020 7920 3d20 3120 2b20 4445 4349      y = 1 + DECI
+00000fa0: 4d41 4c5f 4550 5349 4c4f 4e0a 0a20 2020  MAL_EPSILON..   
+00000fb0: 2077 6974 6820 7478 5f66 6169 6c65 6428   with tx_failed(
+00000fc0: 293a 0a20 2020 2020 2020 2063 2e5f 6e75  ):.        c._nu
+00000fd0: 6d5f 6d75 6c28 782c 2079 290a 0a20 2020  m_mul(x, y)..   
+00000fe0: 2061 7373 6572 7420 632e 5f6e 756d 5f6d   assert c._num_m
+00000ff0: 756c 2878 2c20 4465 6369 6d61 6c28 3129  ul(x, Decimal(1)
+00001000: 2920 3d3d 2078 0a0a 2020 2020 6173 7365  ) == x..    asse
+00001010: 7274 2063 2e5f 6e75 6d5f 6d75 6c28 782c  rt c._num_mul(x,
+00001020: 2031 202d 2044 4543 494d 414c 5f45 5053   1 - DECIMAL_EPS
+00001030: 494c 4f4e 2920 3d3d 2071 7561 6e74 697a  ILON) == quantiz
+00001040: 6528 7820 2a20 2831 202d 2044 4543 494d  e(x * (1 - DECIM
+00001050: 414c 5f45 5053 494c 4f4e 2929 0a0a 2020  AL_EPSILON))..  
+00001060: 2020 7820 3d20 5369 7a65 4c69 6d69 7473    x = SizeLimits
+00001070: 2e4d 494e 5f41 5354 5f44 4543 494d 414c  .MIN_AST_DECIMAL
+00001080: 0a20 2020 2061 7373 6572 7420 632e 5f6e  .    assert c._n
+00001090: 756d 5f6d 756c 2878 2c20 3120 2d20 4445  um_mul(x, 1 - DE
+000010a0: 4349 4d41 4c5f 4550 5349 4c4f 4e29 203d  CIMAL_EPSILON) =
+000010b0: 3d20 7175 616e 7469 7a65 2878 202a 2028  = quantize(x * (
+000010c0: 3120 2d20 4445 4349 4d41 4c5f 4550 5349  1 - DECIMAL_EPSI
+000010d0: 4c4f 4e29 290a 0a0a 2320 6469 7669 7369  LON))...# divisi
+000010e0: 6f6e 2066 6169 6c75 7265 206d 6f64 6573  on failure modes
+000010f0: 2821 290a 6465 6620 7465 7374 5f64 6976  (!).def test_div
+00001100: 5f6f 7665 7266 6c6f 7728 6765 745f 636f  _overflow(get_co
+00001110: 6e74 7261 6374 2c20 7478 5f66 6169 6c65  ntract, tx_faile
+00001120: 6429 3a0a 2020 2020 636f 6465 203d 2022  d):.    code = "
+00001130: 2222 0a40 6578 7465 726e 616c 0a64 6566  "".@external.def
+00001140: 2066 6f6f 2878 3a20 6465 6369 6d61 6c2c   foo(x: decimal,
+00001150: 2079 3a20 6465 6369 6d61 6c29 202d 3e20   y: decimal) -> 
+00001160: 6465 6369 6d61 6c3a 0a20 2020 2072 6574  decimal:.    ret
+00001170: 7572 6e20 7820 2f20 790a 2020 2020 2222  urn x / y.    ""
+00001180: 220a 0a20 2020 2063 203d 2067 6574 5f63  "..    c = get_c
+00001190: 6f6e 7472 6163 7428 636f 6465 290a 0a20  ontract(code).. 
+000011a0: 2020 2078 203d 2053 697a 654c 696d 6974     x = SizeLimit
+000011b0: 732e 4d49 4e5f 4153 545f 4445 4349 4d41  s.MIN_AST_DECIMA
+000011c0: 4c0a 2020 2020 7920 3d20 2d44 4543 494d  L.    y = -DECIM
+000011d0: 414c 5f45 5053 494c 4f4e 0a0a 2020 2020  AL_EPSILON..    
+000011e0: 7769 7468 2074 785f 6661 696c 6564 2829  with tx_failed()
+000011f0: 3a0a 2020 2020 2020 2020 632e 666f 6f28  :.        c.foo(
+00001200: 782c 2079 290a 2020 2020 7769 7468 2074  x, y).    with t
+00001210: 785f 6661 696c 6564 2829 3a0a 2020 2020  x_failed():.    
+00001220: 2020 2020 632e 666f 6f28 782c 2044 6563      c.foo(x, Dec
+00001230: 696d 616c 2830 2929 0a20 2020 2077 6974  imal(0)).    wit
+00001240: 6820 7478 5f66 6169 6c65 6428 293a 0a20  h tx_failed():. 
+00001250: 2020 2020 2020 2063 2e66 6f6f 2879 2c20         c.foo(y, 
+00001260: 4465 6369 6d61 6c28 3029 290a 0a20 2020  Decimal(0))..   
+00001270: 2079 203d 2044 6563 696d 616c 2831 2920   y = Decimal(1) 
+00001280: 2d20 4445 4349 4d41 4c5f 4550 5349 4c4f  - DECIMAL_EPSILO
+00001290: 4e20 2023 2030 2e39 3939 3939 3939 3939  N  # 0.999999999
+000012a0: 0a20 2020 2077 6974 6820 7478 5f66 6169  .    with tx_fai
+000012b0: 6c65 6428 293a 0a20 2020 2020 2020 2063  led():.        c
+000012c0: 2e66 6f6f 2878 2c20 7929 0a0a 2020 2020  .foo(x, y)..    
+000012d0: 7920 3d20 4465 6369 6d61 6c28 2d31 290a  y = Decimal(-1).
+000012e0: 2020 2020 7769 7468 2074 785f 6661 696c      with tx_fail
+000012f0: 6564 2829 3a0a 2020 2020 2020 2020 632e  ed():.        c.
+00001300: 666f 6f28 782c 2079 290a 0a20 2020 2061  foo(x, y)..    a
+00001310: 7373 6572 7420 632e 666f 6f28 782c 2044  ssert c.foo(x, D
+00001320: 6563 696d 616c 2831 2929 203d 3d20 780a  ecimal(1)) == x.
+00001330: 2020 2020 6173 7365 7274 2063 2e66 6f6f      assert c.foo
+00001340: 2878 2c20 3120 2b20 4445 4349 4d41 4c5f  (x, 1 + DECIMAL_
+00001350: 4550 5349 4c4f 4e29 203d 3d20 7175 616e  EPSILON) == quan
+00001360: 7469 7a65 2878 202f 2028 3120 2b20 4445  tize(x / (1 + DE
+00001370: 4349 4d41 4c5f 4550 5349 4c4f 4e29 290a  CIMAL_EPSILON)).
+00001380: 0a20 2020 2078 203d 2053 697a 654c 696d  .    x = SizeLim
+00001390: 6974 732e 4d41 585f 4153 545f 4445 4349  its.MAX_AST_DECI
+000013a0: 4d41 4c0a 0a20 2020 2077 6974 6820 7478  MAL..    with tx
+000013b0: 5f66 6169 6c65 6428 293a 0a20 2020 2020  _failed():.     
+000013c0: 2020 2063 2e66 6f6f 2878 2c20 4445 4349     c.foo(x, DECI
+000013d0: 4d41 4c5f 4550 5349 4c4f 4e29 0a0a 2020  MAL_EPSILON)..  
+000013e0: 2020 7920 3d20 4465 6369 6d61 6c28 3129    y = Decimal(1)
+000013f0: 202d 2044 4543 494d 414c 5f45 5053 494c   - DECIMAL_EPSIL
+00001400: 4f4e 0a20 2020 2077 6974 6820 7478 5f66  ON.    with tx_f
+00001410: 6169 6c65 6428 293a 0a20 2020 2020 2020  ailed():.       
+00001420: 2063 2e66 6f6f 2878 2c20 7929 0a0a 2020   c.foo(x, y)..  
+00001430: 2020 6173 7365 7274 2063 2e66 6f6f 2878    assert c.foo(x
+00001440: 2c20 4465 6369 6d61 6c28 3129 2920 3d3d  , Decimal(1)) ==
+00001450: 2078 0a0a 2020 2020 6173 7365 7274 2063   x..    assert c
+00001460: 2e66 6f6f 2878 2c20 3120 2b20 4445 4349  .foo(x, 1 + DECI
+00001470: 4d41 4c5f 4550 5349 4c4f 4e29 203d 3d20  MAL_EPSILON) == 
+00001480: 7175 616e 7469 7a65 2878 202f 2028 3120  quantize(x / (1 
+00001490: 2b20 4445 4349 4d41 4c5f 4550 5349 4c4f  + DECIMAL_EPSILO
+000014a0: 4e29 290a 0a0a 6465 6620 7465 7374 5f64  N))...def test_d
+000014b0: 6563 696d 616c 5f6d 696e 5f6d 6178 5f6c  ecimal_min_max_l
+000014c0: 6974 6572 616c 7328 7478 5f66 6169 6c65  iterals(tx_faile
+000014d0: 642c 2067 6574 5f63 6f6e 7472 6163 745f  d, get_contract_
+000014e0: 7769 7468 5f67 6173 5f65 7374 696d 6174  with_gas_estimat
+000014f0: 696f 6e29 3a0a 2020 2020 636f 6465 203d  ion):.    code =
+00001500: 2022 2222 0a40 6578 7465 726e 616c 0a64   """.@external.d
+00001510: 6566 206d 6178 696d 756d 2829 3a0a 2020  ef maximum():.  
+00001520: 2020 613a 2064 6563 696d 616c 203d 2031    a: decimal = 1
+00001530: 3837 3037 3232 3039 3537 3833 3535 3537  8707220957835557
+00001540: 3335 3330 3037 3136 3538 3538 3736 3834  3530071658587684
+00001550: 3232 3635 3135 3935 2e39 3336 3535 3030  22651595.9365500
+00001560: 3932 370a 4065 7874 6572 6e61 6c0a 6465  927.@external.de
+00001570: 6620 6d69 6e69 6d75 6d28 293a 0a20 2020  f minimum():.   
+00001580: 2061 3a20 6465 6369 6d61 6c20 3d20 2d31   a: decimal = -1
+00001590: 3837 3037 3232 3039 3537 3833 3535 3537  8707220957835557
+000015a0: 3335 3330 3037 3136 3538 3538 3736 3834  3530071658587684
+000015b0: 3232 3635 3135 3935 2e39 3336 3535 3030  22651595.9365500
+000015c0: 3932 380a 2020 2020 2222 220a 2020 2020  928.    """.    
+000015d0: 6320 3d20 6765 745f 636f 6e74 7261 6374  c = get_contract
+000015e0: 5f77 6974 685f 6761 735f 6573 7469 6d61  _with_gas_estima
+000015f0: 7469 6f6e 2863 6f64 6529 0a0a 2020 2020  tion(code)..    
+00001600: 6173 7365 7274 2063 2e6d 6178 696d 756d  assert c.maximum
+00001610: 2829 203d 3d20 5b5d 0a20 2020 2061 7373  () == [].    ass
+00001620: 6572 7420 632e 6d69 6e69 6d75 6d28 2920  ert c.minimum() 
+00001630: 3d3d 205b 5d0a 0a0a 6465 6620 7465 7374  == []...def test
+00001640: 5f73 6369 656e 7469 6669 635f 6e6f 7461  _scientific_nota
+00001650: 7469 6f6e 2867 6574 5f63 6f6e 7472 6163  tion(get_contrac
+00001660: 745f 7769 7468 5f67 6173 5f65 7374 696d  t_with_gas_estim
+00001670: 6174 696f 6e29 3a0a 2020 2020 636f 6465  ation):.    code
+00001680: 203d 2022 2222 0a40 6578 7465 726e 616c   = """.@external
+00001690: 0a64 6566 2066 6f6f 2829 202d 3e20 6465  .def foo() -> de
+000016a0: 6369 6d61 6c3a 0a20 2020 2072 6574 7572  cimal:.    retur
+000016b0: 6e20 3165 2d31 300a 0a40 6578 7465 726e  n 1e-10..@extern
+000016c0: 616c 0a64 6566 2062 6172 286e 756d 3a20  al.def bar(num: 
+000016d0: 6465 6369 6d61 6c29 202d 3e20 6465 6369  decimal) -> deci
+000016e0: 6d61 6c3a 0a20 2020 2072 6574 7572 6e20  mal:.    return 
+000016f0: 6e75 6d20 2b20 2d31 6533 380a 2020 2020  num + -1e38.    
+00001700: 2222 220a 2020 2020 6320 3d20 6765 745f  """.    c = get_
+00001710: 636f 6e74 7261 6374 5f77 6974 685f 6761  contract_with_ga
+00001720: 735f 6573 7469 6d61 7469 6f6e 2863 6f64  s_estimation(cod
+00001730: 6529 0a0a 2020 2020 6173 7365 7274 2063  e)..    assert c
+00001740: 2e66 6f6f 2829 203d 3d20 4465 6369 6d61  .foo() == Decima
+00001750: 6c28 2231 652d 3130 2229 2020 2320 536d  l("1e-10")  # Sm
+00001760: 616c 6c65 7374 2070 6f73 7369 626c 6520  allest possible 
+00001770: 6465 6369 6d61 6c0a 2020 2020 6173 7365  decimal.    asse
+00001780: 7274 2063 2e62 6172 2844 6563 696d 616c  rt c.bar(Decimal
+00001790: 2822 3165 3337 2229 2920 3d3d 2044 6563  ("1e37")) == Dec
+000017a0: 696d 616c 2822 2d39 6533 3722 2920 2023  imal("-9e37")  #
+000017b0: 204d 6174 6820 6c69 6e65 7320 7570 0a0a   Math lines up..
+000017c0: 0a64 6566 2074 6573 745f 6578 706f 6e65  .def test_expone
+000017d0: 6e74 7328 293a 0a20 2020 2063 6f64 6520  nts():.    code 
+000017e0: 3d20 2222 220a 4065 7874 6572 6e61 6c0a  = """.@external.
+000017f0: 6465 6620 666f 6f28 2920 2d3e 2064 6563  def foo() -> dec
+00001800: 696d 616c 3a0a 2020 2020 7265 7475 726e  imal:.    return
+00001810: 2032 2e32 202a 2a20 322e 300a 2020 2020   2.2 ** 2.0.    
+00001820: 2222 220a 0a20 2020 2077 6974 6820 7079  """..    with py
+00001830: 7465 7374 2e72 6169 7365 7328 5479 7065  test.raises(Type
+00001840: 4d69 736d 6174 6368 293a 0a20 2020 2020  Mismatch):.     
+00001850: 2020 2063 6f6d 7069 6c65 5f63 6f64 6528     compile_code(
+00001860: 636f 6465 290a 0a0a 6465 6620 7465 7374  code)...def test
+00001870: 5f64 6563 696d 616c 5f6e 6573 7465 645f  _decimal_nested_
+00001880: 696e 7465 726d 6564 6961 7465 5f6f 7665  intermediate_ove
+00001890: 7266 6c6f 7728 293a 0a20 2020 2063 6f64  rflow():.    cod
+000018a0: 6520 3d20 2222 220a 4065 7874 6572 6e61  e = """.@externa
+000018b0: 6c0a 6465 6620 666f 6f28 293a 0a20 2020  l.def foo():.   
+000018c0: 2061 3a20 6465 6369 6d61 6c20 3d20 3138   a: decimal = 18
+000018d0: 3730 3732 3230 3935 3738 3335 3535 3733  7072209578355573
+000018e0: 3533 3030 3731 3635 3835 3837 3638 3432  5300716585876842
+000018f0: 3236 3531 3539 352e 3933 3635 3530 3039  2651595.93655009
+00001900: 3237 202b 2031 652d 3130 202d 2031 652d  27 + 1e-10 - 1e-
+00001910: 3130 0a20 2020 2022 2222 0a20 2020 2077  10.    """.    w
+00001920: 6974 6820 7079 7465 7374 2e72 6169 7365  ith pytest.raise
+00001930: 7328 4f76 6572 666c 6f77 4578 6365 7074  s(OverflowExcept
+00001940: 696f 6e29 3a0a 2020 2020 2020 2020 636f  ion):.        co
+00001950: 6d70 696c 655f 636f 6465 2863 6f64 6529  mpile_code(code)
+00001960: 0a0a 0a64 6566 2074 6573 745f 7265 706c  ...def test_repl
+00001970: 6163 655f 6465 6369 6d61 6c5f 6e65 7374  ace_decimal_nest
+00001980: 6564 5f69 6e74 6572 6d65 6469 6174 655f  ed_intermediate_
+00001990: 756e 6465 7266 6c6f 7728 6475 6d6d 795f  underflow(dummy_
+000019a0: 696e 7075 745f 6275 6e64 6c65 293a 0a20  input_bundle):. 
+000019b0: 2020 2063 6f64 6520 3d20 2222 220a 4065     code = """.@e
+000019c0: 7874 6572 6e61 6c0a 6465 6620 666f 6f28  xternal.def foo(
+000019d0: 293a 0a20 2020 2061 3a20 6465 6369 6d61  ):.    a: decima
+000019e0: 6c20 3d20 2d31 3837 3037 3232 3039 3537  l = -18707220957
+000019f0: 3833 3535 3537 3335 3330 3037 3136 3538  8355573530071658
+00001a00: 3538 3736 3834 3232 3635 3135 3935 2e39  58768422651595.9
+00001a10: 3336 3535 3030 3932 3820 2d20 3165 2d31  365500928 - 1e-1
+00001a20: 3020 2b20 3165 2d31 300a 2020 2020 2222  0 + 1e-10.    ""
+00001a30: 220a 2020 2020 7769 7468 2070 7974 6573  ".    with pytes
+00001a40: 742e 7261 6973 6573 284f 7665 7266 6c6f  t.raises(Overflo
+00001a50: 7745 7863 6570 7469 6f6e 293a 0a20 2020  wException):.   
+00001a60: 2020 2020 2063 6f6d 7069 6c65 5f63 6f64       compile_cod
+00001a70: 6528 636f 6465 290a 0a0a 6465 6620 7465  e(code)...def te
+00001a80: 7374 5f69 6e76 616c 6964 5f66 6c6f 6f72  st_invalid_floor
+00001a90: 6469 7628 293a 0a20 2020 2063 6f64 6520  div():.    code 
+00001aa0: 3d20 2222 220a 4065 7874 6572 6e61 6c0a  = """.@external.
+00001ab0: 6465 6620 666f 6f28 293a 0a20 2020 2061  def foo():.    a
+00001ac0: 3a20 6465 6369 6d61 6c20 3d20 352e 3020  : decimal = 5.0 
+00001ad0: 2f2f 2039 2e30 0a20 2020 2022 2222 0a20  // 9.0.    """. 
+00001ae0: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+00001af0: 6169 7365 7328 496e 7661 6c69 644f 7065  aises(InvalidOpe
+00001b00: 7261 7469 6f6e 2920 6173 2065 3a0a 2020  ration) as e:.  
+00001b10: 2020 2020 2020 636f 6d70 696c 655f 636f        compile_co
+00001b20: 6465 2863 6f64 6529 0a0a 2020 2020 6173  de(code)..    as
+00001b30: 7365 7274 2065 2e76 616c 7565 2e5f 6869  sert e.value._hi
+00001b40: 6e74 203d 3d20 2264 6964 2079 6f75 206d  nt == "did you m
+00001b50: 6561 6e20 6035 2e30 202f 2039 2e30 603f  ean `5.0 / 9.0`?
+00001b60: 220a                                     ".
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_division.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_division.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_exponents.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_exponents.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 import pytest
 from hypothesis import example, given, settings
 from hypothesis import strategies as st
 
 from vyper.codegen.arithmetic import calculate_largest_base, calculate_largest_power
+from vyper.compiler import compile_code
+from vyper.exceptions import InvalidLiteral
+
+
+def test_compiler_hang():
+    code = """
+@external
+def f0():
+    lv0: uint256 = max_value(int128) ** max_value(int128)
+    """
+    with pytest.raises(InvalidLiteral):
+        compile_code(code)
 
 
 @pytest.mark.fuzzing
 @pytest.mark.parametrize("power", range(2, 255))
 def test_exp_uint256(get_contract, tx_failed, power):
     code = f"""
 @external
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_isqrt.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_isqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_modulo.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_modulo.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_signed_ints.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_signed_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_sqrt.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_sqrt.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/numbers/test_unsigned_ints.py` & `vyper-0.4.0b6/tests/functional/codegen/types/numbers/test_unsigned_ints.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_array_indexing.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_array_indexing.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_bytes.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_bytes_literal.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_bytes_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_bytes_zero_padding.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_bytes_zero_padding.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,12 +21,12 @@
     return self.to_little_endian_64(counter)
     """
     c = get_contract_module(code)
     return c
 
 
 @pytest.mark.fuzzing
-@hypothesis.given(value=hypothesis.strategies.integers(min_value=0, max_value=2**64))
+@hypothesis.given(value=hypothesis.strategies.integers(min_value=0, max_value=(2**64 - 1)))
 def test_zero_pad_range(little_endian_contract, value):
     actual_bytes = value.to_bytes(8, byteorder="little")
     contract_bytes = little_endian_contract.get_count(value)
     assert contract_bytes == actual_bytes
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_dynamic_array.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_dynamic_array.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from vyper.compiler import compile_code
 from vyper.exceptions import (
     ArgumentException,
     ArrayIndexException,
     ImmutableViolation,
     OverflowException,
+    StackTooDeep,
     StateAccessViolation,
     TypeMismatch,
 )
 
 
 def test_list_tester_code(get_contract_with_gas_estimation):
     list_tester_code = """
@@ -56,14 +57,15 @@
     assert c.hoo([3, 4, 5]) == 12
     assert c.joo([[1, 2], [3, 4]]) == 73
     assert c.koo([3, 4, 5]) == 12
     assert c.loo([[1, 2], [3, 4]]) == 73
     print("Passed list tests")
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_string_list(get_contract):
     code = """
 @external
 def foo1(x: DynArray[String[32], 2]) -> DynArray[String[32], 2]:
     return x
 
 @external
@@ -728,14 +730,15 @@
     c = get_contract_with_gas_estimation(code)
     assert c.test_array_num_return() == [[], [3, 4]]
     assert c.test_array_decimal_return1() == [[1.0], [3.0, 4.0]]
     assert c.test_array_decimal_return2() == [[1.0, 2.0]]
     assert c.test_array_decimal_return3() == [[1.0, 2.0], [3.0]]
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_mult_list(get_contract_with_gas_estimation):
     code = """
 nest3: DynArray[DynArray[DynArray[uint256, 2], 2], 2]
 nest4: DynArray[DynArray[DynArray[DynArray[uint256, 2], 2], 2], 2]
 
 @external
 def test_multi3_1() -> DynArray[DynArray[DynArray[uint256, 2], 2], 2]:
@@ -1474,14 +1477,15 @@
     return a[0][0][0] * a[1][1][1]
     """
     c = get_contract(code)
     assert c.bar(7) == [[[7, 14], [21, 28]], [[35, 42], [49, 56]]]
     assert c.foo(7) == 392
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_struct_of_lists(get_contract):
     code = """
 struct Foo:
     a1: DynArray[uint256, 2]
     a2: DynArray[DynArray[uint256, 2], 2]
     a3: DynArray[DynArray[DynArray[uint256, 2], 2], 2]
 
@@ -1562,14 +1566,15 @@
     f: Foo = self._foo(x)
     return f.a
     """
     c = get_contract(code)
     assert c.bar(7) == [7, 14]
 
 
+@pytest.mark.venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
 def test_nested_struct_of_lists(get_contract, assert_compile_failed, optimize):
     code = """
 struct nestedFoo:
     a1: DynArray[DynArray[DynArray[uint256, 2], 2], 2]
 
 struct Foo:
     b1: DynArray[DynArray[DynArray[nestedFoo, 2], 2], 2]
@@ -1691,15 +1696,17 @@
 @pytest.mark.parametrize(
     "typ,val",
     [
         ("DynArray[DynArray[uint256, 5], 5]", [[], []]),
         ("DynArray[DynArray[DynArray[uint256, 5], 5], 5]", [[[], []], []]),
     ],
 )
-def test_empty_nested_dynarray(get_contract, typ, val):
+def test_empty_nested_dynarray(get_contract, typ, val, venom_xfail):
+    if val == [[[], []], []]:
+        venom_xfail(raises=StackTooDeep, reason="stack scheduler regression")
     code = f"""
 @external
 def foo() -> {typ}:
     a: {typ} = {val}
     return a
     """
     c = get_contract(code)
```

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_flag.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_identifier_naming.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_identifier_naming.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_lists.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_lists.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_node_types.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_node_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_string.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_string_literal.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/codegen/types/test_struct.py` & `vyper-0.4.0b6/tests/functional/codegen/types/test_struct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/auctions/test_blind_auction.py` & `vyper-0.4.0b6/tests/functional/examples/auctions/test_blind_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/auctions/test_simple_open_auction.py` & `vyper-0.4.0b6/tests/functional/examples/auctions/test_simple_open_auction.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/company/test_company.py` & `vyper-0.4.0b6/tests/functional/examples/company/test_company.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/crowdfund/test_crowdfund_example.py` & `vyper-0.4.0b6/tests/functional/examples/crowdfund/test_crowdfund_example.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/factory/test_factory.py` & `vyper-0.4.0b6/tests/functional/examples/factory/test_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,22 @@
         exchange.initialize(transact={"from": w3.eth.accounts[0]})
         return exchange
 
     return create_exchange
 
 
 @pytest.fixture
-def factory(get_contract, optimize):
+def factory(get_contract, optimize, experimental_codegen):
     with open("examples/factory/Exchange.vy") as f:
         code = f.read()
 
     exchange_interface = vyper.compile_code(
-        code, output_formats=["bytecode_runtime"], settings=Settings(optimize=optimize)
+        code,
+        output_formats=["bytecode_runtime"],
+        settings=Settings(optimize=optimize, experimental_codegen=experimental_codegen),
     )
     exchange_deployed_bytecode = exchange_interface["bytecode_runtime"]
 
     with open("examples/factory/Factory.vy") as f:
         code = f.read()
 
     # NOTE: We deploy the factory with the hash of the exchange's expected deployment bytecode
```

### Comparing `vyper-0.4.0b5/tests/functional/examples/market_maker/test_on_chain_market_maker.py` & `vyper-0.4.0b6/tests/functional/examples/market_maker/test_on_chain_market_maker.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py` & `vyper-0.4.0b6/tests/functional/examples/safe_remote_purchase/test_safe_remote_purchase.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/storage/test_advanced_storage.py` & `vyper-0.4.0b6/tests/functional/examples/storage/test_advanced_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/storage/test_storage.py` & `vyper-0.4.0b6/tests/functional/examples/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/tokens/test_erc1155.py` & `vyper-0.4.0b6/tests/functional/examples/tokens/test_erc1155.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/tokens/test_erc20.py` & `vyper-0.4.0b6/tests/functional/examples/tokens/test_erc20.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/tokens/test_erc4626.py` & `vyper-0.4.0b6/tests/functional/examples/tokens/test_erc4626.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/tokens/test_erc721.py` & `vyper-0.4.0b6/tests/functional/examples/tokens/test_erc721.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/voting/test_ballot.py` & `vyper-0.4.0b6/tests/functional/examples/voting/test_ballot.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/examples/wallet/test_wallet.py` & `vyper-0.4.0b6/tests/functional/examples/wallet/test_wallet.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/grammar/test_grammar.py` & `vyper-0.4.0b6/tests/functional/grammar/test_grammar.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,44 +33,39 @@
 def test_basic_grammar_empty():
     code = """
     """
     tree = parse_vyper_source(code, dedent=True)
     assert len(tree.children) == 0
 
 
-def utf8_encodable(terminal: str) -> bool:
-    try:
-        if "\x00" not in terminal and "\\ " not in terminal and "\x0c" not in terminal:
-            terminal.encode("utf-8-sig")
-            return True
-        else:
-            return False
-    except UnicodeEncodeError:  # pragma: no cover
-        # Very rarely, a "." in some terminal regex will generate a surrogate
-        # character that cannot be encoded as UTF-8.  We apply this filter to
-        # ensure it doesn't happen at runtime, but don't worry about coverage.
-        return False
+def fix_terminal(terminal: str) -> bool:
+    # these throw exceptions in the grammar
+    for bad in ("\x00", "\\ ", "\x0c"):
+        terminal = terminal.replace(bad, " ")
+    return terminal
+
+
+ALLOWED_CHARS = st.characters(codec="ascii", min_codepoint=1)
 
 
 # With help from hyposmith
 # https://github.com/Zac-HD/hypothesmith/blob/master/src/hypothesmith/syntactic.py
 class GrammarStrategy(LarkStrategy):
     def __init__(self, grammar, start, explicit_strategies):
-        super().__init__(grammar, start, explicit_strategies)
+        super().__init__(grammar, start, explicit_strategies, alphabet=ALLOWED_CHARS)
         self.terminal_strategies = {
-            k: v.map(lambda s: s.replace("\0", "")).filter(utf8_encodable)
-            for k, v in self.terminal_strategies.items()  # type: ignore
+            k: v.map(fix_terminal) for k, v in self.terminal_strategies.items()  # type: ignore
         }
 
     def draw_symbol(self, data, symbol, draw_state):  # type: ignore
-        count = len(draw_state.result)
+        count = len(draw_state)
         super().draw_symbol(data, symbol, draw_state)
         try:
             compile(
-                source="".join(draw_state.result[count:])
+                source="".join(draw_state[count:])
                 .replace("contract", "class")
                 .replace("struct", "class"),  # HACK: Python ast.parse
                 filename="<string>",
                 mode="exec",
             )
         except SyntaxError:
             # Python's grammar doesn't actually fully describe the behaviour of the
@@ -98,14 +93,15 @@
 
 
 def has_no_docstrings(c):
     return not (SINGLE_QUOTE_DOCSTRING.match(c) or DOUBLE_QUOTE_DOCSTRING.match(c))
 
 
 @pytest.mark.fuzzing
-@given(code=from_grammar().filter(lambda c: utf8_encodable(c)))
-@hypothesis.settings(max_examples=500, suppress_health_check=[HealthCheck.too_slow])
+@given(code=from_grammar())
+@hypothesis.settings(
+    max_examples=500, suppress_health_check=[HealthCheck.too_slow, HealthCheck.filter_too_much]
+)
 def test_grammar_bruteforce(code):
-    if utf8_encodable(code):
-        _, _, _, reformatted_code = pre_parse(code + "\n")
-        tree = parse_to_ast(reformatted_code)
-        assert isinstance(tree, Module)
+    _, _, _, reformatted_code = pre_parse(code + "\n")
+    tree = parse_to_ast(reformatted_code)
+    assert isinstance(tree, Module)
```

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_argument_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_argument_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_call_violation.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_call_violation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_constancy_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_constancy_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_function_declaration_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_function_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_instantiation_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_instantiation_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_invalid_literal_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_literal_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_invalid_payable.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_payable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_invalid_reference.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_reference.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_invalid_type_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_invalid_type_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_namespace_collision.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_namespace_collision.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_overflow_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_overflow_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_structure_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_structure_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_syntax_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_type_mismatch_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_type_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_undeclared_definition.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_undeclared_definition.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_variable_declaration_exception.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_variable_declaration_exception.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/exceptions/test_vyper_exception_pos.py` & `vyper-0.4.0b6/tests/functional/syntax/exceptions/test_vyper_exception_pos.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/modules/test_deploy_visibility.py` & `vyper-0.4.0b6/tests/functional/syntax/modules/test_deploy_visibility.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/modules/test_exports.py` & `vyper-0.4.0b6/tests/functional/syntax/modules/test_exports.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/modules/test_implements.py` & `vyper-0.4.0b6/tests/functional/syntax/modules/test_implements.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/modules/test_initializers.py` & `vyper-0.4.0b6/tests/functional/syntax/modules/test_initializers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/names/test_event_names.py` & `vyper-0.4.0b6/tests/functional/syntax/names/test_event_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/names/test_function_names.py` & `vyper-0.4.0b6/tests/functional/syntax/names/test_function_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/names/test_variable_names.py` & `vyper-0.4.0b6/tests/functional/syntax/names/test_variable_names.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/signatures/test_invalid_function_decorators.py` & `vyper-0.4.0b6/tests/functional/syntax/signatures/test_invalid_function_decorators.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/signatures/test_method_id_conflicts.py` & `vyper-0.4.0b6/tests/functional/syntax/signatures/test_method_id_conflicts.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_abi_decode.py` & `vyper-0.4.0b6/tests/functional/syntax/test_abi_decode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_abi_encode.py` & `vyper-0.4.0b6/tests/functional/syntax/test_abi_encode.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_abs.py` & `vyper-0.4.0b6/tests/functional/syntax/test_abs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_addmulmod.py` & `vyper-0.4.0b6/tests/functional/syntax/test_addmulmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_address_code.py` & `vyper-0.4.0b6/tests/functional/syntax/test_address_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,28 +157,28 @@
 """,
     ],
 )
 def test_address_code_compile_success(code: str):
     compiler.compile_code(code)
 
 
-def test_address_code_self_success(get_contract, optimize):
+def test_address_code_self_success(get_contract, optimize, experimental_codegen):
     code = """
 code_deployment: public(Bytes[32])
 
 @deploy
 def __init__():
     self.code_deployment = slice(self.code, 0, 32)
 
 @external
 def code_runtime() -> Bytes[32]:
     return slice(self.code, 0, 32)
 """
     contract = get_contract(code)
-    settings = Settings(optimize=optimize)
+    settings = Settings(optimize=optimize, experimental_codegen=experimental_codegen)
     code_compiled = compiler.compile_code(
         code, output_formats=["bytecode", "bytecode_runtime"], settings=settings
     )
     assert contract.code_deployment() == bytes.fromhex(code_compiled["bytecode"][2:])[:32]
     assert contract.code_runtime() == bytes.fromhex(code_compiled["bytecode_runtime"][2:])[:32]
```

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_ann_assign.py` & `vyper-0.4.0b6/tests/functional/syntax/test_ann_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_as_uint256.py` & `vyper-0.4.0b6/tests/functional/syntax/test_as_uint256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_as_wei_value.py` & `vyper-0.4.0b6/tests/functional/syntax/test_as_wei_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_block.py` & `vyper-0.4.0b6/tests/functional/syntax/test_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     x: uint256 = block.difficulty + 185
     if tx.origin == self:
         y: Bytes[35] = concat(block.prevhash, b"dog")
     """,
     """
 @external
 def foo():
-    x: uint256 = block.prevrandao + 185
+    x: bytes32 = block.prevrandao
     if tx.origin == self:
         y: Bytes[35] = concat(block.prevhash, b"dog")
     """,
     """
 @external
 def foo() -> uint256:
     return tx.gasprice
```

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_blockscope.py` & `vyper-0.4.0b6/tests/functional/syntax/test_blockscope.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_bool.py` & `vyper-0.4.0b6/tests/functional/syntax/test_bool.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_bool_ops.py` & `vyper-0.4.0b6/tests/functional/syntax/test_bool_ops.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_bytes.py` & `vyper-0.4.0b6/tests/functional/syntax/test_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_chainid.py` & `vyper-0.4.0b6/tests/functional/syntax/test_chainid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,12 @@
 import pytest
 
 from vyper import compiler
-from vyper.compiler.settings import Settings
-from vyper.evm.opcodes import EVM_VERSIONS
 from vyper.exceptions import TypeMismatch
 
-
-@pytest.mark.parametrize("evm_version", list(EVM_VERSIONS))
-def test_evm_version(evm_version):
-    code = """
-@external
-def foo():
-    a: uint256 = chain.id
-    """
-    settings = Settings(evm_version=evm_version)
-
-    assert compiler.compile_code(code, settings=settings) is not None
-
-
 fail_list = [
     (
         """
 @external
 def foo() -> int128[2]:
     return [3,chain.id]
     """,
```

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_code_size.py` & `vyper-0.4.0b6/tests/functional/syntax/test_code_size.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_concat.py` & `vyper-0.4.0b6/tests/functional/syntax/test_concat.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_constants.py` & `vyper-0.4.0b6/tests/functional/syntax/test_constants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_create_with_code_of.py` & `vyper-0.4.0b6/tests/functional/syntax/test_create_with_code_of.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_dynamic_array.py` & `vyper-0.4.0b6/tests/functional/syntax/test_dynamic_array.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_external_calls.py` & `vyper-0.4.0b6/tests/functional/syntax/test_external_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_extract32.py` & `vyper-0.4.0b6/tests/functional/syntax/test_extract32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_flag.py` & `vyper-0.4.0b6/tests/functional/syntax/test_flag.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_for_range.py` & `vyper-0.4.0b6/tests/functional/syntax/test_for_range.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_functions_call.py` & `vyper-0.4.0b6/tests/functional/syntax/test_functions_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_immutables.py` & `vyper-0.4.0b6/tests/functional/syntax/test_immutables.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_init.py` & `vyper-0.4.0b6/tests/functional/syntax/test_init.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_interfaces.py` & `vyper-0.4.0b6/tests/functional/syntax/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_invalids.py` & `vyper-0.4.0b6/tests/functional/syntax/test_invalids.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_keccak256.py` & `vyper-0.4.0b6/tests/functional/syntax/test_keccak256.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_len.py` & `vyper-0.4.0b6/tests/functional/syntax/test_len.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_list.py` & `vyper-0.4.0b6/tests/functional/syntax/test_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_logging.py` & `vyper-0.4.0b6/tests/functional/syntax/test_logging.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_method_id.py` & `vyper-0.4.0b6/tests/functional/syntax/test_method_id.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_minmax.py` & `vyper-0.4.0b6/tests/functional/syntax/test_minmax.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_minmax_value.py` & `vyper-0.4.0b6/tests/functional/syntax/test_minmax_value.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_msg_data.py` & `vyper-0.4.0b6/tests/functional/syntax/test_msg_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pytest
 from eth_tester.exceptions import TransactionFailed
 
 from vyper import compiler
 from vyper.exceptions import StructureException, TypeMismatch
+from vyper.utils import method_id
 
 
 def test_variable_assignment(get_contract, keccak):
     code = """
 @external
 def foo() -> Bytes[4]:
     bar: Bytes[4] = slice(msg.data, 0, 4)
     return bar
 """
 
     contract = get_contract(code)
-
-    assert contract.foo() == bytes(keccak(text="foo()")[:4])
+    assert contract.foo() == method_id("foo()")
 
 
 def test_slicing_start_index_other_than_zero(get_contract):
     code = """
 @external
 def foo(_value: uint256) -> uint256:
     bar: Bytes[32] = slice(msg.data, 4, 32)
@@ -37,19 +37,19 @@
 def foo(bar: uint256) -> Bytes[36]:
     data: Bytes[36] = slice(msg.data, 0, 36)
     return data
 """
     contract = get_contract(code)
 
     # 2fbebd38000000000000000000000000000000000000000000000000000000000000002a
-    method_id = keccak(text="foo(uint256)").hex()[2:10]  # 2fbebd38
-    encoded_42 = w3.to_bytes(42).hex()  # 2a
-    expected_result = method_id + "00" * 31 + encoded_42
+    selector_hex = method_id("foo(uint256)")  # 2fbebd38
+    encoded_42 = (42).to_bytes(32, "big")
+    expected_result = selector_hex + encoded_42
 
-    assert contract.foo(42).hex() == expected_result
+    assert contract.foo(42) == expected_result
 
 
 @pytest.mark.parametrize("bar", [0, 1, 42, 2**256 - 1])
 def test_calldata_private(get_contract, bar):
     code = """
 @external
 def foo(bar: uint256) -> uint256:
@@ -69,30 +69,30 @@
     b: Bytes[4] = slice(msg.data, 0, 4)
     c: uint256 = max_value(uint256)
 
     return (a, b, c)
 """
     contract = get_contract(code)
 
-    assert contract.foo() == [2**256 - 1, bytes(keccak(text="foo()")[:4]), 2**256 - 1]
+    assert contract.foo() == [2**256 - 1, method_id("foo()"), 2**256 - 1]
 
 
 def test_assignment_to_storage(w3, get_contract, keccak):
     code = """
 cache: public(Bytes[4])
 
 @external
 def foo():
     self.cache = slice(msg.data, 0, 4)
 """
     acct = w3.eth.accounts[0]
     contract = get_contract(code)
 
     contract.foo(transact={"from": acct})
-    assert contract.cache() == bytes(keccak(text="foo()")[:4])
+    assert contract.cache() == method_id("foo()")
 
 
 def test_get_len(get_contract):
     code = """
 @external
 def foo(bar: uint256) -> uint256:
     return len(msg.data)
```

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_nested_list.py` & `vyper-0.4.0b6/tests/functional/syntax/test_nested_list.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_no_none.py` & `vyper-0.4.0b6/tests/functional/syntax/test_no_none.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_powmod.py` & `vyper-0.4.0b6/tests/functional/syntax/test_powmod.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_print.py` & `vyper-0.4.0b6/tests/functional/syntax/test_print.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_public.py` & `vyper-0.4.0b6/tests/functional/syntax/test_public.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_raw_call.py` & `vyper-0.4.0b6/tests/functional/syntax/test_raw_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_return_tuple.py` & `vyper-0.4.0b6/tests/functional/syntax/test_return_tuple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_selfdestruct.py` & `vyper-0.4.0b6/tests/functional/syntax/test_selfdestruct.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_send.py` & `vyper-0.4.0b6/tests/functional/syntax/test_send.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_slice.py` & `vyper-0.4.0b6/tests/functional/syntax/test_slice.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_string.py` & `vyper-0.4.0b6/tests/functional/syntax/test_string.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_structs.py` & `vyper-0.4.0b6/tests/functional/syntax/test_structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,13 +585,13 @@
 @external
 def foo():
     self.a = A({x: 1})
     """
     with warnings.catch_warnings(record=True) as w:
         assert compiler.compile_code(code) is not None
 
-        expected = "Instantiating a struct using a dictionary is deprecated "
-        expected += "as of v0.4.0 and will be disallowed in a future release. "
-        expected += "Use kwargs instead e.g. Foo(a=1, b=2)"
+    expected = "Instantiating a struct using a dictionary is deprecated "
+    expected += "as of v0.4.0 and will be disallowed in a future release. "
+    expected += "Use kwargs instead e.g. Foo(a=1, b=2)"
 
-        assert len(w) == 1
-        assert str(w[0].message).startswith(expected)
+    assert len(w) == 1, [s.message for s in w]
+    assert str(w[0].message).startswith(expected)
```

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_ternary.py` & `vyper-0.4.0b6/tests/functional/syntax/test_ternary.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_tuple_assign.py` & `vyper-0.4.0b6/tests/functional/syntax/test_tuple_assign.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/functional/syntax/test_unbalanced_return.py` & `vyper-0.4.0b6/tests/functional/syntax/test_unbalanced_return.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/abi_types/test_invalid_abi_types.py` & `vyper-0.4.0b6/tests/unit/abi_types/test_invalid_abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_compare_nodes.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_compare_nodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_binop_decimal.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_binop_decimal.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,25 @@
 
 import pytest
 from hypothesis import example, given, settings
 from hypothesis import strategies as st
 
 from tests.utils import parse_and_fold
 from vyper.exceptions import OverflowException, TypeMismatch, ZeroDivisionException
+from vyper.semantics.analysis.local import ExprVisitor
+from vyper.semantics.types import DecimalT
+
+DECIMAL_T = DecimalT()
 
 st_decimals = st.decimals(
-    min_value=-(2**32), max_value=2**32, allow_nan=False, allow_infinity=False, places=10
+    min_value=DECIMAL_T.decimal_bounds[0],
+    max_value=DECIMAL_T.decimal_bounds[1],
+    allow_nan=False,
+    allow_infinity=False,
+    places=DECIMAL_T._decimal_places,
 )
 
 
 @pytest.mark.fuzzing
 @settings(max_examples=50)
 @given(left=st_decimals, right=st_decimals)
 @example(left=Decimal("0.9999999999"), right=Decimal("0.0000000001"))
@@ -26,18 +34,19 @@
 def foo(a: decimal, b: decimal) -> decimal:
     return a {op} b
     """
     contract = get_contract(source)
 
     try:
         vyper_ast = parse_and_fold(f"{left} {op} {right}")
-        old_node = vyper_ast.body[0].value
-        new_node = old_node.get_folded_value()
+        expr = vyper_ast.body[0].value
+        ExprVisitor().visit(expr, DecimalT())
+        new_node = expr.get_folded_value()
         is_valid = True
-    except ZeroDivisionException:
+    except (OverflowException, ZeroDivisionException):
         is_valid = False
 
     if is_valid:
         assert contract.foo(left, right) == new_node.value
     else:
         with tx_failed():
             contract.foo(left, right)
@@ -67,17 +76,20 @@
     """
     contract = get_contract(source)
 
     literal_op = " ".join(f"{a} {b}" for a, b in zip(values, ops))
     literal_op = literal_op.rsplit(maxsplit=1)[0]
     try:
         vyper_ast = parse_and_fold(literal_op)
-        new_node = vyper_ast.body[0].value.get_folded_value()
+        expr = vyper_ast.body[0].value
+        ExprVisitor().visit(expr, DecimalT())
+        new_node = expr.get_folded_value()
         expected = new_node.value
-        is_valid = -(2**127) <= expected < 2**127
+        lo, hi = DecimalT().decimal_bounds
+        is_valid = lo <= expected < hi
     except (OverflowException, ZeroDivisionException):
         # for overflow or division/modulus by 0, expect the contract call to revert
         is_valid = False
 
     if is_valid:
         assert contract.foo(*values) == expected
     else:
```

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_binop_int.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_binop_int.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_boolop.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_boolop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_compare.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_compare.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_subscript.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_subscript.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_fold_unaryop.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_fold_unaryop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_from_node.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_from_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_get_children.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_get_children.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_get_descendants.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_get_descendants.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/nodes/test_hex.py` & `vyper-0.4.0b6/tests/unit/ast/nodes/test_hex.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/test_annotate_and_optimize_ast.py` & `vyper-0.4.0b6/tests/unit/ast/test_annotate_and_optimize_ast.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/test_ast_dict.py` & `vyper-0.4.0b6/tests/unit/ast/test_ast_dict.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/test_metadata_journal.py` & `vyper-0.4.0b6/tests/unit/ast/test_metadata_journal.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/test_natspec.py` & `vyper-0.4.0b6/tests/unit/ast/test_natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/test_parser.py` & `vyper-0.4.0b6/tests/unit/ast/test_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/test_pre_parser.py` & `vyper-0.4.0b6/tests/unit/ast/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/ast/test_source_annotation.py` & `vyper-0.4.0b6/tests/unit/ast/test_source_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/cli/storage_layout/test_storage_layout.py` & `vyper-0.4.0b6/tests/unit/cli/storage_layout/test_storage_layout.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,25 @@
 from vyper.compiler import compile_code
+from vyper.evm.opcodes import version_check
+
+
+def _adjust_storage_layout_for_cancun(layout):
+    def _go(layout):
+        for _varname, item in layout.items():
+            if "slot" in item and isinstance(item["slot"], int):
+                item["slot"] -= 1
+            else:
+                # recurse to submodule
+                _go(item)
+
+    if version_check(begin="cancun"):
+        layout["transient_storage_layout"] = {
+            "$.nonreentrant_key": layout["storage_layout"].pop("$.nonreentrant_key")
+        }
+        _go(layout["storage_layout"])
 
 
 def test_storage_layout():
     code = """
 foo: HashMap[address, uint256]
 
 @external
@@ -36,21 +53,26 @@
 @nonreentrant
 def public_foo3():
     pass
     """
 
     out = compile_code(code, output_formats=["layout"])
 
-    assert out["layout"]["storage_layout"] == {
-        "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
-        "foo": {"slot": 1, "type": "HashMap[address, uint256]"},
-        "arr": {"slot": 2, "type": "DynArray[uint256, 3]"},
-        "baz": {"slot": 6, "type": "Bytes[65]"},
-        "bar": {"slot": 10, "type": "uint256"},
+    expected = {
+        "storage_layout": {
+            "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
+            "foo": {"slot": 1, "type": "HashMap[address, uint256]"},
+            "arr": {"slot": 2, "type": "DynArray[uint256, 3]"},
+            "baz": {"slot": 6, "type": "Bytes[65]"},
+            "bar": {"slot": 10, "type": "uint256"},
+        }
     }
+    _adjust_storage_layout_for_cancun(expected)
+
+    assert out["layout"] == expected
 
 
 def test_storage_and_immutables_layout():
     code = """
 name: String[32]
 SYMBOL: immutable(String[32])
 DECIMALS: immutable(uint8)
@@ -67,14 +89,15 @@
             "DECIMALS": {"length": 32, "offset": 64, "type": "uint8"},
         },
         "storage_layout": {
             "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
             "name": {"slot": 1, "type": "String[32]"},
         },
     }
+    _adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, output_formats=["layout"])
     assert out["layout"] == expected_layout
 
 
 def test_storage_layout_module(make_input_bundle):
     lib1 = """
@@ -116,14 +139,15 @@
         "storage_layout": {
             "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
             "counter": {"slot": 1, "type": "uint256"},
             "counter2": {"slot": 2, "type": "uint256"},
             "a_library": {"supply": {"slot": 3, "type": "uint256"}},
         },
     }
+    _adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, input_bundle=input_bundle, output_formats=["layout"])
     assert out["layout"] == expected_layout
 
 
 def test_storage_layout_module2(make_input_bundle):
     # test module storage layout, but initializes is in a different order
@@ -165,14 +189,15 @@
         "storage_layout": {
             "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
             "counter": {"slot": 1, "type": "uint256"},
             "a_library": {"supply": {"slot": 2, "type": "uint256"}},
             "counter2": {"slot": 3, "type": "uint256"},
         },
     }
+    _adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, input_bundle=input_bundle, output_formats=["layout"])
     assert out["layout"] == expected_layout
 
 
 def test_storage_layout_module_uses(make_input_bundle):
     # test module storage layout, with initializes/uses and a nonreentrant
@@ -249,14 +274,15 @@
             "$.nonreentrant_key": {"slot": 0, "type": "nonreentrant lock"},
             "counter": {"slot": 1, "type": "uint256"},
             "lib2": {"storage_variable": {"slot": 2, "type": "uint256"}},
             "counter2": {"slot": 3, "type": "uint256"},
             "a_library": {"supply": {"slot": 4, "type": "uint256"}},
         },
     }
+    _adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, input_bundle=input_bundle, output_formats=["layout"])
     assert out["layout"] == expected_layout
 
 
 def test_storage_layout_module_nested_initializes(make_input_bundle):
     # test module storage layout, with initializes in an imported module
@@ -330,10 +356,11 @@
             "lib2": {
                 "lib1": {"supply": {"slot": 2, "type": "uint256"}},
                 "storage_variable": {"slot": 3, "type": "uint256"},
             },
             "counter2": {"slot": 4, "type": "uint256"},
         },
     }
+    _adjust_storage_layout_for_cancun(expected_layout)
 
     out = compile_code(code, input_bundle=input_bundle, output_formats=["layout"])
     assert out["layout"] == expected_layout
```

### Comparing `vyper-0.4.0b5/tests/unit/cli/storage_layout/test_storage_layout_overrides.py` & `vyper-0.4.0b6/tests/unit/cli/storage_layout/test_storage_layout_overrides.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/cli/vyper_compile/test_compile_files.py` & `vyper-0.4.0b6/tests/unit/cli/vyper_compile/test_compile_files.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/cli/vyper_compile/test_parse_args.py` & `vyper-0.4.0b6/tests/unit/cli/vyper_compile/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/cli/vyper_json/test_compile_json.py` & `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_compile_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,19 +109,21 @@
         compile_from_input_dict(input_json)
     with pytest.raises(JSONError):
         compile_json(input_json)
 
 
 def test_compile_json(input_json, input_bundle):
     foo_input = input_bundle.load_file("contracts/foo.vy")
-    # remove bb and bb_runtime from output formats
+    # remove venom related from output formats
     # because they require venom (experimental)
     output_formats = OUTPUT_FORMATS.copy()
     del output_formats["bb"]
     del output_formats["bb_runtime"]
+    del output_formats["cfg"]
+    del output_formats["cfg_runtime"]
     foo = compile_from_file_input(
         foo_input, output_formats=output_formats, input_bundle=input_bundle
     )
 
     library_input = input_bundle.load_file("contracts/library.vy")
     library = compile_from_file_input(
         library_input, output_formats=output_formats, input_bundle=input_bundle
```

### Comparing `vyper-0.4.0b5/tests/unit/cli/vyper_json/test_get_inputs.py` & `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_get_inputs.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/cli/vyper_json/test_get_settings.py` & `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_get_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/cli/vyper_json/test_output_selection.py` & `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_output_selection.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py` & `vyper-0.4.0b6/tests/unit/cli/vyper_json/test_parse_args_vyperjson.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/asm/test_asm_optimizer.py` & `vyper-0.4.0b6/tests/unit/compiler/asm/test_asm_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     assert any(ctor_only in instr for instr in initcode_asm)
     assert all(runtime_only not in instr for instr in initcode_asm)
 
     assert any(runtime_only in instr for instr in runtime_asm)
     assert all(ctor_only not in instr for instr in runtime_asm)
 
 
-def test_library_code_eliminator(make_input_bundle):
+def test_library_code_eliminator(make_input_bundle, experimental_codegen):
     library = """
 @internal
 def unused1():
     pass
 
 @internal
 def unused2():
@@ -116,9 +116,10 @@
 def foo():
     library.some_function()
     """
     input_bundle = make_input_bundle({"library.vy": library})
     res = compile_code(code, input_bundle=input_bundle, output_formats=["asm"])
     asm = res["asm"]
     assert "some_function()" in asm
+
     assert "unused1()" not in asm
     assert "unused2()" not in asm
```

### Comparing `vyper-0.4.0b5/tests/unit/compiler/ir/test_compile_ir.py` & `vyper-0.4.0b6/tests/unit/compiler/ir/test_compile_ir.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
 
 from vyper.codegen.ir_node import IRnode
+from vyper.evm.opcodes import version_check
 from vyper.ir import compile_ir
 from vyper.ir.s_expressions import parse_s_exp
 
 fail_list = [
     [-(2**255) - 3],
     [2**256 + 3],
     ["set", "_poz"],
@@ -64,8 +65,13 @@
     assert c.test(-123456) == -123456
 
 
 def test_pc_debugger():
     debugger_ir = ["seq", ["mstore", 0, 32], ["pc_debugger"]]
     ir_nodes = IRnode.from_list(debugger_ir)
     _, line_number_map = compile_ir.assembly_to_evm(compile_ir.compile_to_assembly(ir_nodes))
-    assert line_number_map["pc_breakpoints"][0] == 4
+    if version_check(begin="shanghai"):
+        offset = 4  # push0 saves a byte
+    else:
+        offset = 5
+
+    assert line_number_map["pc_breakpoints"][0] == offset
```

### Comparing `vyper-0.4.0b5/tests/unit/compiler/ir/test_optimize_ir.py` & `vyper-0.4.0b6/tests/unit/compiler/ir/test_optimize_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/ir/test_with.py` & `vyper-0.4.0b6/tests/unit/compiler/ir/test_with.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_abi.py` & `vyper-0.4.0b6/tests/unit/compiler/test_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_bytecode_runtime.py` & `vyper-0.4.0b6/tests/unit/compiler/test_bytecode_runtime.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_compile_code.py` & `vyper-0.4.0b6/tests/unit/compiler/test_compile_code.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_default_settings.py` & `vyper-0.4.0b6/tests/unit/compiler/test_default_settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_input_bundle.py` & `vyper-0.4.0b6/tests/unit/compiler/test_input_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_opcodes.py` & `vyper-0.4.0b6/tests/unit/compiler/test_opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_pre_parser.py` & `vyper-0.4.0b6/tests/unit/compiler/test_pre_parser.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_sha3_32.py` & `vyper-0.4.0b6/tests/unit/compiler/test_sha3_32.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/test_source_map.py` & `vyper-0.4.0b6/tests/unit/compiler/test_source_map.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/venom/test_convert_basicblock_simple.py` & `vyper-0.4.0b6/tests/unit/compiler/venom/test_convert_basicblock_simple.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/compiler/venom/test_duplicate_operands.py` & `vyper-0.4.0b6/tests/unit/compiler/venom/test_duplicate_operands.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,9 +19,8 @@
     bb = ctx.get_basic_block()
     op = bb.append_instruction("store", 10)
     sum_ = bb.append_instruction("add", op, op)
     bb.append_instruction("mul", sum_, op)
     bb.append_instruction("stop")
 
     asm = generate_assembly_experimental(ctx, optimize=OptimizationLevel.GAS)
-
-    assert asm == ["PUSH1", 10, "DUP1", "DUP1", "DUP1", "ADD", "MUL", "STOP"]
+    assert asm == ["PUSH1", 10, "DUP1", "DUP1", "ADD", "MUL", "STOP"]
```

### Comparing `vyper-0.4.0b5/tests/unit/compiler/venom/test_multi_entry_block.py` & `vyper-0.4.0b6/tests/unit/compiler/venom/test_multi_entry_block.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,23 +30,23 @@
     finish_bb = IRBasicBlock(finish_label, ctx)
     ctx.append_basic_block(finish_bb)
     finish_bb.append_instruction("stop")
 
     calculate_cfg(ctx)
     assert not ctx.normalized, "CFG should not be normalized"
 
-    NormalizationPass.run_pass(ctx)
+    NormalizationPass().run_pass(ctx)
 
     assert ctx.normalized, "CFG should be normalized"
 
     finish_bb = ctx.get_basic_block(finish_label.value)
-    cfg_in = list(finish_bb.cfg_in.keys())
+    cfg_in = list(finish_bb.cfg_in)
     assert cfg_in[0].label.value == "target", "Should contain target"
-    assert cfg_in[1].label.value == "finish_split___global", "Should contain finish_split___global"
-    assert cfg_in[2].label.value == "finish_split_block_1", "Should contain finish_split_block_1"
+    assert cfg_in[1].label.value == "__global_split_finish", "Should contain __global_split_finish"
+    assert cfg_in[2].label.value == "block_1_split_finish", "Should contain block_1_split_finish"
 
 
 # more complicated one
 def test_multi_entry_block_2():
     ctx = IRFunction()
 
     finish_label = IRLabel("finish")
@@ -82,23 +82,23 @@
     finish_bb = IRBasicBlock(finish_label, ctx)
     ctx.append_basic_block(finish_bb)
     finish_bb.append_instruction("stop")
 
     calculate_cfg(ctx)
     assert not ctx.normalized, "CFG should not be normalized"
 
-    NormalizationPass.run_pass(ctx)
+    NormalizationPass().run_pass(ctx)
 
     assert ctx.normalized, "CFG should be normalized"
 
     finish_bb = ctx.get_basic_block(finish_label.value)
-    cfg_in = list(finish_bb.cfg_in.keys())
+    cfg_in = list(finish_bb.cfg_in)
     assert cfg_in[0].label.value == "target", "Should contain target"
-    assert cfg_in[1].label.value == "finish_split___global", "Should contain finish_split___global"
-    assert cfg_in[2].label.value == "finish_split_block_1", "Should contain finish_split_block_1"
+    assert cfg_in[1].label.value == "__global_split_finish", "Should contain __global_split_finish"
+    assert cfg_in[2].label.value == "block_1_split_finish", "Should contain block_1_split_finish"
 
 
 def test_multi_entry_block_with_dynamic_jump():
     ctx = IRFunction()
 
     finish_label = IRLabel("finish")
     target_label = IRLabel("target")
@@ -124,15 +124,15 @@
     finish_bb = IRBasicBlock(finish_label, ctx)
     ctx.append_basic_block(finish_bb)
     finish_bb.append_instruction("stop")
 
     calculate_cfg(ctx)
     assert not ctx.normalized, "CFG should not be normalized"
 
-    NormalizationPass.run_pass(ctx)
+    NormalizationPass().run_pass(ctx)
     assert ctx.normalized, "CFG should be normalized"
 
     finish_bb = ctx.get_basic_block(finish_label.value)
-    cfg_in = list(finish_bb.cfg_in.keys())
+    cfg_in = list(finish_bb.cfg_in)
     assert cfg_in[0].label.value == "target", "Should contain target"
-    assert cfg_in[1].label.value == "finish_split___global", "Should contain finish_split___global"
-    assert cfg_in[2].label.value == "finish_split_block_1", "Should contain finish_split_block_1"
+    assert cfg_in[1].label.value == "__global_split_finish", "Should contain __global_split_finish"
+    assert cfg_in[2].label.value == "block_1_split_finish", "Should contain block_1_split_finish"
```

### Comparing `vyper-0.4.0b5/tests/unit/semantics/analysis/test_array_index.py` & `vyper-0.4.0b6/tests/unit/semantics/analysis/test_array_index.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/analysis/test_cyclic_function_calls.py` & `vyper-0.4.0b6/tests/unit/semantics/analysis/test_cyclic_function_calls.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/analysis/test_for_loop.py` & `vyper-0.4.0b6/tests/unit/semantics/analysis/test_for_loop.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/analysis/test_potential_types.py` & `vyper-0.4.0b6/tests/unit/semantics/analysis/test_potential_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/conftest.py` & `vyper-0.4.0b6/tests/unit/semantics/conftest.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/test_namespace.py` & `vyper-0.4.0b6/tests/unit/semantics/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/test_storage_slots.py` & `vyper-0.4.0b6/tests/unit/semantics/test_storage_slots.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+from vyper.evm.opcodes import version_check
 from vyper.exceptions import StorageLayoutException
 
 code = """
 
 struct StructOne:
     a: String[33]
     b: uint256[3]
@@ -93,16 +94,23 @@
     )
     assert [c.foo(0, i) for i in range(3)] == [987, 654, 321]
     assert [c.foo(1, i) for i in range(3)] == [123, 456, 789]
     assert c.h(0) == 123456789
 
 
 def test_allocator_overflow(get_contract):
-    code = """
-# --> global nonreentrancy slot allocated here <--
+    # cancun allocates reeentrancy slot in transient storage,
+    # so allocate an actual storage variable
+    if version_check(begin="cancun"):
+        slot1 = "x: uint256"
+    else:
+        slot1 = "# --> global nonreentrancy slot allocated here <--"
+    code = f"""
+{slot1}
 y: uint256[max_value(uint256)]
     """
+
     with pytest.raises(
         StorageLayoutException,
         match=f"Invalid storage slot, tried to allocate slots 1 through {2**256}",
     ):
         get_contract(code)
```

### Comparing `vyper-0.4.0b5/tests/unit/semantics/types/test_event.py` & `vyper-0.4.0b6/tests/unit/semantics/types/test_event.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/types/test_pure_types.py` & `vyper-0.4.0b6/tests/unit/semantics/types/test_pure_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/types/test_size_in_bytes.py` & `vyper-0.4.0b6/tests/unit/semantics/types/test_size_in_bytes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/types/test_type_from_abi.py` & `vyper-0.4.0b6/tests/unit/semantics/types/test_type_from_abi.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/tests/unit/semantics/types/test_type_from_annotation.py` & `vyper-0.4.0b6/tests/unit/semantics/types/test_type_from_annotation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/__init__.py` & `vyper-0.4.0b6/vyper/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/__main__.py` & `vyper-0.4.0b6/vyper/__main__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/abi_types.py` & `vyper-0.4.0b6/vyper/abi_types.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ast/README.md` & `vyper-0.4.0b6/vyper/ast/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ast/grammar.lark` & `vyper-0.4.0b6/vyper/ast/grammar.lark`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         | constant_def
         | variable_def
         | enum_def // TODO deprecate at some point in favor of flag
         | flag_def
         | event_def
         | function_def
         | immutable_def
+        | transient_def
         | exports_decl
         | _NEWLINE )*
 
 
 // Import statements (Supports all styles of Python imports)
 _AS: "as"
 _FROM: "from"
@@ -43,17 +44,21 @@
 constant_def: (constant_private | constant_with_getter) "=" expr
 
 // immutable definitions
 // NOTE: Temporary until decorators used
 immutable: "immutable" "(" type ")"
 immutable_def: NAME ":" immutable
 
+// transient definitions
+transient: "transient" "(" type ")"
+transient_def: NAME ":" transient
+
 variable: NAME ":" type
 // NOTE: Temporary until decorators used
-variable_with_getter: NAME ":" "public" "(" (type | immutable) ")"
+variable_with_getter: NAME ":" "public" "(" (type | immutable | transient) ")"
 variable_def: variable | variable_with_getter
 
 // A decorator "wraps" a method, modifying it's context.
 // NOTE: One or more can be applied (some combos might conflict)
 decorator: "@" NAME [ "(" [arguments] ")" ] _NEWLINE
 decorators: decorator+
 
@@ -94,15 +99,15 @@
 // Types
 array_def: (NAME | array_def | dyn_array_def) "[" expr "]"
 dyn_array_def: "DynArray" "[" (NAME | array_def | dyn_array_def) "," expr "]"
 tuple_def: "(" ( NAME | array_def | dyn_array_def | tuple_def ) ( "," ( NAME | array_def | dyn_array_def | tuple_def ) )* [","] ")"
 // NOTE: Map takes a basic type and maps to another type (can be non-basic, including maps)
 _MAP: "HashMap"
 map_def: _MAP "[" ( NAME | array_def ) "," type "]"
-imported_type: NAME "." NAME
+imported_type: NAME ("." NAME)+
 type: ( NAME | imported_type | array_def | tuple_def | map_def | dyn_array_def )
 
 // Structs can be composed of 1+ basic types or other custom_types
 _STRUCT_DECL: "struct"
 struct_member: NAME ":" type
 struct_def: _STRUCT_DECL NAME ":" _NEWLINE _INDENT (struct_member _NEWLINE)+ _DEDENT
```

### Comparing `vyper-0.4.0b5/vyper/ast/grammar.py` & `vyper-0.4.0b6/vyper/ast/grammar.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ast/identifiers.py` & `vyper-0.4.0b6/vyper/ast/identifiers.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ast/metadata.py` & `vyper-0.4.0b6/vyper/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ast/natspec.py` & `vyper-0.4.0b6/vyper/ast/natspec.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ast/nodes.py` & `vyper-0.4.0b6/vyper/ast/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ast as python_ast
 import contextlib
 import copy
 import decimal
 import functools
+import math
 import operator
 import pickle
 import sys
 import warnings
 from typing import Any, Optional, Union
 
 from vyper.ast.metadata import NodeMetadata
@@ -21,15 +22,22 @@
     SyntaxException,
     TypeMismatch,
     UnfoldableNode,
     VariableDeclarationException,
     VyperException,
     ZeroDivisionException,
 )
-from vyper.utils import MAX_DECIMAL_PLACES, SizeLimits, annotate_source_code, evm_div, sha256sum
+from vyper.utils import (
+    MAX_DECIMAL_PLACES,
+    SizeLimits,
+    annotate_source_code,
+    evm_div,
+    quantize,
+    sha256sum,
+)
 
 NODE_BASE_ATTRIBUTES = (
     "_children",
     "_depth",
     "_parent",
     "ast_type",
     "node_id",
@@ -770,15 +778,14 @@
     def is_literal_value(self):
         return True
 
 
 class Num(Constant):
     # inherited class for all numeric constant node types
     __slots__ = ()
-    _translated_fields = {"n": "value"}
 
     @property
     def n(self):
         # TODO phase out use of Num.n and remove this
         return self.value
 
     def validate(self):
@@ -820,14 +827,15 @@
 
     def to_dict(self):
         ast_dict = super().to_dict()
         ast_dict["value"] = self.node_source_code
         return ast_dict
 
     def validate(self):
+        # note: maybe use self.value == quantize(self.value) for this check
         if self.value.as_tuple().exponent < -MAX_DECIMAL_PLACES:
             raise InvalidLiteral("Vyper supports a maximum of ten decimal points", self)
         if self.value < SizeLimits.MIN_AST_DECIMAL:
             raise OverflowException("Value is below lower bound for decimal types", self)
         if self.value > SizeLimits.MAX_AST_DECIMAL:
             raise OverflowException("Value exceeds upper bound for decimal types", self)
 
@@ -839,15 +847,14 @@
     Attributes
     ----------
     value : str
         Value of the node, represented as a string taken directly from the contract source.
     """
 
     __slots__ = ()
-    _translated_fields = {"n": "value"}
 
     def validate(self):
         if "_" in self.value:
             raise InvalidLiteral("Underscores not allowed in hex literals", self)
         if len(self.value) % 2:
             raise InvalidLiteral("Hex notation requires an even number of digits", self)
 
@@ -1007,17 +1014,23 @@
     _pretty = "*"
 
     def _op(self, left, right):
         assert type(left) is type(right)
         value = left * right
         if isinstance(left, decimal.Decimal):
             # ensure that the result is truncated to MAX_DECIMAL_PLACES
-            return value.quantize(
-                decimal.Decimal(f"{1:0.{MAX_DECIMAL_PLACES}f}"), decimal.ROUND_DOWN
-            )
+            try:
+                # if the intermediate result requires too many decimal places,
+                # decimal will puke - catch the error and raise an
+                # OverflowException
+                return quantize(value)
+            except decimal.InvalidOperation:
+                msg = f"{self._description} requires too many decimal places:"
+                msg += f"\n  {left} * {right} => {value}"
+                raise OverflowException(msg, self) from None
         else:
             return value
 
 
 class Div(Operator):
     __slots__ = ()
     _description = "decimal division"
@@ -1033,15 +1046,20 @@
             raise UnfoldableNode("Cannot use `/` on non-decimals (did you mean `//`?)")
 
         value = left / right
         if value < 0:
             # the EVM always truncates toward zero
             value = -(-left / right)
         # ensure that the result is truncated to MAX_DECIMAL_PLACES
-        return value.quantize(decimal.Decimal(f"{1:0.{MAX_DECIMAL_PLACES}f}"), decimal.ROUND_DOWN)
+        try:
+            return quantize(value)
+        except decimal.InvalidOperation:
+            msg = f"{self._description} requires too many decimal places:"
+            msg += f"\n  {left} {self._pretty} {right} => {value}"
+            raise OverflowException(msg, self) from None
 
 
 class FloorDiv(VyperNode):
     __slots__ = ()
     _description = "integer division"
     _pretty = "//"
 
@@ -1078,14 +1096,23 @@
     _pretty = "**"
 
     def _op(self, left, right):
         if isinstance(left, decimal.Decimal):
             raise TypeMismatch("Cannot perform exponentiation on decimal values.", self._parent)
         if right < 0:
             raise InvalidOperation("Cannot calculate a negative power", self._parent)
+        # prevent a compiler hang. we are ok with false positives at this
+        # stage since we are just trying to filter out inputs which can cause
+        # the compiler to hang. the others will get caught during constant
+        # folding or codegen.
+        # l**r > 2**256
+        # r * ln(l) > ln(2 ** 256)
+        # r > ln(2 ** 256) / ln(l)
+        if right > math.log(decimal.Decimal(2**257)) / math.log(decimal.Decimal(left)):
+            raise InvalidLiteral("Out of bounds", self)
         return int(left**right)
 
 
 class BitAnd(Operator):
     __slots__ = ()
     _description = "bitwise and"
     _pretty = "&"
```

### Comparing `vyper-0.4.0b5/vyper/ast/nodes.pyi` & `vyper-0.4.0b6/vyper/ast/nodes.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 class Tuple(VyperNode):
     elements: list = ...
 
 class Dict(VyperNode):
     keys: list = ...
     values: list = ...
 
-class Name(VyperNode):
+class Name(ExprNode):
     id: str = ...
     _type: str = ...
 
 class Expr(VyperNode):
     value: ExprNode = ...
 
 class ExtCall(VyperNode):
```

### Comparing `vyper-0.4.0b5/vyper/ast/parse.py` & `vyper-0.4.0b6/vyper/ast/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     if "\x00" in vyper_source:
         raise ParserException("No null bytes (\\x00) allowed in the source code.")
     settings, class_types, for_loop_annotations, python_source = pre_parse(vyper_source)
     try:
         py_ast = python_ast.parse(python_source)
     except SyntaxError as e:
         # TODO: Ensure 1-to-1 match of source_code:reformatted_code SyntaxErrors
-        raise SyntaxException(str(e), vyper_source, e.lineno, e.offset) from e
+        raise SyntaxException(str(e), vyper_source, e.lineno, e.offset) from None
 
     # Add dummy function node to ensure local variables are treated as `AnnAssign`
     # instead of state variables (`VariableDecl`)
     if add_fn_node:
         fn_node = python_ast.FunctionDef(add_fn_node, py_ast.body, [], [])
         fn_node.body = py_ast.body
         fn_node.args = python_ast.arguments(defaults=[])
@@ -431,37 +431,37 @@
                 raise SyntaxException(
                     "Hex notation requires an even number of digits",
                     self._source_code,
                     node.lineno,
                     node.col_offset,
                 )
             node.ast_type = "Hex"
-            node.n = value
+            node.value = value
 
         elif value.lower()[:2] == "0b":
             node.ast_type = "Bytes"
             mod = (len(value) - 2) % 8
             if mod:
                 raise SyntaxException(
                     f"Bit notation requires a multiple of 8 bits. {8-mod} bit(s) are missing.",
                     self._source_code,
                     node.lineno,
                     node.col_offset,
                 )
             node.value = int(value, 2).to_bytes(len(value) // 8, "big")
 
-        elif isinstance(node.n, float):
+        elif isinstance(node.value, float):
             node.ast_type = "Decimal"
-            node.n = Decimal(value)
+            node.value = Decimal(value)
 
-        elif isinstance(node.n, int):
+        elif isinstance(node.value, int):
             node.ast_type = "Int"
 
-        else:
-            raise CompilerPanic(f"Unexpected type for Constant value: {type(node.n).__name__}")
+        else:  # pragma: nocover
+            raise CompilerPanic(f"Unexpected type for Constant value: {type(node.value).__name__}")
 
         return node
 
     def visit_UnaryOp(self, node):
         """
         Adjust operand value and discard unary operations, where possible.
```

### Comparing `vyper-0.4.0b5/vyper/ast/pre_parser.py` & `vyper-0.4.0b6/vyper/ast/pre_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,14 +199,20 @@
                     elif pragma.startswith("evm-version "):
                         if settings.evm_version is not None:
                             raise StructureException("pragma evm-version specified twice!", start)
                         evm_version = pragma.removeprefix("evm-version").strip()
                         if evm_version not in EVM_VERSIONS:
                             raise StructureException("Invalid evm version: `{evm_version}`", start)
                         settings.evm_version = evm_version
+                    elif pragma.startswith("experimental-codegen"):
+                        if settings.experimental_codegen is not None:
+                            raise StructureException(
+                                "pragma experimental-codegen specified twice!", start
+                            )
+                        settings.experimental_codegen = True
 
                     else:
                         raise StructureException(f"Unknown pragma `{pragma.split()[0]}`")
 
             if typ == NAME and string in ("class", "yield"):
                 raise SyntaxException(
                     f"The `{string}` keyword is not allowed. ", code, start[0], start[1]
```

### Comparing `vyper-0.4.0b5/vyper/ast/utils.py` & `vyper-0.4.0b6/vyper/ast/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ast/validation.py` & `vyper-0.4.0b6/vyper/ast/validation.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/builtins/_convert.py` & `vyper-0.4.0b6/vyper/builtins/_convert.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/builtins/_signatures.py` & `vyper-0.4.0b6/vyper/builtins/_signatures.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/builtins/_utils.py` & `vyper-0.4.0b6/vyper/builtins/_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/builtins/functions.py` & `vyper-0.4.0b6/vyper/builtins/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from vyper import ast as vy_ast
 from vyper.abi_types import ABI_Tuple
 from vyper.ast.validation import validate_call_args
 from vyper.codegen.abi_encoder import abi_encode
 from vyper.codegen.context import Context, VariableRecord
 from vyper.codegen.core import (
+    LOAD,
     STORE,
     IRnode,
     add_ofst,
     bytes_data_ptr,
     calculate_type_for_external_return,
     check_external_call,
     clamp,
@@ -32,15 +33,15 @@
     shl,
     shr,
     unwrap_location,
 )
 from vyper.codegen.expr import Expr
 from vyper.codegen.ir_node import Encoding, scope_multi
 from vyper.codegen.keccak256_helper import keccak256_helper
-from vyper.evm.address_space import MEMORY, STORAGE
+from vyper.evm.address_space import MEMORY
 from vyper.exceptions import (
     ArgumentException,
     CompilerPanic,
     InvalidLiteral,
     InvalidType,
     StateAccessViolation,
     StructureException,
@@ -225,53 +226,64 @@
     def build_IR(self, expr, context):
         return convert(expr, context)
 
 
 ADHOC_SLICE_NODE_MACROS = ["~calldata", "~selfcode", "~extcode"]
 
 
+# make sure we don't overrun the source buffer, checking for overflow:
+# valid inputs satisfy:
+#   `assert !(start+length > src_len || start+length < start`
+def _make_slice_bounds_check(start, length, src_len):
+    with start.cache_when_complex("start") as (b1, start):
+        with add_ofst(start, length).cache_when_complex("end") as (b2, end):
+            arithmetic_overflow = ["lt", end, start]
+            buffer_oob = ["gt", end, src_len]
+            ok = ["iszero", ["or", arithmetic_overflow, buffer_oob]]
+            return b1.resolve(b2.resolve(["assert", ok]))
+
+
 def _build_adhoc_slice_node(sub: IRnode, start: IRnode, length: IRnode, context: Context) -> IRnode:
     assert length.is_literal, "typechecker failed"
     assert isinstance(length.value, int)  # mypy hint
 
     dst_typ = BytesT(length.value)
     # allocate a buffer for the return value
     np = context.new_internal_variable(dst_typ)
 
     # `msg.data` by `calldatacopy`
     if sub.value == "~calldata":
         node = [
             "seq",
-            ["assert", ["le", ["add", start, length], "calldatasize"]],  # runtime bounds check
+            _make_slice_bounds_check(start, length, "calldatasize"),
             ["mstore", np, length],
             ["calldatacopy", np + 32, start, length],
             np,
         ]
 
     # `self.code` by `codecopy`
     elif sub.value == "~selfcode":
         node = [
             "seq",
-            ["assert", ["le", ["add", start, length], "codesize"]],  # runtime bounds check
+            _make_slice_bounds_check(start, length, "codesize"),
             ["mstore", np, length],
             ["codecopy", np + 32, start, length],
             np,
         ]
 
     # `<address>.code` by `extcodecopy`
     else:
         assert sub.value == "~extcode" and len(sub.args) == 1
         node = [
             "with",
             "_extcode_address",
             sub.args[0],
             [
                 "seq",
-                # runtime bounds check
-                ["assert", ["le", ["add", start, length], ["extcodesize", "_extcode_address"]]],
+                _make_slice_bounds_check(start, length, ["extcodesize", "_extcode_address"]),
                 ["mstore", np, length],
                 ["extcodecopy", "_extcode_address", np + 32, start, length],
                 np,
             ],
         ]
 
     assert isinstance(length.value, int)  # mypy hint
@@ -363,15 +375,15 @@
 
             dst_maxlen = length.value if length.is_literal else src_maxlen
 
             buflen = dst_maxlen
 
             # add 32 bytes to the buffer size bc word access might
             # be unaligned (see below)
-            if src.location == STORAGE:
+            if src.location.word_addressable:
                 buflen += 32
 
             # Get returntype string or bytes
             assert isinstance(src.typ, _BytestringT) or is_bytes32
             # TODO: try to get dst_typ from semantic analysis
             if isinstance(src.typ, StringT):
                 dst_typ = StringT(dst_maxlen)
@@ -390,16 +402,16 @@
                 src_len = 32
                 src_data = src
             else:
                 src_len = get_bytearray_length(src)
                 src_data = bytes_data_ptr(src)
 
             # general case. byte-for-byte copy
-            if src.location == STORAGE:
-                # because slice uses byte-addressing but storage
+            if src.location.word_addressable:
+                # because slice uses byte-addressing but storage/tstorage
                 # is word-aligned, this algorithm starts at some number
                 # of bytes before the data section starts, and might copy
                 # an extra word. the pseudocode is:
                 #   dst_data = dst + 32
                 #   copy_dst = dst_data - start % 32
                 #   src_data = src + 32
                 #   copy_src = src_data + (start - start % 32) / 32
@@ -436,16 +448,15 @@
                 copy_len = length
                 copy_maxlen = buflen
 
             do_copy = copy_bytes(copy_dst, copy_src, copy_len, copy_maxlen)
 
             ret = [
                 "seq",
-                # make sure we don't overrun the source buffer
-                ["assert", ["le", ["add", start, length], src_len]],  # bounds check
+                _make_slice_bounds_check(start, length, src_len),
                 do_copy,
                 ["mstore", dst, length],  # set length
                 dst,  # return pointer to dst
             ]
             ret = IRnode.from_list(ret, typ=dst_typ, location=MEMORY)
             return b1.resolve(b2.resolve(b3.resolve(ret)))
 
@@ -824,27 +835,14 @@
 class ECMul(_ECArith):
     _id = "ecmul"
     _inputs = [("point", SArrayT(UINT256_T, 2)), ("scalar", UINT256_T)]
     _return_type = SArrayT(UINT256_T, 2)
     _precompile = 0x7
 
 
-def _generic_element_getter(op):
-    def f(index):
-        return IRnode.from_list(
-            [op, ["add", "_sub", ["add", 32, ["mul", 32, index]]]], typ=INT128_T
-        )
-
-    return f
-
-
-def _storage_element_getter(index):
-    return IRnode.from_list(["sload", ["add", "_sub", ["add", 1, index]]], typ=INT128_T)
-
-
 class Extract32(BuiltinFunctionT):
     _id = "extract32"
     _inputs = [("b", BytesT.any()), ("start", IntegerT.unsigneds())]
     _kwargs = {"output_type": KwargSettings(TYPE_T.any(), BYTES32_T)}
 
     def fetch_call_return(self, node):
         self._validate_arg_types(node)
@@ -868,89 +866,55 @@
         else:
             output_typedef = TYPE_T(BYTES32_T)
 
         return {"output_type": output_typedef}
 
     @process_inputs
     def build_IR(self, expr, args, kwargs, context):
-        sub, index = args
+        bytez, index = args
         ret_type = kwargs["output_type"]
 
-        # Get length and specific element
-        if sub.location == STORAGE:
-            lengetter = IRnode.from_list(["sload", "_sub"], typ=INT128_T)
-            elementgetter = _storage_element_getter
+        def finalize(ret):
+            annotation = "extract32"
+            ret = IRnode.from_list(ret, typ=ret_type, annotation=annotation)
+            return clamp_basetype(ret)
+
+        with bytez.cache_when_complex("_sub") as (b1, bytez):
+            # merge
+            length = get_bytearray_length(bytez)
+            index = clamp2(0, index, ["sub", length, 32], signed=True)
+            with index.cache_when_complex("_index") as (b2, index):
+                assert not index.typ.is_signed
+
+                # "easy" case, byte- addressed locations:
+                if bytez.location.word_scale == 32:
+                    word = LOAD(add_ofst(bytes_data_ptr(bytez), index))
+                    return finalize(b1.resolve(b2.resolve(word)))
+
+                # storage and transient storage, word-addressed
+                assert bytez.location.word_scale == 1
+
+                slot = IRnode.from_list(["div", index, 32])
+                # byte offset within the slot
+                byte_ofst = IRnode.from_list(["mod", index, 32])
+
+                with byte_ofst.cache_when_complex("byte_ofst") as (
+                    b3,
+                    byte_ofst,
+                ), slot.cache_when_complex("slot") as (b4, slot):
+                    # perform two loads and merge
+                    w1 = LOAD(add_ofst(bytes_data_ptr(bytez), slot))
+                    w2 = LOAD(add_ofst(bytes_data_ptr(bytez), ["add", slot, 1]))
+
+                    left_bytes = shl(["mul", 8, byte_ofst], w1)
+                    right_bytes = shr(["mul", 8, ["sub", 32, byte_ofst]], w2)
+                    merged = ["or", left_bytes, right_bytes]
 
-        else:
-            op = sub.location.load_op
-            lengetter = IRnode.from_list([op, "_sub"], typ=INT128_T)
-            elementgetter = _generic_element_getter(op)
-
-        # TODO rewrite all this with cache_when_complex and bitshifts
-
-        # Special case: index known to be a multiple of 32
-        if isinstance(index.value, int) and not index.value % 32:
-            o = IRnode.from_list(
-                [
-                    "with",
-                    "_sub",
-                    sub,
-                    elementgetter(
-                        ["div", clamp2(0, index, ["sub", lengetter, 32], signed=True), 32]
-                    ),
-                ],
-                typ=ret_type,
-                annotation="extracting 32 bytes",
-            )
-        # General case
-        else:
-            o = IRnode.from_list(
-                [
-                    "with",
-                    "_sub",
-                    sub,
-                    [
-                        "with",
-                        "_len",
-                        lengetter,
-                        [
-                            "with",
-                            "_index",
-                            clamp2(0, index, ["sub", "_len", 32], signed=True),
-                            [
-                                "with",
-                                "_mi32",
-                                ["mod", "_index", 32],
-                                [
-                                    "with",
-                                    "_di32",
-                                    ["div", "_index", 32],
-                                    [
-                                        "if",
-                                        "_mi32",
-                                        [
-                                            "add",
-                                            ["mul", elementgetter("_di32"), ["exp", 256, "_mi32"]],
-                                            [
-                                                "div",
-                                                elementgetter(["add", "_di32", 1]),
-                                                ["exp", 256, ["sub", 32, "_mi32"]],
-                                            ],
-                                        ],
-                                        elementgetter("_di32"),
-                                    ],
-                                ],
-                            ],
-                        ],
-                    ],
-                ],
-                typ=ret_type,
-                annotation="extract32",
-            )
-        return IRnode.from_list(clamp_basetype(o), typ=ret_type)
+                    ret = ["if", byte_ofst, merged, left_bytes]
+                    return finalize(b1.resolve(b2.resolve(b3.resolve(b4.resolve(ret)))))
 
 
 class AsWeiValue(BuiltinFunctionT):
     _id = "as_wei_value"
     _inputs = [("value", (IntegerT.any(), DecimalT())), ("unit", StringT.any())]
     _return_type = UINT256_T
```

### Comparing `vyper-0.4.0b5/vyper/builtins/interfaces/IERC20.vyi` & `vyper-0.4.0b6/vyper/builtins/interfaces/IERC20.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/builtins/interfaces/IERC4626.vyi` & `vyper-0.4.0b6/vyper/builtins/interfaces/IERC4626.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/builtins/interfaces/IERC721.vyi` & `vyper-0.4.0b6/vyper/builtins/interfaces/IERC721.vyi`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/cli/vyper_compile.py` & `vyper-0.4.0b6/vyper/cli/vyper_compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import sys
 import warnings
 from pathlib import Path
 from typing import Any, Iterable, Iterator, Optional, Set, TypeVar
 
 import vyper
 import vyper.codegen.ir_node as ir_node
+import vyper.evm.opcodes as evm
 from vyper.cli import vyper_json
 from vyper.compiler.input_bundle import FileInput, FilesystemInputBundle
 from vyper.compiler.settings import (
     VYPER_TRACEBACK_LIMIT,
     OptimizationLevel,
     Settings,
     _set_debug_mode,
 )
-from vyper.evm.opcodes import DEFAULT_EVM_VERSION, EVM_VERSIONS
 from vyper.typing import ContractPath, OutputFormats
 
 T = TypeVar("T")
 
 format_options_help = """Format to print, one or more of:
 bytecode (default) - Deployable bytecode
 bytecode_runtime   - Bytecode at runtime
@@ -61,14 +61,15 @@
 
 def _parse_cli_args():
     return _parse_args(sys.argv[1:])
 
 
 def _cli_helper(f, output_formats, compiled):
     if output_formats == ("combined_json",):
+        compiled = {str(path): v for (path, v) in compiled.items()}
         print(json.dumps(compiled), file=f)
         return
 
     for contract_data in compiled.values():
         for data in contract_data.values():
             if isinstance(data, (list, dict)):
                 print(json.dumps(data), file=f)
@@ -102,17 +103,17 @@
         "--storage-layout-file",
         help="Override storage slots provided by compiler",
         dest="storage_layout",
         nargs="+",
     )
     parser.add_argument(
         "--evm-version",
-        help=f"Select desired EVM version (default {DEFAULT_EVM_VERSION}). "
+        help=f"Select desired EVM version (default {evm.DEFAULT_EVM_VERSION}). "
         "note: cancun support is EXPERIMENTAL",
-        choices=list(EVM_VERSIONS),
+        choices=list(evm.EVM_VERSIONS),
         dest="evm_version",
     )
     parser.add_argument("--no-optimize", help="Do not optimize", action="store_true")
     parser.add_argument(
         "-O",
         "--optimize",
         help="Optimization flag (defaults to 'gas')",
```

### Comparing `vyper-0.4.0b5/vyper/cli/vyper_ir.py` & `vyper-0.4.0b6/vyper/cli/vyper_ir.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/cli/vyper_json.py` & `vyper-0.4.0b6/vyper/cli/vyper_json.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/abi_encoder.py` & `vyper-0.4.0b6/vyper/codegen/abi_encoder.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/arithmetic.py` & `vyper-0.4.0b6/vyper/codegen/arithmetic.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/context.py` & `vyper-0.4.0b6/vyper/codegen/context.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/core.py` & `vyper-0.4.0b6/vyper/codegen/core.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/events.py` & `vyper-0.4.0b6/vyper/codegen/events.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/expr.py` & `vyper-0.4.0b6/vyper/codegen/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,20 +202,17 @@
             ret._referenced_variables = {varinfo}
             return ret
 
     # x.y or x[5]
     def parse_Attribute(self):
         typ = self.expr._metadata["type"]
 
-        # MyFlag.foo
-        if (
-            isinstance(typ, FlagT)
-            and isinstance(self.expr.value, vy_ast.Name)
-            and typ.name == self.expr.value.id
-        ):
+        # check if we have a flag constant, e.g.
+        # [lib1].MyFlag.FOO
+        if isinstance(typ, FlagT) and is_type_t(self.expr.value._metadata["type"], FlagT):
             # 0, 1, 2, .. 255
             flag_id = typ._flag_members[self.expr.attr]
             value = 2**flag_id  # 0 => 0001, 1 => 0010, 2 => 0100, etc.
             return IRnode.from_list(value, typ=typ)
 
         # x.balance: balance of address x
         if self.expr.attr == "balance":
@@ -269,15 +266,15 @@
             elif key == "msg.gas":
                 return IRnode.from_list(["gas"], typ=UINT256_T)
             elif key == "block.prevrandao":
                 if not version_check(begin="paris"):
                     warning = "tried to use block.prevrandao in pre-Paris "
                     warning += "environment! Suggest using block.difficulty instead."
                     vyper_warn(warning, self.expr)
-                return IRnode.from_list(["prevrandao"], typ=UINT256_T)
+                return IRnode.from_list(["prevrandao"], typ=BYTES32_T)
             elif key == "block.difficulty":
                 if version_check(begin="paris"):
                     warning = "tried to use block.difficulty in post-Paris "
                     warning += "environment! Suggest using block.prevrandao instead."
                     vyper_warn(warning, self.expr)
                 return IRnode.from_list(["difficulty"], typ=UINT256_T)
             elif key == "block.timestamp":
```

### Comparing `vyper-0.4.0b5/vyper/codegen/external_call.py` & `vyper-0.4.0b6/vyper/codegen/external_call.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/function_definitions/common.py` & `vyper-0.4.0b6/vyper/codegen/function_definitions/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/function_definitions/external_function.py` & `vyper-0.4.0b6/vyper/codegen/function_definitions/external_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,18 +150,14 @@
     # (note: internal functions do not need to adjust gas estimate since
     frame_info = func_t._ir_info.frame_info
 
     mem_expansion_cost = calc_mem_gas(frame_info.mem_used)
     common_ir.add_gas_estimate += mem_expansion_cost
     func_t._ir_info.gas_estimate = common_ir.gas
 
-    # pass metadata through for venom pipeline:
-    common_ir.passthrough_metadata["func_t"] = func_t
-    common_ir.passthrough_metadata["frame_info"] = frame_info
-
 
 def generate_ir_for_external_function(code, compilation_target):
     # TODO type hints:
     # def generate_ir_for_external_function(
     #    code: vy_ast.FunctionDef,
     #    compilation_target: ModuleT,
     # ) -> IRnode:
```

### Comparing `vyper-0.4.0b5/vyper/codegen/function_definitions/internal_function.py` & `vyper-0.4.0b6/vyper/codegen/function_definitions/internal_function.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,14 +76,10 @@
         ["seq"] + nonreentrant_post + [["exit_to", "return_pc"]],
     ]
 
     ir_node = IRnode.from_list(["seq", body, cleanup_routine])
 
     # tag gas estimate and frame info
     func_t._ir_info.gas_estimate = ir_node.gas
-    frame_info = tag_frame_info(func_t, context)
-
-    # pass metadata through for venom pipeline:
-    ir_node.passthrough_metadata["frame_info"] = frame_info
-    ir_node.passthrough_metadata["func_t"] = func_t
+    tag_frame_info(func_t, context)
 
     return InternalFuncIR(ir_node)
```

### Comparing `vyper-0.4.0b5/vyper/codegen/ir_node.py` & `vyper-0.4.0b6/vyper/codegen/ir_node.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/jumptable_utils.py` & `vyper-0.4.0b6/vyper/codegen/jumptable_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/keccak256_helper.py` & `vyper-0.4.0b6/vyper/codegen/keccak256_helper.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/memory_allocator.py` & `vyper-0.4.0b6/vyper/codegen/memory_allocator.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/module.py` & `vyper-0.4.0b6/vyper/codegen/module.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/codegen/return_.py` & `vyper-0.4.0b6/vyper/codegen/return_.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,14 @@
         fill_return_buffer = IRnode.from_list(
             fill_return_buffer, annotation=f"fill return buffer {func_t._ir_info.ir_identifier}"
         )
         cleanup_loops = "cleanup_repeat" if context.forvars else "seq"
         # NOTE: because stack analysis is incomplete, cleanup_repeat must
         # come after fill_return_buffer otherwise the stack will break
         jump_to_exit_ir = IRnode.from_list(jump_to_exit)
-        jump_to_exit_ir.passthrough_metadata["func_t"] = func_t
         return IRnode.from_list(["seq", fill_return_buffer, cleanup_loops, jump_to_exit_ir])
 
     if context.return_type is None:
         if context.is_internal:
             jump_to_exit += ["return_pc"]
         return finalize(["seq"])
```

### Comparing `vyper-0.4.0b5/vyper/codegen/self_call.py` & `vyper-0.4.0b6/vyper/codegen/self_call.py`

 * *Files 10% similar despite different names*

```diff
@@ -108,10 +108,8 @@
         call_sequence,
         typ=func_t.return_type,
         location=MEMORY,
         annotation=stmt_expr.get("node_source_code"),
         add_gas_estimate=func_t._ir_info.gas_estimate,
     )
     o.is_self_call = True
-    o.passthrough_metadata["func_t"] = func_t
-    o.passthrough_metadata["args_ir"] = args_ir
     return o
```

### Comparing `vyper-0.4.0b5/vyper/codegen/stmt.py` & `vyper-0.4.0b6/vyper/codegen/stmt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 import vyper.codegen.events as events
 import vyper.utils as util
 from vyper import ast as vy_ast
+from vyper.codegen.abi_encoder import abi_encode
 from vyper.codegen.context import Constancy, Context
 from vyper.codegen.core import (
     LOAD,
     STORE,
     IRnode,
     clamp_le,
     get_dyn_array_count,
     get_element_ptr,
-    make_byte_array_copier,
+    get_type_for_exact_size,
     make_setter,
-    zero_pad,
+    wrap_value_for_external_return,
 )
 from vyper.codegen.expr import Expr
 from vyper.codegen.return_ import make_return_stmt
 from vyper.evm.address_space import MEMORY, STORAGE
-from vyper.exceptions import (
-    CodegenPanic,
-    CompilerPanic,
-    StructureException,
-    TypeCheckFailure,
-    tag_exceptions,
-)
+from vyper.exceptions import CodegenPanic, StructureException, TypeCheckFailure, tag_exceptions
 from vyper.semantics.types import DArrayT
 from vyper.semantics.types.shortcuts import UINT256_T
 
 
 class Stmt:
     def __init__(self, node: vy_ast.VyperNode, context: Context) -> None:
         self.stmt = node
@@ -128,47 +123,34 @@
         try:
             tmp = self.context.constancy
             self.context.constancy = Constancy.Constant
             msg_ir = Expr(msg, self.context).ir_node
         finally:
             self.context.constancy = tmp
 
-        # TODO this is probably useful in codegen.core
-        # compare with eval_seq.
-        def _get_last(ir):
-            if len(ir.args) == 0:
-                return ir.value
-            return _get_last(ir.args[-1])
-
-        # TODO maybe use ensure_in_memory
-        if msg_ir.location != MEMORY:
-            buf = self.context.new_internal_variable(msg_ir.typ)
-            instantiate_msg = make_byte_array_copier(buf, msg_ir)
-        else:
-            buf = _get_last(msg_ir)
-            if not isinstance(buf, int):  # pragma: nocover
-                raise CompilerPanic(f"invalid bytestring {buf}\n{self}")
-            instantiate_msg = msg_ir
+        msg_ir = wrap_value_for_external_return(msg_ir)
+        bufsz = 64 + msg_ir.typ.memory_bytes_required
+        buf = self.context.new_internal_variable(get_type_for_exact_size(bufsz))
 
         # offset of bytes in (bytes,)
         method_id = util.method_id_int("Error(string)")
 
-        # abi encode method_id + bytestring
-        assert buf >= 36, "invalid buffer"
-        # we don't mind overwriting other memory because we are
-        # getting out of here anyway.
-        _runtime_length = ["mload", buf]
-        revert_seq = [
-            "seq",
-            instantiate_msg,
-            zero_pad(buf),
-            ["mstore", buf - 64, method_id],
-            ["mstore", buf - 32, 0x20],
-            ["revert", buf - 36, ["add", 4 + 32 + 32, ["ceil32", _runtime_length]]],
-        ]
+        # abi encode method_id + bytestring to `buf+32`, then
+        # write method_id to `buf` and get out of here
+        payload_buf = buf + 32
+        bufsz -= 32  # reduce buffer by size of `method_id` slot
+        encoded_length = abi_encode(payload_buf, msg_ir, self.context, bufsz, returns_len=True)
+        with encoded_length.cache_when_complex("encoded_len") as (b1, encoded_length):
+            revert_seq = [
+                "seq",
+                ["mstore", buf, method_id],
+                ["revert", buf + 28, ["add", 4, encoded_length]],
+            ]
+            revert_seq = b1.resolve(revert_seq)
+
         if is_raise:
             ir_node = revert_seq
         else:
             ir_node = ["if", ["iszero", test_expr], revert_seq]
         return IRnode.from_list(ir_node, error_msg="user revert with reason")
 
     def parse_Assert(self):
```

### Comparing `vyper-0.4.0b5/vyper/compiler/README.md` & `vyper-0.4.0b6/vyper/compiler/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/compiler/__init__.py` & `vyper-0.4.0b6/vyper/compiler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import vyper.ast as vy_ast  # break an import cycle
 import vyper.codegen.core as codegen
 import vyper.compiler.output as output
 from vyper.compiler.input_bundle import FileInput, InputBundle, PathLike
 from vyper.compiler.phases import CompilerData
 from vyper.compiler.settings import Settings
-from vyper.evm.opcodes import DEFAULT_EVM_VERSION, anchor_evm_version
+from vyper.evm.opcodes import anchor_evm_version
 from vyper.typing import ContractPath, OutputFormats, StorageLayout
 
 OUTPUT_FORMATS = {
     # requires vyper_module
     "ast_dict": output.build_ast_dict,
     # requires annotated_vyper_module
     "annotated_ast_dict": output.build_annotated_ast_dict,
@@ -21,14 +21,16 @@
     "devdoc": output.build_devdoc,
     "userdoc": output.build_userdoc,
     # requires ir_node
     "external_interface": output.build_external_interface_output,
     "interface": output.build_interface_output,
     "bb": output.build_bb_output,
     "bb_runtime": output.build_bb_runtime_output,
+    "cfg": output.build_cfg_output,
+    "cfg_runtime": output.build_cfg_runtime_output,
     "ir": output.build_ir_output,
     "ir_runtime": output.build_ir_runtime_output,
     "ir_dict": output.build_ir_dict_output,
     "ir_runtime_dict": output.build_ir_runtime_dict_output,
     "method_identifiers": output.build_method_identifiers_output,
     "metadata": output.build_metadata_output,
     # requires assembly
```

### Comparing `vyper-0.4.0b5/vyper/compiler/input_bundle.py` & `vyper-0.4.0b6/vyper/compiler/input_bundle.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/compiler/output.py` & `vyper-0.4.0b6/vyper/compiler/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,22 @@
     return compiler_data.venom_functions[0]
 
 
 def build_bb_runtime_output(compiler_data: CompilerData) -> IRnode:
     return compiler_data.venom_functions[1]
 
 
+def build_cfg_output(compiler_data: CompilerData) -> str:
+    return compiler_data.venom_functions[0].as_graph()
+
+
+def build_cfg_runtime_output(compiler_data: CompilerData) -> str:
+    return compiler_data.venom_functions[1].as_graph()
+
+
 def build_ir_output(compiler_data: CompilerData) -> IRnode:
     if compiler_data.show_gas_estimates:
         IRnode.repr_show_gas = True
     return compiler_data.ir_nodes
 
 
 def build_ir_runtime_output(compiler_data: CompilerData) -> IRnode:
```

### Comparing `vyper-0.4.0b5/vyper/compiler/phases.py` & `vyper-0.4.0b6/vyper/compiler/phases.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,14 @@
         settings: Settings
             Set optimization mode.
         show_gas_estimates: bool, optional
             Show gas estimates for abi and ir output modes
         no_bytecode_metadata: bool, optional
             Do not add metadata to bytecode. Defaults to False
         """
-        # to force experimental codegen, uncomment:
-        # settings.experimental_codegen = True
 
         if isinstance(file_input, str):
             file_input = FileInput(
                 source_code=file_input,
                 source_id=-1,
                 path=DEFAULT_CONTRACT_PATH,
                 resolved_path=DEFAULT_CONTRACT_PATH,
```

### Comparing `vyper-0.4.0b5/vyper/compiler/settings.py` & `vyper-0.4.0b6/vyper/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/compiler/utils.py` & `vyper-0.4.0b6/vyper/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/evm/address_space.py` & `vyper-0.4.0b6/vyper/evm/address_space.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 
     name: str
     word_scale: int
     load_op: str
     # TODO maybe make positional instead of defaulting to None
     store_op: Optional[str] = None
 
+    @property
+    def word_addressable(self) -> bool:
+        return self.word_scale == 1
+
 
 # alternative:
 # class Memory(AddrSpace):
 #   @property
 #   def word_scale(self):
 #     return 32
 # # implement more properties...
```

### Comparing `vyper-0.4.0b5/vyper/evm/opcodes.py` & `vyper-0.4.0b6/vyper/evm/opcodes.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/exceptions.py` & `vyper-0.4.0b6/vyper/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,16 +123,17 @@
                 line_numbers=VYPER_ERROR_LINE_NUMBERS,
             )
         except Exception:
             # necessary for certain types of syntax exceptions
             return None
 
         if isinstance(node, vy_ast.VyperNode):
-            module_node = node.get_ancestor(vy_ast.Module)
+            module_node = node.module_node
 
+            # TODO: handle cases where module is None or vy_ast.Module
             if module_node.get("path") not in (None, "<unknown>"):
                 node_msg = f'{node_msg}contract "{module_node.path}:{node.lineno}", '
 
             fn_node = node.get_ancestor(vy_ast.FunctionDef)
             if fn_node:
                 node_msg = f'{node_msg}function "{fn_node.name}", '
 
@@ -381,14 +382,18 @@
     """General unexpected error during compilation."""
 
 
 class CodegenPanic(VyperInternalException):
     """Invalid code generated during codegen phase"""
 
 
+class StackTooDeep(CodegenPanic):
+    """Stack too deep"""  # (should not happen)
+
+
 class UnexpectedNodeType(VyperInternalException):
     """Unexpected AST node type."""
 
 
 class UnexpectedValue(VyperInternalException):
     """Unexpected Value."""
```

### Comparing `vyper-0.4.0b5/vyper/ir/README.md` & `vyper-0.4.0b6/vyper/ir/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ir/compile_ir.py` & `vyper-0.4.0b6/vyper/ir/compile_ir.py`

 * *Files 0% similar despite different names*

```diff
@@ -1016,15 +1016,19 @@
         # usually generated by nested with statements that don't return like
         # (with x (with y ...))
         if assembly[i : i + 3] == ["SWAP1", "POP", "POP"]:
             # SWAP1 POP POP == POP POP
             changed = True
             del assembly[i]
             continue
-        if assembly[i : i + 2] == ["SWAP1", "SWAP1"]:
+        if (
+            isinstance(assembly[i], str)
+            and assembly[i].startswith("SWAP")
+            and assembly[i] == assembly[i + 1]
+        ):
             changed = True
             del assembly[i : i + 2]
         if assembly[i] == "SWAP1" and assembly[i + 1].lower() in COMMUTATIVE_OPS:
             changed = True
             del assembly[i]
         i += 1
```

### Comparing `vyper-0.4.0b5/vyper/ir/optimizer.py` & `vyper-0.4.0b6/vyper/ir/optimizer.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/ir/s_expressions.py` & `vyper-0.4.0b6/vyper/ir/s_expressions.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/README.md` & `vyper-0.4.0b6/vyper/semantics/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/base.py` & `vyper-0.4.0b6/vyper/semantics/analysis/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Union
 
 from vyper import ast as vy_ast
 from vyper.compiler.input_bundle import CompilerInput, FileInput
 from vyper.exceptions import CompilerPanic, StructureException
 from vyper.semantics.data_locations import DataLocation
 from vyper.semantics.types.base import VyperType
+from vyper.semantics.types.primitives import SelfT
 from vyper.utils import OrderedSet, StringEnum
 
 if TYPE_CHECKING:
     from vyper.semantics.types.function import ContractFunctionT
     from vyper.semantics.types.module import InterfaceT, ModuleT
 
 
@@ -195,16 +196,19 @@
 
     def set_position(self, position: VarOffset) -> None:
         if self.position is not None:
             raise CompilerPanic("Position was already assigned")
         assert isinstance(position, VarOffset)  # sanity check
         self.position = position
 
-    def is_module_variable(self):
-        return self.location not in (DataLocation.UNSET, DataLocation.MEMORY)
+    def is_state_variable(self):
+        non_state_locations = (DataLocation.UNSET, DataLocation.MEMORY, DataLocation.CALLDATA)
+        # `self` gets a VarInfo, but it is not considered a state
+        # variable (it is magic), so we ignore it here.
+        return self.location not in non_state_locations and not isinstance(self.typ, SelfT)
 
     def get_size(self) -> int:
         return self.typ.get_size_in(self.location)
 
     @property
     def is_transient(self):
         return self.location == DataLocation.TRANSIENT
```

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/common.py` & `vyper-0.4.0b6/vyper/semantics/analysis/common.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/constant_folding.py` & `vyper-0.4.0b6/vyper/semantics/analysis/constant_folding.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/data_positions.py` & `vyper-0.4.0b6/vyper/semantics/analysis/data_positions.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,17 +278,17 @@
             module_alias = module_info.alias
             for layout_key in module_layout.keys():
                 assert layout_key in _LAYOUT_KEYS.values()
                 ret[layout_key][module_alias] = module_layout[layout_key]
             continue
 
         assert isinstance(node, vy_ast.VariableDecl)
-        # skip non-storage variables
+        # skip non-state variables
         varinfo = node.target._metadata["varinfo"]
-        if not varinfo.is_module_variable():
+        if not varinfo.is_state_variable():
             continue
         location = varinfo.location
 
         if immutables_only and location != DataLocation.CODE:
             continue
 
         allocator = allocators.get_allocator(location)
```

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/getters.py` & `vyper-0.4.0b6/vyper/semantics/analysis/getters.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/global_.py` & `vyper-0.4.0b6/vyper/semantics/analysis/global_.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/import_graph.py` & `vyper-0.4.0b6/vyper/semantics/analysis/import_graph.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/levenshtein_utils.py` & `vyper-0.4.0b6/vyper/semantics/analysis/levenshtein_utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/local.py` & `vyper-0.4.0b6/vyper/semantics/analysis/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,27 +34,28 @@
     get_expr_info,
     get_possible_types_from_node,
     validate_expected_type,
 )
 from vyper.semantics.data_locations import DataLocation
 
 # TODO consolidate some of these imports
-from vyper.semantics.environment import CONSTANT_ENVIRONMENT_VARS, MUTABLE_ENVIRONMENT_VARS
+from vyper.semantics.environment import CONSTANT_ENVIRONMENT_VARS
 from vyper.semantics.namespace import get_namespace
 from vyper.semantics.types import (
     TYPE_T,
     VOID_TYPE,
     AddressT,
     BoolT,
     DArrayT,
     EventT,
     FlagT,
     HashMapT,
     IntegerT,
     SArrayT,
+    SelfT,
     StringT,
     StructT,
     TupleT,
     VyperType,
     _BytestringT,
     is_type_t,
     map_void,
@@ -160,29 +161,43 @@
 
 
 def _validate_msg_value_access(node: vy_ast.Attribute) -> None:
     if isinstance(node.value, vy_ast.Name) and node.attr == "value" and node.value.id == "msg":
         raise NonPayableViolation("msg.value is not allowed in non-payable functions", node)
 
 
-def _validate_pure_access(node: vy_ast.Attribute, typ: VyperType) -> None:
-    env_vars = set(CONSTANT_ENVIRONMENT_VARS.keys()) | set(MUTABLE_ENVIRONMENT_VARS.keys())
-    if isinstance(node.value, vy_ast.Name) and node.value.id in env_vars:
-        if isinstance(typ, ContractFunctionT) and typ.mutability == StateMutability.PURE:
-            return
+def _validate_pure_access(node: vy_ast.Attribute | vy_ast.Name, typ: VyperType) -> None:
+    if isinstance(typ, TYPE_T):
+        return
 
-        raise StateAccessViolation(
-            "not allowed to query contract or environment variables in pure functions", node
-        )
+    info = get_expr_info(node)
 
+    env_vars = CONSTANT_ENVIRONMENT_VARS
+    # check env variable access like `block.number`
+    if isinstance(node, vy_ast.Attribute):
+        if node.get("value.id") in env_vars:
+            raise StateAccessViolation(
+                "not allowed to query environment variables in pure functions"
+            )
+        parent_info = get_expr_info(node.value)
+        if isinstance(parent_info.typ, AddressT) and node.attr in AddressT._type_members:
+            raise StateAccessViolation("not allowed to query address members in pure functions")
+
+    if (varinfo := info.var_info) is None:
+        return
+    # self is magic. we only need to check it if it is not the root of an Attribute
+    # node. (i.e. it is bare like `self`, not `self.foo`)
+    is_naked_self = isinstance(varinfo.typ, SelfT) and not isinstance(
+        node.get_ancestor(), vy_ast.Attribute
+    )
+    if is_naked_self:
+        raise StateAccessViolation("not allowed to query `self` in pure functions")
 
-def _validate_self_reference(node: vy_ast.Name) -> None:
-    # CMC 2023-10-19 this detector seems sus, things like `a.b(self)` could slip through
-    if node.id == "self" and not isinstance(node.get_ancestor(), vy_ast.Attribute):
-        raise StateAccessViolation("not allowed to query self in pure functions", node)
+    if varinfo.is_state_variable() or is_naked_self:
+        raise StateAccessViolation("not allowed to query state variables in pure functions")
 
 
 # analyse the variable access for the attribute chain for a node
 # e.x. `x` will return varinfo for `x`
 # `module.foo` will return VarAccess for `module.foo`
 # `self.my_struct.x.y` will return VarAccess for `self.my_struct.x.y`
 def _get_variable_access(node: vy_ast.ExprNode) -> Optional[VarAccess]:
@@ -425,15 +440,15 @@
 
         var_access = _get_variable_access(target)
         assert var_access is not None
 
         info._writes.add(var_access)
 
     def _handle_module_access(self, var_access: VarAccess, target: vy_ast.ExprNode):
-        if not var_access.variable.is_module_variable():
+        if not var_access.variable.is_state_variable():
             return
 
         root_module_info = check_module_uses(target)
 
         if root_module_info is not None:
             # log the access
             self.func.mark_used_module(root_module_info)
@@ -761,18 +776,18 @@
                     kind = node.kind_str
                     msg = f"Calls to internal functions cannot use the `{kind}` keyword."
                     hint = f"remove the `{kind}` keyword"
                     raise CallViolation(msg, node.parent, hint=hint)
 
             if not func_type.from_interface:
                 for s in func_type.get_variable_writes():
-                    if s.variable.is_module_variable():
+                    if s.variable.is_state_variable():
                         func_info._writes.add(s)
                 for s in func_type.get_variable_reads():
-                    if s.variable.is_module_variable():
+                    if s.variable.is_state_variable():
                         func_info._reads.add(s)
 
             if self.function_analyzer:
                 self._check_call_mutability(func_type.mutability)
 
                 for s in func_type.get_variable_accesses():
                     self.function_analyzer._handle_module_access(s, node.func)
@@ -869,18 +884,16 @@
 
     def visit_List(self, node: vy_ast.List, typ: VyperType) -> None:
         assert isinstance(typ, (SArrayT, DArrayT))
         for element in node.elements:
             self.visit(element, typ.value_type)
 
     def visit_Name(self, node: vy_ast.Name, typ: VyperType) -> None:
-        if self.func:
-            # TODO: refactor to use expr_info mutability
-            if self.func.mutability == StateMutability.PURE:
-                _validate_self_reference(node)
+        if self.func and self.func.mutability == StateMutability.PURE:
+            _validate_pure_access(node, typ)
 
     def visit_Subscript(self, node: vy_ast.Subscript, typ: VyperType) -> None:
         if isinstance(typ, TYPE_T):
             # don't recurse; can't annotate AST children of type definition
             return
 
         if isinstance(node.value, (vy_ast.List, vy_ast.Subscript)):
```

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/module.py` & `vyper-0.4.0b6/vyper/semantics/analysis/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     InputBundle,
 )
 from vyper.evm.opcodes import version_check
 from vyper.exceptions import (
     BorrowException,
     CallViolation,
     DuplicateImport,
+    EvmVersionException,
     ExceptionList,
     ImmutableViolation,
     InitializerException,
     InvalidLiteral,
     InvalidType,
     ModuleNotFound,
     StateAccessViolation,
@@ -520,27 +521,27 @@
 
             else:
                 # regular function
                 func_t = info.typ
                 decl_node = func_t.decl_node
 
             if not isinstance(func_t, ContractFunctionT):
-                raise StructureException("not a function!", decl_node, item)
+                raise StructureException(f"not a function: `{func_t}`", decl_node, item)
             if not func_t.is_external:
                 raise StructureException("can't export non-external functions!", decl_node, item)
 
             self._add_exposed_function(func_t, item, relax=False)
             with tag_exceptions(item):  # tag with specific item
                 self._self_t.typ.add_member(func_t.name, func_t)
 
             funcs.append(func_t)
 
             # check module uses
             var_accesses = func_t.get_variable_accesses()
-            if any(s.variable.is_module_variable() for s in var_accesses):
+            if any(s.variable.is_state_variable() for s in var_accesses):
                 module_info = check_module_uses(item)
                 assert module_info is not None  # guaranteed by above checks
                 used_modules.add(module_info)
 
         node._metadata["exports_info"] = ExportsInfo(funcs, used_modules)
 
     @property
@@ -604,15 +605,15 @@
             if node.is_constant
             else Modifiability.MODIFIABLE
         )
 
         type_ = type_from_annotation(node.annotation, data_loc)
 
         if node.is_transient and not version_check(begin="cancun"):
-            raise StructureException("`transient` is not available pre-cancun", node.annotation)
+            raise EvmVersionException("`transient` is not available pre-cancun", node.annotation)
 
         var_info = VarInfo(
             type_,
             decl_node=node,
             location=data_loc,
             modifiability=modifiability,
             is_public=node.is_public,
@@ -653,14 +654,15 @@
 
         self.namespace.validate_assignment(name)
 
         return _finalize()
 
     def visit_FlagDef(self, node):
         obj = FlagT.from_FlagDef(node)
+        node._metadata["flag_type"] = obj
         self.namespace[node.name] = obj
 
     def visit_EventDef(self, node):
         obj = EventT.from_EventDef(node)
         node._metadata["event_type"] = obj
         self.namespace[node.name] = obj
         self._events.append(obj)
```

### Comparing `vyper-0.4.0b5/vyper/semantics/analysis/utils.py` & `vyper-0.4.0b6/vyper/semantics/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/environment.py` & `vyper-0.4.0b6/vyper/semantics/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class _Block(_EnvType):
     _id = "block"
     _type_members = {
         "coinbase": AddressT(),
         "difficulty": UINT256_T,
-        "prevrandao": UINT256_T,
+        "prevrandao": BYTES32_T,
         "number": UINT256_T,
         "gaslimit": UINT256_T,
         "basefee": UINT256_T,
         "prevhash": BYTES32_T,
         "timestamp": UINT256_T,
     }
```

### Comparing `vyper-0.4.0b5/vyper/semantics/namespace.py` & `vyper-0.4.0b6/vyper/semantics/namespace.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/types/__init__.py` & `vyper-0.4.0b6/vyper/semantics/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/types/base.py` & `vyper-0.4.0b6/vyper/semantics/types/base.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/types/bytestrings.py` & `vyper-0.4.0b6/vyper/semantics/types/bytestrings.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/types/function.py` & `vyper-0.4.0b6/vyper/semantics/types/function.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/types/module.py` & `vyper-0.4.0b6/vyper/semantics/types/module.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,18 +292,26 @@
         self._helper = VyperType()
         self._helper._id = self._id
 
         for f in self.function_defs:
             # note: this checks for collisions
             self.add_member(f.name, f._metadata["func_type"])
 
+        for item in self.exports_decls:
+            for fn_t in item._metadata["exports_info"].functions:
+                self.add_member(fn_t.name, fn_t)
+
         for e in self.event_defs:
             # add the type of the event so it can be used in call position
             self.add_member(e.name, TYPE_T(e._metadata["event_type"]))  # type: ignore
 
+        for f in self.flag_defs:
+            self.add_member(f.name, TYPE_T(f._metadata["flag_type"]))
+            self._helper.add_member(f.name, TYPE_T(f._metadata["flag_type"]))
+
         for s in self.struct_defs:
             # add the type of the struct so it can be used in call position
             self.add_member(s.name, TYPE_T(s._metadata["struct_type"]))  # type: ignore
             self._helper.add_member(s.name, TYPE_T(s._metadata["struct_type"]))  # type: ignore
 
         for i in self.interface_defs:
             # add the type of the interface so it can be used in call position
@@ -343,14 +351,18 @@
     def function_defs(self):
         return self._module.get_children(vy_ast.FunctionDef)
 
     @cached_property
     def event_defs(self):
         return self._module.get_children(vy_ast.EventDef)
 
+    @cached_property
+    def flag_defs(self):
+        return self._module.get_children(vy_ast.FlagDef)
+
     @property
     def struct_defs(self):
         return self._module.get_children(vy_ast.StructDef)
 
     @property
     def interface_defs(self):
         return self._module.get_children(vy_ast.InterfaceDef)
```

### Comparing `vyper-0.4.0b5/vyper/semantics/types/primitives.py` & `vyper-0.4.0b6/vyper/semantics/types/primitives.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/types/subscriptable.py` & `vyper-0.4.0b6/vyper/semantics/types/subscriptable.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/types/user.py` & `vyper-0.4.0b6/vyper/semantics/types/user.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/semantics/types/utils.py` & `vyper-0.4.0b6/vyper/semantics/types/utils.py`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/utils.py` & `vyper-0.4.0b6/vyper/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,75 +11,100 @@
 from typing import Generic, List, TypeVar, Union
 
 from vyper.exceptions import CompilerPanic, DecimalOverrideException, InvalidLiteral, VyperException
 
 _T = TypeVar("_T")
 
 
-class OrderedSet(Generic[_T], dict[_T, None]):
+class OrderedSet(Generic[_T]):
     """
     a minimal "ordered set" class. this is needed in some places
     because, while dict guarantees you can recover insertion order
     vanilla sets do not.
     no attempt is made to fully implement the set API, will add
     functionality as needed.
     """
 
     def __init__(self, iterable=None):
-        super().__init__()
+        self._data = dict()
         if iterable is not None:
-            for item in iterable:
-                self.add(item)
+            self.update(iterable)
 
     def __repr__(self):
-        keys = ", ".join(repr(k) for k in self.keys())
+        keys = ", ".join(repr(k) for k in self)
         return f"{{{keys}}}"
 
-    def get(self, *args, **kwargs):
-        raise RuntimeError("can't call get() on OrderedSet!")
+    def __iter__(self):
+        return iter(self._data)
+
+    def __contains__(self, item):
+        return self._data.__contains__(item)
+
+    def __len__(self):
+        return len(self._data)
 
     def first(self):
         return next(iter(self))
 
     def add(self, item: _T) -> None:
-        self[item] = None
+        self._data[item] = None
 
     def remove(self, item: _T) -> None:
-        del self[item]
+        del self._data[item]
+
+    def drop(self, item: _T):
+        # friendly version of remove
+        self._data.pop(item, None)
+
+    def dropmany(self, iterable):
+        for item in iterable:
+            self._data.pop(item, None)
 
     def difference(self, other):
         ret = self.copy()
-        for k in other.keys():
-            if k in ret:
-                ret.remove(k)
+        ret.dropmany(other)
         return ret
 
+    def update(self, other):
+        # CMC 2024-03-22 for some reason, this is faster than dict.update?
+        # (maybe size dependent)
+        for item in other:
+            self._data[item] = None
+
     def union(self, other):
         return self | other
 
-    def update(self, other):
-        super().update(self.__class__.fromkeys(other))
+    def __ior__(self, other):
+        self.update(other)
+        return self
 
     def __or__(self, other):
-        return self.__class__(super().__or__(other))
+        ret = self.copy()
+        ret.update(other)
+        return ret
+
+    def __eq__(self, other):
+        return self._data == other._data
 
     def copy(self):
-        return self.__class__(super().copy())
+        cls = self.__class__
+        ret = cls.__new__(cls)
+        ret._data = self._data.copy()
+        return ret
 
     @classmethod
     def intersection(cls, *sets):
-        res = OrderedSet()
         if len(sets) == 0:
             raise ValueError("undefined: intersection of no sets")
-        if len(sets) == 1:
-            return sets[0].copy()
-        for e in sets[0].keys():
-            if all(e in s for s in sets[1:]):
-                res.add(e)
-        return res
+
+        ret = sets[0].copy()
+        for e in sets[0]:
+            if any(e not in s for s in sets[1:]):
+                ret.remove(e)
+        return ret
 
 
 class StringEnum(enum.Enum):
     # Must be first, or else won't work, specifies what .value is
     @staticmethod
     def _generate_next_value_(name, start, count, last_values):
         return name.lower()
@@ -378,14 +403,19 @@
     MIN_AST_DECIMAL = -decimal.Decimal(2**167) / DECIMAL_DIVISOR
     # max decimal allowed as Python value
     MAX_AST_DECIMAL = decimal.Decimal(2**167 - 1) / DECIMAL_DIVISOR
     MAX_UINT8 = 2**8 - 1
     MAX_UINT256 = 2**256 - 1
 
 
+def quantize(d: decimal.Decimal, places=MAX_DECIMAL_PLACES, rounding_mode=decimal.ROUND_DOWN):
+    quantizer = decimal.Decimal(f"{1:0.{places}f}")
+    return d.quantize(quantizer, rounding_mode)
+
+
 # List of valid IR macros.
 # TODO move this somewhere else, like ir_node.py
 VALID_IR_MACROS = {
     "assert",
     "break",
     "iload",
     "istore",
```

### Comparing `vyper-0.4.0b5/vyper/venom/README.md` & `vyper-0.4.0b6/vyper/venom/README.md`

 * *Files identical despite different names*

### Comparing `vyper-0.4.0b5/vyper/venom/__init__.py` & `vyper-0.4.0b6/vyper/venom/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,18 +7,22 @@
 from vyper.compiler.settings import OptimizationLevel
 from vyper.venom.analysis import DFG, calculate_cfg, calculate_liveness
 from vyper.venom.bb_optimizer import (
     ir_pass_optimize_empty_blocks,
     ir_pass_optimize_unused_variables,
     ir_pass_remove_unreachable_blocks,
 )
+from vyper.venom.dominators import DominatorTree
 from vyper.venom.function import IRFunction
 from vyper.venom.ir_node_to_venom import ir_node_to_venom
 from vyper.venom.passes.constant_propagation import ir_pass_constant_propagation
 from vyper.venom.passes.dft import DFTPass
+from vyper.venom.passes.make_ssa import MakeSSA
+from vyper.venom.passes.normalization import NormalizationPass
+from vyper.venom.passes.simplify_cfg import SimplifyCFGPass
 from vyper.venom.venom_to_assembly import VenomCompiler
 
 DEFAULT_OPT_LEVEL = OptimizationLevel.default()
 
 
 def generate_assembly_experimental(
     runtime_code: IRFunction,
@@ -34,29 +38,47 @@
     compiler = VenomCompiler(functions)
     return compiler.generate_evm(optimize == OptimizationLevel.NONE)
 
 
 def _run_passes(ctx: IRFunction, optimize: OptimizationLevel) -> None:
     # Run passes on Venom IR
     # TODO: Add support for optimization levels
+
+    ir_pass_optimize_empty_blocks(ctx)
+    ir_pass_remove_unreachable_blocks(ctx)
+
+    internals = [
+        bb
+        for bb in ctx.basic_blocks
+        if bb.label.value.startswith("internal") and len(bb.cfg_in) == 0
+    ]
+
+    SimplifyCFGPass().run_pass(ctx, ctx.basic_blocks[0])
+    for entry in internals:
+        SimplifyCFGPass().run_pass(ctx, entry)
+
+    make_ssa_pass = MakeSSA()
+    make_ssa_pass.run_pass(ctx, ctx.basic_blocks[0])
+    for entry in internals:
+        make_ssa_pass.run_pass(ctx, entry)
+
     while True:
         changes = 0
 
         changes += ir_pass_optimize_empty_blocks(ctx)
         changes += ir_pass_remove_unreachable_blocks(ctx)
 
         calculate_liveness(ctx)
 
         changes += ir_pass_optimize_unused_variables(ctx)
 
         calculate_cfg(ctx)
         calculate_liveness(ctx)
 
-        changes += ir_pass_constant_propagation(ctx)
-        changes += DFTPass.run_pass(ctx)
+        changes += DFTPass().run_pass(ctx)
 
         calculate_cfg(ctx)
         calculate_liveness(ctx)
 
         if changes == 0:
             break
```

### Comparing `vyper-0.4.0b5/vyper/venom/analysis.py` & `vyper-0.4.0b6/vyper/venom/analysis.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from vyper.exceptions import CompilerPanic
 from vyper.utils import OrderedSet
 from vyper.venom.basicblock import (
     BB_TERMINATORS,
     CFG_ALTERING_INSTRUCTIONS,
     IRBasicBlock,
     IRInstruction,
@@ -34,36 +36,36 @@
     for bb in ctx.basic_blocks:
         for in_bb in bb.cfg_in:
             in_bb.add_cfg_out(bb)
 
 
 def _reset_liveness(ctx: IRFunction) -> None:
     for bb in ctx.basic_blocks:
+        bb.out_vars = OrderedSet()
         for inst in bb.instructions:
             inst.liveness = OrderedSet()
 
 
 def _calculate_liveness(bb: IRBasicBlock) -> bool:
     """
     Compute liveness of each instruction in the basic block.
     Returns True if liveness changed
     """
     orig_liveness = bb.instructions[0].liveness.copy()
     liveness = bb.out_vars.copy()
     for instruction in reversed(bb.instructions):
-        ops = instruction.get_inputs()
+        ins = instruction.get_inputs()
+        outs = instruction.get_outputs()
+
+        if ins or outs:
+            # perf: only copy if changed
+            liveness = liveness.copy()
+            liveness.update(ins)
+            liveness.dropmany(outs)
 
-        for op in ops:
-            if op in liveness:
-                instruction.dup_requirements.add(op)
-
-        liveness = liveness.union(OrderedSet.fromkeys(ops))
-        out = instruction.get_outputs()[0] if len(instruction.get_outputs()) > 0 else None
-        if out in liveness:
-            liveness.remove(out)
         instruction.liveness = liveness
 
     return orig_liveness != bb.instructions[0].liveness
 
 
 def _calculate_out_vars(bb: IRBasicBlock) -> bool:
     """
@@ -85,14 +87,26 @@
             changed |= _calculate_out_vars(bb)
             changed |= _calculate_liveness(bb)
 
         if not changed:
             break
 
 
+def calculate_dup_requirements(ctx: IRFunction) -> None:
+    for bb in ctx.basic_blocks:
+        last_liveness = bb.out_vars
+        for inst in reversed(bb.instructions):
+            inst.dup_requirements = OrderedSet()
+            ops = inst.get_inputs()
+            for op in ops:
+                if op in last_liveness:
+                    inst.dup_requirements.add(op)
+            last_liveness = inst.liveness
+
+
 # calculate the input variables into self from source
 def input_vars_from(source: IRBasicBlock, target: IRBasicBlock) -> OrderedSet[IRVariable]:
     liveness = target.instructions[0].liveness.copy()
     assert isinstance(liveness, OrderedSet)
 
     for inst in target.instructions:
         if inst.opcode == "phi":
@@ -100,27 +114,25 @@
             # live variables set (dependent on how we traversed into this
             # basic block). the argument will be replaced by the destination
             # operand during instruction selection.
             # for instance, `%56 = phi %label1 %12 %label2 %14`
             # will arbitrarily choose either %12 or %14 to be in the liveness
             # set, and then during instruction selection, after this instruction,
             # %12 will be replaced by %56 in the liveness set
-            source1, source2 = inst.operands[0], inst.operands[2]
-            phi1, phi2 = inst.operands[1], inst.operands[3]
-            if source.label == source1:
-                liveness.add(phi1)
-                if phi2 in liveness:
-                    liveness.remove(phi2)
-            elif source.label == source2:
-                liveness.add(phi2)
-                if phi1 in liveness:
-                    liveness.remove(phi1)
-            else:
-                # bad path into this phi node
-                raise CompilerPanic(f"unreachable: {inst}")
+
+            # bad path into this phi node
+            if source.label not in inst.operands:
+                raise CompilerPanic(f"unreachable: {inst} from {source.label}")
+
+            for label, var in inst.phi_operands:
+                if label == source.label:
+                    liveness.add(var)
+                else:
+                    if var in liveness:
+                        liveness.remove(var)
 
     return liveness
 
 
 # DataFlow Graph
 # this could be refactored into its own file, but it's only used here
 # for now
@@ -133,16 +145,16 @@
         self._dfg_outputs = dict()
 
     # return uses of a given variable
     def get_uses(self, op: IRVariable) -> list[IRInstruction]:
         return self._dfg_inputs.get(op, [])
 
     # the instruction which produces this variable.
-    def get_producing_instruction(self, op: IRVariable) -> IRInstruction:
-        return self._dfg_outputs[op]
+    def get_producing_instruction(self, op: IRVariable) -> Optional[IRInstruction]:
+        return self._dfg_outputs.get(op)
 
     @classmethod
     def build_dfg(cls, ctx: IRFunction) -> "DFG":
         dfg = cls()
 
         # Build DFG
 
@@ -159,7 +171,24 @@
                     inputs = dfg._dfg_inputs.setdefault(op, [])
                     inputs.append(inst)
 
                 for op in res:  # type: ignore
                     dfg._dfg_outputs[op] = inst
 
         return dfg
+
+    def as_graph(self) -> str:
+        """
+        Generate a graphviz representation of the dfg
+        """
+        lines = ["digraph dfg_graph {"]
+        for var, inputs in self._dfg_inputs.items():
+            for input in inputs:
+                for op in input.get_outputs():
+                    if isinstance(op, IRVariable):
+                        lines.append(f'    " {var.name} " -> " {op.name} "')
+
+        lines.append("}")
+        return "\n".join(lines)
+
+    def __repr__(self) -> str:
+        return self.as_graph()
```

### Comparing `vyper-0.4.0b5/vyper/venom/basicblock.py` & `vyper-0.4.0b6/vyper/venom/basicblock.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-from enum import Enum, auto
-from typing import TYPE_CHECKING, Any, Iterator, Optional, Union
+from typing import TYPE_CHECKING, Any, Generator, Iterator, Optional, Union
 
 from vyper.utils import OrderedSet
 
 # instructions which can terminate a basic block
-BB_TERMINATORS = frozenset(["jmp", "djmp", "jnz", "ret", "return", "revert", "stop"])
+BB_TERMINATORS = frozenset(["jmp", "djmp", "jnz", "ret", "return", "revert", "stop", "exit"])
 
 VOLATILE_INSTRUCTIONS = frozenset(
     [
         "param",
         "alloca",
         "call",
         "staticcall",
+        "delegatecall",
         "invoke",
         "sload",
         "sstore",
         "iload",
         "istore",
+        "tload",
+        "tstore",
         "assert",
+        "assert_unreachable",
         "mstore",
         "mload",
         "calldatacopy",
+        "mcopy",
+        "extcodecopy",
+        "returndatacopy",
         "codecopy",
         "dloadbytes",
         "dload",
         "return",
         "ret",
         "jmp",
         "jnz",
@@ -35,27 +41,32 @@
     [
         "mstore",
         "sstore",
         "dstore",
         "istore",
         "dloadbytes",
         "calldatacopy",
+        "mcopy",
+        "returndatacopy",
         "codecopy",
+        "extcodecopy",
         "return",
         "ret",
         "revert",
         "assert",
+        "assert_unreachable",
         "selfdestruct",
         "stop",
         "invalid",
         "invoke",
         "jmp",
         "djmp",
         "jnz",
         "log",
+        "exit",
     ]
 )
 
 CFG_ALTERING_INSTRUCTIONS = frozenset(["jmp", "djmp", "jnz"])
 
 if TYPE_CHECKING:
     from vyper.venom.function import IRFunction
@@ -83,14 +94,18 @@
     """
     IROperand represents an operand in IR. An operand is anything that can
     be an argument to an IRInstruction
     """
 
     value: Any
 
+    @property
+    def name(self) -> str:
+        return self.value
+
 
 class IRValue(IROperand):
     """
     IRValue represents a value in IR. A value is anything that can be
     operated by non-control flow instructions. That is, IRValues can be
     IRVariables or IRLiterals.
     """
@@ -105,43 +120,62 @@
 
     value: int
 
     def __init__(self, value: int) -> None:
         assert isinstance(value, int), "value must be an int"
         self.value = value
 
-    def __repr__(self) -> str:
-        return str(self.value)
+    def __hash__(self) -> int:
+        return self.value.__hash__()
 
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, type(self)):
+            return False
+        return self.value == other.value
 
-class MemType(Enum):
-    OPERAND_STACK = auto()
-    MEMORY = auto()
+    def __repr__(self) -> str:
+        return str(self.value)
 
 
 class IRVariable(IRValue):
     """
     IRVariable represents a variable in IR. A variable is a string that starts with a %.
     """
 
     value: str
     offset: int = 0
 
-    # some variables can be in memory for conversion from legacy IR to venom
-    mem_type: MemType = MemType.OPERAND_STACK
-    mem_addr: Optional[int] = None
-
-    def __init__(
-        self, value: str, mem_type: MemType = MemType.OPERAND_STACK, mem_addr: int = None
-    ) -> None:
+    def __init__(self, value: str, version: Optional[str | int] = None) -> None:
         assert isinstance(value, str)
+        assert ":" not in value, "Variable name cannot contain ':'"
+        if version:
+            assert isinstance(value, str) or isinstance(value, int), "value must be an str or int"
+            value = f"{value}:{version}"
+        if value[0] != "%":
+            value = f"%{value}"
         self.value = value
         self.offset = 0
-        self.mem_type = mem_type
-        self.mem_addr = mem_addr
+
+    @property
+    def name(self) -> str:
+        return self.value.split(":")[0]
+
+    @property
+    def version(self) -> int:
+        if ":" not in self.value:
+            return 0
+        return int(self.value.split(":")[1])
+
+    def __hash__(self) -> int:
+        return self.value.__hash__()
+
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, type(self)):
+            return False
+        return self.value == other.value
 
     def __repr__(self) -> str:
         return self.value
 
 
 class IRLabel(IROperand):
     """
@@ -154,14 +188,22 @@
     value: str
 
     def __init__(self, value: str, is_symbol: bool = False) -> None:
         assert isinstance(value, str), "value must be an str"
         self.value = value
         self.is_symbol = is_symbol
 
+    def __hash__(self) -> int:
+        return hash(self.value)
+
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, type(self)):
+            return False
+        return self.value == other.value
+
     def __repr__(self) -> str:
         return self.value
 
 
 class IRInstruction:
     """
     IRInstruction represents an instruction in IR. Each instruction has an opcode,
@@ -178,14 +220,16 @@
     output: Optional[IROperand]
     # set of live variables at this instruction
     liveness: OrderedSet[IRVariable]
     dup_requirements: OrderedSet[IRVariable]
     parent: Optional["IRBasicBlock"]
     fence_id: int
     annotation: Optional[str]
+    ast_source: Optional[int]
+    error_msg: Optional[str]
 
     def __init__(
         self,
         opcode: str,
         operands: list[IROperand] | Iterator[IROperand],
         output: Optional[IROperand] = None,
     ):
@@ -196,14 +240,16 @@
         self.operands = list(operands)  # in case we get an iterator
         self.output = output
         self.liveness = OrderedSet()
         self.dup_requirements = OrderedSet()
         self.parent = None
         self.fence_id = -1
         self.annotation = None
+        self.ast_source = None
+        self.error_msg = None
 
     def get_label_operands(self) -> list[IRLabel]:
         """
         Get all labels in instruction.
         """
         return [op for op in self.operands if isinstance(op, IRLabel)]
 
@@ -242,30 +288,45 @@
         replacements are represented using a dict: "key" is replaced by "value".
         """
         replacements = {k.value: v for k, v in replacements.items()}
         for i, operand in enumerate(self.operands):
             if isinstance(operand, IRLabel) and operand.value in replacements:
                 self.operands[i] = replacements[operand.value]
 
+    @property
+    def phi_operands(self) -> Generator[tuple[IRLabel, IRVariable], None, None]:
+        """
+        Get phi operands for instruction.
+        """
+        assert self.opcode == "phi", "instruction must be a phi"
+        for i in range(0, len(self.operands), 2):
+            label = self.operands[i]
+            var = self.operands[i + 1]
+            assert isinstance(label, IRLabel), "phi operand must be a label"
+            assert isinstance(var, IRVariable), "phi operand must be a variable"
+            yield label, var
+
     def __repr__(self) -> str:
         s = ""
         if self.output:
             s += f"{self.output} = "
         opcode = f"{self.opcode} " if self.opcode != "store" else ""
         s += opcode
-        operands = ", ".join(
-            [(f"label %{op}" if isinstance(op, IRLabel) else str(op)) for op in self.operands]
+        operands = self.operands
+        if opcode not in ["jmp", "jnz", "invoke"]:
+            operands = reversed(operands)  # type: ignore
+        s += ", ".join(
+            [(f"label %{op}" if isinstance(op, IRLabel) else str(op)) for op in operands]
         )
-        s += operands
 
         if self.annotation:
             s += f" <{self.annotation}>"
 
-        # if self.liveness:
-        #     return f"{s: <30} # {self.liveness}"
+        if self.liveness:
+            return f"{s: <30} # {self.liveness}"
 
         return s
 
 
 def _ir_operand_from_value(val: Any) -> IROperand:
     if isinstance(val, IROperand):
         return val
@@ -303,22 +364,27 @@
     # basic blocks which can jump to this basic block
     cfg_in: OrderedSet["IRBasicBlock"]
     # basic blocks which this basic block can jump to
     cfg_out: OrderedSet["IRBasicBlock"]
     # stack items which this basic block produces
     out_vars: OrderedSet[IRVariable]
 
+    reachable: OrderedSet["IRBasicBlock"]
+    is_reachable: bool = False
+
     def __init__(self, label: IRLabel, parent: "IRFunction") -> None:
         assert isinstance(label, IRLabel), "label must be an IRLabel"
         self.label = label
         self.parent = parent
         self.instructions = []
         self.cfg_in = OrderedSet()
         self.cfg_out = OrderedSet()
         self.out_vars = OrderedSet()
+        self.reachable = OrderedSet()
+        self.is_reachable = False
 
     def add_cfg_in(self, bb: "IRBasicBlock") -> None:
         self.cfg_in.add(bb)
 
     def remove_cfg_in(self, bb: "IRBasicBlock") -> None:
         assert bb in self.cfg_in
         self.cfg_in.remove(bb)
@@ -329,80 +395,123 @@
         # if we have this assumption)
         self.cfg_out.add(bb)
 
     def remove_cfg_out(self, bb: "IRBasicBlock") -> None:
         assert bb in self.cfg_out
         self.cfg_out.remove(bb)
 
-    @property
-    def is_reachable(self) -> bool:
-        return len(self.cfg_in) > 0
-
-    def append_instruction(self, opcode: str, *args: Union[IROperand, int]) -> Optional[IRVariable]:
+    def append_instruction(
+        self, opcode: str, *args: Union[IROperand, int], ret: IRVariable = None
+    ) -> Optional[IRVariable]:
         """
         Append an instruction to the basic block
 
         Returns the output variable if the instruction supports one
         """
-        ret = self.parent.get_next_variable() if opcode not in NO_OUTPUT_INSTRUCTIONS else None
+        assert not self.is_terminated, self
+
+        if ret is None:
+            ret = self.parent.get_next_variable() if opcode not in NO_OUTPUT_INSTRUCTIONS else None
 
         # Wrap raw integers in IRLiterals
         inst_args = [_ir_operand_from_value(arg) for arg in args]
 
         inst = IRInstruction(opcode, inst_args, ret)
         inst.parent = self
+        inst.ast_source = self.parent.ast_source
+        inst.error_msg = self.parent.error_msg
         self.instructions.append(inst)
         return ret
 
     def append_invoke_instruction(
         self, args: list[IROperand | int], returns: bool
     ) -> Optional[IRVariable]:
         """
-        Append an instruction to the basic block
-
-        Returns the output variable if the instruction supports one
+        Append an invoke to the basic block
         """
+        assert not self.is_terminated, self
         ret = None
         if returns:
             ret = self.parent.get_next_variable()
 
         # Wrap raw integers in IRLiterals
         inst_args = [_ir_operand_from_value(arg) for arg in args]
 
+        assert isinstance(inst_args[0], IRLabel), "Invoked non label"
+
         inst = IRInstruction("invoke", inst_args, ret)
         inst.parent = self
+        inst.ast_source = self.parent.ast_source
+        inst.error_msg = self.parent.error_msg
         self.instructions.append(inst)
         return ret
 
-    def insert_instruction(self, instruction: IRInstruction, index: int) -> None:
+    def insert_instruction(self, instruction: IRInstruction, index: Optional[int] = None) -> None:
         assert isinstance(instruction, IRInstruction), "instruction must be an IRInstruction"
+
+        if index is None:
+            assert not self.is_terminated, self
+            index = len(self.instructions)
         instruction.parent = self
+        instruction.ast_source = self.parent.ast_source
+        instruction.error_msg = self.parent.error_msg
         self.instructions.insert(index, instruction)
 
+    def remove_instruction(self, instruction: IRInstruction) -> None:
+        assert isinstance(instruction, IRInstruction), "instruction must be an IRInstruction"
+        self.instructions.remove(instruction)
+
     def clear_instructions(self) -> None:
         self.instructions = []
 
     def replace_operands(self, replacements: dict) -> None:
         """
         Update operands with replacements.
         """
         for instruction in self.instructions:
             instruction.replace_operands(replacements)
 
+    def get_assignments(self):
+        """
+        Get all assignments in basic block.
+        """
+        return [inst.output for inst in self.instructions if inst.output]
+
+    @property
+    def is_empty(self) -> bool:
+        """
+        Check if the basic block is empty, i.e. it has no instructions.
+        """
+        return len(self.instructions) == 0
+
     @property
     def is_terminated(self) -> bool:
         """
         Check if the basic block is terminal, i.e. the last instruction is a terminator.
         """
         # it's ok to return False here, since we use this to check
         # if we can/need to append instructions to the basic block.
         if len(self.instructions) == 0:
             return False
         return self.instructions[-1].opcode in BB_TERMINATORS
 
+    @property
+    def is_terminal(self) -> bool:
+        """
+        Check if the basic block is terminal.
+        """
+        return len(self.cfg_out) == 0
+
+    @property
+    def in_vars(self) -> OrderedSet[IRVariable]:
+        for inst in self.instructions:
+            if inst.opcode != "phi":
+                return inst.liveness
+        return OrderedSet()
+
     def copy(self):
         bb = IRBasicBlock(self.label, self.parent)
         bb.instructions = self.instructions.copy()
         bb.cfg_in = self.cfg_in.copy()
         bb.cfg_out = self.cfg_out.copy()
         bb.out_vars = self.out_vars.copy()
         return bb
```

### Comparing `vyper-0.4.0b5/vyper/venom/bb_optimizer.py` & `vyper-0.4.0b6/vyper/venom/bb_optimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,33 @@
         ctx.basic_blocks.remove(bb)
         i -= 1
         count += 1
 
     return count
 
 
+def _daisychain_empty_basicblocks(ctx: IRFunction) -> int:
+    count = 0
+    i = 0
+    while i < len(ctx.basic_blocks):
+        bb = ctx.basic_blocks[i]
+        i += 1
+        if bb.is_terminated:
+            continue
+
+        if i < len(ctx.basic_blocks) - 1:
+            bb.append_instruction("jmp", ctx.basic_blocks[i + 1].label)
+        else:
+            bb.append_instruction("stop")
+
+        count += 1
+
+    return count
+
+
 @ir_pass
 def ir_pass_optimize_empty_blocks(ctx: IRFunction) -> int:
     changes = _optimize_empty_basicblocks(ctx)
     calculate_cfg(ctx)
     return changes
```

### Comparing `vyper-0.4.0b5/vyper/venom/passes/base_pass.py` & `vyper-0.4.0b6/vyper/venom/passes/base_pass.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 class IRPass:
     """
     Decorator for IR passes. This decorator will run the pass repeatedly
     until no more changes are made.
     """
 
-    @classmethod
-    def run_pass(cls, *args, **kwargs):
-        t = cls()
+    def run_pass(self, *args, **kwargs):
         count = 0
 
-        while True:
-            changes_count = t._run_pass(*args, **kwargs) or 0
+        for _ in range(1000):
+            changes_count = self._run_pass(*args, **kwargs) or 0
             count += changes_count
             if changes_count == 0:
                 break
+        else:
+            raise Exception("Too many iterations in IR pass!", self.__class__)
 
         return count
 
     def _run_pass(self, *args, **kwargs):
         raise NotImplementedError(f"Not implemented! {self.__class__}.run_pass()")
```

### Comparing `vyper-0.4.0b5/vyper/venom/passes/normalization.py` & `vyper-0.4.0b6/vyper/venom/passes/normalization.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,29 @@
                 break
 
     def _insert_split_basicblock(self, bb: IRBasicBlock, in_bb: IRBasicBlock) -> IRBasicBlock:
         # Create an intermediary basic block and append it
         source = in_bb.label.value
         target = bb.label.value
 
-        split_label = IRLabel(f"{target}_split_{source}")
+        split_label = IRLabel(f"{source}_split_{target}")
         in_terminal = in_bb.instructions[-1]
         in_terminal.replace_label_operands({bb.label: split_label})
 
         split_bb = IRBasicBlock(split_label, self.ctx)
         split_bb.append_instruction("jmp", bb.label)
         self.ctx.append_basic_block(split_bb)
 
+        for inst in bb.instructions:
+            if inst.opcode != "phi":
+                continue
+            for i in range(0, len(inst.operands), 2):
+                if inst.operands[i] == in_bb.label:
+                    inst.operands[i] = split_bb.label
+
         # Update the labels in the data segment
         for inst in self.ctx.data_segment:
             if inst.opcode == "db" and inst.operands[0] == bb.label:
                 inst.operands[0] = split_bb.label
 
         return split_bb
 
@@ -51,9 +58,10 @@
         for bb in ctx.basic_blocks:
             if len(bb.cfg_in) > 1:
                 self._split_basic_block(bb)
 
         # If we made changes, recalculate the cfg
         if self.changes > 0:
             calculate_cfg(ctx)
+            ctx.remove_unreachable_blocks()
 
         return self.changes
```

### Comparing `vyper-0.4.0b5/vyper/venom/stack_model.py` & `vyper-0.4.0b6/vyper/venom/stack_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,42 +26,44 @@
         """
         assert isinstance(op, IROperand), f"{type(op)}: {op}"
         self._stack.append(op)
 
     def pop(self, num: int = 1) -> None:
         del self._stack[len(self._stack) - num :]
 
-    def get_depth(self, op: IROperand) -> int:
+    def get_depth(self, op: IROperand, n: int = 1) -> int:
         """
-        Returns the depth of the first matching operand in the stack map.
+        Returns the depth of the n-th matching operand in the stack map.
         If the operand is not in the stack map, returns NOT_IN_STACK.
         """
         assert isinstance(op, IROperand), f"{type(op)}: {op}"
 
         for i, stack_op in enumerate(reversed(self._stack)):
             if stack_op.value == op.value:
-                return -i
+                if n <= 1:
+                    return -i
+                else:
+                    n -= 1
 
         return StackModel.NOT_IN_STACK  # type: ignore
 
-    def get_phi_depth(self, phi1: IRVariable, phi2: IRVariable) -> int:
+    def get_phi_depth(self, phis: list[IRVariable]) -> int:
         """
         Returns the depth of the first matching phi variable in the stack map.
         If the none of the phi operands are in the stack, returns NOT_IN_STACK.
-        Asserts that exactly one of phi1 and phi2 is found.
+        Asserts that exactly one of phis is found.
         """
-        assert isinstance(phi1, IRVariable)
-        assert isinstance(phi2, IRVariable)
+        assert isinstance(phis, list)
 
         ret = StackModel.NOT_IN_STACK
         for i, stack_item in enumerate(reversed(self._stack)):
-            if stack_item in (phi1, phi2):
+            if stack_item in phis:
                 assert (
                     ret is StackModel.NOT_IN_STACK
-                ), f"phi argument is not unique! {phi1}, {phi2}, {self._stack}"
+                ), f"phi argument is not unique! {phis}, {self._stack}"
                 ret = -i
 
         return ret  # type: ignore
 
     def peek(self, depth: int) -> IROperand:
         """
         Returns the top of the stack map.
```

### Comparing `vyper-0.4.0b5/vyper/venom/venom_to_assembly.py` & `vyper-0.4.0b6/vyper/venom/venom_to_assembly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,125 @@
+from collections import Counter
 from typing import Any
 
-from vyper.ir.compile_ir import PUSH, DataHeader, RuntimeHeader, optimize_assembly
+from vyper.exceptions import CompilerPanic, StackTooDeep
+from vyper.ir.compile_ir import (
+    PUSH,
+    DataHeader,
+    Instruction,
+    RuntimeHeader,
+    mksymbol,
+    optimize_assembly,
+)
 from vyper.utils import MemoryPositions, OrderedSet
-from vyper.venom.analysis import calculate_cfg, calculate_liveness, input_vars_from
+from vyper.venom.analysis import (
+    calculate_cfg,
+    calculate_dup_requirements,
+    calculate_liveness,
+    input_vars_from,
+)
 from vyper.venom.basicblock import (
     IRBasicBlock,
     IRInstruction,
     IRLabel,
     IRLiteral,
     IROperand,
     IRVariable,
-    MemType,
 )
 from vyper.venom.function import IRFunction
 from vyper.venom.passes.normalization import NormalizationPass
 from vyper.venom.stack_model import StackModel
 
 # instructions which map one-to-one from venom to EVM
 _ONE_TO_ONE_INSTRUCTIONS = frozenset(
     [
         "revert",
         "coinbase",
         "calldatasize",
         "calldatacopy",
+        "mcopy",
         "calldataload",
         "gas",
         "gasprice",
         "gaslimit",
+        "chainid",
         "address",
         "origin",
         "number",
         "extcodesize",
         "extcodehash",
+        "extcodecopy",
         "returndatasize",
         "returndatacopy",
         "callvalue",
         "selfbalance",
         "sload",
         "sstore",
         "mload",
         "mstore",
+        "tload",
+        "tstore",
         "timestamp",
         "caller",
+        "blockhash",
         "selfdestruct",
         "signextend",
         "stop",
         "shr",
         "shl",
+        "sar",
         "and",
         "xor",
         "or",
         "add",
         "sub",
         "mul",
         "div",
+        "smul",
+        "sdiv",
         "mod",
+        "smod",
         "exp",
+        "addmod",
+        "mulmod",
         "eq",
         "iszero",
         "not",
         "lg",
         "lt",
         "slt",
         "sgt",
+        "create",
+        "create2",
+        "msize",
+        "balance",
+        "call",
+        "staticcall",
+        "delegatecall",
+        "codesize",
+        "basefee",
+        "prevrandao",
+        "difficulty",
+        "invalid",
     ]
 )
 
 _REVERT_POSTAMBLE = ["_sym___revert", "JUMPDEST", *PUSH(0), "DUP1", "REVERT"]
 
 
+def apply_line_numbers(inst: IRInstruction, asm) -> list[str]:
+    ret = []
+    for op in asm:
+        if isinstance(op, str) and not isinstance(op, Instruction):
+            ret.append(Instruction(op, inst.ast_source, inst.error_msg))
+        else:
+            ret.append(op)
+    return ret  # type: ignore
+
+
 # TODO: "assembly" gets into the recursion due to how the original
 # IR was structured recursively in regards with the deploy instruction.
 # There, recursing into the deploy instruction was by design, and
 # made it easier to make the assembly generated "recursive" (i.e.
 # instructions being lists of instructions). We don't have this restriction
 # anymore, so we can probably refactor this to be iterative in coordination
 # with the assembler. My suggestion is to let this be for now, and we can
@@ -95,32 +142,32 @@
         self.label_counter = 0
 
         asm: list[Any] = []
         top_asm = asm
 
         # Before emitting the assembly, we need to make sure that the
         # CFG is normalized. Calling calculate_cfg() will denormalize IR (reset)
-        # so it should not be called after calling NormalizationPass.run_pass().
+        # so it should not be called after calling NormalizationPass().run_pass().
         # Liveness is then computed for the normalized IR, and we can proceed to
         # assembly generation.
         # This is a side-effect of how dynamic jumps are temporarily being used
         # to support the O(1) dispatcher. -> look into calculate_cfg()
         for ctx in self.ctxs:
+            NormalizationPass().run_pass(ctx)
             calculate_cfg(ctx)
-            NormalizationPass.run_pass(ctx)
             calculate_liveness(ctx)
+            calculate_dup_requirements(ctx)
 
             assert ctx.normalized, "Non-normalized CFG!"
 
             self._generate_evm_for_basicblock_r(asm, ctx.basic_blocks[0], StackModel())
 
             # TODO make this property on IRFunction
+            asm.extend(["_sym__ctor_exit", "JUMPDEST"])
             if ctx.immutables_len is not None and ctx.ctor_mem_size is not None:
-                while asm[-1] != "JUMPDEST":
-                    asm.pop()
                 asm.extend(
                     ["_sym_subcode_size", "_sym_runtime_begin", "_mem_deploy_start", "CODECOPY"]
                 )
                 asm.extend(["_OFST", "_sym_subcode_size", ctx.immutables_len])  # stack: len
                 asm.extend(["_mem_deploy_start"])  # stack: len mem_ofst
                 asm.extend(["RETURN"])
                 asm.extend(_REVERT_POSTAMBLE)
@@ -135,38 +182,49 @@
             # Append data segment
             data_segments: dict = dict()
             for inst in ctx.data_segment:
                 if inst.opcode == "dbname":
                     label = inst.operands[0].value
                     data_segments[label] = [DataHeader(f"_sym_{label}")]
                 elif inst.opcode == "db":
-                    data_segments[label].append(f"_sym_{inst.operands[0].value}")
+                    data = inst.operands[0]
+                    if isinstance(data, IRLabel):
+                        data_segments[label].append(f"_sym_{data.value}")
+                    else:
+                        data_segments[label].append(data)
 
             asm.extend(list(data_segments.values()))
 
         if no_optimize is False:
             optimize_assembly(top_asm)
 
         return top_asm
 
     def _stack_reorder(
-        self, assembly: list, stack: StackModel, _stack_ops: OrderedSet[IRVariable]
+        self, assembly: list, stack: StackModel, stack_ops: list[IRVariable]
     ) -> None:
-        # make a list so we can index it
-        stack_ops = [x for x in _stack_ops.keys()]
-        stack_ops_count = len(_stack_ops)
+        stack_ops_count = len(stack_ops)
+
+        counts = Counter(stack_ops)
 
         for i in range(stack_ops_count):
             op = stack_ops[i]
             final_stack_depth = -(stack_ops_count - i - 1)
-            depth = stack.get_depth(op)  # type: ignore
+            depth = stack.get_depth(op, counts[op])  # type: ignore
+            counts[op] -= 1
+
+            if depth == StackModel.NOT_IN_STACK:
+                raise CompilerPanic(f"Variable {op} not in stack")
 
             if depth == final_stack_depth:
                 continue
 
+            if op == stack.peek(final_stack_depth):
+                continue
+
             self.swap(assembly, stack, depth)
             self.swap(assembly, stack, final_stack_depth)
 
     def _emit_input_operands(
         self, assembly: list, inst: IRInstruction, ops: list[IROperand], stack: StackModel
     ) -> None:
         # PRE: we already have all the items on the stack that have
@@ -188,31 +246,28 @@
                 # but we need to add it to the stack map
                 if inst.opcode != "invoke":
                     assembly.append(f"_sym_{op.value}")
                 stack.push(op)
                 continue
 
             if isinstance(op, IRLiteral):
-                assembly.extend([*PUSH(op.value)])
+                if op.value < -(2**255):
+                    raise Exception(f"Value too low: {op.value}")
+                elif op.value >= 2**256:
+                    raise Exception(f"Value too high: {op.value}")
+                assembly.extend(PUSH(op.value % 2**256))
                 stack.push(op)
                 continue
 
-            if op in inst.dup_requirements:
+            if op in inst.dup_requirements and op not in emitted_ops:
                 self.dup_op(assembly, stack, op)
 
             if op in emitted_ops:
                 self.dup_op(assembly, stack, op)
 
-            # REVIEW: this seems like it can be reordered across volatile
-            # boundaries (which includes memory fences). maybe just
-            # remove it entirely at this point
-            if isinstance(op, IRVariable) and op.mem_type == MemType.MEMORY:
-                assembly.extend([*PUSH(op.mem_addr)])
-                assembly.append("MLOAD")
-
             emitted_ops.add(op)
 
     def _generate_evm_for_basicblock_r(
         self, asm: list, basicblock: IRBasicBlock, stack: StackModel
     ) -> None:
         if basicblock in self.visited_basicblocks:
             return
@@ -220,20 +275,42 @@
 
         # assembly entry point into the block
         asm.append(f"_sym_{basicblock.label}")
         asm.append("JUMPDEST")
 
         self.clean_stack_from_cfg_in(asm, basicblock, stack)
 
-        for inst in basicblock.instructions:
-            asm = self._generate_evm_for_instruction(asm, inst, stack)
+        param_insts = [inst for inst in basicblock.instructions if inst.opcode == "param"]
+        main_insts = [inst for inst in basicblock.instructions if inst.opcode != "param"]
+
+        for inst in param_insts:
+            asm.extend(self._generate_evm_for_instruction(inst, stack))
+
+        self._clean_unused_params(asm, basicblock, stack)
+
+        for i, inst in enumerate(main_insts):
+            next_liveness = main_insts[i + 1].liveness if i + 1 < len(main_insts) else OrderedSet()
+
+            asm.extend(self._generate_evm_for_instruction(inst, stack, next_liveness))
 
-        for bb in basicblock.cfg_out:
+        for bb in basicblock.reachable:
             self._generate_evm_for_basicblock_r(asm, bb, stack.copy())
 
+    def _clean_unused_params(self, asm: list, bb: IRBasicBlock, stack: StackModel) -> None:
+        for i, inst in enumerate(bb.instructions):
+            if inst.opcode != "param":
+                break
+            if inst.volatile and i + 1 < len(bb.instructions):
+                liveness = bb.instructions[i + 1].liveness
+                if inst.output is not None and inst.output not in liveness:
+                    depth = stack.get_depth(inst.output)
+                    if depth != 0:
+                        self.swap(asm, stack, depth)
+                    self.pop(asm, stack)
+
     # pop values from stack at entry to bb
     # note this produces the same result(!) no matter which basic block
     # we enter from in the CFG.
     def clean_stack_from_cfg_in(
         self, asm: list, basicblock: IRBasicBlock, stack: StackModel
     ) -> None:
         if len(basicblock.cfg_in) == 0:
@@ -254,74 +331,92 @@
         for var in to_pop:
             depth = stack.get_depth(var)
             # don't pop phantom phi inputs
             if depth is StackModel.NOT_IN_STACK:
                 continue
 
             if depth != 0:
-                stack.swap(depth)
+                self.swap(asm, stack, depth)
             self.pop(asm, stack)
 
     def _generate_evm_for_instruction(
-        self, assembly: list, inst: IRInstruction, stack: StackModel
+        self, inst: IRInstruction, stack: StackModel, next_liveness: OrderedSet = None
     ) -> list[str]:
+        assembly: list[str | int] = []
+        next_liveness = next_liveness or OrderedSet()
         opcode = inst.opcode
 
         #
         # generate EVM for op
         #
 
         # Step 1: Apply instruction special stack manipulations
 
         if opcode in ["jmp", "djmp", "jnz", "invoke"]:
             operands = inst.get_non_label_operands()
         elif opcode == "alloca":
             operands = inst.operands[1:2]
+
+        # iload and istore are special cases because they can take a literal
+        # that is handled specialy with the _OFST macro. Look below, after the
+        # stack reordering.
         elif opcode == "iload":
-            operands = []
+            addr = inst.operands[0]
+            if isinstance(addr, IRLiteral):
+                operands = []
+            else:
+                operands = inst.operands
         elif opcode == "istore":
-            operands = inst.operands[0:1]
+            addr = inst.operands[1]
+            if isinstance(addr, IRLiteral):
+                operands = inst.operands[:1]
+            else:
+                operands = inst.operands
         elif opcode == "log":
             log_topic_count = inst.operands[0].value
             assert log_topic_count in [0, 1, 2, 3, 4], "Invalid topic count"
             operands = inst.operands[1:]
         else:
             operands = inst.operands
 
         if opcode == "phi":
             ret = inst.get_outputs()[0]
-            phi1, phi2 = inst.get_inputs()
-            depth = stack.get_phi_depth(phi1, phi2)
+            phis = inst.get_inputs()
+            depth = stack.get_phi_depth(phis)
             # collapse the arguments to the phi node in the stack.
             # example, for `%56 = %label1 %13 %label2 %14`, we will
             # find an instance of %13 *or* %14 in the stack and replace it with %56.
             to_be_replaced = stack.peek(depth)
             if to_be_replaced in inst.dup_requirements:
                 # %13/%14 is still live(!), so we make a copy of it
                 self.dup(assembly, stack, depth)
                 stack.poke(0, ret)
             else:
                 stack.poke(depth, ret)
-            return assembly
+            return apply_line_numbers(inst, assembly)
 
         # Step 2: Emit instruction's input operands
         self._emit_input_operands(assembly, inst, operands, stack)
 
         # Step 3: Reorder stack
         if opcode in ["jnz", "djmp", "jmp"]:
             # prepare stack for jump into another basic block
             assert inst.parent and isinstance(inst.parent.cfg_out, OrderedSet)
             b = next(iter(inst.parent.cfg_out))
             target_stack = input_vars_from(inst.parent, b)
             # TODO optimize stack reordering at entry and exit from basic blocks
-            self._stack_reorder(assembly, stack, target_stack)
+            # NOTE: stack in general can contain multiple copies of the same variable,
+            # however we are safe in the case of jmp/djmp/jnz as it's not going to
+            # have multiples.
+            target_stack_list = list(target_stack)
+            self._stack_reorder(assembly, stack, target_stack_list)
 
         # final step to get the inputs to this instruction ordered
         # correctly on the stack
-        self._stack_reorder(assembly, stack, OrderedSet(operands))
+        self._stack_reorder(assembly, stack, operands)  # type: ignore
 
         # some instructions (i.e. invoke) need to do stack manipulations
         # with the stack model containing the return value(s), so we fiddle
         # with the stack model beforehand.
 
         # Step 4: Push instruction's return value to stack
         stack.pop(len(operands))
@@ -355,89 +450,101 @@
             assembly.append("JUMP")
 
         elif opcode == "jmp":
             assert isinstance(inst.operands[0], IRLabel)
             assembly.append(f"_sym_{inst.operands[0].value}")
             assembly.append("JUMP")
         elif opcode == "djmp":
-            assert isinstance(inst.operands[0], IRVariable)
+            assert isinstance(
+                inst.operands[0], IRVariable
+            ), f"Expected IRVariable, got {inst.operands[0]}"
             assembly.append("JUMP")
         elif opcode == "gt":
             assembly.append("GT")
         elif opcode == "lt":
             assembly.append("LT")
         elif opcode == "invoke":
             target = inst.operands[0]
-            assert isinstance(target, IRLabel), "invoke target must be a label"
+            assert isinstance(
+                target, IRLabel
+            ), f"invoke target must be a label (is ${type(target)} ${target})"
             assembly.extend(
                 [
                     f"_sym_label_ret_{self.label_counter}",
                     f"_sym_{target.value}",
                     "JUMP",
                     f"_sym_label_ret_{self.label_counter}",
                     "JUMPDEST",
                 ]
             )
             self.label_counter += 1
-            if stack.height > 0 and stack.peek(0) in inst.dup_requirements:
-                self.pop(assembly, stack)
-        elif opcode == "call":
-            assembly.append("CALL")
-        elif opcode == "staticcall":
-            assembly.append("STATICCALL")
         elif opcode == "ret":
             assembly.append("JUMP")
         elif opcode == "return":
             assembly.append("RETURN")
+        elif opcode == "exit":
+            assembly.extend(["_sym__ctor_exit", "JUMP"])
         elif opcode == "phi":
             pass
         elif opcode == "sha3":
             assembly.append("SHA3")
         elif opcode == "sha3_64":
             assembly.extend(
                 [
-                    *PUSH(MemoryPositions.FREE_VAR_SPACE2),
-                    "MSTORE",
                     *PUSH(MemoryPositions.FREE_VAR_SPACE),
                     "MSTORE",
+                    *PUSH(MemoryPositions.FREE_VAR_SPACE2),
+                    "MSTORE",
                     *PUSH(64),
                     *PUSH(MemoryPositions.FREE_VAR_SPACE),
                     "SHA3",
                 ]
             )
         elif opcode == "ceil32":
             assembly.extend([*PUSH(31), "ADD", *PUSH(31), "NOT", "AND"])
         elif opcode == "assert":
             assembly.extend(["ISZERO", "_sym___revert", "JUMPI"])
+        elif opcode == "assert_unreachable":
+            end_symbol = mksymbol("reachable")
+            assembly.extend([end_symbol, "JUMPI", "INVALID", end_symbol, "JUMPDEST"])
         elif opcode == "iload":
-            loc = inst.operands[0].value
-            assembly.extend(["_OFST", "_mem_deploy_end", loc, "MLOAD"])
+            addr = inst.operands[0]
+            if isinstance(addr, IRLiteral):
+                assembly.extend(["_OFST", "_mem_deploy_end", addr.value])
+            else:
+                assembly.extend(["_mem_deploy_end", "ADD"])
+            assembly.append("MLOAD")
         elif opcode == "istore":
-            loc = inst.operands[1].value
-            assembly.extend(["_OFST", "_mem_deploy_end", loc, "MSTORE"])
+            addr = inst.operands[1]
+            if isinstance(addr, IRLiteral):
+                assembly.extend(["_OFST", "_mem_deploy_end", addr.value])
+            else:
+                assembly.extend(["_mem_deploy_end", "ADD"])
+            assembly.append("MSTORE")
         elif opcode == "log":
             assembly.extend([f"LOG{log_topic_count}"])
         else:
             raise Exception(f"Unknown opcode: {opcode}")
 
         # Step 6: Emit instructions output operands (if any)
         if inst.output is not None:
-            assert isinstance(inst.output, IRVariable), "Return value must be a variable"
-            if inst.output.mem_type == MemType.MEMORY:
-                assembly.extend([*PUSH(inst.output.mem_addr)])
+            if "call" in inst.opcode and inst.output not in next_liveness:
+                self.pop(assembly, stack)
 
-        return assembly
+        return apply_line_numbers(inst, assembly)
 
     def pop(self, assembly, stack, num=1):
         stack.pop(num)
         assembly.extend(["POP"] * num)
 
     def swap(self, assembly, stack, depth):
+        # Swaps of the top is no op
         if depth == 0:
             return
+
         stack.swap(depth)
         assembly.append(_evm_swap_for(depth))
 
     def dup(self, assembly, stack, depth):
         stack.dup(depth)
         assembly.append(_evm_dup_for(depth))
 
@@ -446,15 +553,17 @@
 
     def dup_op(self, assembly, stack, op):
         self.dup(assembly, stack, stack.get_depth(op))
 
 
 def _evm_swap_for(depth: int) -> str:
     swap_idx = -depth
-    assert 1 <= swap_idx <= 16, "Unsupported swap depth"
+    if not (1 <= swap_idx <= 16):
+        raise StackTooDeep(f"Unsupported swap depth {swap_idx}")
     return f"SWAP{swap_idx}"
 
 
 def _evm_dup_for(depth: int) -> str:
     dup_idx = 1 - depth
-    assert 1 <= dup_idx <= 16, "Unsupported dup depth"
+    if not (1 <= dup_idx <= 16):
+        raise StackTooDeep(f"Unsupported dup depth {dup_idx}")
     return f"DUP{dup_idx}"
```

### Comparing `vyper-0.4.0b5/vyper.egg-info/PKG-INFO` & `vyper-0.4.0b6/vyper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vyper
-Version: 0.4.0b5
+Version: 0.4.0b6
 Summary: Vyper: the Pythonic Programming Language for the EVM
 Home-page: https://github.com/vyperlang/vyper
 Author: Vyper Team
 Author-email: 
 License: Apache License 2.0
 Keywords: ethereum evm smart contract language
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
-Provides-Extra: docs
 Provides-Extra: dev
 License-File: LICENSE
 
 <img src="https://raw.githubusercontent.com/vyperlang/vyper/master/docs/logo.svg?sanitize=true" alt="" width="110">
 
 [![Build Status](https://github.com/vyperlang/vyper/workflows/Test/badge.svg)](https://github.com/vyperlang/vyper/actions/workflows/test.yml)
 [![Documentation Status](https://readthedocs.org/projects/vyper/badge/?version=latest)](http://docs.vyperlang.org/en/latest/?badge=latest "ReadTheDocs")
```

### Comparing `vyper-0.4.0b5/vyper.egg-info/SOURCES.txt` & `vyper-0.4.0b6/vyper.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 SECURITY.md
 make.cmd
 pyproject.toml
 quicktest.sh
 requirements-docs.txt
 setup.cfg
 setup.py
-tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/vip.md
 .github/workflows/build.yml
 .github/workflows/codeql.yml
 .github/workflows/era-tester.yml
 .github/workflows/ghcr.yml
-.github/workflows/publish.yml
+.github/workflows/pull-request.yaml
+.github/workflows/release-pypi.yml
 .github/workflows/test.yml
 docs/Makefile
 docs/built-in-functions.rst
 docs/compiler-exceptions.rst
 docs/compiling-a-contract.rst
 docs/conf.py
 docs/constants-and-vars.rst
@@ -169,14 +169,15 @@
 tests/functional/codegen/features/iteration/test_range_in.py
 tests/functional/codegen/integration/test_basics.py
 tests/functional/codegen/integration/test_crowdfund.py
 tests/functional/codegen/integration/test_escrow.py
 tests/functional/codegen/modules/__init__.py
 tests/functional/codegen/modules/test_events.py
 tests/functional/codegen/modules/test_exports.py
+tests/functional/codegen/modules/test_flag_imports.py
 tests/functional/codegen/modules/test_interface_imports.py
 tests/functional/codegen/modules/test_module_constants.py
 tests/functional/codegen/modules/test_module_variables.py
 tests/functional/codegen/modules/test_stateless_functions.py
 tests/functional/codegen/storage_variables/test_getters.py
 tests/functional/codegen/storage_variables/test_setters.py
 tests/functional/codegen/storage_variables/test_storage_variable.py
@@ -350,29 +351,34 @@
 tests/unit/compiler/ir/__init__.py
 tests/unit/compiler/ir/test_calldatacopy.py
 tests/unit/compiler/ir/test_compile_ir.py
 tests/unit/compiler/ir/test_optimize_ir.py
 tests/unit/compiler/ir/test_repeat.py
 tests/unit/compiler/ir/test_with.py
 tests/unit/compiler/venom/test_convert_basicblock_simple.py
+tests/unit/compiler/venom/test_dominator_tree.py
 tests/unit/compiler/venom/test_duplicate_operands.py
+tests/unit/compiler/venom/test_liveness_simple_loop.py
+tests/unit/compiler/venom/test_make_ssa.py
 tests/unit/compiler/venom/test_multi_entry_block.py
 tests/unit/compiler/venom/test_stack_at_external_return.py
+tests/unit/compiler/venom/test_variables.py
 tests/unit/semantics/conftest.py
 tests/unit/semantics/test_namespace.py
 tests/unit/semantics/test_storage_slots.py
 tests/unit/semantics/analysis/test_array_index.py
 tests/unit/semantics/analysis/test_cyclic_function_calls.py
 tests/unit/semantics/analysis/test_for_loop.py
 tests/unit/semantics/analysis/test_potential_types.py
 tests/unit/semantics/types/test_event.py
 tests/unit/semantics/types/test_pure_types.py
 tests/unit/semantics/types/test_size_in_bytes.py
 tests/unit/semantics/types/test_type_from_abi.py
 tests/unit/semantics/types/test_type_from_annotation.py
+tests/unit/utils/test_keccak256.py
 vyper/__init__.py
 vyper/__main__.py
 vyper/abi_types.py
 vyper/exceptions.py
 vyper/typing.py
 vyper/utils.py
 vyper/version.py
@@ -475,15 +481,19 @@
 vyper/semantics/types/user.py
 vyper/semantics/types/utils.py
 vyper/venom/README.md
 vyper/venom/__init__.py
 vyper/venom/analysis.py
 vyper/venom/basicblock.py
 vyper/venom/bb_optimizer.py
+vyper/venom/dominators.py
 vyper/venom/function.py
 vyper/venom/ir_node_to_venom.py
 vyper/venom/stack_model.py
 vyper/venom/venom_to_assembly.py
 vyper/venom/passes/base_pass.py
 vyper/venom/passes/constant_propagation.py
 vyper/venom/passes/dft.py
-vyper/venom/passes/normalization.py
+vyper/venom/passes/make_ssa.py
+vyper/venom/passes/normalization.py
+vyper/venom/passes/simplify_cfg.py
+vyper/venom/passes/stack_reorder.py
```

### Comparing `vyper-0.4.0b5/vyper.egg-info/requires.txt` & `vyper-0.4.0b6/vyper.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -2,61 +2,55 @@
 asttokens<3,>=2.0.5
 pycryptodome<4,>=3.5.1
 packaging<24,>=23.1
 importlib-metadata
 wheel
 
 [dev]
-pytest<7.0,>=6.2.5
-pytest-cov<3.0,>=2.10
+ipython
+pre-commit
+pyinstaller
+twine
+pytest<9.0,>=8.0
+pytest-cov<5.0,>=4.1
 pytest-instafail<1.0,>=0.4
-pytest-xdist<3.0,>=2.5
+pytest-xdist<3.4,>=3.0
 pytest-split<1.0,>=0.7.0
-eth-tester[py-evm]<0.10,>=0.9.0b1
+eth-tester[py-evm]<0.11,>=0.10.0b4
 eth_abi<5.0.0,>=4.0.0
-py-evm<0.8,>=0.7.0a1
+py-evm<0.11,>=0.10.0b4
 web3==6.0.0
-tox<4.0,>=3.15
 lark==1.1.9
-hypothesis[lark]<6.0,>=5.37.1
-eth-stdlib==0.2.6
+hypothesis[lark]<7.0,>=6.0
+eth-stdlib==0.2.7
+setuptools
+hexbytes>=1.2
 black==23.12.0
 flake8==6.1.0
 flake8-bugbear==23.12.2
 flake8-use-fstring==1.4
 isort==5.13.2
 mypy==1.5
-recommonmark
-sphinx<7.0,>=6.0
-sphinx_rtd_theme<1.3,>=1.2
-ipython
-pre-commit
-pyinstaller
-twine
-
-[docs]
-recommonmark
-sphinx<7.0,>=6.0
-sphinx_rtd_theme<1.3,>=1.2
 
 [lint]
 black==23.12.0
 flake8==6.1.0
 flake8-bugbear==23.12.2
 flake8-use-fstring==1.4
 isort==5.13.2
 mypy==1.5
 
 [test]
-pytest<7.0,>=6.2.5
-pytest-cov<3.0,>=2.10
+pytest<9.0,>=8.0
+pytest-cov<5.0,>=4.1
 pytest-instafail<1.0,>=0.4
-pytest-xdist<3.0,>=2.5
+pytest-xdist<3.4,>=3.0
 pytest-split<1.0,>=0.7.0
-eth-tester[py-evm]<0.10,>=0.9.0b1
+eth-tester[py-evm]<0.11,>=0.10.0b4
 eth_abi<5.0.0,>=4.0.0
-py-evm<0.8,>=0.7.0a1
+py-evm<0.11,>=0.10.0b4
 web3==6.0.0
-tox<4.0,>=3.15
 lark==1.1.9
-hypothesis[lark]<6.0,>=5.37.1
-eth-stdlib==0.2.6
+hypothesis[lark]<7.0,>=6.0
+eth-stdlib==0.2.7
+setuptools
+hexbytes>=1.2
```

