# Comparing `tmp/mmcif-0.86.0.tar.gz` & `tmp/mmcif-0.87.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcif-0.86.0.tar", last modified: Mon Feb 26 17:28:07 2024, max compression
+gzip compressed data, was "mmcif-0.87.0.tar", last modified: Sat Apr  6 20:36:33 2024, max compression
```

## Comparing `mmcif-0.86.0.tar` & `mmcif-0.87.0.tar`

### file list

```diff
@@ -1,730 +1,730 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.655418 mmcif-0.86.0/
--rw-r--r--   0 vsts      (1001) docker     (127)    12721 2024-02-26 17:24:21.000000 mmcif-0.86.0/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     7501 2024-02-26 17:24:21.000000 mmcif-0.86.0/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-02-26 17:24:21.000000 mmcif-0.86.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      441 2024-02-26 17:24:21.000000 mmcif-0.86.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     3337 2024-02-26 17:28:07.655418 mmcif-0.86.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2075 2024-02-26 17:24:21.000000 mmcif-0.86.0/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.523408 mmcif-0.86.0/mmcif/
--rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.527408 mmcif-0.86.0/mmcif/api/
--rw-r--r--   0 vsts      (1001) docker     (127)    21941 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/DataCategory.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17192 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/DataCategoryBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13272 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/DataCategoryFormatted.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11542 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/DataCategoryTyped.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10128 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/DictMethodRunner.py
--rw-r--r--   0 vsts      (1001) docker     (127)    85436 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/DictionaryApi.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24778 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/DictionaryInclude.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3844 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/Method.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5017 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/MethodUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10640 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/PdbxContainers.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.527408 mmcif-0.86.0/mmcif/core/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/core/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.527408 mmcif-0.86.0/mmcif/io/
--rw-r--r--   0 vsts      (1001) docker     (127)    19069 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/BinaryCifReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28179 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/BinaryCifWriter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2922 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/BuildDictionaryExec.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1551 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/CifFile.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12835 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/IoAdapterBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20047 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/IoAdapterCore.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19111 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/IoAdapterPy.py
--rw-r--r--   0 vsts      (1001) docker     (127)      524 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/PdbxExceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18397 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/PdbxReader.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11640 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/PdbxWriter.py
--rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-02-26 17:24:21.000000 mmcif-0.86.0/mmcif/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.651417 mmcif-0.86.0/mmcif.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     3337 2024-02-26 17:28:07.000000 mmcif-0.86.0/mmcif.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    29562 2024-02-26 17:28:07.000000 mmcif-0.86.0/mmcif.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-26 17:28:07.000000 mmcif-0.86.0/mmcif.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-02-26 17:28:07.000000 mmcif-0.86.0/mmcif.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-26 17:24:43.000000 mmcif-0.86.0/mmcif.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      130 2024-02-26 17:28:07.000000 mmcif-0.86.0/mmcif.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-02-26 17:28:07.000000 mmcif-0.86.0/mmcif.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.511407 mmcif-0.86.0/modules/cc-regex/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.527408 mmcif-0.86.0/modules/cc-regex/include/
--rw-r--r--   0 vsts      (1001) docker     (127)      943 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/cclass.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2057 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/cname.h
--rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/debug.ih
--rw-r--r--   0 vsts      (1001) docker     (127)     1379 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/engine.ih
--rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/main.ih
--rw-r--r--   0 vsts      (1001) docker     (127)     2723 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/regcomp.ih
--rw-r--r--   0 vsts      (1001) docker     (127)      267 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/regerror.ih
--rw-r--r--   0 vsts      (1001) docker     (127)     1891 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/regex.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5365 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/regex2.h
--rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/include/utils.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.531409 mmcif-0.86.0/modules/cc-regex/src/
--rw-r--r--   0 vsts      (1001) docker     (127)     5092 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/debug.c
--rw-r--r--   0 vsts      (1001) docker     (127)    25587 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/engine.c
--rw-r--r--   0 vsts      (1001) docker     (127)    11193 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/main.c
--rw-r--r--   0 vsts      (1001) docker     (127)     1825 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/mkh
--rw-r--r--   0 vsts      (1001) docker     (127)    37342 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/regcomp.c
--rw-r--r--   0 vsts      (1001) docker     (127)     3212 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/regerror.c
--rw-r--r--   0 vsts      (1001) docker     (127)     4259 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/regexec.c
--rw-r--r--   0 vsts      (1001) docker     (127)      736 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/regfree.c
--rw-r--r--   0 vsts      (1001) docker     (127)     7061 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cc-regex/src/split.c
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/cpp-cif-file/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.531409 mmcif-0.86.0/modules/cpp-cif-file/include/
--rw-r--r--   0 vsts      (1001) docker     (127)     1746 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/include/CifDataInfo.h
--rw-r--r--   0 vsts      (1001) docker     (127)      688 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/include/CifExcept.h
--rw-r--r--   0 vsts      (1001) docker     (127)    23567 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/include/CifFile.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1945 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/include/CifParentChild.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5484 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/include/DicFile.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2782 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/include/ParentChild.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.531409 mmcif-0.86.0/modules/cpp-cif-file/src/
--rw-r--r--   0 vsts      (1001) docker     (127)     6274 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/src/CifDataInfo.C
--rw-r--r--   0 vsts      (1001) docker     (127)    36103 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/src/CifExcept.C
--rw-r--r--   0 vsts      (1001) docker     (127)    85654 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/src/CifFile.C
--rw-r--r--   0 vsts      (1001) docker     (127)    32221 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/src/CifParentChild.C
--rw-r--r--   0 vsts      (1001) docker     (127)    47643 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/src/DicFile.C
--rw-r--r--   0 vsts      (1001) docker     (127)    23231 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file/src/ParentChild.C
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.511407 mmcif-0.86.0/modules/cpp-cif-file-util/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.531409 mmcif-0.86.0/modules/cpp-cif-file-util/include/
--rw-r--r--   0 vsts      (1001) docker     (127)     3264 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file-util/include/CifCorrector.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2444 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file-util/include/CifFileUtil.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.531409 mmcif-0.86.0/modules/cpp-cif-file-util/src/
--rw-r--r--   0 vsts      (1001) docker     (127)    47136 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file-util/src/CifCorrector.C
--rw-r--r--   0 vsts      (1001) docker     (127)     4509 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-file-util/src/CifFileUtil.C
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/cpp-cif-parser/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.535409 mmcif-0.86.0/modules/cpp-cif-parser/include/
--rw-r--r--   0 vsts      (1001) docker     (127)     1518 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/CifFileReadDef.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6318 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/CifParserBase.h
--rw-r--r--   0 vsts      (1001) docker     (127)      898 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/CifParserInt.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1390 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/CifScannerBase.h
--rw-r--r--   0 vsts      (1001) docker     (127)      750 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/CifScannerInt.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6970 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/DICParserBase.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1032 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/DICParserInt.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1471 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/DICScannerBase.h
--rw-r--r--   0 vsts      (1001) docker     (127)      912 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/include/DICScannerInt.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.535409 mmcif-0.86.0/modules/cpp-cif-parser/src/
--rw-r--r--   0 vsts      (1001) docker     (127)     3768 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/CifFileReadDef.C
--rw-r--r--   0 vsts      (1001) docker     (127)     2206 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/CifParser.y
--rw-r--r--   0 vsts      (1001) docker     (127)    23419 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/CifParserBase.C
--rw-r--r--   0 vsts      (1001) docker     (127)     2475 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/CifScanner.l
--rw-r--r--   0 vsts      (1001) docker     (127)     9603 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/CifScannerBase.C
--rw-r--r--   0 vsts      (1001) docker     (127)     2376 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/DICParser.y
--rw-r--r--   0 vsts      (1001) docker     (127)    41071 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/DICParserBase.C
--rw-r--r--   0 vsts      (1001) docker     (127)     2985 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/DICScanner.l
--rw-r--r--   0 vsts      (1001) docker     (127)    10258 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-cif-parser/src/DICScannerBase.C
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/cpp-common/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.535409 mmcif-0.86.0/modules/cpp-common/include/
--rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/BlockIO.h
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2398 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/CifDefs.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6737 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/CifString.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2901 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/DataInfo.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3175 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/Exceptions.h
--rw-r--r--   0 vsts      (1001) docker     (127)      635 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/GenCont.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6109 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/GenString.h
--rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/RcsbFile.h
--rw-r--r--   0 vsts      (1001) docker     (127)      335 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/RcsbPlatform.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5664 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/Serializer.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/mapped_ptr_vector.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1543 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/mapped_vector.h
--rw-r--r--   0 vsts      (1001) docker     (127)      210 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/rcsb_math.h
--rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/include/rcsb_types.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.539409 mmcif-0.86.0/modules/cpp-common/src/
--rw-r--r--   0 vsts      (1001) docker     (127)     1240 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/BlockIO.C
--rw-r--r--   0 vsts      (1001) docker     (127)    10498 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/CifString.C
--rw-r--r--   0 vsts      (1001) docker     (127)     9606 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/DataInfo.C
--rw-r--r--   0 vsts      (1001) docker     (127)     2314 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/Exceptions.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1085 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/GenCont.C
--rw-r--r--   0 vsts      (1001) docker     (127)    14827 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/GenString.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1236 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/RcsbFile.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)      356 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/RcsbPlatform.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)    40038 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/Serializer.C
--rw-r--r--   0 vsts      (1001) docker     (127)    10675 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/mapped_ptr_vector.C
--rw-r--r--   0 vsts      (1001) docker     (127)     5759 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-common/src/mapped_vector.C
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.539409 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/
--rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifDataInfo.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    12223 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFile.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     3130 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileReadDef.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     3592 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileUtil.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     3791 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDicFile.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     2003 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDictDataInfo.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    14081 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapISTable.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     6137 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapTableFile.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      690 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapmmciflib.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wraprcsb_types.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/cpp-dict-obj-file/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.539409 mmcif-0.86.0/modules/cpp-dict-obj-file/include/
--rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictDataInfo.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7726 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictObjCont.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4564 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictObjContInfo.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5597 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictObjFile.h
--rw-r--r--   0 vsts      (1001) docker     (127)      876 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictParentChild.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.539409 mmcif-0.86.0/modules/cpp-dict-obj-file/src/
--rw-r--r--   0 vsts      (1001) docker     (127)     3975 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictDataInfo.C
--rw-r--r--   0 vsts      (1001) docker     (127)    19477 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjCont.C
--rw-r--r--   0 vsts      (1001) docker     (127)    12717 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjContInfo.C
--rw-r--r--   0 vsts      (1001) docker     (127)     6349 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjFile.C
--rw-r--r--   0 vsts      (1001) docker     (127)     1979 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjFileCreator.C
--rw-r--r--   0 vsts      (1001) docker     (127)      741 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjFileReader.C
--rw-r--r--   0 vsts      (1001) docker     (127)    13027 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjFileSelectiveReader.C
--rw-r--r--   0 vsts      (1001) docker     (127)     8311 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictParentChild.C
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/cpp-mmciflib-test/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.547410 mmcif-0.86.0/modules/cpp-mmciflib-test/src/
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1333 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/BigCifTest.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     5347 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/CifDiff.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     3115 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/CifInfo.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2788 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/CifReader.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2673 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/DataChecking.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1929 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/DictInfo.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1894 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest1.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1073 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest10.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2061 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest11.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2406 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest12.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)      539 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest13.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     3930 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest14.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     3211 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest2.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1385 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest3.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2410 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest4.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1417 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest5.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1174 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest6.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1863 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest7.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)      406 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest8.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)      611 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest9.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1316 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/GroupTableTest2.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)      582 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/SdbReader.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1519 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/checkdictionary.C
--rwxr-xr-x   0 vsts      (1001) docker     (127)      655 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/cpp-mmciflib-test/src/selective-reading.C
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/cpp-tables/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.547410 mmcif-0.86.0/modules/cpp-tables/include/
--rw-r--r--   0 vsts      (1001) docker     (127)    52000 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/include/ISTable.h
--rw-r--r--   0 vsts      (1001) docker     (127)    44528 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/include/ITTable.h
--rw-r--r--   0 vsts      (1001) docker     (127)    20019 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/include/TTable.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1270 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/include/TableError.h
--rw-r--r--   0 vsts      (1001) docker     (127)    21422 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/include/TableFile.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.547410 mmcif-0.86.0/modules/cpp-tables/src/
--rw-r--r--   0 vsts      (1001) docker     (127)    77385 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/src/ISTable.C
--rw-r--r--   0 vsts      (1001) docker     (127)    43788 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/src/ITTable.C
--rw-r--r--   0 vsts      (1001) docker     (127)    15437 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/src/TTable.C
--rw-r--r--   0 vsts      (1001) docker     (127)    26031 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/cpp-tables/src/TableFile.C
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.551410 mmcif-0.86.0/modules/pybind11/
--rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.appveyor.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.clang-format
--rw-r--r--   0 vsts      (1001) docker     (127)     2605 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.clang-tidy
--rw-r--r--   0 vsts      (1001) docker     (127)     2196 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.cmake-format.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)     1308 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.codespell-ignore-lines
--rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.git
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.gitattributes
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.551410 mmcif-0.86.0/modules/pybind11/.github/
--rw-r--r--   0 vsts      (1001) docker     (127)      182 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/CODEOWNERS
--rw-r--r--   0 vsts      (1001) docker     (127)    15271 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/CONTRIBUTING.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.551410 mmcif-0.86.0/modules/pybind11/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 vsts      (1001) docker     (127)     2016 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      328 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/dependabot.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/labeler.yml
--rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/labeler_merged.yml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.551410 mmcif-0.86.0/modules/pybind11/.github/matchers/
--rw-r--r--   0 vsts      (1001) docker     (127)      668 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/matchers/pylint.json
--rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.555410 mmcif-0.86.0/modules/pybind11/.github/workflows/
--rw-r--r--   0 vsts      (1001) docker     (127)    28486 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/workflows/ci.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2095 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/workflows/configure.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/workflows/format.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/workflows/labeler.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2558 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/workflows/pip.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2837 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.github/workflows/upstream.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      487 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (127)     4331 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.pre-commit-config.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    11911 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     7686 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.555410 mmcif-0.86.0/modules/pybind11/docs/
--rw-r--r--   0 vsts      (1001) docker     (127)      607 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/Doxyfile
--rw-r--r--   0 vsts      (1001) docker     (127)     7417 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/Makefile
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/pybind11/docs/_static/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.555410 mmcif-0.86.0/modules/pybind11/docs/_static/css/
--rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/_static/css/custom.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.559411 mmcif-0.86.0/modules/pybind11/docs/advanced/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.559411 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/
--rw-r--r--   0 vsts      (1001) docker     (127)     3937 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/chrono.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3429 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/custom.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    14283 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/eigen.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3889 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/functional.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     1556 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    12371 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/overview.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     9586 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/stl.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     8863 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/cast/strings.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    47796 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/classes.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/embedding.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    17772 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/exceptions.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    26729 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/functions.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    13634 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/misc.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.559411 mmcif-0.86.0/modules/pybind11/docs/advanced/pycpp/
--rw-r--r--   0 vsts      (1001) docker     (127)      278 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/pycpp/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    17161 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     9030 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/pycpp/object.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     5710 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     6377 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     9240 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/basics.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     2856 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/benchmark.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3168 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/benchmark.rst
--rw-r--r--   0 vsts      (1001) docker     (127)   111105 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/changelog.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    16380 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/classes.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.559411 mmcif-0.86.0/modules/pybind11/docs/cmake/
--rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/cmake/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    25777 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/compiling.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    11559 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13177 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/faq.rst
--rw-r--r--   0 vsts      (1001) docker     (127)      613 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3277 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/installing.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3079 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/limitations.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    61034 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/pybind11-logo.png
--rw-r--r--   0 vsts      (1001) docker     (127)    44653 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 vsts      (1001) docker     (127)    87708 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 vsts      (1001) docker     (127)    41121 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 vsts      (1001) docker     (127)    85853 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     2647 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/reference.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     4414 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/release.rst
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    23489 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/docs/upgrade.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.515408 mmcif-0.86.0/modules/pybind11/include/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.563411 mmcif-0.86.0/modules/pybind11/include/pybind11/
--rw-r--r--   0 vsts      (1001) docker     (127)    23979 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/attr.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7069 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 vsts      (1001) docker     (127)    65638 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/cast.h
--rw-r--r--   0 vsts      (1001) docker     (127)     8458 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/common.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2096 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.567411 mmcif-0.86.0/modules/pybind11/include/pybind11/detail/
--rw-r--r--   0 vsts      (1001) docker     (127)    28251 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 vsts      (1001) docker     (127)    50369 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5491 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 vsts      (1001) docker     (127)    17981 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 vsts      (1001) docker     (127)    25057 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 vsts      (1001) docker     (127)    42266 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1625 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 vsts      (1001) docker     (127)    32147 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 vsts      (1001) docker     (127)    11792 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/embed.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4731 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/eval.h
--rw-r--r--   0 vsts      (1001) docker     (127)     4695 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/functional.h
--rw-r--r--   0 vsts      (1001) docker     (127)     8262 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/gil.h
--rw-r--r--   0 vsts      (1001) docker     (127)     8862 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 vsts      (1001) docker     (127)    79524 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 vsts      (1001) docker     (127)     9103 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/operators.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2181 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/options.h
--rw-r--r--   0 vsts      (1001) docker     (127)   125761 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 vsts      (1001) docker     (127)    93848 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.567411 mmcif-0.86.0/modules/pybind11/include/pybind11/stl/
--rw-r--r--   0 vsts      (1001) docker     (127)     4185 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 vsts      (1001) docker     (127)    15337 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/stl.h
--rw-r--r--   0 vsts      (1001) docker     (127)    27013 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/include/pybind11/stl_bind.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/noxfile.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.567411 mmcif-0.86.0/modules/pybind11/pybind11/
--rw-r--r--   0 vsts      (1001) docker     (127)      414 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/pybind11/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1360 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/pybind11/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      228 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/pybind11/_version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1226 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/pybind11/commands.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/pybind11/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)    17609 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/pybind11/setup_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1261 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1622 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     4877 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)    20608 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     5006 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11736 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/constructor_stats.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3578 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1776 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/cross_module_interleaved_error_already_set.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/env.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/extra_python_package/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/extra_python_package/pytest.ini
--rw-r--r--   0 vsts      (1001) docker     (127)     8142 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/extra_setuptools/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 vsts      (1001) docker     (127)     4153 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2847 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/local_bindings.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5743 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/object.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6264 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4517 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/pybind11_tests.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     2685 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 vsts      (1001) docker     (127)      768 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/pytest.ini
--rw-r--r--   0 vsts      (1001) docker     (127)      600 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_async.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      534 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_async.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_buffers.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4841 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_buffers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15990 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_builtin_casters.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    17245 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_builtin_casters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4118 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_call_policies.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     6549 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_call_policies.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9243 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_callbacks.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     5906 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_callbacks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3370 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_chrono.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     5695 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_chrono.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_class.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    14575 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_class.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/
--rw-r--r--   0 vsts      (1001) docker     (127)     2639 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      673 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 vsts      (1001) docker     (127)     1171 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 vsts      (1001) docker     (127)     1293 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 vsts      (1001) docker     (127)     1685 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 vsts      (1001) docker     (127)     1163 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.591413 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 vsts      (1001) docker     (127)     1368 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      198 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/test.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3831 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_const_name.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      589 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_const_name.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5853 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_constants_and_functions.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_constants_and_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10886 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_copy_move.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4796 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_copy_move.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7280 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_custom_type_casters.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     3980 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_custom_type_casters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1259 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_custom_type_setup.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_custom_type_setup.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2816 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_docstring_options.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1606 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_docstring_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19409 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_eigen.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    28860 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_eigen.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.595413 mmcif-0.86.0/modules/pybind11/tests/test_embed/
--rw-r--r--   0 vsts      (1001) docker     (127)     1798 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     1338 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_embed/catch.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_embed/external_module.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    14260 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_embed/test_interpreter.py
--rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_embed/test_trampoline.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5722 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_enum.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     8903 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_enum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3168 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_eval.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_eval.py
--rw-r--r--   0 vsts      (1001) docker     (127)      119 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_eval_call.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11904 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_exceptions.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      399 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_exceptions.h
--rw-r--r--   0 vsts      (1001) docker     (127)    12702 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18155 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_factory_constructors.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    16519 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_factory_constructors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5311 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_gil_scoped.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     8565 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_gil_scoped.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3960 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_iostream.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     7286 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_iostream.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9535 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    13757 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4401 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_local_bindings.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     8049 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_local_bindings.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21388 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    18134 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_methods_and_attributes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4121 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_modules.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4191 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_modules.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12305 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    11874 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_multiple_inheritance.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19800 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_numpy_array.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    20228 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_numpy_array.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21114 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    14394 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_numpy_dtypes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4487 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     9686 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_numpy_vectorize.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2777 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_opaque_types.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1847 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_opaque_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9463 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_operator_overloading.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4333 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_operator_overloading.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6719 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_pickling.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     2720 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_pickling.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30650 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_pytypes.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    23467 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_pytypes.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21153 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     8021 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_sequences_and_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18898 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_smart_ptr.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     9530 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_smart_ptr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21587 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_stl.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    12235 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_stl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4622 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_stl_binders.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     7912 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_stl_binders.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4617 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      741 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1855 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_thread.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_thread.py
--rw-r--r--   0 vsts      (1001) docker     (127)      603 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_union.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      148 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_union.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22983 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_virtual_functions.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    12919 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/test_virtual_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3226 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 vsts      (1001) docker     (127)     2657 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tests/valgrind-python.supp
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.599413 mmcif-0.86.0/modules/pybind11/tools/
--rw-r--r--   0 vsts      (1001) docker     (127)     2350 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)     3105 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)    11103 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)      817 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/JoinPaths.cmake
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1423 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/check-style.sh
--rw-r--r--   0 vsts      (1001) docker     (127)      952 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1040 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/codespell_ignore_lines_from_errors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1031 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/libsize.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1282 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/make_changelog.py
--rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/pybind11.pc.in
--rw-r--r--   0 vsts      (1001) docker     (127)    13487 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)     6930 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (127)     8955 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)     8359 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1965 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/setup_global.py.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1139 2024-02-26 17:24:26.000000 mmcif-0.86.0/modules/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.599413 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.appveyor.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.clang-format
--rw-r--r--   0 vsts      (1001) docker     (127)      242 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.clang-tidy
--rw-r--r--   0 vsts      (1001) docker     (127)     2196 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.cmake-format.yaml
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.603414 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/
--rw-r--r--   0 vsts      (1001) docker     (127)    14415 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.603414 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 vsts      (1001) docker     (127)     1270 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 vsts      (1001) docker     (127)      172 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      669 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 vsts      (1001) docker     (127)      559 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/dependabot.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/labeler.yml
--rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/labeler_merged.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      404 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/pull_request_template.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.603414 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/
--rw-r--r--   0 vsts      (1001) docker     (127)    24508 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/ci.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2117 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/configure.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/format.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/labeler.yml
--rw-r--r--   0 vsts      (1001) docker     (127)     2497 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/pip.yml
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (127)     2460 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.pre-commit-config.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (127)    10438 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     8064 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.607414 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/
--rw-r--r--   0 vsts      (1001) docker     (127)      705 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/Doxyfile
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.611414 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/_static/
--rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/_static/theme_overrides.css
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.611414 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.611414 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/
--rw-r--r--   0 vsts      (1001) docker     (127)     3937 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/chrono.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3398 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/custom.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    14288 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/eigen.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3889 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/functional.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     1556 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    11680 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/overview.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     9703 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/stl.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     9372 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/strings.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    45878 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/classes.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     8420 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/embedding.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    14171 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/exceptions.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    25082 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/functions.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    12444 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/misc.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.615415 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/
--rw-r--r--   0 vsts      (1001) docker     (127)      278 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    16538 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/numpy.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     7878 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/object.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/utilities.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     6366 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/smart_ptrs.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     9369 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/basics.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     2974 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/benchmark.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3168 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/benchmark.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    74047 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/changelog.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    16122 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/classes.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.615415 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/cmake/
--rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/cmake/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    25511 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/compiling.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    12095 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14593 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/faq.rst
--rw-r--r--   0 vsts      (1001) docker     (127)      613 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3277 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/installing.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     3062 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/limitations.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    58510 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11-logo.png
--rw-r--r--   0 vsts      (1001) docker     (127)    44653 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.png
--rw-r--r--   0 vsts      (1001) docker     (127)    87708 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.svg
--rw-r--r--   0 vsts      (1001) docker     (127)    41121 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.png
--rw-r--r--   0 vsts      (1001) docker     (127)    85853 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.svg
--rw-r--r--   0 vsts      (1001) docker     (127)     2511 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/reference.rst
--rw-r--r--   0 vsts      (1001) docker     (127)     4028 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/release.rst
--rw-r--r--   0 vsts      (1001) docker     (127)      168 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    23059 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/upgrade.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.519408 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.619415 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/
--rw-r--r--   0 vsts      (1001) docker     (127)    21412 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/attr.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6118 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/buffer_info.h
--rw-r--r--   0 vsts      (1001) docker     (127)    57522 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/cast.h
--rw-r--r--   0 vsts      (1001) docker     (127)     8516 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/chrono.h
--rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/common.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2037 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/complex.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.619415 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/
--rw-r--r--   0 vsts      (1001) docker     (127)    27823 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/class.h
--rw-r--r--   0 vsts      (1001) docker     (127)    42083 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/common.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3602 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/descr.h
--rw-r--r--   0 vsts      (1001) docker     (127)    16397 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/init.h
--rw-r--r--   0 vsts      (1001) docker     (127)    16375 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/internals.h
--rw-r--r--   0 vsts      (1001) docker     (127)    40663 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1486 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/typeid.h
--rw-r--r--   0 vsts      (1001) docker     (127)    29086 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/eigen.h
--rw-r--r--   0 vsts      (1001) docker     (127)     7843 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/embed.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5079 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/eval.h
--rw-r--r--   0 vsts      (1001) docker     (127)     3709 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/functional.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6532 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/gil.h
--rw-r--r--   0 vsts      (1001) docker     (127)     6084 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/iostream.h
--rw-r--r--   0 vsts      (1001) docker     (127)    69820 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/numpy.h
--rw-r--r--   0 vsts      (1001) docker     (127)     9085 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/operators.h
--rw-r--r--   0 vsts      (1001) docker     (127)     2049 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/options.h
--rw-r--r--   0 vsts      (1001) docker     (127)   105679 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/pybind11.h
--rw-r--r--   0 vsts      (1001) docker     (127)    67597 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/pytypes.h
--rw-r--r--   0 vsts      (1001) docker     (127)    14162 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/stl.h
--rw-r--r--   0 vsts      (1001) docker     (127)    23912 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/stl_bind.h
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.623415 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/
--rw-r--r--   0 vsts      (1001) docker     (127)      217 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1158 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      207 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/_version.py
--rw-r--r--   0 vsts      (1001) docker     (127)      137 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/_version.pyi
--rw-r--r--   0 vsts      (1001) docker     (127)      663 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/commands.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)    15167 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1899 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.pyi
--rw-r--r--   0 vsts      (1001) docker     (127)      118 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     2185 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     3499 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.643417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)    15372 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     4841 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11157 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/constructor_stats.h
--rw-r--r--   0 vsts      (1001) docker     (127)     1819 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/cross_module_gil_utils.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1022 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/env.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.643417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/extra_python_package/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/extra_python_package/pytest.ini
--rw-r--r--   0 vsts      (1001) docker     (127)     7154 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/extra_python_package/test_files.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.643417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/pytest.ini
--rw-r--r--   0 vsts      (1001) docker     (127)     2581 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/test_setuphelper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2144 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/local_bindings.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5389 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/object.h
--rw-r--r--   0 vsts      (1001) docker     (127)     5285 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/pybind11_cross_module_tests.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     3647 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     2733 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.h
--rw-r--r--   0 vsts      (1001) docker     (127)      693 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/pytest.ini
--rw-r--r--   0 vsts      (1001) docker     (127)      843 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      864 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_async.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_async.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8048 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_buffers.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4946 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_buffers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13475 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    17617 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3702 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_call_policies.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     5728 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_call_policies.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6754 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_callbacks.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     5447 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_callbacks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_chrono.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     5726 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_chrono.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21548 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_class.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    14273 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_class.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.647417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/
--rw-r--r--   0 vsts      (1001) docker     (127)     2639 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      656 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/embed.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.647417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 vsts      (1001) docker     (127)     1175 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.647417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/
--rw-r--r--   0 vsts      (1001) docker     (127)     1259 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.647417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/
--rw-r--r--   0 vsts      (1001) docker     (127)     1653 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/main.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.647417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 vsts      (1001) docker     (127)     1357 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.647417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 vsts      (1001) docker     (127)     1126 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.647417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/test.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5346 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1522 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9629 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_copy_move.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4645 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_copy_move.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5513 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4015 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2514 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1630 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16867 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eigen.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    28282 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eigen.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.647417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/
--rw-r--r--   0 vsts      (1001) docker     (127)     1758 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      637 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/catch.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      554 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/external_module.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    10209 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2610 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_enum.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     7694 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_enum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2628 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eval.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      768 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eval.py
--rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eval_call.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7862 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_exceptions.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     6753 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16562 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    16731 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1760 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     3128 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3381 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_iostream.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     5799 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_iostream.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6489 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    10048 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4333 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     8102 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19446 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    17310 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3742 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_modules.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     2841 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_modules.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9148 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     9495 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17781 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    18647 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18421 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    13614 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3832 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     9709 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2731 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1906 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8431 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4945 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_pickling.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     1191 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_pickling.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14656 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_pytypes.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    16590 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_pytypes.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13120 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     5966 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18187 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     9620 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12793 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_stl.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     8557 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_stl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4403 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)     7182 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4458 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      765 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.py
--rw-r--r--   0 vsts      (1001) docker     (127)      603 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_union.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)      172 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_union.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18454 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.cpp
--rw-r--r--   0 vsts      (1001) docker     (127)    11646 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3238 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/valgrind-numpy-scipy.supp
--rw-r--r--   0 vsts      (1001) docker     (127)     2657 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/valgrind-python.supp
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-26 17:28:07.651417 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/
--rw-r--r--   0 vsts      (1001) docker     (127)     2295 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/FindCatch.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)     3105 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/FindEigen3.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)     9977 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1427 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/check-style.sh
--rw-r--r--   0 vsts      (1001) docker     (127)      952 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (127)     1121 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/libsize.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)     1202 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/make_changelog.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14164 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pybind11Common.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)     7010 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pybind11Config.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (127)     9173 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pybind11NewTools.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)     7276 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pybind11Tools.cmake
--rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1822 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/setup_global.py.in
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-02-26 17:24:21.000000 mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/setup_main.py.in
--rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-02-26 17:24:21.000000 mmcif-0.86.0/requirements-doc.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-02-26 17:24:21.000000 mmcif-0.86.0/requirements-test.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-02-26 17:24:21.000000 mmcif-0.86.0/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-02-26 17:28:07.655418 mmcif-0.86.0/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     6982 2024-02-26 17:24:21.000000 mmcif-0.86.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.846378 mmcif-0.87.0/
+-rw-r--r--   0 vsts      (1001) docker     (127)    12721 2024-04-06 20:32:10.000000 mmcif-0.87.0/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     7596 2024-04-06 20:32:10.000000 mmcif-0.87.0/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-06 20:32:10.000000 mmcif-0.87.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      441 2024-04-06 20:32:10.000000 mmcif-0.87.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     3337 2024-04-06 20:36:33.846378 mmcif-0.87.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2075 2024-04-06 20:32:10.000000 mmcif-0.87.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.702375 mmcif-0.87.0/mmcif/
+-rw-r--r--   0 vsts      (1001) docker     (127)      186 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.706375 mmcif-0.87.0/mmcif/api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21941 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/DataCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17192 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/DataCategoryBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13272 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/DataCategoryFormatted.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11542 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/DataCategoryTyped.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10128 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/DictMethodRunner.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    85436 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/DictionaryApi.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24778 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/DictionaryInclude.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3844 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/Method.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5017 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/MethodUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10683 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/PdbxContainers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.706375 mmcif-0.87.0/mmcif/core/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.706375 mmcif-0.87.0/mmcif/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)    19069 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/BinaryCifReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28179 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/BinaryCifWriter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2922 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/BuildDictionaryExec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1551 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/CifFile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12835 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/IoAdapterBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20047 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/IoAdapterCore.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19111 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/IoAdapterPy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      524 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/PdbxExceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18397 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/PdbxReader.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11640 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/PdbxWriter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-06 20:32:10.000000 mmcif-0.87.0/mmcif/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.842378 mmcif-0.87.0/mmcif.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3337 2024-04-06 20:36:33.000000 mmcif-0.87.0/mmcif.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    29562 2024-04-06 20:36:33.000000 mmcif-0.87.0/mmcif.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-06 20:36:33.000000 mmcif-0.87.0/mmcif.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-04-06 20:36:33.000000 mmcif-0.87.0/mmcif.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-06 20:32:48.000000 mmcif-0.87.0/mmcif.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      130 2024-04-06 20:36:33.000000 mmcif-0.87.0/mmcif.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-06 20:36:33.000000 mmcif-0.87.0/mmcif.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.698375 mmcif-0.87.0/modules/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.694375 mmcif-0.87.0/modules/cc-regex/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.706375 mmcif-0.87.0/modules/cc-regex/include/
+-rw-r--r--   0 vsts      (1001) docker     (127)      943 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/cclass.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2057 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/cname.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      329 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/debug.ih
+-rw-r--r--   0 vsts      (1001) docker     (127)     1379 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/engine.ih
+-rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/main.ih
+-rw-r--r--   0 vsts      (1001) docker     (127)     2723 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/regcomp.ih
+-rw-r--r--   0 vsts      (1001) docker     (127)      267 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/regerror.ih
+-rw-r--r--   0 vsts      (1001) docker     (127)     1891 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/regex.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5365 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/regex2.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      500 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/include/utils.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.710375 mmcif-0.87.0/modules/cc-regex/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5092 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/debug.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    25587 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/engine.c
+-rw-r--r--   0 vsts      (1001) docker     (127)    11193 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/main.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     1825 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/mkh
+-rw-r--r--   0 vsts      (1001) docker     (127)    37342 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/regcomp.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     3212 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/regerror.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     4259 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/regexec.c
+-rw-r--r--   0 vsts      (1001) docker     (127)      736 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/regfree.c
+-rw-r--r--   0 vsts      (1001) docker     (127)     7061 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cc-regex/src/split.c
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.694375 mmcif-0.87.0/modules/cpp-cif-file/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.710375 mmcif-0.87.0/modules/cpp-cif-file/include/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1746 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/include/CifDataInfo.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      688 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/include/CifExcept.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    23567 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/include/CifFile.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1945 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/include/CifParentChild.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5484 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/include/DicFile.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2782 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/include/ParentChild.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.710375 mmcif-0.87.0/modules/cpp-cif-file/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)     6274 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/src/CifDataInfo.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    36103 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/src/CifExcept.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    85654 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/src/CifFile.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    32221 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/src/CifParentChild.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    47643 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/src/DicFile.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    23231 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file/src/ParentChild.C
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.694375 mmcif-0.87.0/modules/cpp-cif-file-util/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.710375 mmcif-0.87.0/modules/cpp-cif-file-util/include/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3264 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file-util/include/CifCorrector.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2444 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file-util/include/CifFileUtil.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.710375 mmcif-0.87.0/modules/cpp-cif-file-util/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)    47136 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file-util/src/CifCorrector.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     4509 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-file-util/src/CifFileUtil.C
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.694375 mmcif-0.87.0/modules/cpp-cif-parser/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.714376 mmcif-0.87.0/modules/cpp-cif-parser/include/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1518 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/CifFileReadDef.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6318 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/CifParserBase.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      898 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/CifParserInt.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1390 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/CifScannerBase.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      750 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/CifScannerInt.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6970 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/DICParserBase.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1032 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/DICParserInt.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1471 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/DICScannerBase.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      912 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/include/DICScannerInt.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.714376 mmcif-0.87.0/modules/cpp-cif-parser/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3768 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/CifFileReadDef.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     2206 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/CifParser.y
+-rw-r--r--   0 vsts      (1001) docker     (127)    23419 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/CifParserBase.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     2475 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/CifScanner.l
+-rw-r--r--   0 vsts      (1001) docker     (127)     9603 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/CifScannerBase.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     2376 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/DICParser.y
+-rw-r--r--   0 vsts      (1001) docker     (127)    41071 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/DICParserBase.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     2985 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/DICScanner.l
+-rw-r--r--   0 vsts      (1001) docker     (127)    10258 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-cif-parser/src/DICScannerBase.C
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.694375 mmcif-0.87.0/modules/cpp-common/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.714376 mmcif-0.87.0/modules/cpp-common/include/
+-rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/BlockIO.h
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2398 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/CifDefs.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6737 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/CifString.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2901 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/DataInfo.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3175 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/Exceptions.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      635 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/GenCont.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6109 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/GenString.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      484 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/RcsbFile.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      335 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/RcsbPlatform.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5664 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/Serializer.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2665 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/mapped_ptr_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1543 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/mapped_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      210 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/rcsb_math.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      711 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/include/rcsb_types.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.718376 mmcif-0.87.0/modules/cpp-common/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1240 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/BlockIO.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    10498 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/CifString.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     9606 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/DataInfo.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     2314 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/Exceptions.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1085 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/GenCont.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    14827 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/GenString.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1236 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/RcsbFile.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      356 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/RcsbPlatform.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    40038 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/Serializer.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    10675 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/mapped_ptr_vector.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     5759 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-common/src/mapped_vector.C
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.694375 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.718376 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2072 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifDataInfo.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    12223 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFile.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     3130 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileReadDef.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     3592 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileUtil.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     3791 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDicFile.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     2003 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDictDataInfo.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    14081 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapISTable.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     6137 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapTableFile.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      690 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapmmciflib.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wraprcsb_types.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.698375 mmcif-0.87.0/modules/cpp-dict-obj-file/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.718376 mmcif-0.87.0/modules/cpp-dict-obj-file/include/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictDataInfo.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7726 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictObjCont.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4564 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictObjContInfo.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5597 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictObjFile.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      876 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictParentChild.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.718376 mmcif-0.87.0/modules/cpp-dict-obj-file/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3975 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictDataInfo.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    19477 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjCont.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    12717 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjContInfo.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     6349 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjFile.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     1979 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjFileCreator.C
+-rw-r--r--   0 vsts      (1001) docker     (127)      741 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjFileReader.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    13027 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjFileSelectiveReader.C
+-rw-r--r--   0 vsts      (1001) docker     (127)     8311 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictParentChild.C
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.698375 mmcif-0.87.0/modules/cpp-mmciflib-test/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.722376 mmcif-0.87.0/modules/cpp-mmciflib-test/src/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1333 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/BigCifTest.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     5347 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/CifDiff.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     3115 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/CifInfo.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2788 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/CifReader.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2673 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/DataChecking.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1929 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/DictInfo.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1894 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest1.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1073 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest10.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2061 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest11.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2406 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest12.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      539 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest13.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     3930 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest14.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     3211 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest2.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1385 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest3.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2410 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest4.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1417 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest5.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1174 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest6.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1863 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest7.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      406 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest8.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      611 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest9.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1316 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/GroupTableTest2.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      582 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/SdbReader.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1519 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/checkdictionary.C
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      655 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/cpp-mmciflib-test/src/selective-reading.C
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.698375 mmcif-0.87.0/modules/cpp-tables/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.722376 mmcif-0.87.0/modules/cpp-tables/include/
+-rw-r--r--   0 vsts      (1001) docker     (127)    52000 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/include/ISTable.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    44528 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/include/ITTable.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    20019 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/include/TTable.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1270 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/include/TableError.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    21422 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/include/TableFile.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.722376 mmcif-0.87.0/modules/cpp-tables/src/
+-rw-r--r--   0 vsts      (1001) docker     (127)    77385 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/src/ISTable.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    43788 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/src/ITTable.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    15437 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/src/TTable.C
+-rw-r--r--   0 vsts      (1001) docker     (127)    26031 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/cpp-tables/src/TableFile.C
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.726376 mmcif-0.87.0/modules/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1271 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.appveyor.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.clang-format
+-rw-r--r--   0 vsts      (1001) docker     (127)     2605 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.clang-tidy
+-rw-r--r--   0 vsts      (1001) docker     (127)     2196 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.cmake-format.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1308 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.codespell-ignore-lines
+-rw-r--r--   0 vsts      (1001) docker     (127)       44 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.git
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.gitattributes
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.726376 mmcif-0.87.0/modules/pybind11/.github/
+-rw-r--r--   0 vsts      (1001) docker     (127)      182 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/CODEOWNERS
+-rw-r--r--   0 vsts      (1001) docker     (127)    15271 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/CONTRIBUTING.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.726376 mmcif-0.87.0/modules/pybind11/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2016 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      328 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      162 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/dependabot.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/labeler.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/labeler_merged.yml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.726376 mmcif-0.87.0/modules/pybind11/.github/matchers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      668 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/matchers/pylint.json
+-rw-r--r--   0 vsts      (1001) docker     (127)      645 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.730376 mmcif-0.87.0/modules/pybind11/.github/workflows/
+-rw-r--r--   0 vsts      (1001) docker     (127)    28486 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/workflows/ci.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     2095 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/workflows/configure.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/workflows/format.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/workflows/labeler.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     2558 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/workflows/pip.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     2837 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.github/workflows/upstream.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      487 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (127)     4331 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.pre-commit-config.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/.readthedocs.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)    11911 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      223 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     7686 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.730376 mmcif-0.87.0/modules/pybind11/docs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      607 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/Doxyfile
+-rw-r--r--   0 vsts      (1001) docker     (127)     7417 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/Makefile
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.698375 mmcif-0.87.0/modules/pybind11/docs/_static/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.730376 mmcif-0.87.0/modules/pybind11/docs/_static/css/
+-rw-r--r--   0 vsts      (1001) docker     (127)       37 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/_static/css/custom.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.734376 mmcif-0.87.0/modules/pybind11/docs/advanced/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.734376 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3937 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     3429 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/custom.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    14283 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     3889 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/functional.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     1556 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    12371 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/overview.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     9586 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/stl.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     8863 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/cast/strings.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    47796 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/classes.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/embedding.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    17772 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/exceptions.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    26729 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/functions.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    13634 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/misc.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.734376 mmcif-0.87.0/modules/pybind11/docs/advanced/pycpp/
+-rw-r--r--   0 vsts      (1001) docker     (127)      278 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    17161 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     9030 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     5710 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     6377 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     9240 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/basics.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     2856 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/benchmark.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3168 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/benchmark.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)   111105 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/changelog.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    16380 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/classes.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.734376 mmcif-0.87.0/modules/pybind11/docs/cmake/
+-rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/cmake/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    25777 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/compiling.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    11559 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13177 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/faq.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)      613 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     3277 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/installing.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     3079 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/limitations.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    61034 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/pybind11-logo.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    44653 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    87708 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)    41121 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    85853 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2647 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/reference.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     4414 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/release.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    23489 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/docs/upgrade.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.698375 mmcif-0.87.0/modules/pybind11/include/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.738376 mmcif-0.87.0/modules/pybind11/include/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (127)    23979 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7069 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    65638 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     8458 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/common.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2096 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.738376 mmcif-0.87.0/modules/pybind11/include/pybind11/detail/
+-rw-r--r--   0 vsts      (1001) docker     (127)    28251 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    50369 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5491 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    17981 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    25057 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    42266 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1625 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    32147 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    11792 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4731 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     4695 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     8262 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     8862 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    79524 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     9103 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2181 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/options.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   125761 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    93848 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.738376 mmcif-0.87.0/modules/pybind11/include/pybind11/stl/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4185 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    15337 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    27013 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/include/pybind11/stl_bind.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2765 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/noxfile.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.738376 mmcif-0.87.0/modules/pybind11/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (127)      414 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/pybind11/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1360 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/pybind11/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      228 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/pybind11/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1226 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/pybind11/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/pybind11/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)    17609 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/pybind11/setup_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1261 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1622 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     4877 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)    20608 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     5006 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11736 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3578 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1776 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/cross_module_interleaved_error_already_set.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      940 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/env.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/extra_python_package/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (127)     8142 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/extra_setuptools/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (127)     4153 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2847 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/local_bindings.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5743 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/object.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6264 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4517 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/pybind11_tests.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     2685 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      768 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (127)      600 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      855 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_async.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      534 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_async.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_buffers.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4841 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_buffers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15990 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_builtin_casters.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    17245 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_builtin_casters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4118 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_call_policies.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     6549 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_call_policies.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9243 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_callbacks.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     5906 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_callbacks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3370 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_chrono.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     5695 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_chrono.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_class.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    14575 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_class.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2639 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      673 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1171 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1293 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1685 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1353 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1163 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.762377 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1368 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      198 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/test.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3831 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_const_name.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      589 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_const_name.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5853 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_constants_and_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10886 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_copy_move.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4796 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_copy_move.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7280 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     3980 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_custom_type_casters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1259 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_custom_type_setup.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_custom_type_setup.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2816 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_docstring_options.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1606 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_docstring_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19409 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_eigen.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    28860 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_eigen.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.766377 mmcif-0.87.0/modules/pybind11/tests/test_embed/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1798 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1338 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_embed/catch.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      543 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_embed/external_module.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    14260 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      237 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      275 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_embed/test_trampoline.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5722 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_enum.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     8903 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_enum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3168 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_eval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1143 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_eval.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      119 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_eval_call.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11904 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_exceptions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      399 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_exceptions.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    12702 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18155 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_factory_constructors.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    16519 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_factory_constructors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5311 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_gil_scoped.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     8565 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_gil_scoped.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3960 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_iostream.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     7286 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_iostream.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9535 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    13757 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4401 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_local_bindings.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     8049 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_local_bindings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21388 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    18134 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_methods_and_attributes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4121 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_modules.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4191 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_modules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12305 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    11874 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_multiple_inheritance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19800 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_numpy_array.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    20228 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_numpy_array.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21114 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    14394 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_numpy_dtypes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4487 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     9686 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_numpy_vectorize.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2777 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_opaque_types.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1847 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_opaque_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9463 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_operator_overloading.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4333 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_operator_overloading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6719 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_pickling.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     2720 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_pickling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30650 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_pytypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    23467 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_pytypes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21153 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     8021 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18898 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_smart_ptr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     9530 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_smart_ptr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21587 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_stl.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    12235 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_stl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4622 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_stl_binders.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     7912 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_stl_binders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4617 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      741 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1855 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_thread.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_thread.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      603 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_union.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      148 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_union.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22983 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_virtual_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    12919 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/test_virtual_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3226 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 vsts      (1001) docker     (127)     2657 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tests/valgrind-python.supp
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.770377 mmcif-0.87.0/modules/pybind11/tools/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2350 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)     3105 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)    11103 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)      817 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/JoinPaths.cmake
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1423 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/check-style.sh
+-rw-r--r--   0 vsts      (1001) docker     (127)      952 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1040 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/codespell_ignore_lines_from_errors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1031 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/libsize.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1282 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/make_changelog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      196 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/pybind11.pc.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    13487 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)     6930 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     8955 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)     8359 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1965 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1139 2024-04-06 20:32:15.000000 mmcif-0.87.0/modules/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.774377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.appveyor.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.clang-format
+-rw-r--r--   0 vsts      (1001) docker     (127)      242 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.clang-tidy
+-rw-r--r--   0 vsts      (1001) docker     (127)     2196 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.cmake-format.yaml
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.774377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/
+-rw-r--r--   0 vsts      (1001) docker     (127)    14415 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.774377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1270 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      172 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      669 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1180 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      559 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/dependabot.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/labeler.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)       50 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/labeler_merged.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      404 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/pull_request_template.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.778377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/
+-rw-r--r--   0 vsts      (1001) docker     (127)    24508 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/ci.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     2117 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/configure.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/format.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      333 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/labeler.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)     2497 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/pip.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (127)     2460 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.pre-commit-config.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.readthedocs.yml
+-rw-r--r--   0 vsts      (1001) docker     (127)    10438 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      256 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     8064 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.786377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      705 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/Doxyfile
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.786377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/_static/
+-rw-r--r--   0 vsts      (1001) docker     (127)      254 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/_static/theme_overrides.css
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.786377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.790377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3937 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/chrono.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     3398 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/custom.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    14288 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/eigen.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     3889 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/functional.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     1556 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    11680 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/overview.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     9703 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/stl.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     9372 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/strings.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    45878 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/classes.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     8420 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/embedding.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    14171 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/exceptions.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    25082 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/functions.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    12444 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/misc.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.790377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/
+-rw-r--r--   0 vsts      (1001) docker     (127)      278 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    16538 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/numpy.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     7878 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/object.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     5125 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/utilities.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     6366 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/smart_ptrs.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     9369 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/basics.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     2974 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/benchmark.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3168 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/benchmark.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    74047 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/changelog.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    16122 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/classes.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.790377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/cmake/
+-rw-r--r--   0 vsts      (1001) docker     (127)      273 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/cmake/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    25511 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/compiling.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    12095 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/conf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14593 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/faq.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)      613 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/index.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     3277 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/installing.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     3062 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/limitations.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    58510 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11-logo.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    44653 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    87708 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)    41121 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.png
+-rw-r--r--   0 vsts      (1001) docker     (127)    85853 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.svg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2511 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/reference.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)     4028 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/release.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)      168 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    23059 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/upgrade.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.698375 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.798377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21412 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/attr.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6118 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/buffer_info.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    57522 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/cast.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     8516 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/chrono.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/common.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2037 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/complex.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.802377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/
+-rw-r--r--   0 vsts      (1001) docker     (127)    27823 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/class.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    42083 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/common.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3602 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/descr.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    16397 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/init.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    16375 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/internals.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    40663 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1486 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/typeid.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    29086 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/eigen.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     7843 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/embed.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5079 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/eval.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     3709 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/functional.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6532 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/gil.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     6084 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/iostream.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    69820 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/numpy.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     9085 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/operators.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     2049 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/options.h
+-rw-r--r--   0 vsts      (1001) docker     (127)   105679 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/pybind11.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    67597 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/pytypes.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    14162 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/stl.h
+-rw-r--r--   0 vsts      (1001) docker     (127)    23912 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/stl_bind.h
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.802377 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/
+-rw-r--r--   0 vsts      (1001) docker     (127)      217 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1158 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      207 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      137 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/_version.pyi
+-rw-r--r--   0 vsts      (1001) docker     (127)      663 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)    15167 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1899 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.pyi
+-rw-r--r--   0 vsts      (1001) docker     (127)      118 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     2185 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     3499 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.834378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15372 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     4841 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11157 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/constructor_stats.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     1819 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/cross_module_gil_utils.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1022 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/env.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.834378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/extra_python_package/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/extra_python_package/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (127)     7154 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/extra_python_package/test_files.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.834378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (127)     2581 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/test_setuphelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2144 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/local_bindings.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5389 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/object.h
+-rw-r--r--   0 vsts      (1001) docker     (127)     5285 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/pybind11_cross_module_tests.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     3647 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     2733 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.h
+-rw-r--r--   0 vsts      (1001) docker     (127)      693 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/pytest.ini
+-rw-r--r--   0 vsts      (1001) docker     (127)      843 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      864 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_async.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_async.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8048 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_buffers.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4946 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_buffers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13475 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    17617 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3702 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_call_policies.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     5728 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_call_policies.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6754 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_callbacks.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     5447 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_callbacks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_chrono.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     5726 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_chrono.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21548 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_class.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    14273 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_class.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.834378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2639 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      656 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/embed.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.834378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1175 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.834378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1259 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.834378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1653 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/main.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.838378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1357 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.838378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1126 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.838378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      166 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/test.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5346 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1522 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9629 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_copy_move.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4645 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_copy_move.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5513 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4015 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2514 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1630 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16867 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eigen.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    28282 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eigen.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.838378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1758 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      637 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/catch.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      554 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/external_module.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    10209 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      219 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2610 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_enum.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     7694 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_enum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2628 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      768 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eval.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      143 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eval_call.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7862 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_exceptions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     6753 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16562 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    16731 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1760 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     3128 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3381 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_iostream.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     5799 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_iostream.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6489 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    10048 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4333 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     8102 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19446 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    17310 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3742 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_modules.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     2841 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_modules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9148 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     9495 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17781 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    18647 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18421 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    13614 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3832 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     9709 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2731 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1906 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8431 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4945 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_pickling.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     1191 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_pickling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14656 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_pytypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    16590 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_pytypes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13120 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     5966 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18187 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     9620 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12793 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_stl.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     8557 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_stl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4403 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)     7182 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4458 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      765 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      603 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_union.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)      172 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_union.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18454 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (127)    11646 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3238 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/valgrind-numpy-scipy.supp
+-rw-r--r--   0 vsts      (1001) docker     (127)     2657 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/valgrind-python.supp
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-06 20:36:33.842378 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2295 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/FindCatch.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)     3105 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/FindEigen3.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)     9977 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1427 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/check-style.sh
+-rw-r--r--   0 vsts      (1001) docker     (127)      952 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1121 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/libsize.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     1202 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/make_changelog.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14164 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pybind11Common.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)     7010 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pybind11Config.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     9173 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pybind11NewTools.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)     7276 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pybind11Tools.cmake
+-rw-r--r--   0 vsts      (1001) docker     (127)       94 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1822 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/setup_global.py.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-06 20:32:10.000000 mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/setup_main.py.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      120 2024-04-06 20:32:10.000000 mmcif-0.87.0/requirements-doc.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       13 2024-04-06 20:32:10.000000 mmcif-0.87.0/requirements-test.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-06 20:32:10.000000 mmcif-0.87.0/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-06 20:36:33.846378 mmcif-0.87.0/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     6982 2024-04-06 20:32:10.000000 mmcif-0.87.0/setup.py
```

### Comparing `mmcif-0.86.0/CMakeLists.txt` & `mmcif-0.87.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/HISTORY.txt` & `mmcif-0.87.0/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -83,7 +83,8 @@
 16-Jan-2024    V0.85.0 - Update BinaryCifReader to read in DataCategory data items into lists instead of tuples;
                          Update BinaryCifWriter to set version tag to that of the active mmcif package installation,
                          to enable compatibility with Mol* and other tools (which requires >= 0.3.0, in that format);
                          Update package version format to `major.minor.patch` (!!! MUST USE THIS FORMAT MOVING FORWARD !!!)
 17-Jan-2024    V0.85.1 - Set BinaryCIF version tag to specifically 0.3.0 to ensure compatibility with Mol* and other tools
 23-Feb-2024    V0.86.0 - BinaryCIF writer properly tracks integer types to ensure
                          proper types passed through encoders.  Ensure compatibility with ciftools-java and Mol*.
+ 6-Apr-2024    V0.87.0 - Correct internal data of PdbxContainers when rename operation is used
```

### Comparing `mmcif-0.86.0/LICENSE` & `mmcif-0.87.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/PKG-INFO` & `mmcif-0.87.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcif
-Version: 0.86.0
+Version: 0.87.0
 Summary: mmCIF Core Access Library
 Home-page: http://mmcif.wwpdb.org
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mmcif-0.86.0/README.md` & `mmcif-0.87.0/README.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/DataCategory.py` & `mmcif-0.87.0/mmcif/api/DataCategory.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/DataCategoryBase.py` & `mmcif-0.87.0/mmcif/api/DataCategoryBase.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/DataCategoryFormatted.py` & `mmcif-0.87.0/mmcif/api/DataCategoryFormatted.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/DataCategoryTyped.py` & `mmcif-0.87.0/mmcif/api/DataCategoryTyped.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/DictMethodRunner.py` & `mmcif-0.87.0/mmcif/api/DictMethodRunner.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/DictionaryApi.py` & `mmcif-0.87.0/mmcif/api/DictionaryApi.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/DictionaryInclude.py` & `mmcif-0.87.0/mmcif/api/DictionaryInclude.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/Method.py` & `mmcif-0.87.0/mmcif/api/Method.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/MethodUtils.py` & `mmcif-0.87.0/mmcif/api/MethodUtils.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/api/PdbxContainers.py` & `mmcif-0.87.0/mmcif/api/PdbxContainers.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,15 @@
     def rename(self, curName, newName):
         """Change the name of an object in place -"""
         try:
             i = self.__objNameList.index(curName)
             self.__objNameList[i] = newName
             self.__objCatalog[newName] = self.__objCatalog[curName]
             self.__objCatalog[newName].setName(newName)
+            del self.__objCatalog[curName]
             return True
         except Exception:
             return False
 
     def remove(self, curName):
         """Remove object by name.  Return True on success or False otherwise."""
         try:
```

### Comparing `mmcif-0.86.0/mmcif/io/BinaryCifReader.py` & `mmcif-0.87.0/mmcif/io/BinaryCifReader.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/BinaryCifWriter.py` & `mmcif-0.87.0/mmcif/io/BinaryCifWriter.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/BuildDictionaryExec.py` & `mmcif-0.87.0/mmcif/io/BuildDictionaryExec.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/CifFile.py` & `mmcif-0.87.0/mmcif/io/CifFile.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/IoAdapterBase.py` & `mmcif-0.87.0/mmcif/io/IoAdapterBase.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/IoAdapterCore.py` & `mmcif-0.87.0/mmcif/io/IoAdapterCore.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/IoAdapterPy.py` & `mmcif-0.87.0/mmcif/io/IoAdapterPy.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/PdbxExceptions.py` & `mmcif-0.87.0/mmcif/io/PdbxExceptions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/PdbxReader.py` & `mmcif-0.87.0/mmcif/io/PdbxReader.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif/io/PdbxWriter.py` & `mmcif-0.87.0/mmcif/io/PdbxWriter.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/mmcif.egg-info/PKG-INFO` & `mmcif-0.87.0/mmcif.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcif
-Version: 0.86.0
+Version: 0.87.0
 Summary: mmCIF Core Access Library
 Home-page: http://mmcif.wwpdb.org
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mmcif-0.86.0/mmcif.egg-info/SOURCES.txt` & `mmcif-0.87.0/mmcif.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/include/cclass.h` & `mmcif-0.87.0/modules/cc-regex/include/cclass.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/include/cname.h` & `mmcif-0.87.0/modules/cc-regex/include/cname.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/include/engine.ih` & `mmcif-0.87.0/modules/cc-regex/include/engine.ih`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/include/regcomp.ih` & `mmcif-0.87.0/modules/cc-regex/include/regcomp.ih`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/include/regex.h` & `mmcif-0.87.0/modules/cc-regex/include/regex.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/include/regex2.h` & `mmcif-0.87.0/modules/cc-regex/include/regex2.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/debug.c` & `mmcif-0.87.0/modules/cc-regex/src/debug.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/engine.c` & `mmcif-0.87.0/modules/cc-regex/src/engine.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/main.c` & `mmcif-0.87.0/modules/cc-regex/src/main.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/mkh` & `mmcif-0.87.0/modules/cc-regex/src/mkh`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/regcomp.c` & `mmcif-0.87.0/modules/cc-regex/src/regcomp.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/regerror.c` & `mmcif-0.87.0/modules/cc-regex/src/regerror.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/regexec.c` & `mmcif-0.87.0/modules/cc-regex/src/regexec.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/regfree.c` & `mmcif-0.87.0/modules/cc-regex/src/regfree.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cc-regex/src/split.c` & `mmcif-0.87.0/modules/cc-regex/src/split.c`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/include/CifDataInfo.h` & `mmcif-0.87.0/modules/cpp-cif-file/include/CifDataInfo.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/include/CifExcept.h` & `mmcif-0.87.0/modules/cpp-cif-file/include/CifExcept.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/include/CifFile.h` & `mmcif-0.87.0/modules/cpp-cif-file/include/CifFile.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/include/CifParentChild.h` & `mmcif-0.87.0/modules/cpp-cif-file/include/CifParentChild.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/include/DicFile.h` & `mmcif-0.87.0/modules/cpp-cif-file/include/DicFile.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/include/ParentChild.h` & `mmcif-0.87.0/modules/cpp-cif-file/include/ParentChild.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/src/CifDataInfo.C` & `mmcif-0.87.0/modules/cpp-cif-file/src/CifDataInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/src/CifExcept.C` & `mmcif-0.87.0/modules/cpp-cif-file/src/CifExcept.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/src/CifFile.C` & `mmcif-0.87.0/modules/cpp-cif-file/src/CifFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/src/CifParentChild.C` & `mmcif-0.87.0/modules/cpp-cif-file/src/CifParentChild.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/src/DicFile.C` & `mmcif-0.87.0/modules/cpp-cif-file/src/DicFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file/src/ParentChild.C` & `mmcif-0.87.0/modules/cpp-cif-file/src/ParentChild.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file-util/include/CifCorrector.h` & `mmcif-0.87.0/modules/cpp-cif-file-util/include/CifCorrector.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file-util/include/CifFileUtil.h` & `mmcif-0.87.0/modules/cpp-cif-file-util/include/CifFileUtil.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file-util/src/CifCorrector.C` & `mmcif-0.87.0/modules/cpp-cif-file-util/src/CifCorrector.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-file-util/src/CifFileUtil.C` & `mmcif-0.87.0/modules/cpp-cif-file-util/src/CifFileUtil.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/CifFileReadDef.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/CifFileReadDef.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/CifParserBase.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/CifParserBase.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/CifParserInt.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/CifParserInt.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/CifScannerBase.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/CifScannerBase.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/CifScannerInt.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/CifScannerInt.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/DICParserBase.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/DICParserBase.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/DICParserInt.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/DICParserInt.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/DICScannerBase.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/DICScannerBase.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/include/DICScannerInt.h` & `mmcif-0.87.0/modules/cpp-cif-parser/include/DICScannerInt.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/CifFileReadDef.C` & `mmcif-0.87.0/modules/cpp-cif-parser/src/CifFileReadDef.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/CifParser.y` & `mmcif-0.87.0/modules/cpp-cif-parser/src/CifParser.y`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/CifParserBase.C` & `mmcif-0.87.0/modules/cpp-cif-parser/src/CifParserBase.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/CifScanner.l` & `mmcif-0.87.0/modules/cpp-cif-parser/src/CifScanner.l`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/CifScannerBase.C` & `mmcif-0.87.0/modules/cpp-cif-parser/src/CifScannerBase.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/DICParser.y` & `mmcif-0.87.0/modules/cpp-cif-parser/src/DICParser.y`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/DICParserBase.C` & `mmcif-0.87.0/modules/cpp-cif-parser/src/DICParserBase.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/DICScanner.l` & `mmcif-0.87.0/modules/cpp-cif-parser/src/DICScanner.l`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-cif-parser/src/DICScannerBase.C` & `mmcif-0.87.0/modules/cpp-cif-parser/src/DICScannerBase.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/BlockIO.h` & `mmcif-0.87.0/modules/cpp-common/include/BlockIO.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/CifDefs.h` & `mmcif-0.87.0/modules/cpp-common/include/CifDefs.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/CifString.h` & `mmcif-0.87.0/modules/cpp-common/include/CifString.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/DataInfo.h` & `mmcif-0.87.0/modules/cpp-common/include/DataInfo.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/Exceptions.h` & `mmcif-0.87.0/modules/cpp-common/include/Exceptions.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/GenCont.h` & `mmcif-0.87.0/modules/cpp-common/include/GenCont.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/GenString.h` & `mmcif-0.87.0/modules/cpp-common/include/GenString.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/Serializer.h` & `mmcif-0.87.0/modules/cpp-common/include/Serializer.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/mapped_ptr_vector.h` & `mmcif-0.87.0/modules/cpp-common/include/mapped_ptr_vector.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/mapped_vector.h` & `mmcif-0.87.0/modules/cpp-common/include/mapped_vector.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/include/rcsb_types.h` & `mmcif-0.87.0/modules/cpp-common/include/rcsb_types.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/BlockIO.C` & `mmcif-0.87.0/modules/cpp-common/src/BlockIO.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/CifString.C` & `mmcif-0.87.0/modules/cpp-common/src/CifString.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/DataInfo.C` & `mmcif-0.87.0/modules/cpp-common/src/DataInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/Exceptions.C` & `mmcif-0.87.0/modules/cpp-common/src/Exceptions.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/GenCont.C` & `mmcif-0.87.0/modules/cpp-common/src/GenCont.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/GenString.C` & `mmcif-0.87.0/modules/cpp-common/src/GenString.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/RcsbFile.C` & `mmcif-0.87.0/modules/cpp-common/src/RcsbFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/Serializer.C` & `mmcif-0.87.0/modules/cpp-common/src/Serializer.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/mapped_ptr_vector.C` & `mmcif-0.87.0/modules/cpp-common/src/mapped_ptr_vector.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-common/src/mapped_vector.C` & `mmcif-0.87.0/modules/cpp-common/src/mapped_vector.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifDataInfo.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifDataInfo.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFile.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFile.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileReadDef.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileReadDef.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileUtil.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapCifFileUtil.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDicFile.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDicFile.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDictDataInfo.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapDictDataInfo.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapISTable.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapISTable.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapTableFile.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapTableFile.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapmmciflib.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wrapmmciflib.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-core-mmciflib-wrapper-gen/src/wraprcsb_types.cpp` & `mmcif-0.87.0/modules/cpp-core-mmciflib-wrapper-gen/src/wraprcsb_types.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictDataInfo.h` & `mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictDataInfo.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictObjCont.h` & `mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictObjCont.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictObjContInfo.h` & `mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictObjContInfo.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictObjFile.h` & `mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictObjFile.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/include/DictParentChild.h` & `mmcif-0.87.0/modules/cpp-dict-obj-file/include/DictParentChild.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictDataInfo.C` & `mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictDataInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjCont.C` & `mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjCont.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjContInfo.C` & `mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjContInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjFile.C` & `mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjFileCreator.C` & `mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjFileCreator.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjFileReader.C` & `mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjFileReader.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictObjFileSelectiveReader.C` & `mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictObjFileSelectiveReader.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-dict-obj-file/src/DictParentChild.C` & `mmcif-0.87.0/modules/cpp-dict-obj-file/src/DictParentChild.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/BigCifTest.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/BigCifTest.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/CifDiff.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/CifDiff.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/CifInfo.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/CifInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/CifReader.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/CifReader.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/DataChecking.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/DataChecking.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/DictInfo.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/DictInfo.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest1.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest1.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest10.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest10.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest11.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest11.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest12.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest12.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest13.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest13.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest14.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest14.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest2.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest2.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest3.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest3.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest4.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest4.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest5.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest5.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest6.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest6.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest7.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest7.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/FOtest9.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/FOtest9.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/GroupTableTest2.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/GroupTableTest2.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/SdbReader.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/SdbReader.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/checkdictionary.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/checkdictionary.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-mmciflib-test/src/selective-reading.C` & `mmcif-0.87.0/modules/cpp-mmciflib-test/src/selective-reading.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/include/ISTable.h` & `mmcif-0.87.0/modules/cpp-tables/include/ISTable.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/include/ITTable.h` & `mmcif-0.87.0/modules/cpp-tables/include/ITTable.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/include/TTable.h` & `mmcif-0.87.0/modules/cpp-tables/include/TTable.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/include/TableError.h` & `mmcif-0.87.0/modules/cpp-tables/include/TableError.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/include/TableFile.h` & `mmcif-0.87.0/modules/cpp-tables/include/TableFile.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/src/ISTable.C` & `mmcif-0.87.0/modules/cpp-tables/src/ISTable.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/src/ITTable.C` & `mmcif-0.87.0/modules/cpp-tables/src/ITTable.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/src/TTable.C` & `mmcif-0.87.0/modules/cpp-tables/src/TTable.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/cpp-tables/src/TableFile.C` & `mmcif-0.87.0/modules/cpp-tables/src/TableFile.C`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.appveyor.yml` & `mmcif-0.87.0/modules/pybind11/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.clang-format` & `mmcif-0.87.0/modules/pybind11/.clang-format`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.clang-tidy` & `mmcif-0.87.0/modules/pybind11/.clang-tidy`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.cmake-format.yaml` & `mmcif-0.87.0/modules/pybind11/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.codespell-ignore-lines` & `mmcif-0.87.0/modules/pybind11/.codespell-ignore-lines`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/CONTRIBUTING.md` & `mmcif-0.87.0/modules/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml` & `mmcif-0.87.0/modules/pybind11/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/matchers/pylint.json` & `mmcif-0.87.0/modules/pybind11/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/pull_request_template.md` & `mmcif-0.87.0/modules/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/workflows/ci.yml` & `mmcif-0.87.0/modules/pybind11/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/workflows/configure.yml` & `mmcif-0.87.0/modules/pybind11/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/workflows/format.yml` & `mmcif-0.87.0/modules/pybind11/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/workflows/pip.yml` & `mmcif-0.87.0/modules/pybind11/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.github/workflows/upstream.yml` & `mmcif-0.87.0/modules/pybind11/.github/workflows/upstream.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/.pre-commit-config.yaml` & `mmcif-0.87.0/modules/pybind11/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/LICENSE` & `mmcif-0.87.0/modules/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/README.rst` & `mmcif-0.87.0/modules/pybind11/README.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/Doxyfile` & `mmcif-0.87.0/modules/pybind11/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/Makefile` & `mmcif-0.87.0/modules/pybind11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/cast/chrono.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/cast/custom.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/cast/eigen.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/cast/functional.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/cast/index.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/cast/overview.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/cast/stl.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/cast/strings.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/classes.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/embedding.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/exceptions.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/functions.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/misc.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/pycpp/numpy.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/pycpp/object.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/pycpp/utilities.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/advanced/smart_ptrs.rst` & `mmcif-0.87.0/modules/pybind11/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/basics.rst` & `mmcif-0.87.0/modules/pybind11/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/benchmark.py` & `mmcif-0.87.0/modules/pybind11/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/benchmark.rst` & `mmcif-0.87.0/modules/pybind11/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/changelog.rst` & `mmcif-0.87.0/modules/pybind11/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/classes.rst` & `mmcif-0.87.0/modules/pybind11/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/compiling.rst` & `mmcif-0.87.0/modules/pybind11/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/conf.py` & `mmcif-0.87.0/modules/pybind11/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/faq.rst` & `mmcif-0.87.0/modules/pybind11/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/index.rst` & `mmcif-0.87.0/modules/pybind11/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/installing.rst` & `mmcif-0.87.0/modules/pybind11/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/limitations.rst` & `mmcif-0.87.0/modules/pybind11/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/pybind11-logo.png` & `mmcif-0.87.0/modules/pybind11/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/pybind11_vs_boost_python1.png` & `mmcif-0.87.0/modules/pybind11/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/pybind11_vs_boost_python1.svg` & `mmcif-0.87.0/modules/pybind11/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/pybind11_vs_boost_python2.png` & `mmcif-0.87.0/modules/pybind11/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/pybind11_vs_boost_python2.svg` & `mmcif-0.87.0/modules/pybind11/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/reference.rst` & `mmcif-0.87.0/modules/pybind11/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/release.rst` & `mmcif-0.87.0/modules/pybind11/docs/release.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/docs/upgrade.rst` & `mmcif-0.87.0/modules/pybind11/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/attr.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/buffer_info.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/cast.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/chrono.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/complex.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/detail/class.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/detail/common.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/detail/descr.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/detail/init.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/detail/internals.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/detail/type_caster_base.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/detail/typeid.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/eigen.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/embed.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/eval.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/functional.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/gil.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/iostream.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/numpy.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/operators.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/options.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/pybind11.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/pytypes.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/stl/filesystem.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/stl.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/include/pybind11/stl_bind.h` & `mmcif-0.87.0/modules/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/noxfile.py` & `mmcif-0.87.0/modules/pybind11/noxfile.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/pybind11/__main__.py` & `mmcif-0.87.0/modules/pybind11/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/pybind11/commands.py` & `mmcif-0.87.0/modules/pybind11/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/pybind11/setup_helpers.py` & `mmcif-0.87.0/modules/pybind11/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/pyproject.toml` & `mmcif-0.87.0/modules/pybind11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/setup.cfg` & `mmcif-0.87.0/modules/pybind11/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/setup.py` & `mmcif-0.87.0/modules/pybind11/setup.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/conftest.py` & `mmcif-0.87.0/modules/pybind11/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/constructor_stats.h` & `mmcif-0.87.0/modules/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/cross_module_gil_utils.cpp` & `mmcif-0.87.0/modules/pybind11/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/cross_module_interleaved_error_already_set.cpp` & `mmcif-0.87.0/modules/pybind11/tests/cross_module_interleaved_error_already_set.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/env.py` & `mmcif-0.87.0/modules/pybind11/tests/env.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/extra_python_package/test_files.py` & `mmcif-0.87.0/modules/pybind11/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/extra_setuptools/test_setuphelper.py` & `mmcif-0.87.0/modules/pybind11/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/local_bindings.h` & `mmcif-0.87.0/modules/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/object.h` & `mmcif-0.87.0/modules/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/pybind11_cross_module_tests.cpp` & `mmcif-0.87.0/modules/pybind11/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/pybind11_tests.cpp` & `mmcif-0.87.0/modules/pybind11/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/pybind11_tests.h` & `mmcif-0.87.0/modules/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/pytest.ini` & `mmcif-0.87.0/modules/pybind11/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/requirements.txt` & `mmcif-0.87.0/modules/pybind11/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_async.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_async.py` & `mmcif-0.87.0/modules/pybind11/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_buffers.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_buffers.py` & `mmcif-0.87.0/modules/pybind11/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_builtin_casters.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_builtin_casters.py` & `mmcif-0.87.0/modules/pybind11/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_call_policies.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_call_policies.py` & `mmcif-0.87.0/modules/pybind11/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_callbacks.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_callbacks.py` & `mmcif-0.87.0/modules/pybind11/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_chrono.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_chrono.py` & `mmcif-0.87.0/modules/pybind11/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_class.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_class.py` & `mmcif-0.87.0/modules/pybind11/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/embed.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_const_name.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_const_name.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_const_name.py` & `mmcif-0.87.0/modules/pybind11/tests/test_const_name.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_constants_and_functions.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_constants_and_functions.py` & `mmcif-0.87.0/modules/pybind11/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_copy_move.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_copy_move.py` & `mmcif-0.87.0/modules/pybind11/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_custom_type_casters.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_custom_type_casters.py` & `mmcif-0.87.0/modules/pybind11/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_custom_type_setup.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_custom_type_setup.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_custom_type_setup.py` & `mmcif-0.87.0/modules/pybind11/tests/test_custom_type_setup.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_docstring_options.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_docstring_options.py` & `mmcif-0.87.0/modules/pybind11/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_eigen.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_eigen.py` & `mmcif-0.87.0/modules/pybind11/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_embed/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_embed/catch.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_embed/external_module.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_embed/test_interpreter.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_enum.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_enum.py` & `mmcif-0.87.0/modules/pybind11/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_eval.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_eval.py` & `mmcif-0.87.0/modules/pybind11/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_exceptions.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_exceptions.py` & `mmcif-0.87.0/modules/pybind11/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_factory_constructors.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_factory_constructors.py` & `mmcif-0.87.0/modules/pybind11/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_gil_scoped.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_gil_scoped.py` & `mmcif-0.87.0/modules/pybind11/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_iostream.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_iostream.py` & `mmcif-0.87.0/modules/pybind11/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_kwargs_and_defaults.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_kwargs_and_defaults.py` & `mmcif-0.87.0/modules/pybind11/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_local_bindings.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_local_bindings.py` & `mmcif-0.87.0/modules/pybind11/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_methods_and_attributes.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_methods_and_attributes.py` & `mmcif-0.87.0/modules/pybind11/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_modules.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_modules.py` & `mmcif-0.87.0/modules/pybind11/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_multiple_inheritance.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_multiple_inheritance.py` & `mmcif-0.87.0/modules/pybind11/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_numpy_array.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_numpy_array.py` & `mmcif-0.87.0/modules/pybind11/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_numpy_dtypes.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_numpy_dtypes.py` & `mmcif-0.87.0/modules/pybind11/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_numpy_vectorize.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_numpy_vectorize.py` & `mmcif-0.87.0/modules/pybind11/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_opaque_types.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_opaque_types.py` & `mmcif-0.87.0/modules/pybind11/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_operator_overloading.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_operator_overloading.py` & `mmcif-0.87.0/modules/pybind11/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_pickling.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_pickling.py` & `mmcif-0.87.0/modules/pybind11/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_pytypes.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_pytypes.py` & `mmcif-0.87.0/modules/pybind11/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_sequences_and_iterators.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_sequences_and_iterators.py` & `mmcif-0.87.0/modules/pybind11/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_smart_ptr.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_smart_ptr.py` & `mmcif-0.87.0/modules/pybind11/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_stl.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_stl.py` & `mmcif-0.87.0/modules/pybind11/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_stl_binders.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_stl_binders.py` & `mmcif-0.87.0/modules/pybind11/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_tagbased_polymorphic.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_tagbased_polymorphic.py` & `mmcif-0.87.0/modules/pybind11/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_thread.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_thread.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_thread.py` & `mmcif-0.87.0/modules/pybind11/tests/test_thread.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_union.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_virtual_functions.cpp` & `mmcif-0.87.0/modules/pybind11/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/test_virtual_functions.py` & `mmcif-0.87.0/modules/pybind11/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/valgrind-numpy-scipy.supp` & `mmcif-0.87.0/modules/pybind11/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tests/valgrind-python.supp` & `mmcif-0.87.0/modules/pybind11/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/FindCatch.cmake` & `mmcif-0.87.0/modules/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/FindEigen3.cmake` & `mmcif-0.87.0/modules/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/FindPythonLibsNew.cmake` & `mmcif-0.87.0/modules/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/JoinPaths.cmake` & `mmcif-0.87.0/modules/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/check-style.sh` & `mmcif-0.87.0/modules/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/cmake_uninstall.cmake.in` & `mmcif-0.87.0/modules/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/codespell_ignore_lines_from_errors.py` & `mmcif-0.87.0/modules/pybind11/tools/codespell_ignore_lines_from_errors.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/libsize.py` & `mmcif-0.87.0/modules/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/make_changelog.py` & `mmcif-0.87.0/modules/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/pybind11Common.cmake` & `mmcif-0.87.0/modules/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/pybind11Config.cmake.in` & `mmcif-0.87.0/modules/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/pybind11NewTools.cmake` & `mmcif-0.87.0/modules/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/pybind11Tools.cmake` & `mmcif-0.87.0/modules/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/setup_global.py.in` & `mmcif-0.87.0/modules/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11/tools/setup_main.py.in` & `mmcif-0.87.0/modules/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.appveyor.yml` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.clang-format` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.clang-format`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.cmake-format.yaml` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.cmake-format.yaml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/CONTRIBUTING.md` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/bug-report.md` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/feature-request.md` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/question.md` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/dependabot.yml` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/ci.yml` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/configure.yml` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/configure.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/format.yml` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.github/workflows/pip.yml` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/.pre-commit-config.yaml` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/LICENSE` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/README.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/README.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/Doxyfile` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/chrono.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/chrono.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/custom.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/custom.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/eigen.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/eigen.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/functional.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/functional.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/index.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/index.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/overview.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/overview.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/stl.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/stl.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/strings.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/cast/strings.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/classes.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/classes.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/embedding.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/embedding.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/exceptions.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/exceptions.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/functions.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/functions.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/misc.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/misc.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/numpy.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/numpy.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/object.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/object.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/utilities.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/pycpp/utilities.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/advanced/smart_ptrs.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/advanced/smart_ptrs.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/basics.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/basics.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/benchmark.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/benchmark.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/benchmark.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/benchmark.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/changelog.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/classes.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/compiling.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/compiling.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/conf.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/faq.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/index.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/installing.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/limitations.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11-logo.png` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11-logo.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.png` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.svg` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python1.svg`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.png` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.png`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.svg` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/pybind11_vs_boost_python2.svg`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/reference.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/release.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/release.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/docs/upgrade.rst` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/attr.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/buffer_info.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/cast.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/chrono.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/complex.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/class.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/common.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/descr.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/init.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/internals.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/type_caster_base.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/typeid.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/eigen.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/embed.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/eval.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/functional.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/gil.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/iostream.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/numpy.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/operators.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/options.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/pybind11.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/pytypes.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/stl.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/include/pybind11/stl_bind.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/__main__.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/__main__.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/commands.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/commands.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.pyi` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/pybind11/setup_helpers.pyi`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/setup.cfg` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/setup.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/setup.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/conftest.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/constructor_stats.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/cross_module_gil_utils.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/cross_module_gil_utils.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/env.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/env.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/extra_python_package/test_files.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/extra_python_package/test_files.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/test_setuphelper.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/extra_setuptools/test_setuphelper.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/local_bindings.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/object.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/object.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/pybind11_cross_module_tests.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/pybind11_cross_module_tests.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.h` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/pytest.ini` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/pytest.ini`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/requirements.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_async.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_async.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_async.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_buffers.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_buffers.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_buffers.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_buffers.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_builtin_casters.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_call_policies.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_call_policies.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_call_policies.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_call_policies.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_callbacks.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_callbacks.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_callbacks.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_chrono.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_chrono.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_chrono.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_chrono.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_class.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_class.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_class.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/embed.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/embed.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_constants_and_functions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_copy_move.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_copy_move.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_copy_move.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_copy_move.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_custom_type_casters.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_docstring_options.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eigen.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eigen.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eigen.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eigen.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/CMakeLists.txt` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/catch.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/catch.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/external_module.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/external_module.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_embed/test_interpreter.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_enum.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_enum.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_enum.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eval.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eval.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_eval.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_exceptions.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_exceptions.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_factory_constructors.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_gil_scoped.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_iostream.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_iostream.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_iostream.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_iostream.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_kwargs_and_defaults.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_local_bindings.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_methods_and_attributes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_modules.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_modules.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_modules.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_multiple_inheritance.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_array.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_dtypes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_numpy_vectorize.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_opaque_types.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_operator_overloading.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_pickling.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_pickling.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_pickling.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_pytypes.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_pytypes.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_pytypes.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_pytypes.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_sequences_and_iterators.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_smart_ptr.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_stl.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_stl.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_stl.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_stl.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_stl_binders.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_tagbased_polymorphic.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_union.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_union.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.cpp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.cpp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/test_virtual_functions.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/valgrind-numpy-scipy.supp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/valgrind-numpy-scipy.supp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tests/valgrind-python.supp` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tests/valgrind-python.supp`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/FindCatch.cmake` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/FindEigen3.cmake` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/FindPythonLibsNew.cmake` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/check-style.sh` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/cmake_uninstall.cmake.in` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/libsize.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/make_changelog.py` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pybind11Common.cmake` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pybind11Config.cmake.in` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pybind11NewTools.cmake` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/pybind11Tools.cmake` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/setup_global.py.in` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/modules/pybind11_2_6_3_dev1/tools/setup_main.py.in` & `mmcif-0.87.0/modules/pybind11_2_6_3_dev1/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `mmcif-0.86.0/setup.py` & `mmcif-0.87.0/setup.py`

 * *Files identical despite different names*

