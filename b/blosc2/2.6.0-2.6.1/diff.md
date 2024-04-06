# Comparing `tmp/blosc2-2.6.0.tar.gz` & `tmp/blosc2-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blosc2-2.6.0.tar", last modified: Mon Apr  1 17:37:30 2024, max compression
+gzip compressed data, was "blosc2-2.6.1.tar", last modified: Thu Apr  4 09:52:29 2024, max compression
```

## Comparing `blosc2-2.6.0.tar` & `blosc2-2.6.1.tar`

### file list

```diff
@@ -1,1206 +1,1206 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.148718 blosc2-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 17:37:16.000000 blosc2-2.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.980719 blosc2-2.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-01 17:37:16.000000 blosc2-2.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.980719 blosc2-2.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-01 17:37:16.000000 blosc2-2.6.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-01 17:37:16.000000 blosc2-2.6.0/.github/workflows/cibuildwheels.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-01 17:37:16.000000 blosc2-2.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 17:37:16.000000 blosc2-2.6.0/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.960719 blosc2-2.6.0/.guix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.980719 blosc2-2.6.0/.guix/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-01 17:37:16.000000 blosc2-2.6.0/.guix/modules/python-blosc2-package.scm
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 17:37:16.000000 blosc2-2.6.0/.guix-channel
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-01 17:37:16.000000 blosc2-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-01 17:37:16.000000 blosc2-2.6.0/ANNOUNCE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 17:37:16.000000 blosc2-2.6.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-01 17:37:16.000000 blosc2-2.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-01 17:37:16.000000 blosc2-2.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-01 17:37:30.148718 blosc2-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-01 17:37:16.000000 blosc2-2.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-01 17:37:16.000000 blosc2-2.6.0/README_DEVELOPERS.md
--rw-r--r--   0 runner    (1001) docker     (127)    14934 2024-04-01 17:37:16.000000 blosc2-2.6.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-01 17:37:16.000000 blosc2-2.6.0/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 17:37:16.000000 blosc2-2.6.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.984719 blosc2-2.6.0/bench/
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/compress_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)   208392 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/encode-itrunc-Linux-i13900K.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   202922 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/encode-itrunc-MacOS-M1.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   179771 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/encode-sparse-MacOS-Intel.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/get_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.984719 blosc2-2.6.0/bench/ndarray/
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/compare_getslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/copy_postfilter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1326 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/download_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.984719 blosc2-2.6.0/bench/ndarray/era5-pds/
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/era5-pds/measurements-i10k.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16516 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/era5-pds/measurements-i13k.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/era5-pds/measurements-m1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/era5-pds/measurements-ryzen3.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/plot_transcode_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/ndarray/transcode_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/pack_compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/pack_large.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/pack_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/set_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-01 17:37:16.000000 blosc2-2.6.0/bench/sum_postfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.988719 blosc2-2.6.0/blosc2/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-01 17:37:16.000000 blosc2-2.6.0/blosc2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-01 17:37:16.000000 blosc2-2.6.0/blosc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    93448 2024-04-01 17:37:16.000000 blosc2-2.6.0/blosc2/blosc2_ext.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.992719 blosc2-2.6.0/blosc2/c-blosc2/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.992719 blosc2-2.6.0/blosc2/c-blosc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.992719 blosc2-2.6.0/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.992719 blosc2-2.6.0/blosc2/c-blosc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.github/workflows/cmake.yml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.github/workflows/fuzz.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.964719 blosc2-2.6.0/blosc2/c-blosc2/.guix/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.992719 blosc2-2.6.0/blosc2/c-blosc2/.guix/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.guix/modules/c-blosc2-package.scm
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.guix-channel
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.mailmap
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/ANNOUNCE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/Blosc2Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/DEVELOPING-GUIDE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.992719 blosc2-2.6.0/blosc2/c-blosc2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/LICENSES/FASTLZ.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/LICENSES/LZ4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/LICENSES/ZLIB.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/LICENSES/ZSTD.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/README_ARM.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/README_B2ND_METALAYER.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/README_CFRAME_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/README_CHUNK_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/README_FUZZER.md
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/README_SFRAME_FORMAT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/README_THREADED.rst
--rw-r--r--   0 runner    (1001) docker     (127)    33665 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/ROADMAP.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/THANKS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/TODO-refactorization.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.996719 blosc2-2.6.0/blosc2/c-blosc2/bench/
--rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/Makefile.mingw
--rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/b2bench.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.996719 blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/bench_stack_append.c
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/create_frame.c
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/delta_schunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/plot-speeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/plot-sum_openmp-results.py
--rw-r--r--   0 runner    (1001) docker     (127)    18639 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/read-grid-150x150.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.996719 blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (127)    29803 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (127)    29683 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out
--rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/sframe_bench.c
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/sum_openmp.c
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/trunc_prec_schunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/bench/zero_runlen.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.004719 blosc2-2.6.0/blosc2/c-blosc2/blosc/
--rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/b2nd-private.h
--rw-r--r--   0 runner    (1001) docker     (127)    68396 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/b2nd.c
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/b2nd_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)    21536 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-altivec.c
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-altivec.h
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-avx2.c
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-avx2.h
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-avx512.c
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-avx512.h
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-generic.c
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-generic.h
--rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-neon.c
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-neon.h
--rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-sse2.c
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-sse2.h
--rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/blosc-private.h
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/blosc2-stdio.c
--rw-r--r--   0 runner    (1001) docker     (127)   154426 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/blosc2.c
--rw-r--r--   0 runner    (1001) docker     (127)    24335 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/blosclz.c
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/blosclz.h
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/config.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/context.h
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/delta.c
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/delta.h
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/directories.c
--rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/fastcopy.c
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/fastcopy.h
--rw-r--r--   0 runner    (1001) docker     (127)   117812 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/frame.c
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/frame.h
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/schunk-private.h
--rw-r--r--   0 runner    (1001) docker     (127)    57257 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/schunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/sframe.c
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/sframe.h
--rw-r--r--   0 runner    (1001) docker     (127)    15711 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-altivec.c
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-altivec.h
--rw-r--r--   0 runner    (1001) docker     (127)    31644 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-avx2.c
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-avx2.h
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-generic.c
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-generic.h
--rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-neon.c
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-neon.h
--rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-sse2.c
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-sse2.h
--rw-r--r--   0 runner    (1001) docker     (127)    20057 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle.c
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle.h
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/stune.c
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/stune.h
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/timestamp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/transpose-altivec.h
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/trunc-prec.c
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/trunc-prec.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.004719 blosc2-2.6.0/blosc2/c-blosc2/blosc/win32/
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/win32/pthread.c
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc/win32/pthread.h
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/blosc2.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.004719 blosc2-2.6.0/blosc2/c-blosc2/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake/FindIPP.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake/FindLZ4.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake/FindSIMD.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake/FindZSTD.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake/toolchain-armhf.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake/toolchain-armsf.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/compat/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    33610 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    32485 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    16176 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    36256 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    36263 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    20530 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata
--rw-r--r--   0 runner    (1001) docker     (127)   141205 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    22760 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    27787 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    22760 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    36349 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    31963 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    31963 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/compat/filegen.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.964719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6974 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    23072 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     8642 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    11457 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    14436 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10706 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    16818 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1420 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     4846 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2262 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle
--rwxr-xr-x   0 runner    (1001) docker     (127)     7574 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3708 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     7910 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5792 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    11472 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8199 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    24719 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1376 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     4233 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2214 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     7559 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.012719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3616 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    13037 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.016719 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4479 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    15834 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.968719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.016719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10906 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2162 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2769 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     6545 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.016719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3943 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     7713 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     4630 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     8365 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.016719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2577 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.016719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2997 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.016719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2268 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     4883 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2711 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     6813 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2010 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     5787 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.016719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3949 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     7649 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     7353 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.020719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)      656 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2212 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.020719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.020719 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2279 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     5550 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     2737 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c
--rwxr-xr-x   0 runner    (1001) docker     (127)     4987 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.020719 blosc2-2.6.0/blosc2/c-blosc2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.020719 blosc2-2.6.0/blosc2/c-blosc2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/_static/blosc-logo_256.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.020719 blosc2-2.6.0/blosc2/c-blosc2/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/c-blosc2.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.020719 blosc2-2.6.0/blosc2/c-blosc2/doc/development/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/development/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/development/releasing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/development/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.020719 blosc2-2.6.0/blosc2/c-blosc2/doc/format/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/format/cframe_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/format/chunk_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/format/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/format/sframe_format.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.024719 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/b2nd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/blosc1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/context.rst
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/metalayers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/schunk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/utility_functions.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/reference/utility_variables.rst
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.028719 blosc2-2.6.0/blosc2/c-blosc2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.028719 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_oindex.c
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_print_meta.c
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_serialize.c
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_stack_images.c
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/compress_file.c
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/contexts.c
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/decompress_file.c
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/delta_schunk_ex.c
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/find_roots.c
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/frame_backed_schunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/frame_big.c
--rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/frame_metalayers.c
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/frame_offset.c
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/frame_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/frame_simple.c
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/frame_vlmetalayers.c
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/get_blocksize.c
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/get_set_slice.c
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/instrument_codec.c
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/many_compressors.c
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/multithread.c
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/noinit.c
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/schunk_postfilter.c
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/schunk_simple.c
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/sframe_simple.c
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/simple.c
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/urcodecs.c
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/urfilters.c
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/win-dynamic-linking.c
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/examples/zstd_dict.c
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/guix.scm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.028719 blosc2-2.6.0/blosc2/c-blosc2/images/
--rw-r--r--   0 runner    (1001) docker     (127)   116429 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (127)   113029 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (127)   314966 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/images/b2nd-2level-parts.png
--rw-r--r--   0 runner    (1001) docker     (127)    45440 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/images/blosc2-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (127)   491569 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/images/blosc2-pipeline.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.028719 blosc2-2.6.0/blosc2/c-blosc2/include/
--rw-r--r--   0 runner    (1001) docker     (127)    21361 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/include/b2nd.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.032719 blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/blosc2-common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/blosc2-export.h
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/codecs-registry.h
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/filters-registry.h
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/tuners-registry.h
--rw-r--r--   0 runner    (1001) docker     (127)    96600 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/include/blosc2.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.972719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.032719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)   113390 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c
--rw-r--r--   0 runner    (1001) docker     (127)    43263 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h
--rw-r--r--   0 runner    (1001) docker     (127)    70129 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c
--rw-r--r--   0 runner    (1001) docker     (127)    20179 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.044719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc
--rw-r--r--   0 runner    (1001) docker     (127)    53620 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11765 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.044719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.044719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/arm.h
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/ctzl.h
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.044719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/Makefile.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.044719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.c
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.h
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.048719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.048719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.968719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.968719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.048719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      991 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner
--rwxr-xr-x   0 runner    (1001) docker     (127)      740 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/qemu-user-static.service
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.048719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/INDEX.md
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c
--rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.h
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.052719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c
--rwxr-xr-x   0 runner    (1001) docker     (127)    63492 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c
--rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h
--rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_p.h
--rw-r--r--   0 runner    (1001) docker     (127)    26517 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h
--rw-r--r--   0 runner    (1001) docker     (127)    26517 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h
--rw-r--r--   0 runner    (1001) docker     (127)    69027 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c
--rw-r--r--   0 runner    (1001) docker     (127)    15612 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c
--rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.052719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36944 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h
--rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h
--rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c
--rw-r--r--   0 runner    (1001) docker     (127)    16106 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c
--rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c
--rw-r--r--   0 runner    (1001) docker     (127)    15022 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h
--rw-r--r--   0 runner    (1001) docker     (127)    48765 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c
--rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h
--rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.056719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.056719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2003-0107.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.056719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.056719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.056719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/test.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.056719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/
--rw-r--r--   0 runner    (1001) docker     (127)    48192 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt
--rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.056719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.056719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/test.bin
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.060719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/defneg3.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.060719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/
--rw-r--r--   0 runner    (1001) docker     (127)   180001 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.060719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/
--rw-r--r--   0 runner    (1001) docker     (127)   106840 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.060719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/ignore
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi
--rw-r--r--   0 runner    (1001) docker     (127)    90251 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     4281 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.060719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)   123093 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   419233 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt
--rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c
--rw-r--r--   0 runner    (1001) docker     (127)    33965 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.060719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c
--rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c
--rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.060719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c
--rwxr-xr-x   0 runner    (1001) docker     (127)      833 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.064719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/codecov-upload.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      678 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c
--rw-r--r--   0 runner    (1001) docker     (127)    31487 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.064719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/
--rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h
--rw-r--r--   0 runner    (1001) docker     (127)    94727 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map
--rw-r--r--   0 runner    (1001) docker     (127)    94178 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.cmakein
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c
--rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.064719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.068719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h
--rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h
--rw-r--r--   0 runner    (1001) docker     (127)    30110 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h
--rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (127)   212896 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.076719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h
--rw-r--r--   0 runner    (1001) docker     (127)    24096 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h
--rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)   312776 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)    64416 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h
--rw-r--r--   0 runner    (1001) docker     (127)    20004 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h
--rw-r--r--   0 runner    (1001) docker     (127)    28499 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h
--rw-r--r--   0 runner    (1001) docker     (127)    27872 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h
--rw-r--r--   0 runner    (1001) docker     (127)    34479 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h
--rw-r--r--   0 runner    (1001) docker     (127)    36950 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h
--rw-r--r--   0 runner    (1001) docker     (127)   101952 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h
--rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h
--rw-r--r--   0 runner    (1001) docker     (127)    67459 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h
--rw-r--r--   0 runner    (1001) docker     (127)    81334 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.076719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/
--rw-r--r--   0 runner    (1001) docker     (127)    73701 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    14207 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S
--rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h
--rw-r--r--   0 runner    (1001) docker     (127)    99701 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)    99641 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h
--rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.076719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c
--rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.080719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    42898 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h
--rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h
--rw-r--r--   0 runner    (1001) docker     (127)    28561 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c
--rw-r--r--   0 runner    (1001) docker     (127)    44008 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.972719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.080719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln
--rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.084719 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h
--rw-r--r--   0 runner    (1001) docker     (127)    69465 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h
--rw-r--r--   0 runner    (1001) docker     (127)   125639 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h
--rw-r--r--   0 runner    (1001) docker     (127)   111749 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h
--rw-r--r--   0 runner    (1001) docker     (127)   132791 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h
--rw-r--r--   0 runner    (1001) docker     (127)   153658 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h
--rw-r--r--   0 runner    (1001) docker     (127)   163699 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h
--rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.pc.in
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap
--rw-r--r--   0 runner    (1001) docker     (127)    26433 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h
--rw-r--r--   0 runner    (1001) docker     (127)   171378 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.084719 blosc2-2.6.0/blosc2/c-blosc2/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.084719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/codecs-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.084719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h
--rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h
--rw-r--r--   0 runner    (1001) docker     (127)    19307 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (127)   205061 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.088719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    26695 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.088719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.088719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/macros.h
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h
--rw-r--r--   0 runner    (1001) docker     (127)    34968 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.096719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/bitstream.c
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/block1.h
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/block2.h
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/block3.h
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/block4.h
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1d.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1f.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1i.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1l.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2d.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2f.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2i.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2l.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3d.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3f.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3i.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3l.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4d.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4f.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4i.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4l.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1d.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1f.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1i.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1l.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2d.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2f.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2i.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2l.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3d.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3f.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3i.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3l.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4d.c
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4f.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4i.c
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4l.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.096719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/
--rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/inline.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.096719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/share/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.100719 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.c
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.h
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec1.c
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c
--rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodei.c
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revcodecf.c
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode1.c
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode2.c
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode1.c
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode2.c
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/template.h
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsi.h
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsl.h
--rw-r--r--   0 runner    (1001) docker     (127)    32747 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c
--rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.100719 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.100719 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/filters-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.104719 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/int_trunc.c
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/int_trunc.h
--rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/test_int_trunc.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.104719 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.104719 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h
--rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/plugin_utils.c
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/plugin_utils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.104719 blosc2-2.6.0/blosc2/c-blosc2/plugins/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/test_data/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd
--rw-r--r--   0 runner    (1001) docker     (127)   141455 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.104719 blosc2-2.6.0/blosc2/c-blosc2/plugins/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/tuners/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/plugins/tuners/tuners-registry.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.116718 blosc2-2.6.0/blosc2/c-blosc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.120719 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/cutest.h
--rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy_buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c
--rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/cutest.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.120719 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.120719 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    33187 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame
--rw-r--r--   0 runner    (1001) docker     (127)    41393 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame
--rw-r--r--   0 runner    (1001) docker     (127)    24087 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame
--rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame
--rw-r--r--   0 runner    (1001) docker     (127)    11408 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/standalone.c
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/gcc-segfault-issue.c
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/print_versions.c
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_all.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_api.c
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_blosc1_compat.c
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_change_nthreads_append.c
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_compress_roundtrip.c
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_compress_roundtrip.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_compressor.c
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_contexts.c
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_copy.c
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_delete_chunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_delta.c
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_delta_schunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_dict_schunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_empty_buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_fill_special.c
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_filters.c
--rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_frame.c
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_frame_get_offsets.c
--rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_frame_offset.c
--rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_get_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_get_slice_nchunks.c
--rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_getitem.c
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_getitem.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_getitem_delta.c
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_insert_chunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_lazychunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_maskout.c
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_maxout.c
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_noinit.c
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_nolock.c
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_nthreads.c
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_postfilter.c
--rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_prefilter.c
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_reorder_offsets.c
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_schunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_schunk_frame.c
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_schunk_header.c
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_set_slice_buffer.c
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_sframe.c
--rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_sframe_lazychunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c
--rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_small_chunks.c
--rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_udio.c
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_update_chunk.c
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_urcodecs.c
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_urfilters.c
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-01 17:37:17.000000 blosc2-2.6.0/blosc2/c-blosc2/tests/test_zero_runlen.c
--rw-r--r--   0 runner    (1001) docker     (127)    48476 2024-04-01 17:37:16.000000 blosc2-2.6.0/blosc2/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-01 17:37:16.000000 blosc2-2.6.0/blosc2/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    18354 2024-04-01 17:37:16.000000 blosc2-2.6.0/blosc2/lazyexpr.py
--rw-r--r--   0 runner    (1001) docker     (127)    39252 2024-04-01 17:37:16.000000 blosc2-2.6.0/blosc2/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    32454 2024-04-01 17:37:16.000000 blosc2-2.6.0/blosc2/schunk.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 17:37:29.000000 blosc2-2.6.0/blosc2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.148718 blosc2-2.6.0/blosc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-01 17:37:29.000000 blosc2-2.6.0/blosc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    54757 2024-04-01 17:37:29.000000 blosc2-2.6.0/blosc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:37:29.000000 blosc2-2.6.0/blosc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 17:37:29.000000 blosc2-2.6.0/blosc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-01 17:37:29.000000 blosc2-2.6.0/blosc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-01 17:37:16.000000 blosc2-2.6.0/code_of_conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.120719 blosc2-2.6.0/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.120719 blosc2-2.6.0/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/_static/blosc-logo_128.png
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/_static/blosc-logo_256.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.120719 blosc2-2.6.0/doc/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.120719 blosc2-2.6.0/doc/development/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/development/code-of-conduct.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/development/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/development/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.124719 blosc2-2.6.0/doc/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.124719 blosc2-2.6.0/doc/getting_started/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/00.schunk-basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/01.schunk-slicing_and_beyond.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    21544 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/02.ndarray-basics.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19380 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/10.ucodecs-ufilters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/11.prefilters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/12.postfilters.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.124719 blosc2-2.6.0/doc/getting_started/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (127)    45440 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/blosc2-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (127)   491569 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/blosc2-pipeline.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.128718 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/
--rw-r--r--   0 runner    (1001) docker     (127)   107624 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/backward.png
--rw-r--r--   0 runner    (1001) docker     (127)    38548 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/backward.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/decoder.png
--rw-r--r--   0 runner    (1001) docker     (127)    31483 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/decoder.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.png
--rw-r--r--   0 runner    (1001) docker     (127)    35540 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/encoder.png
--rw-r--r--   0 runner    (1001) docker     (127)    23248 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/encoder.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24481 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.svg
--rw-r--r--   0 runner    (1001) docker     (127)   110817 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/forward.png
--rw-r--r--   0 runner    (1001) docker     (127)    41521 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/forward.svg
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/getting_started/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/python-blosc2.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.128718 blosc2-2.6.0/doc/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:29.976719 blosc2-2.6.0/doc/reference/autofiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.128718 blosc2-2.6.0/doc/reference/autofiles/schunk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.132718 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.blocksize.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cbytes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunkshape.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunksize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.contiguous.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cparams.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cratio.rst
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.dparams.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.nbytes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.typesize.rst
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.urlpath.rst
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/meta.rst
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/vlmeta.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__getitem__.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__init__.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__len__.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__setitem__.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.append_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.decompress_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.delete_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.fill_special.rst
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.filler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_slice.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks_info.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.postfilter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.prefilter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_postfilter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_prefilter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.to_cframe.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_chunk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_data.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.132718 blosc2-2.6.0/doc/reference/autofiles/top_level/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/top_level/blosc2.Codec.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/top_level/blosc2.Filter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/top_level/blosc2.SpecialValue.rst
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/top_level/blosc2.SplitMode.rst
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/top_level/blosc2.Tuner.rst
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/autofiles/top_level/blosc2.nthreads.rst
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/ndarray_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/schunk_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/reference/top_level.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.132718 blosc2-2.6.0/doc/release_notes/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 17:37:16.000000 blosc2-2.6.0/doc/release_notes/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.136718 blosc2-2.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/btune.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/compress2_decompress2.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/compress_decompress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/filler.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/gil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.136718 blosc2-2.6.0/examples/ndarray/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/asarray_.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/bytedelta_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/copy_.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/empty_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/eval_expr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/getitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/iterchunks_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/ndarray_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/ndmean.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/persistency.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/resize_.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/work_with_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ndarray/zfp_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/pack_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/pack_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/postfilter1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/postfilter2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/postfilter3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/prefilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/save_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/schunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/schunk_roundtrip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ucodecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/ufilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 17:37:16.000000 blosc2-2.6.0/examples/vlmeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-01 17:37:16.000000 blosc2-2.6.0/guix.scm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.140718 blosc2-2.6.0/images/
--rw-r--r--   0 runner    (1001) docker     (127)   116429 2024-04-01 17:37:16.000000 blosc2-2.6.0/images/Complete-Write-Read-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (127)    64898 2024-04-01 17:37:16.000000 blosc2-2.6.0/images/M1-i386-vs-arm64-pack.png
--rw-r--r--   0 runner    (1001) docker     (127)    62528 2024-04-01 17:37:16.000000 blosc2-2.6.0/images/M1-i386-vs-arm64-unpack.png
--rw-r--r--   0 runner    (1001) docker     (127)   113029 2024-04-01 17:37:16.000000 blosc2-2.6.0/images/Read-Partial-Slices-B2ND.png
--rw-r--r--   0 runner    (1001) docker     (127)   314966 2024-04-01 17:37:16.000000 blosc2-2.6.0/images/b2nd-2level-parts.png
--rw-r--r--   0 runner    (1001) docker     (127)    77813 2024-04-01 17:37:16.000000 blosc2-2.6.0/images/linspace-compress.png
--rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-04-01 17:37:16.000000 blosc2-2.6.0/images/linspace-decompress.png
--rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-01 17:37:16.000000 blosc2-2.6.0/images/pack-array-cratios.png
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-01 17:37:16.000000 blosc2-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 17:37:16.000000 blosc2-2.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 17:37:16.000000 blosc2-2.6.0/requirements-build.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-01 17:37:16.000000 blosc2-2.6.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-01 17:37:16.000000 blosc2-2.6.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-01 17:37:16.000000 blosc2-2.6.0/requirements-runtime.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-01 17:37:16.000000 blosc2-2.6.0/requirements-test-wheels.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 17:37:16.000000 blosc2-2.6.0/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:37:30.148718 blosc2-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-01 17:37:16.000000 blosc2-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.144718 blosc2-2.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:37:30.144718 blosc2-2.6.0/tests/ndarray/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/persistency.cat
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_auto_parts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_full.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_get_slice_nchunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_getitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_iterchunks_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_lazyexpr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_lossy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_metalayers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_persistency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_setitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_squeeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_struct_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/ndarray/test_zeros.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_bytes_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_comp_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_compress2.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_compression_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_compressors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_decompress.py
--rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_iterchunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_postfilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_prefilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_python_blosc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_schunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_schunk_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_schunk_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_schunk_get_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_schunk_get_slice_nchunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_schunk_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_schunk_set_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_schunk_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_ucodecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_ufilters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-01 17:37:16.000000 blosc2-2.6.0/tests/test_vlmeta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.901418 blosc2-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-04 09:52:15.000000 blosc2-2.6.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.717416 blosc2-2.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-04 09:52:15.000000 blosc2-2.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.717416 blosc2-2.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-04 09:52:15.000000 blosc2-2.6.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-04 09:52:15.000000 blosc2-2.6.1/.github/workflows/cibuildwheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-04 09:52:15.000000 blosc2-2.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 09:52:15.000000 blosc2-2.6.1/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.697416 blosc2-2.6.1/.guix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.717416 blosc2-2.6.1/.guix/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-04 09:52:15.000000 blosc2-2.6.1/.guix/modules/python-blosc2-package.scm
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 09:52:15.000000 blosc2-2.6.1/.guix-channel
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 09:52:15.000000 blosc2-2.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 09:52:15.000000 blosc2-2.6.1/ANNOUNCE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 09:52:15.000000 blosc2-2.6.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-04 09:52:15.000000 blosc2-2.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-04 09:52:15.000000 blosc2-2.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-04 09:52:29.901418 blosc2-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-04 09:52:15.000000 blosc2-2.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-04 09:52:15.000000 blosc2-2.6.1/README_DEVELOPERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15091 2024-04-04 09:52:15.000000 blosc2-2.6.1/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-04 09:52:15.000000 blosc2-2.6.1/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 09:52:15.000000 blosc2-2.6.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.717416 blosc2-2.6.1/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/compress_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   208392 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/encode-itrunc-Linux-i13900K.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   202922 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/encode-itrunc-MacOS-M1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   179771 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/encode-sparse-MacOS-Intel.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/get_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.721416 blosc2-2.6.1/bench/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/compare_getslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/copy_postfilter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1326 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.721416 blosc2-2.6.1/bench/ndarray/era5-pds/
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/era5-pds/measurements-i10k.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16516 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16476 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/era5-pds/measurements-i13k.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16500 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/era5-pds/measurements-m1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/era5-pds/measurements-ryzen3.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/plot_transcode_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/ndarray/transcode_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/pack_compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/pack_large.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/pack_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/set_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-04 09:52:15.000000 blosc2-2.6.1/bench/sum_postfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.721416 blosc2-2.6.1/blosc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-04 09:52:15.000000 blosc2-2.6.1/blosc2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-04 09:52:15.000000 blosc2-2.6.1/blosc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93448 2024-04-04 09:52:15.000000 blosc2-2.6.1/blosc2/blosc2_ext.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.729416 blosc2-2.6.1/blosc2/c-blosc2/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.729416 blosc2-2.6.1/blosc2/c-blosc2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.729416 blosc2-2.6.1/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.729416 blosc2-2.6.1/blosc2/c-blosc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.github/workflows/cmake.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.github/workflows/fuzz.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.701416 blosc2-2.6.1/blosc2/c-blosc2/.guix/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.729416 blosc2-2.6.1/blosc2/c-blosc2/.guix/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.guix/modules/c-blosc2-package.scm
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.guix-channel
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/ANNOUNCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/Blosc2Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/DEVELOPING-GUIDE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.729416 blosc2-2.6.1/blosc2/c-blosc2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/LICENSES/FASTLZ.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/LICENSES/LZ4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/LICENSES/ZLIB.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/LICENSES/ZSTD.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/README_ARM.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/README_B2ND_METALAYER.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/README_CFRAME_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/README_CHUNK_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/README_FUZZER.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/README_SFRAME_FORMAT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/README_THREADED.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    33890 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/ROADMAP.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/THANKS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/TODO-refactorization.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.733416 blosc2-2.6.1/blosc2/c-blosc2/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)     7655 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/Makefile.mingw
+-rw-r--r--   0 runner    (1001) docker     (127)    16664 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/b2bench.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.733416 blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/bench_stack_append.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/create_frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/delta_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/plot-speeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/plot-sum_openmp-results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18639 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/read-grid-150x150.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.733416 blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (127)    29803 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (127)    29683 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out
+-rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out
+-rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/sframe_bench.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/sum_openmp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/trunc_prec_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/bench/zero_runlen.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.745416 blosc2-2.6.1/blosc2/c-blosc2/blosc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15752 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/b2nd-private.h
+-rw-r--r--   0 runner    (1001) docker     (127)    68396 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/b2nd.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/b2nd_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21536 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-altivec.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-avx2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-avx512.c
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-avx512.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-generic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-generic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18673 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-neon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-sse2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/blosc-private.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/blosc2-stdio.c
+-rw-r--r--   0 runner    (1001) docker     (127)   154426 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/blosc2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    24335 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/blosclz.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/blosclz.h
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/config.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/context.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/delta.c
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/delta.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/directories.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16719 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/fastcopy.c
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/fastcopy.h
+-rw-r--r--   0 runner    (1001) docker     (127)   117812 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/frame.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/schunk-private.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57257 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/schunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/sframe.c
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/sframe.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15711 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-altivec.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31644 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-avx2.h
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-generic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-generic.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22000 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-neon.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-sse2.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20057 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/stune.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/stune.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/timestamp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/transpose-altivec.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/trunc-prec.c
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/trunc-prec.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.745416 blosc2-2.6.1/blosc2/c-blosc2/blosc/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/win32/pthread.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc/win32/pthread.h
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/blosc2.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.745416 blosc2-2.6.1/blosc2/c-blosc2/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake/FindIPP.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake/FindLZ4.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake/FindSIMD.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake/FindZSTD.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake/toolchain-armhf.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake/toolchain-armsf.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.749416 blosc2-2.6.1/blosc2/c-blosc2/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    26736 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    33610 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    32485 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    16176 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36256 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36263 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    20530 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)   141205 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    22760 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    27787 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    22760 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36349 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    31963 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    36267 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    31963 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    15763 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/compat/filegen.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.749416 blosc2-2.6.1/blosc2/c-blosc2/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.701416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6974 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23072 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8642 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11457 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14436 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10706 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16818 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1420 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4846 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2262 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7896 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7574 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3708 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7910 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5792 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11472 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8199 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24719 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1376 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4233 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2214 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7559 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3616 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13037 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.753416 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4479 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15834 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.705416 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.757416 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10906 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2162 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2769 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6545 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.757416 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3943 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7713 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4630 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8365 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.757416 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2577 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.757416 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      756 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2997 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.757416 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2268 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4883 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2711 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6813 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2010 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5787 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.757416 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3949 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7649 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4177 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7353 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.757416 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      656 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2212 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.761417 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.761417 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2279 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5550 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2737 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4987 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.761417 blosc2-2.6.1/blosc2/c-blosc2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.761417 blosc2-2.6.1/blosc2/c-blosc2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/_static/blosc-logo_256.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.761417 blosc2-2.6.1/blosc2/c-blosc2/doc/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/c-blosc2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.761417 blosc2-2.6.1/blosc2/c-blosc2/doc/development/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/development/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/development/releasing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/development/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.761417 blosc2-2.6.1/blosc2/c-blosc2/doc/format/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/format/cframe_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/format/chunk_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/format/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/format/sframe_format.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.765416 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/b2nd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/blosc1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/context.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/metalayers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/schunk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/utility_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/reference/utility_variables.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.769417 blosc2-2.6.1/blosc2/c-blosc2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.769417 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_oindex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_print_meta.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_serialize.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_stack_images.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/compress_file.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/contexts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/decompress_file.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/delta_schunk_ex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/find_roots.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/frame_backed_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/frame_big.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/frame_metalayers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/frame_offset.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/frame_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/frame_simple.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/frame_vlmetalayers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/get_blocksize.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/get_set_slice.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/instrument_codec.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/many_compressors.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/multithread.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/noinit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/schunk_postfilter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/schunk_simple.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/sframe_simple.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/simple.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/urcodecs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/urfilters.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/win-dynamic-linking.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/examples/zstd_dict.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/guix.scm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.773417 blosc2-2.6.1/blosc2/c-blosc2/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   116429 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (127)   113029 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (127)   314966 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/images/b2nd-2level-parts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45440 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/images/blosc2-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   491569 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/images/blosc2-pipeline.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.773417 blosc2-2.6.1/blosc2/c-blosc2/include/
+-rw-r--r--   0 runner    (1001) docker     (127)    21361 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/include/b2nd.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.773417 blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/blosc2-common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/blosc2-export.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/codecs-registry.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/filters-registry.h
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/tuners-registry.h
+-rw-r--r--   0 runner    (1001) docker     (127)    96600 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/include/blosc2.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.709416 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.773417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)   113390 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c
+-rw-r--r--   0 runner    (1001) docker     (127)    43263 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h
+-rw-r--r--   0 runner    (1001) docker     (127)    70129 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20179 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.789417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc
+-rw-r--r--   0 runner    (1001) docker     (127)    53620 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16681 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13120 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11765 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.789417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.789417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/arm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/ctzl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.789417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/generic/Makefile.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.789417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.c
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/power.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.793417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11854 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.793417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.705416 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.705416 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.793417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      991 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner
+-rwxr-xr-x   0 runner    (1001) docker     (127)      740 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/qemu-user-static.service
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.797417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/INDEX.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16308 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.797417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     8934 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)    63492 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)    26517 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (127)    26517 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69027 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15612 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.801417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20502 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36944 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25040 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14849 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c
+-rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16106 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18689 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15022 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    48765 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12915 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2003-0107.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2004-0797/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-1849/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2005-2096/test.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/
+-rw-r--r--   0 runner    (1001) docker     (127)    48192 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    32768 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-361/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-364/test.bin
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-382/defneg3.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/
+-rw-r--r--   0 runner    (1001) docker     (127)   180001 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-751/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/
+-rw-r--r--   0 runner    (1001) docker     (127)   106840 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.805417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/ignore
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi
+-rw-r--r--   0 runner    (1001) docker     (127)    90251 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4281 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.809417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   123093 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   419233 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   102400 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c
+-rw-r--r--   0 runner    (1001) docker     (127)    33965 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.809417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11473 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.809417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c
+-rwxr-xr-x   0 runner    (1001) docker     (127)      833 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.809417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/codecov-upload.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      678 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c
+-rw-r--r--   0 runner    (1001) docker     (127)    31487 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.813417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/
+-rw-r--r--   0 runner    (1001) docker     (127)    17920 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6991 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h
+-rw-r--r--   0 runner    (1001) docker     (127)    94727 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map
+-rw-r--r--   0 runner    (1001) docker     (127)    94178 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.cmakein
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8297 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.813417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK
+-rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.821417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13012 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (127)    30110 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (127)   212896 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.825417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24096 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h
+-rw-r--r--   0 runner    (1001) docker     (127)    57710 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)   312776 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    64416 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h
+-rw-r--r--   0 runner    (1001) docker     (127)    20004 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28499 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27872 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34479 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36950 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h
+-rw-r--r--   0 runner    (1001) docker     (127)   101952 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28437 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67459 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h
+-rw-r--r--   0 runner    (1001) docker     (127)    81334 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.825417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/
+-rw-r--r--   0 runner    (1001) docker     (127)    73701 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14207 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S
+-rw-r--r--   0 runner    (1001) docker     (127)     9182 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h
+-rw-r--r--   0 runner    (1001) docker     (127)    99701 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)    99641 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.829417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.829417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    42898 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h
+-rw-r--r--   0 runner    (1001) docker     (127)    54649 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28561 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c
+-rw-r--r--   0 runner    (1001) docker     (127)    44008 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.709416 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.829417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln
+-rw-r--r--   0 runner    (1001) docker     (127)    10105 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.833417 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)    14318 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h
+-rw-r--r--   0 runner    (1001) docker     (127)    69465 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h
+-rw-r--r--   0 runner    (1001) docker     (127)   125639 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h
+-rw-r--r--   0 runner    (1001) docker     (127)   111749 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h
+-rw-r--r--   0 runner    (1001) docker     (127)   132791 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h
+-rw-r--r--   0 runner    (1001) docker     (127)   153658 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h
+-rw-r--r--   0 runner    (1001) docker     (127)   163699 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h
+-rw-r--r--   0 runner    (1001) docker     (127)   182559 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.pc.in
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap
+-rw-r--r--   0 runner    (1001) docker     (127)    26433 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h
+-rw-r--r--   0 runner    (1001) docker     (127)   171378 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.833417 blosc2-2.6.1/blosc2/c-blosc2/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6562 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.833417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/codecs-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.837417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23091 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h
+-rw-r--r--   0 runner    (1001) docker     (127)    19307 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (127)   205061 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.837417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    26695 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.841417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.841417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/macros.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h
+-rw-r--r--   0 runner    (1001) docker     (127)    34968 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.845417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/bitstream.c
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/block1.h
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/block2.h
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/block3.h
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/block4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1d.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1f.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1i.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode1l.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2d.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2f.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2i.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode2l.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3d.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3f.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3i.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode3l.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4d.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4f.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4i.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/decode4l.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1d.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1f.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1i.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode1l.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2d.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2f.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2i.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode2l.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3d.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3f.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3i.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode3l.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4d.c
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4f.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4i.c
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/encode4l.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.849417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/
+-rw-r--r--   0 runner    (1001) docker     (127)    12957 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/inline.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.849417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.853417 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.c
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec.h
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec1.c
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9466 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodei.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revcodecf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode1.c
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode2.c
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode1.c
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode2.c
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/template.h
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsi.h
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    32747 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10264 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.853417 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.853417 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/filters-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.857417 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/int_trunc.c
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/int_trunc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14641 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/test_int_trunc.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.857417 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.857417 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10406 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/plugin_utils.c
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/plugin_utils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.857417 blosc2-2.6.1/blosc2/c-blosc2/plugins/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/test_data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd
+-rw-r--r--   0 runner    (1001) docker     (127)   141455 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.857417 blosc2-2.6.1/blosc2/c-blosc2/plugins/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/tuners/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/plugins/tuners/tuners-registry.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.865417 blosc2-2.6.1/blosc2/c-blosc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.869418 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/cutest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5034 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/cutest.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.869418 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.873417 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    33187 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame
+-rw-r--r--   0 runner    (1001) docker     (127)    41393 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame
+-rw-r--r--   0 runner    (1001) docker     (127)    24087 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame
+-rw-r--r--   0 runner    (1001) docker     (127)    21570 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame
+-rw-r--r--   0 runner    (1001) docker     (127)    11408 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/standalone.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/gcc-segfault-issue.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/print_versions.c
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_all.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_api.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_blosc1_compat.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_change_nthreads_append.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_compress_roundtrip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_compress_roundtrip.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9936 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_compressor.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_contexts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_copy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_delete_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_delta.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_delta_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_dict_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_empty_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_fill_special.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_filters.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11742 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_frame_get_offsets.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_frame_offset.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_get_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_get_slice_nchunks.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4299 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_getitem.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_getitem.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_getitem_delta.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_insert_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_lazychunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_maskout.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_maxout.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_noinit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_nolock.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_nthreads.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_postfilter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6959 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_prefilter.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_reorder_offsets.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_schunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_schunk_frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_schunk_header.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_set_slice_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_sframe.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_sframe_lazychunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_small_chunks.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4725 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_udio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_update_chunk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_urcodecs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_urfilters.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-04 09:52:16.000000 blosc2-2.6.1/blosc2/c-blosc2/tests/test_zero_runlen.c
+-rw-r--r--   0 runner    (1001) docker     (127)    48396 2024-04-04 09:52:15.000000 blosc2-2.6.1/blosc2/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-04 09:52:15.000000 blosc2-2.6.1/blosc2/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18354 2024-04-04 09:52:15.000000 blosc2-2.6.1/blosc2/lazyexpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39252 2024-04-04 09:52:15.000000 blosc2-2.6.1/blosc2/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32454 2024-04-04 09:52:15.000000 blosc2-2.6.1/blosc2/schunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 09:52:29.000000 blosc2-2.6.1/blosc2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.901418 blosc2-2.6.1/blosc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-04 09:52:29.000000 blosc2-2.6.1/blosc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    54757 2024-04-04 09:52:29.000000 blosc2-2.6.1/blosc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:52:29.000000 blosc2-2.6.1/blosc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 09:52:29.000000 blosc2-2.6.1/blosc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 09:52:29.000000 blosc2-2.6.1/blosc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 09:52:15.000000 blosc2-2.6.1/code_of_conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.873417 blosc2-2.6.1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.873417 blosc2-2.6.1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/_static/blosc-logo_128.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/_static/blosc-logo_256.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.873417 blosc2-2.6.1/doc/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.873417 blosc2-2.6.1/doc/development/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/development/code-of-conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/development/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/development/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.873417 blosc2-2.6.1/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.873417 blosc2-2.6.1/doc/getting_started/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/00.schunk-basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/01.schunk-slicing_and_beyond.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21544 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/02.ndarray-basics.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19380 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/10.ucodecs-ufilters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/11.prefilters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/12.postfilters.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.873417 blosc2-2.6.1/doc/getting_started/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    45440 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/blosc2-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (127)   491569 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/blosc2-pipeline.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.877418 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/
+-rw-r--r--   0 runner    (1001) docker     (127)   107624 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/backward.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38548 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/backward.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/decoder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31483 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/decoder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35540 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/encoder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23248 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/encoder.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12906 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24481 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   110817 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/forward.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41521 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/forward.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/getting_started/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/python-blosc2.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.877418 blosc2-2.6.1/doc/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.713416 blosc2-2.6.1/doc/reference/autofiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.881418 blosc2-2.6.1/doc/reference/autofiles/schunk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.885418 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.blocksize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cbytes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunkshape.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.chunksize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.contiguous.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cparams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.cratio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.dparams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.nbytes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.typesize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/blosc2.schunk.SChunk.urlpath.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/meta.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/vlmeta.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__getitem__.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__init__.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__len__.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.__setitem__.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.append_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.decompress_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.delete_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.fill_special.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.filler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.get_slice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.insert_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.iterchunks_info.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.postfilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.prefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_postfilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.remove_prefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.to_cframe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_chunk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/schunk/blosc2.schunk.SChunk.update_data.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.885418 blosc2-2.6.1/doc/reference/autofiles/top_level/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/top_level/blosc2.Codec.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/top_level/blosc2.Filter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/top_level/blosc2.SpecialValue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/top_level/blosc2.SplitMode.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/top_level/blosc2.Tuner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/autofiles/top_level/blosc2.nthreads.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/ndarray_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/schunk_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/reference/top_level.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.885418 blosc2-2.6.1/doc/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 09:52:15.000000 blosc2-2.6.1/doc/release_notes/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.889418 blosc2-2.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/btune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/compress2_decompress2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/compress_decompress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/filler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/gil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.889418 blosc2-2.6.1/examples/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/asarray_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/bytedelta_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/copy_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/empty_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/eval_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/iterchunks_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/ndarray_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/ndmean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/persistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/resize_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/work_with_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ndarray/zfp_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/pack_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/pack_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/postfilter1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/postfilter2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/postfilter3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/prefilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/save_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/schunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/schunk_roundtrip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ucodecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/ufilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-04 09:52:15.000000 blosc2-2.6.1/examples/vlmeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-04 09:52:15.000000 blosc2-2.6.1/guix.scm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.893418 blosc2-2.6.1/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   116429 2024-04-04 09:52:15.000000 blosc2-2.6.1/images/Complete-Write-Read-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64898 2024-04-04 09:52:15.000000 blosc2-2.6.1/images/M1-i386-vs-arm64-pack.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62528 2024-04-04 09:52:15.000000 blosc2-2.6.1/images/M1-i386-vs-arm64-unpack.png
+-rw-r--r--   0 runner    (1001) docker     (127)   113029 2024-04-04 09:52:15.000000 blosc2-2.6.1/images/Read-Partial-Slices-B2ND.png
+-rw-r--r--   0 runner    (1001) docker     (127)   314966 2024-04-04 09:52:15.000000 blosc2-2.6.1/images/b2nd-2level-parts.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77813 2024-04-04 09:52:15.000000 blosc2-2.6.1/images/linspace-compress.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24888 2024-04-04 09:52:15.000000 blosc2-2.6.1/images/linspace-decompress.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-04 09:52:15.000000 blosc2-2.6.1/images/pack-array-cratios.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-04 09:52:15.000000 blosc2-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-04 09:52:15.000000 blosc2-2.6.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 09:52:15.000000 blosc2-2.6.1/requirements-build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-04 09:52:15.000000 blosc2-2.6.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-04 09:52:15.000000 blosc2-2.6.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-04 09:52:15.000000 blosc2-2.6.1/requirements-runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 09:52:15.000000 blosc2-2.6.1/requirements-test-wheels.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-04 09:52:15.000000 blosc2-2.6.1/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:52:29.901418 blosc2-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-04 09:52:15.000000 blosc2-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.897418 blosc2-2.6.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:52:29.901418 blosc2-2.6.1/tests/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/persistency.cat
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_auto_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_get_slice_nchunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_iterchunks_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_lazyexpr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_lossy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_metalayers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_persistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_setitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_struct_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/ndarray/test_zeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_bytes_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_comp_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_compress2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_compression_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_compressors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_decompress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_iterchunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_postfilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_prefilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9876 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_python_blosc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_schunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_schunk_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_schunk_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_schunk_get_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_schunk_get_slice_nchunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_schunk_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_schunk_set_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_schunk_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_ucodecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_ufilters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-04 09:52:15.000000 blosc2-2.6.1/tests/test_vlmeta.py
```

### Comparing `blosc2-2.6.0/.github/workflows/build.yml` & `blosc2-2.6.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/.github/workflows/cibuildwheels.yml` & `blosc2-2.6.1/.github/workflows/cibuildwheels.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/.gitignore` & `blosc2-2.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/.guix/modules/python-blosc2-package.scm` & `blosc2-2.6.1/.guix/modules/python-blosc2-package.scm`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/ANNOUNCE.rst` & `blosc2-2.6.1/ANNOUNCE.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-Announcing Python-Blosc2 2.6.0
+Announcing Python-Blosc2 2.6.1
 ==============================
 
-New evaluation engine (based on numexpr) for NDArray instances.  Now,
-you can evaluate expressions like `a + b + 1` where `a` and `b` are
-NDArray instances.  This is a powerful feature that allows for
-efficient computations on compressed data.  See this
-[example](https://github.com/Blosc/python-blosc2/blob/main/examples/ndarray/eval_expr.py)
-to see how this works.  Thanks to @omaech for her help in the `pow` function.
-
-Also, this is the first version supporting NumPy 2.0.0.  Please tell us
-if you find any issues with this new version of NumPy.
+Updated to latest C-Blosc2 2.14.1. This was necessary to be able to
+load dynamics plugins on Windows.
 
 For more info, you can have a look at the release notes in:
 
 https://github.com/Blosc/python-blosc2/releases
 
 More docs and examples are available in the documentation site:
```

### Comparing `blosc2-2.6.0/CONTRIBUTING.rst` & `blosc2-2.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/LICENSE.txt` & `blosc2-2.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/PKG-INFO` & `blosc2-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blosc2
-Version: 2.6.0
+Version: 2.6.1
 Summary: Python wrapper for the C-Blosc2 library
 Author-email: Blosc Development Team <blosc@blosc.org>
 Maintainer-email: Blosc Development Team <blosc@blosc.org>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/Blosc/python-blosc2
 Project-URL: documentation, https://www.blosc.org/python-blosc2/python-blosc2.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `blosc2-2.6.0/README.rst` & `blosc2-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/RELEASE_NOTES.md` & `blosc2-2.6.1/RELEASE_NOTES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # Release notes
 
+## Changes from 2.6.0 to 2.6.1
+
+* Updated to latest C-Blosc2 2.14.1. This was necessary to be able to
+  load dynamics plugins on Windows.
+
 ## Changes from 2.5.1 to 2.6.0
 
-* New evaluation engine (based on numexpr) for NDArray instances.  Now,
-  you can evaluate expressions like `a + b + 1` where `a` and `b` are
-  NDArray instances.  This is a powerful feature that allows for
+* [EXP] New evaluation engine (based on numexpr) for NDArray instances.
+  Now, you can evaluate expressions like `a + b + 1` where `a` and `b`
+  are NDArray instances.  This is a powerful feature that allows for
   efficient computations on compressed data.  See this
   [example](https://github.com/Blosc/python-blosc2/blob/main/examples/ndarray/eval_expr.py)
   to see how this works.  Thanks to @omaech for her help in the `pow` function.
 
-* As a consequence, there are many new functions to operate with NDArray
-  instances.  See the function section in
+* As a consequence of the above, there are many new functions to operate with
+  NDArray instances.  See the function section in
   [NDArray API](https://www.blosc.org/python-blosc2/reference/ndarray_api.html#functions)
   for more information.
 
 * Support for NumPy 2.0.0 is here!  Now, the wheels are built with NumPy 2.0.0rc1.
   Please tell us in case you see any issues with this new version.
 
 * Add `**kwargs` to `load_tensor()` function.  This allows to
```

### Comparing `blosc2-2.6.0/RELEASING.rst` & `blosc2-2.6.1/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/compress_numpy.py` & `blosc2-2.6.1/bench/compress_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/encode-itrunc-Linux-i13900K.ipynb` & `blosc2-2.6.1/bench/encode-itrunc-Linux-i13900K.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/encode-itrunc-MacOS-M1.ipynb` & `blosc2-2.6.1/bench/encode-itrunc-MacOS-M1.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/encode-sparse-MacOS-Intel.ipynb` & `blosc2-2.6.1/bench/encode-sparse-MacOS-Intel.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/get_slice.py` & `blosc2-2.6.1/bench/get_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/compare_getslice.py` & `blosc2-2.6.1/bench/ndarray/compare_getslice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/copy_postfilter.py` & `blosc2-2.6.1/bench/ndarray/copy_postfilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/download_data.py` & `blosc2-2.6.1/bench/ndarray/download_data.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/era5-pds/measurements-i10k.parquet` & `blosc2-2.6.1/bench/ndarray/era5-pds/measurements-i10k.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet` & `blosc2-2.6.1/bench/ndarray/era5-pds/measurements-i13k-always-split.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet` & `blosc2-2.6.1/bench/ndarray/era5-pds/measurements-i13k-never-split.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/era5-pds/measurements-i13k.parquet` & `blosc2-2.6.1/bench/ndarray/era5-pds/measurements-i13k.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/era5-pds/measurements-m1.parquet` & `blosc2-2.6.1/bench/ndarray/era5-pds/measurements-m1.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/era5-pds/measurements-ryzen3.parquet` & `blosc2-2.6.1/bench/ndarray/era5-pds/measurements-ryzen3.parquet`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/plot_transcode_data.ipynb` & `blosc2-2.6.1/bench/ndarray/plot_transcode_data.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/ndarray/transcode_data.py` & `blosc2-2.6.1/bench/ndarray/transcode_data.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/pack_compress.py` & `blosc2-2.6.1/bench/pack_compress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/pack_large.py` & `blosc2-2.6.1/bench/pack_large.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/pack_tensor.py` & `blosc2-2.6.1/bench/pack_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/set_slice.py` & `blosc2-2.6.1/bench/set_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/bench/sum_postfilter.py` & `blosc2-2.6.1/bench/sum_postfilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/CMakeLists.txt` & `blosc2-2.6.1/blosc2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/__init__.py` & `blosc2-2.6.1/blosc2/__init__.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/blosc2_ext.pyx` & `blosc2-2.6.1/blosc2/blosc2_ext.pyx`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md` & `blosc2-2.6.1/blosc2/c-blosc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/.github/workflows/cmake.yml` & `blosc2-2.6.1/blosc2/c-blosc2/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/.github/workflows/fuzz.yml` & `blosc2-2.6.1/blosc2/c-blosc2/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/.guix/modules/c-blosc2-package.scm` & `blosc2-2.6.1/blosc2/c-blosc2/.guix/modules/c-blosc2-package.scm`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/.readthedocs.yaml` & `blosc2-2.6.1/blosc2/c-blosc2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/ANNOUNCE.md` & `blosc2-2.6.1/blosc2/c-blosc2/ANNOUNCE.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Announcing C-Blosc2 2.14.0
+# Announcing C-Blosc2 2.14.1
 A fast, compressed and persistent binary data store library for C.
 
 ## What is new?
 
-This is a minor release for adding an accelerated path in `b2nd_append()`.
-Also, many fixes and improvements have been added.
+This is a maintenance release. When loading plugins, first try with
+`python` and then `python3`. This is because many linux distros
+do not have `python` as a symlink to `python3` anymore.
 
 For more info, please see the release notes in:
 
 https://github.com/Blosc/c-blosc2/blob/main/RELEASE_NOTES.md
 
 Also, there is blog post introducing the most relevant changes in Blosc2:
```

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/Blosc2Config.cmake.in` & `blosc2-2.6.1/blosc2/c-blosc2/Blosc2Config.cmake.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst` & `blosc2-2.6.1/blosc2/c-blosc2/COMPILING_WITH_WHEELS.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/CONTRIBUTING.rst` & `blosc2-2.6.1/blosc2/c-blosc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/DEVELOPING-GUIDE.rst` & `blosc2-2.6.1/blosc2/c-blosc2/DEVELOPING-GUIDE.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/FAQ.md` & `blosc2-2.6.1/blosc2/c-blosc2/FAQ.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/LICENSE.txt` & `blosc2-2.6.1/blosc2/c-blosc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt` & `blosc2-2.6.1/blosc2/c-blosc2/LICENSES/BITSHUFFLE.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/LICENSES/FASTLZ.txt` & `blosc2-2.6.1/blosc2/c-blosc2/LICENSES/FASTLZ.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/LICENSES/LZ4.txt` & `blosc2-2.6.1/blosc2/c-blosc2/LICENSES/LZ4.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/LICENSES/ZLIB.txt` & `blosc2-2.6.1/blosc2/c-blosc2/LICENSES/ZLIB.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/LICENSES/ZSTD.txt` & `blosc2-2.6.1/blosc2/c-blosc2/LICENSES/ZSTD.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/README.rst` & `blosc2-2.6.1/blosc2/c-blosc2/README.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/README_ARM.rst` & `blosc2-2.6.1/blosc2/c-blosc2/README_ARM.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/README_B2ND_METALAYER.rst` & `blosc2-2.6.1/blosc2/c-blosc2/README_B2ND_METALAYER.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/README_CFRAME_FORMAT.rst` & `blosc2-2.6.1/blosc2/c-blosc2/README_CFRAME_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/README_CHUNK_FORMAT.rst` & `blosc2-2.6.1/blosc2/c-blosc2/README_CHUNK_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/README_FUZZER.md` & `blosc2-2.6.1/blosc2/c-blosc2/README_FUZZER.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/README_SFRAME_FORMAT.rst` & `blosc2-2.6.1/blosc2/c-blosc2/README_SFRAME_FORMAT.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/README_THREADED.rst` & `blosc2-2.6.1/blosc2/c-blosc2/README_THREADED.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/RELEASE_NOTES.md` & `blosc2-2.6.1/blosc2/c-blosc2/RELEASE_NOTES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Release notes for C-Blosc2
 ==========================
 
+Changes from 2.14.0 to 2.14.1
+=============================
+
+* When loading plugins, first try with `python` and then `python3`.
+  This is because many linux distros do not have `python` as a
+  symlink to `python3` anymore.
+
 Changes from 2.13.2 to 2.14.0
 =============================
 
 * Fixed a bug preventing buffers to be appended to empty (0-sized) b2nd arrays.
 
 * New acceleration path for `b2nd_append()`.  This new path is
   much faster (up to 4x) than the previous one, specially for large arrays.
```

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/RELEASING.rst` & `blosc2-2.6.1/blosc2/c-blosc2/RELEASING.rst`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 Announcing
 ----------
 
 - Send an announcement to the blosc and comp.compression mailing lists.
   Use the ``ANNOUNCE.md`` file as skeleton (likely as the definitive version).
 
-- Tweet about it from the @Blosc2 account.
+- Toot about it from the @Blosc2 account in https://fosstodon.org.
 
 
 Post-release actions
 --------------------
 
 - Edit *VERSION* symbols in blosc/blosc2.h in master to increment the
   version to the next minor one (i.e. X.Y.Z --> X.Y.(Z+1).dev).
```

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/ROADMAP.rst` & `blosc2-2.6.1/blosc2/c-blosc2/ROADMAP.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/THANKS.rst` & `blosc2-2.6.1/blosc2/c-blosc2/THANKS.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/bench/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/Makefile` & `blosc2-2.6.1/blosc2/c-blosc2/bench/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/Makefile.mingw` & `blosc2-2.6.1/blosc2/c-blosc2/bench/Makefile.mingw`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/b2bench.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/b2bench.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/bench_get_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/bench_stack_append.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/bench_stack_append.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/b2nd/bench_zfp_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/create_frame.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/create_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/delta_schunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/delta_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/plot-speeds.py` & `blosc2-2.6.1/blosc2/c-blosc2/bench/plot-speeds.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/plot-sum_openmp-results.py` & `blosc2-2.6.1/blosc2/c-blosc2/bench/plot-sum_openmp-results.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin` & `blosc2-2.6.1/blosc2/c-blosc2/bench/rainfall-grid-150x150.bin`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/read-grid-150x150.py` & `blosc2-2.6.1/blosc2/c-blosc2/bench/read-grid-150x150.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out` & `blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/blosclz-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out` & `blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/blosclz-suite-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out` & `blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/lz4-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out` & `blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/lz4-suite-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out` & `blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/lz4hc-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out` & `blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/zlib-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out` & `blosc2-2.6.1/blosc2/c-blosc2/bench/results-corex/zstd-cl1-sum_openmp-corex.out`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/sframe_bench.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/sframe_bench.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/sum_openmp.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/sum_openmp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/trunc_prec_schunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/trunc_prec_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/bench/zero_runlen.c` & `blosc2-2.6.1/blosc2/c-blosc2/bench/zero_runlen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/b2nd-private.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/b2nd-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/b2nd.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/b2nd.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/b2nd_utils.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/b2nd_utils.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-altivec.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-altivec.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-avx2.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-avx2.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-avx2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-avx512.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-avx512.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-avx512.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-avx512.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-generic.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-generic.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-generic.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-neon.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-neon.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-sse2.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/bitshuffle-sse2.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/bitshuffle-sse2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/blosc-private.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/blosc-private.h`

 * *Files 11% similar despite different names*

```diff
@@ -242,28 +242,40 @@
   }
 }
 #else
 #include <dlfcn.h>
 #endif
 
 
-static inline void* load_lib(char *plugin_name, char *libpath) {
+static inline int get_libpath(char *plugin_name, char *libpath, char *python_version) {
+  BLOSC_TRACE_INFO("Trying to get plugin path with python%s\n", python_version);
   char python_cmd[PATH_MAX] = {0};
-  sprintf(python_cmd, "python3 -c \"import blosc2_%s; blosc2_%s.print_libpath()\"", plugin_name, plugin_name);
+  sprintf(python_cmd, "python%s -c \"import blosc2_%s; blosc2_%s.print_libpath()\"", python_version, plugin_name, plugin_name);
   FILE *fp = popen(python_cmd, "r");
   if (fp == NULL) {
     BLOSC_TRACE_ERROR("Could not run python");
-    return NULL;
+    return BLOSC2_ERROR_FAILURE;
   }
   if (fgets(libpath, PATH_MAX, fp) == NULL) {
     BLOSC_TRACE_ERROR("Could not read python output");
     pclose(fp);
-    return NULL;
+    return BLOSC2_ERROR_FAILURE;
   }
   pclose(fp);
+
+  return BLOSC2_ERROR_SUCCESS;
+}
+
+
+static inline void* load_lib(char *plugin_name, char *libpath) {
+  if (get_libpath(plugin_name, libpath, "") < 0 && get_libpath(plugin_name, libpath, "3") < 0) {
+    BLOSC_TRACE_ERROR("Problems when running python or python3 for getting plugin path");
+    return NULL;
+  }
+
   if (strlen(libpath) == 0) {
     BLOSC_TRACE_ERROR("Could not find plugin libpath");
     return NULL;
   }
   void* loaded_lib;
   BLOSC_TRACE_INFO("libpath for plugin blosc2_%s: %s\n", plugin_name, libpath);
   loaded_lib = dlopen(libpath, RTLD_LAZY);
```

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/blosc2-stdio.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/blosc2-stdio.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/blosc2.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/blosc2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/blosclz.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/blosclz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/blosclz.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/blosclz.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/context.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/context.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/delta.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/delta.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/delta.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/directories.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/directories.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/fastcopy.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/fastcopy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/fastcopy.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/fastcopy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/frame.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/frame.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/frame.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/schunk-private.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/schunk-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/schunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/sframe.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/sframe.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/sframe.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/sframe.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-altivec.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-altivec.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-avx2.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-avx2.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-avx2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-generic.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-generic.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-generic.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-neon.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-neon.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-sse2.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle-sse2.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle-sse2.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/shuffle.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/shuffle.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/stune.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/stune.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/stune.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/stune.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/timestamp.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/timestamp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/transpose-altivec.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/transpose-altivec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/trunc-prec.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/trunc-prec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/trunc-prec.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/trunc-prec.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/win32/pthread.c` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/win32/pthread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/blosc/win32/pthread.h` & `blosc2-2.6.1/blosc2/c-blosc2/blosc/win32/pthread.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/cmake/FindIPP.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/cmake/FindIPP.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/cmake/FindSIMD.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/cmake/FindSIMD.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/cmake/FindZLIB_NG.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/cmake/toolchain-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/cmake/toolchain-armhf.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/cmake/toolchain-armhf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/cmake/toolchain-armsf.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/cmake/toolchain-armsf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/cmake_uninstall.cmake.in` & `blosc2-2.6.1/blosc2/c-blosc2/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/compat/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.11.1-zstd.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.14.0-zstd.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.17.1-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.18.0-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.3.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.3.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.3.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.3.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.7.0-blosclz.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.7.0-lz4.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.7.0-lz4hc.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-1.7.0-zlib.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle4-memcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata` & `blosc2-2.6.1/blosc2/c-blosc2/compat/blosc-2.0.0-lz4-bitshuffle8-nomemcpy.cdata`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/compat/filegen.c` & `blosc2-2.6.1/blosc2/c-blosc2/compat/filegen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test16.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/Test/bitshuffle_bitunshuffle_test8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle16_neon/bitshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle1_neon/bitshuffle1_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle2_neon/bitshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle4_neon/bitshuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitshuffle8_neon/bitshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle16_neon/bitunshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle1_neon/bitunshuffle1_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle2_neon/bitunshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle4_neon/bitunshuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/bitshuffle_neon/bitunshuffle8_neon/bitunshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test16.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/Test/shuffle_unshuffle_test8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle16_neon/shuffle16_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle2_neon/shuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle4_neon/shuffle4_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_opt_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/shuffle8_neon/shuffle8_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle16_neon/unshuffle16_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle2_neon/unshuffle2_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle4_neon/unshuffle4_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c` & `blosc2-2.6.1/blosc2/c-blosc2/contrib/shuffle_neon/unshuffle8_neon/unshuffle8_neon_vtbx_bucle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/_static/blosc-logo_256.png` & `blosc2-2.6.1/blosc2/c-blosc2/doc/_static/blosc-logo_256.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/_static/css/custom.css` & `blosc2-2.6.1/blosc2/c-blosc2/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/conf.py` & `blosc2-2.6.1/blosc2/c-blosc2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/b2nd.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/b2nd.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/blosc1.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/blosc1.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/context.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/context.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/index.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/index.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/metalayers.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/metalayers.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/plugins.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/plugins.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/schunk.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/schunk.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/utility_functions.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/utility_functions.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/doc/reference/utility_variables.rst` & `blosc2-2.6.1/blosc2/c-blosc2/doc/reference/utility_variables.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/README.rst` & `blosc2-2.6.1/blosc2/c-blosc2/examples/README.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_empty_shape.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_frame_generator.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_oindex.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_oindex.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_plainbuffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_plugins_codecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_plugins_filters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_print_meta.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_print_meta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_serialize.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_serialize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/b2nd/example_stack_images.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/b2nd/example_stack_images.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/compress_file.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/compress_file.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/contexts.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/contexts.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/decompress_file.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/decompress_file.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/delta_schunk_ex.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/delta_schunk_ex.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/find_roots.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/find_roots.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/frame_backed_schunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/frame_backed_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/frame_big.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/frame_big.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/frame_metalayers.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/frame_metalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/frame_offset.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/frame_offset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/frame_roundtrip.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/frame_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/frame_simple.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/frame_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/frame_vlmetalayers.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/frame_vlmetalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/get_blocksize.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/get_blocksize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/get_set_slice.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/get_set_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/instrument_codec.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/instrument_codec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/many_compressors.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/many_compressors.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/multithread.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/multithread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/noinit.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/noinit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/schunk_postfilter.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/schunk_postfilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/schunk_simple.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/schunk_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/sframe_simple.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/sframe_simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/simple.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/simple.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/urcodecs.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/urcodecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/urfilters.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/urfilters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/win-dynamic-linking.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/win-dynamic-linking.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/examples/zstd_dict.c` & `blosc2-2.6.1/blosc2/c-blosc2/examples/zstd_dict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/guix.scm` & `blosc2-2.6.1/blosc2/c-blosc2/guix.scm`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png` & `blosc2-2.6.1/blosc2/c-blosc2/images/Complete-Write-Read-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png` & `blosc2-2.6.1/blosc2/c-blosc2/images/Read-Partial-Slices-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/images/b2nd-2level-parts.png` & `blosc2-2.6.1/blosc2/c-blosc2/images/b2nd-2level-parts.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/images/blosc2-pipeline.png` & `blosc2-2.6.1/blosc2/c-blosc2/images/blosc2-pipeline.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/images/blosc2-pipeline.svg` & `blosc2-2.6.1/blosc2/c-blosc2/images/blosc2-pipeline.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/include/b2nd.h` & `blosc2-2.6.1/blosc2/c-blosc2/include/b2nd.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/blosc2-common.h` & `blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/blosc2-common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/blosc2-export.h` & `blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/blosc2-export.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h` & `blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/blosc2-stdio.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/codecs-registry.h` & `blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/codecs-registry.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/filters-registry.h` & `blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/filters-registry.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/include/blosc2/tuners-registry.h` & `blosc2-2.6.1/blosc2/c-blosc2/include/blosc2/tuners-registry.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/include/blosc2.h` & `blosc2-2.6.1/blosc2/c-blosc2/include/blosc2.h`

 * *Files 0% similar despite different names*

```diff
@@ -79,18 +79,18 @@
   #define blosc_cbuffer_complib blosc2_cbuffer_complib
 #endif
 
 
 /* Version numbers */
 #define BLOSC2_VERSION_MAJOR    2    /* for major interface/format changes  */
 #define BLOSC2_VERSION_MINOR    14   /* for minor interface/format changes  */
-#define BLOSC2_VERSION_RELEASE  0    /* for tweaks, bug-fixes, or development */
+#define BLOSC2_VERSION_RELEASE  1    /* for tweaks, bug-fixes, or development */
 
-#define BLOSC2_VERSION_STRING   "2.14.0"  /* string version.  Sync with above! */
-#define BLOSC2_VERSION_DATE     "$Date:: 2023-04-01 #$"    /* date version */
+#define BLOSC2_VERSION_STRING   "2.14.1"  /* string version.  Sync with above! */
+#define BLOSC2_VERSION_DATE     "$Date:: 2023-04-04 #$"    /* date version */
 
 
 /* The maximum number of dimensions for Blosc2 NDim arrays */
 #define BLOSC2_MAX_DIM 8
 
 
 /* Tracing macros */
```

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/lz4-1.9.4/lz4hc.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/.shellcheckrc`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/FAQ.zlib`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/INDEX.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/PORTING.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/adler32_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/adler32_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/armfeature.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/chunkset_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/crc32_acle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/insert_string_acle.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/arm/slide_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/adler32_power8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/power/slide_hash_power8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_deflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_detail.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/dfltcc_inflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.Dockerfile`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/actions-runner.service`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/actions-runner`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/s390/self-hosted-builder/fs/usr/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/adler32_ssse3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/chunkset_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/compare258_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/crc_folding.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/insert_string_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_avx.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/slide_sse.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/arch/x86/x86.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/chunkset_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-arch.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-coverage.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-install-dirs.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/detect-sanitizer.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-compare.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/run-and-redirect.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-compress.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/test-tools.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-aarch64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-arm.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-armhf.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-i686.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-mingw-x86_64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-powerpc64le.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-s390x.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/cmake/toolchain-sparc64.cmake`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compare258.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/configure`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_comb_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/crc32_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_medium.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_quick.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/deflate_slow.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/algorithm.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1950.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1951.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/rfc1952.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/doc/txtvsbin.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/fallback_builtins.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/functable.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzguts.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzlib.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzread.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/gzwrite.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/infback.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inffixed_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inflate_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/inftrees.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/insert_string_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/match_tpl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2002-0059/test.gz`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/default.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/CVE-2018-25032/fixed.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/GH-979/pigz-2.6.tar.gz`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/Makefile.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-arm-linux-gnueabihf.abi`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abi/zlib-v1.2.11-x86_64-linux-gnu.abi`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/abicheck.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/adler32_test.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/crc32_test.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/fireworks.jpg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/lcet10.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/data/paper-100k.pdf`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_bi_valid.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/deflate_quick_block_open.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/example.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/checksum_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/compress_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_dict_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_flush_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_large_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/example_small_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/minigzip_fuzzer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/fuzz/standalone_fuzz_target_runner.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/gh1235.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/hash_head_0.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/infcover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/inflate_adler32.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minideflate.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/minigzip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pigz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/pkgcheck.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/switchlevels.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/test/testCVEinputs.sh`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/config.sub`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makecrct.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/makefixed.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/tools/maketrees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_emit.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl._h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/trees_tbl.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/uncompr.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/DLL_FAQ.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.a64`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.arm`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/Makefile.msc`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/README-WIN32.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib-ng1.rc`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlib1.rc`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/win32/zlibcompat.def`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zbuild.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf-ng.h.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.in`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zconf.h.included`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zendian.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib-ng.map`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zlib.map`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zlib-ng-2.0.7/zutil_p.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/BUCK`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/allocations.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bits.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/compiler.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/cpu.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/debug.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/error_private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/huf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/mem.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/pool.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/portability_macros.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/threading.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/common/zstd_trace.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/clevels.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/fse_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/hist.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/huf_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_literals.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_sequences.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_compress_superblock.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_cwksp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_double_fast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_fast.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_lazy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_ldm_geartab.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstd_opt.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/compress/zstdmt_compress.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/huf_decompress_amd64.S`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_common.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/deprecated/zbuff_decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/cover.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/divsufsort.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/fastcover.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dictBuilder/zdict.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.sln`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/dll/example/fullbench-dll.vcxproj`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_legacy.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v01.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v02.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v03.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v04.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v05.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v06.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/legacy/zstd_v07.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/libzstd.mk`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/module.modulemap`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zdict.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h` & `blosc2-2.6.1/blosc2/c-blosc2/internal-complibs/zstd-1.5.5/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/codecs-registry.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/codecs-registry.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz4x4.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/ndlz8x8.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/test_ndlz.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/ndlz/xxhash.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/blosc2-zfp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/bitstream.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/system.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/types.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp/version.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/include/zfp.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/inline/bitstream.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/omp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/share/parallel.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codec4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/codecf.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/compress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/decompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode1.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/encodei.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/ompcompress.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revdecodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode3.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencode4.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/template/revencodef.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsd.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/traitsf.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/src/zfp.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_acc_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_prec_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_float.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/test_zfp_rate_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/codecs/zfp/zfp-private.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/bytedelta.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/bytedelta/test_bytedelta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/filters-registry.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/filters-registry.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/int_trunc.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/int_trunc.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/int_trunc.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/int_trunc.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/int_trunc/test_int_trunc.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/int_trunc/test_int_trunc.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/ndcell.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndcell/test_ndcell.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/ndmean.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_mean.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/filters/ndmean/test_ndmean_repart.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/plugin_utils.c` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/plugin_utils.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/test_data/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/test_data/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/test_data/example_day_month_temp.b2nd`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd` & `blosc2-2.6.1/blosc2/c-blosc2/plugins/test_data/example_item_prices.b2nd`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/Makefile` & `blosc2-2.6.1/blosc2/c-blosc2/tests/Makefile`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/cutest.h` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/cutest.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_append.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy_buffer.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_copy_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_delete.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_full.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_get_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_insert.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_metalayers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_open_offset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_persistency.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_resize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_save.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_serialize.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_set_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_squeeze_index.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_uninit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_b2nd_zeros.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/b2nd/test_common.h` & `blosc2-2.6.1/blosc2/c-blosc2/tests/b2nd/test_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/cutest.h` & `blosc2-2.6.1/blosc2/c-blosc2/tests/cutest.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/README.md` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/README.md`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-blosclz.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-lz4hc.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zlib.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/corpus/frame_simple-zstd.b2frame`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/fuzz_compress_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/fuzz_compress_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/fuzz_decompress_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/generate_inputs_corpus.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/fuzz/standalone.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/fuzz/standalone.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/gcc-segfault-issue.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/gcc-segfault-issue.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/print_versions.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/print_versions.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_api.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_api.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_bitshuffle_leftovers.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_blosc1_compat.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_blosc1_compat.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_change_nthreads_append.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_change_nthreads_append.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_common.h` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_common.h`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_compress_roundtrip.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_compress_roundtrip.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_compress_roundtrip.csv` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_compress_roundtrip.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_compressor.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_compressor.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_contexts.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_contexts.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_copy.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_copy.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_delete_chunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_delete_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_delta.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_delta_schunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_delta_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_dict_schunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_dict_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_empty_buffer.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_empty_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_fill_special.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_fill_special.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_filters.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_filters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_frame.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_frame_get_offsets.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_frame_get_offsets.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_frame_offset.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_frame_offset.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_get_slice_buffer.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_get_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_get_slice_nchunks.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_get_slice_nchunks.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_getitem.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_getitem.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_getitem.csv` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_getitem.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_getitem_delta.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_getitem_delta.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_insert_chunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_insert_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_lazychunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_lazychunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_lazychunk_memcpyed.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_maskout.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_maskout.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_maxout.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_maxout.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_noinit.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_noinit.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_nolock.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_nolock.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_nthreads.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_nthreads.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_postfilter.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_postfilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_prefilter.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_prefilter.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_reorder_offsets.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_reorder_offsets.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_schunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_schunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_schunk_frame.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_schunk_frame.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_schunk_header.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_schunk_header.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_set_slice_buffer.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_set_slice_buffer.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_sframe.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_sframe.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_sframe_lazychunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_sframe_lazychunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_altivec.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_avx2.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_generic.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_neon.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_shuffle_roundtrip_sse2.csv`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_small_chunks.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_small_chunks.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_udio.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_udio.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_update_chunk.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_update_chunk.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_urcodecs.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_urcodecs.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_urfilters.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_urfilters.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/c-blosc2/tests/test_zero_runlen.c` & `blosc2-2.6.1/blosc2/c-blosc2/tests/test_zero_runlen.c`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/core.py` & `blosc2-2.6.1/blosc2/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,16 +390,14 @@
     >>> np.array_equal(a, a2)
     True
     """
     pickled_array = decompress(packed_array)
     if kwargs:
         arr = pickle.loads(pickled_array, **kwargs)
         if all(isinstance(x, bytes) for x in arr.tolist()):
-            import numpy as np
-
             arr = np.array([x.decode("utf-8") for x in arr.tolist()])
     else:
         arr = pickle.loads(pickled_array)
 
     return arr
 
 
@@ -614,16 +612,14 @@
     ...
 
     See also
     --------
     :func:`~blosc2.unpack_tensor`
     :func:`~blosc2.save_tensor`
     """
-    import numpy as np
-
     arr = np.asarray(tensor)
 
     schunk = blosc2.SChunk(chunksize=chunksize, data=arr, **kwargs)
 
     # Guess the kind of tensor / array
     repr_tensor = repr(tensor)
     if "tensor" in repr_tensor:
@@ -643,16 +639,14 @@
     if schunk.urlpath is None:
         return schunk.to_cframe()
     else:
         return os.stat(schunk.urlpath).st_size
 
 
 def _unpack_tensor(schunk):
-    import numpy as np
-
     kind, shape, dtype = schunk.vlmeta["__pack_tensor__"]
     out = np.empty(shape, dtype=dtype)
     schunk.get_slice(out=out)
 
     if kind == "torch":
         import torch
```

### Comparing `blosc2-2.6.0/blosc2/info.py` & `blosc2-2.6.1/blosc2/info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/lazyexpr.py` & `blosc2-2.6.1/blosc2/lazyexpr.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/ndarray.py` & `blosc2-2.6.1/blosc2/ndarray.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2/schunk.py` & `blosc2-2.6.1/blosc2/schunk.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/blosc2.egg-info/PKG-INFO` & `blosc2-2.6.1/blosc2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blosc2
-Version: 2.6.0
+Version: 2.6.1
 Summary: Python wrapper for the C-Blosc2 library
 Author-email: Blosc Development Team <blosc@blosc.org>
 Maintainer-email: Blosc Development Team <blosc@blosc.org>
 License: BSD-3-Clause
 Project-URL: homepage, https://github.com/Blosc/python-blosc2
 Project-URL: documentation, https://www.blosc.org/python-blosc2/python-blosc2.html
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `blosc2-2.6.0/blosc2.egg-info/SOURCES.txt` & `blosc2-2.6.1/blosc2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/_static/blosc-logo_128.png` & `blosc2-2.6.1/doc/_static/blosc-logo_128.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/_static/blosc-logo_256.png` & `blosc2-2.6.1/doc/_static/blosc-logo_256.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/_static/css/custom.css` & `blosc2-2.6.1/doc/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/conf.py` & `blosc2-2.6.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/installation.rst` & `blosc2-2.6.1/doc/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/overview.rst` & `blosc2-2.6.1/doc/getting_started/overview.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/00.schunk-basics.ipynb` & `blosc2-2.6.1/doc/getting_started/tutorials/00.schunk-basics.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/01.schunk-slicing_and_beyond.ipynb` & `blosc2-2.6.1/doc/getting_started/tutorials/01.schunk-slicing_and_beyond.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/02.ndarray-basics.ipynb` & `blosc2-2.6.1/doc/getting_started/tutorials/02.ndarray-basics.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/10.ucodecs-ufilters.ipynb` & `blosc2-2.6.1/doc/getting_started/tutorials/10.ucodecs-ufilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/11.prefilters.ipynb` & `blosc2-2.6.1/doc/getting_started/tutorials/11.prefilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/12.postfilters.ipynb` & `blosc2-2.6.1/doc/getting_started/tutorials/12.postfilters.ipynb`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/blosc2-pipeline.png` & `blosc2-2.6.1/doc/getting_started/tutorials/images/blosc2-pipeline.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/blosc2-pipeline.svg` & `blosc2-2.6.1/doc/getting_started/tutorials/images/blosc2-pipeline.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/backward.png` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/backward.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/backward.svg` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/backward.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/decoder.png` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/decoder.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/decoder.svg` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/decoder.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.png` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.svg` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/decoder2.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/encoder.png` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/encoder.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/encoder.svg` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/encoder.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.png` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.svg` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/encoder2.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/forward.png` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/forward.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/getting_started/tutorials/images/ucodecs-filters/forward.svg` & `blosc2-2.6.1/doc/getting_started/tutorials/images/ucodecs-filters/forward.svg`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/python-blosc2.rst` & `blosc2-2.6.1/doc/python-blosc2.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/meta.rst` & `blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/meta.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/reference/autofiles/schunk/attributes/vlmeta.rst` & `blosc2-2.6.1/doc/reference/autofiles/schunk/attributes/vlmeta.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/reference/ndarray_api.rst` & `blosc2-2.6.1/doc/reference/ndarray_api.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/reference/schunk_api.rst` & `blosc2-2.6.1/doc/reference/schunk_api.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/doc/reference/top_level.rst` & `blosc2-2.6.1/doc/reference/top_level.rst`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/btune.py` & `blosc2-2.6.1/examples/btune.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/compress2_decompress2.py` & `blosc2-2.6.1/examples/compress2_decompress2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/compress_decompress.py` & `blosc2-2.6.1/examples/compress_decompress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/filler.py` & `blosc2-2.6.1/examples/filler.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/asarray_.py` & `blosc2-2.6.1/examples/ndarray/asarray_.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/buffer.py` & `blosc2-2.6.1/examples/ndarray/buffer.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/bytedelta_filter.py` & `blosc2-2.6.1/examples/ndarray/bytedelta_filter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/copy_.py` & `blosc2-2.6.1/examples/ndarray/copy_.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/empty_.py` & `blosc2-2.6.1/examples/ndarray/empty_.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/eval_expr.py` & `blosc2-2.6.1/examples/ndarray/eval_expr.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/formats.py` & `blosc2-2.6.1/examples/ndarray/formats.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/getitem.py` & `blosc2-2.6.1/examples/ndarray/getitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/iterchunks_info.py` & `blosc2-2.6.1/examples/ndarray/iterchunks_info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/meta.py` & `blosc2-2.6.1/examples/ndarray/meta.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/ndarray_copy.py` & `blosc2-2.6.1/examples/ndarray/ndarray_copy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/ndmean.py` & `blosc2-2.6.1/examples/ndarray/ndmean.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/persistency.py` & `blosc2-2.6.1/examples/ndarray/persistency.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/resize_.py` & `blosc2-2.6.1/examples/ndarray/resize_.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/work_with_numpy.py` & `blosc2-2.6.1/examples/ndarray/work_with_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ndarray/zfp_codec.py` & `blosc2-2.6.1/examples/ndarray/zfp_codec.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/pack_array.py` & `blosc2-2.6.1/examples/pack_array.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/pack_tensor.py` & `blosc2-2.6.1/examples/pack_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/postfilter1.py` & `blosc2-2.6.1/examples/postfilter1.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/postfilter2.py` & `blosc2-2.6.1/examples/postfilter2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/postfilter3.py` & `blosc2-2.6.1/examples/postfilter3.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/prefilter.py` & `blosc2-2.6.1/examples/prefilter.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/save_tensor.py` & `blosc2-2.6.1/examples/save_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/schunk.py` & `blosc2-2.6.1/examples/schunk.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/schunk_roundtrip.py` & `blosc2-2.6.1/examples/schunk_roundtrip.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ucodecs.py` & `blosc2-2.6.1/examples/ucodecs.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/ufilters.py` & `blosc2-2.6.1/examples/ufilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/examples/vlmeta.py` & `blosc2-2.6.1/examples/vlmeta.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/guix.scm` & `blosc2-2.6.1/guix.scm`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/images/Complete-Write-Read-B2ND.png` & `blosc2-2.6.1/images/Complete-Write-Read-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/images/M1-i386-vs-arm64-pack.png` & `blosc2-2.6.1/images/M1-i386-vs-arm64-pack.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/images/M1-i386-vs-arm64-unpack.png` & `blosc2-2.6.1/images/M1-i386-vs-arm64-unpack.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/images/Read-Partial-Slices-B2ND.png` & `blosc2-2.6.1/images/Read-Partial-Slices-B2ND.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/images/b2nd-2level-parts.png` & `blosc2-2.6.1/images/b2nd-2level-parts.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/images/linspace-compress.png` & `blosc2-2.6.1/images/linspace-compress.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/images/linspace-decompress.png` & `blosc2-2.6.1/images/linspace-decompress.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/images/pack-array-cratios.png` & `blosc2-2.6.1/images/pack-array-cratios.png`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/pyproject.toml` & `blosc2-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/setup.py` & `blosc2-2.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_auto_parts.py` & `blosc2-2.6.1/tests/ndarray/test_auto_parts.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_buffer.py` & `blosc2-2.6.1/tests/ndarray/test_buffer.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_copy.py` & `blosc2-2.6.1/tests/ndarray/test_copy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_empty.py` & `blosc2-2.6.1/tests/ndarray/test_empty.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_full.py` & `blosc2-2.6.1/tests/ndarray/test_full.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_get_slice_nchunks.py` & `blosc2-2.6.1/tests/ndarray/test_get_slice_nchunks.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_getitem.py` & `blosc2-2.6.1/tests/ndarray/test_getitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_iterchunks_info.py` & `blosc2-2.6.1/tests/ndarray/test_iterchunks_info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_lazyexpr.py` & `blosc2-2.6.1/tests/ndarray/test_lazyexpr.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_lossy.py` & `blosc2-2.6.1/tests/ndarray/test_lossy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_metalayers.py` & `blosc2-2.6.1/tests/ndarray/test_metalayers.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_mode.py` & `blosc2-2.6.1/tests/ndarray/test_mode.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_ndarray.py` & `blosc2-2.6.1/tests/ndarray/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_numpy.py` & `blosc2-2.6.1/tests/ndarray/test_numpy.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_persistency.py` & `blosc2-2.6.1/tests/ndarray/test_persistency.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_resize.py` & `blosc2-2.6.1/tests/ndarray/test_resize.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_setitem.py` & `blosc2-2.6.1/tests/ndarray/test_setitem.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_slice.py` & `blosc2-2.6.1/tests/ndarray/test_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_squeeze.py` & `blosc2-2.6.1/tests/ndarray/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_struct_dtype.py` & `blosc2-2.6.1/tests/ndarray/test_struct_dtype.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/ndarray/test_zeros.py` & `blosc2-2.6.1/tests/ndarray/test_zeros.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_bytes_array.py` & `blosc2-2.6.1/tests/test_bytes_array.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_comp_info.py` & `blosc2-2.6.1/tests/test_comp_info.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_compress2.py` & `blosc2-2.6.1/tests/test_compress2.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_compression_parameters.py` & `blosc2-2.6.1/tests/test_compression_parameters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_compressors.py` & `blosc2-2.6.1/tests/test_compressors.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_decompress.py` & `blosc2-2.6.1/tests/test_decompress.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_iterchunks.py` & `blosc2-2.6.1/tests/test_iterchunks.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_open.py` & `blosc2-2.6.1/tests/test_open.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_pathlib.py` & `blosc2-2.6.1/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_postfilters.py` & `blosc2-2.6.1/tests/test_postfilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_prefilters.py` & `blosc2-2.6.1/tests/test_prefilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_python_blosc.py` & `blosc2-2.6.1/tests/test_python_blosc.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_schunk.py` & `blosc2-2.6.1/tests/test_schunk.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_schunk_constructor.py` & `blosc2-2.6.1/tests/test_schunk_constructor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_schunk_delete.py` & `blosc2-2.6.1/tests/test_schunk_delete.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_schunk_get_slice.py` & `blosc2-2.6.1/tests/test_schunk_get_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_schunk_get_slice_nchunks.py` & `blosc2-2.6.1/tests/test_schunk_get_slice_nchunks.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_schunk_insert.py` & `blosc2-2.6.1/tests/test_schunk_insert.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_schunk_set_slice.py` & `blosc2-2.6.1/tests/test_schunk_set_slice.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_schunk_update.py` & `blosc2-2.6.1/tests/test_schunk_update.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_tensor.py` & `blosc2-2.6.1/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_ucodecs.py` & `blosc2-2.6.1/tests/test_ucodecs.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_ufilters.py` & `blosc2-2.6.1/tests/test_ufilters.py`

 * *Files identical despite different names*

### Comparing `blosc2-2.6.0/tests/test_vlmeta.py` & `blosc2-2.6.1/tests/test_vlmeta.py`

 * *Files identical despite different names*

