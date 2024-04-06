# Comparing `tmp/iderare-pheno-0.1.7.tar.gz` & `tmp/iderare-pheno-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iderare-pheno-0.1.7.tar", last modified: Sat Apr  6 11:00:43 2024, max compression
+gzip compressed data, was "iderare-pheno-0.1.8.tar", last modified: Sat Apr  6 11:14:19 2024, max compression
```

## Comparing `iderare-pheno-0.1.7.tar` & `iderare-pheno-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:00:43.857509 iderare-pheno-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 11:00:31.000000 iderare-pheno-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-06 11:00:43.857509 iderare-pheno-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-04-06 11:00:31.000000 iderare-pheno-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:00:43.853510 iderare-pheno-0.1.7/iderare_pheno/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 11:00:31.000000 iderare-pheno-0.1.7/iderare_pheno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:00:31.000000 iderare-pheno-0.1.7/iderare_pheno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 11:00:31.000000 iderare-pheno-0.1.7/iderare_pheno/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:00:43.853510 iderare-pheno-0.1.7/iderare_pheno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-06 11:00:43.000000 iderare-pheno-0.1.7/iderare_pheno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-06 11:00:43.000000 iderare-pheno-0.1.7/iderare_pheno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:00:43.000000 iderare-pheno-0.1.7/iderare_pheno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-06 11:00:43.000000 iderare-pheno-0.1.7/iderare_pheno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 11:00:43.000000 iderare-pheno-0.1.7/iderare_pheno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-06 11:00:31.000000 iderare-pheno-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:00:43.857509 iderare-pheno-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:14:19.276228 iderare-pheno-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-06 11:14:19.276228 iderare-pheno-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:14:19.272228 iderare-pheno-0.1.8/iderare_pheno/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/iderare_pheno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/iderare_pheno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/iderare_pheno/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:14:19.272228 iderare-pheno-0.1.8/iderare_pheno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-06 11:14:19.000000 iderare-pheno-0.1.8/iderare_pheno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-06 11:14:06.000000 iderare-pheno-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:14:19.276228 iderare-pheno-0.1.8/setup.cfg
```

### Comparing `iderare-pheno-0.1.7/LICENSE` & `iderare-pheno-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.1.7/PKG-INFO` & `iderare-pheno-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6964 6572  : 2.1.Name: ider
 00000020: 6172 652d 7068 656e 6f0a 5665 7273 696f  are-pheno.Versio
-00000030: 6e3a 2030 2e31 2e37 0a41 7574 686f 722d  n: 0.1.7.Author-
+00000030: 6e3a 2030 2e31 2e38 0a41 7574 686f 722d  n: 0.1.8.Author-
 00000040: 656d 6169 6c3a 2049 7661 6e20 5769 6c6c  email: Ivan Will
 00000050: 6961 6d20 4861 7273 6f6e 6f20 3c63 6f6e  iam Harsono <con
 00000060: 7461 6374 4069 7661 6e77 696c 6c69 616d  tact@ivanwilliam
 00000070: 6d64 2e6f 7267 3e0a 4c69 6365 6e73 653a  md.org>.License:
 00000080: 2042 5344 2033 2d43 6c61 7573 6520 4c69   BSD 3-Clause Li
 00000090: 6365 6e73 650a 2020 2020 2020 2020 0a20  cense.        . 
 000000a0: 2020 2020 2020 2043 6f70 7972 6967 6874         Copyright
@@ -202,15 +202,15 @@
 00000c90: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
 00000ca0: 782d 6175 746f 646f 632d 7479 7065 6869  x-autodoc-typehi
 00000cb0: 6e74 733d 3d31 2e32 332e 333b 2065 7874  nts==1.23.3; ext
 00000cc0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
 00000cd0: 6972 6573 2d44 6973 743a 2070 6163 6b61  ires-Dist: packa
 00000ce0: 6769 6e67 3b20 6578 7472 6120 3d3d 2022  ging; extra == "
 00000cf0: 6465 7622 0a0a 2320 5b49 4465 5261 7265  dev"..# [IDeRare
-00000d00: 2d70 6865 6e6f 5d28 6874 7470 733a 2f2f  -pheno](https://
+00000d00: 2d50 6865 6e6f 5d28 6874 7470 733a 2f2f  -Pheno](https://
 00000d10: 6964 6572 6172 652d 7068 656e 6f2e 7265  iderare-pheno.re
 00000d20: 6164 7468 6564 6f63 732e 696f 2f29 0a0a  adthedocs.io/)..
 00000d30: 3c21 2d2d 2073 7461 7274 2074 6167 6c69  <!-- start tagli
 00000d40: 6e65 202d 2d3e 0a0a 4944 6552 6172 6520  ne -->..IDeRare 
 00000d50: 6f72 2022 496e 646f 6e65 7369 6120 4578  or "Indonesia Ex
 00000d60: 6f6d 6520 5261 7265 2044 6973 6561 7365  ome Rare Disease
 00000d70: 2056 6172 6961 6e74 2044 6973 636f 7665   Variant Discove
@@ -218,224 +218,236 @@
 00000d90: 7369 6d70 6c65 2061 6e64 2072 6561 6479  simple and ready
 00000da0: 2074 6f20 7573 6520 7661 7269 616e 7420   to use variant 
 00000db0: 6469 7363 6f76 6572 7920 7069 7065 6c69  discovery pipeli
 00000dc0: 6e65 2074 6f20 6469 7363 6f76 6572 2072  ne to discover r
 00000dd0: 6172 6520 6469 7365 6173 6520 7661 7269  are disease vari
 00000de0: 616e 7473 2066 726f 6d20 6578 6f6d 6520  ants from exome 
 00000df0: 7365 7175 656e 6369 6e67 2064 6174 612e  sequencing data.
-00000e00: 0a0a 496e 7465 7261 6374 6976 6520 5765  ..Interactive We
-00000e10: 6261 7070 7320 496d 706c 656d 656e 7461  bapps Implementa
-00000e20: 7469 6f6e 206f 6620 2a2a 6964 6572 6172  tion of **iderar
-00000e30: 655f 7068 656e 6f2e 7079 2a2a 2068 6f73  e_pheno.py** hos
-00000e40: 7465 6420 6174 205b 5374 7265 616d 6c69  ted at [Streamli
-00000e50: 745d 2868 7474 7073 3a2f 2f62 696f 696e  t](https://bioin
-00000e60: 666f 726d 6174 6963 732d 6976 616e 7769  formatics-ivanwi
-00000e70: 6c6c 6961 6d68 6172 736f 6e6f 2e73 7472  lliamharsono.str
-00000e80: 6561 6d6c 6974 6170 702e 636f 6d2f 4944  eamlitapp.com/ID
-00000e90: 6552 6172 655f 5068 656e 6f29 0a0a 5468  eRare_Pheno)..Th
-00000ea0: 6973 2073 6372 6970 7420 6973 2072 6563  is script is rec
-00000eb0: 6f6d 6d65 6e64 6564 2069 6620 796f 7520  ommended if you 
-00000ec0: 776f 756c 6420 6c69 6b65 2074 6f20 646f  would like to do
-00000ed0: 2063 6f6e 7665 7273 696f 6e2c 206c 696e   conversion, lin
-00000ee0: 6b61 6765 2061 6e61 6c79 7369 732c 2073  kage analysis, s
-00000ef0: 696d 696c 6172 6974 7920 7363 6f72 696e  imilarity scorin
-00000f00: 672c 2061 6e64 2067 656e 652d 6469 7365  g, and gene-dise
-00000f10: 6173 6520 7265 636f 6d6d 656e 6461 7469  ase recommendati
-00000f20: 6f6e 2062 6173 6564 206f 6e20 7468 6520  on based on the 
-00000f30: 7068 656e 6f74 7970 6520 6461 7461 2070  phenotype data p
-00000f40: 726f 7669 6465 6420 6174 205b 636c 696e  rovided at [clin
-00000f50: 6963 616c 5f64 6174 612e 7478 745d 2863  ical_data.txt](c
-00000f60: 6c69 6e69 6361 6c5f 6461 7461 2e74 7874  linical_data.txt
-00000f70: 292e 2046 756c 6c20 6665 6174 7572 6520  ). Full feature 
-00000f80: 3a20 0a31 2e20 436f 6e76 6572 7420 7468  : .1. Convert th
-00000f90: 6520 7068 656e 6f74 7970 6520 6461 7461  e phenotype data
-00000fa0: 2074 6f20 4850 4f20 636f 6465 2028 6163   to HPO code (ac
-00000fb0: 6365 7074 206d 6978 6564 2053 4e4f 4d45  cept mixed SNOME
-00000fc0: 442c 204c 4f49 4e43 2c20 616e 6420 4850  D, LOINC, and HP
-00000fd0: 4f20 636f 6465 290a 322e 2053 696d 696c  O code).2. Simil
-00000fe0: 6172 6974 7920 7363 6f72 696e 6720 6f66  arity scoring of
-00000ff0: 2064 6966 6665 7265 6e74 6961 6c20 6469   differential di
-00001000: 6167 6e6f 7369 730a 332e 204c 696e 6b61  agnosis.3. Linka
-00001010: 6765 2061 6e61 6c79 7369 7320 6f66 2064  ge analysis of d
-00001020: 6966 6665 7265 6e74 6961 6c20 6469 6167  ifferential diag
-00001030: 6e6f 7369 7320 2861 6363 6570 7420 6d69  nosis (accept mi
-00001040: 7865 6420 534e 4f4d 4544 2c20 4943 442d  xed SNOMED, ICD-
-00001050: 3130 2c20 4f52 5048 412c 204f 4d49 4d20  10, ORPHA, OMIM 
-00001060: 636f 6465 292c 2069 6e63 6c75 6465 2064  code), include d
-00001070: 656e 6472 6f67 7261 6d20 7472 6565 2076  endrogram tree v
-00001080: 6973 7561 6c69 7a61 7469 6f6e 2e0a 2020  isualization..  
-00001090: 2020 2d20 5468 6973 2073 686f 756c 6420    - This should 
-000010a0: 6865 6c70 2063 6c69 6e69 6369 616e 2074  help clinician t
-000010b0: 6f20 2a2a 7379 7374 656d 6174 6963 616c  o **systematical
-000010c0: 6c79 2064 6f69 6e67 2077 6f72 6b2d 7570  ly doing work-up
-000010d0: 2061 6e64 2065 7863 6c75 6469 6e67 2073   and excluding s
-000010e0: 696d 696c 6172 2064 6961 676e 6f73 6973  imilar diagnosis
-000010f0: 2074 6f67 6574 6865 722a 2a20 6261 7365   together** base
-00001100: 6420 6f6e 2074 6865 2070 6174 6965 6e74  d on the patient
-00001110: 5c27 7320 7068 656e 6f74 7970 652e 0a34  \'s phenotype..4
-00001120: 2e20 4765 6e65 2061 6e64 2064 6973 6561  . Gene and disea
-00001130: 7365 2072 6563 6f6d 6d65 6e64 6174 696f  se recommendatio
-00001140: 6e20 6261 7365 6420 6f6e 2074 6865 2070  n based on the p
-00001150: 6865 6e6f 7479 7065 2064 6174 6120 7369  henotype data si
-00001160: 6d69 6c61 7269 7479 2073 636f 7269 6e67  milarity scoring
-00001170: 2062 6574 7765 656e 202a 2a70 6865 6e6f   between **pheno
-00001180: 7479 7065 2a2a 2061 6e64 204f 4d49 4d20  type** and OMIM 
-00001190: 6765 6e65 2061 6e64 2064 6973 6561 7365  gene and disease
-000011a0: 2064 6174 6162 616e 6b2e 0a35 2e20 4c69   databank..5. Li
-000011b0: 6e6b 6167 6520 616e 616c 7973 6973 206f  nkage analysis o
-000011c0: 6620 7265 636f 6d6d 656e 6465 6420 6361  f recommended ca
-000011d0: 7573 6174 6976 6520 6765 6e65 2061 6e64  usative gene and
-000011e0: 2064 6973 6561 7365 2062 6173 6564 206f   disease based o
-000011f0: 6e20 7068 656e 6f74 7970 6520 6461 7461  n phenotype data
-00001200: 2028 696e 636c 7564 6520 6465 6e64 726f   (include dendro
-00001210: 6772 616d 2074 7265 6520 7669 7375 616c  gram tree visual
-00001220: 697a 6174 696f 6e29 2e0a 2020 2020 2d20  ization)..    - 
-00001230: 5468 6973 2073 686f 756c 6420 6865 6c70  This should help
-00001240: 2063 6c69 6e69 6369 616e 2074 6f20 2a2a   clinician to **
-00001250: 6578 706c 6f72 6520 2f20 656e 7269 6368  explore / enrich
-00001260: 2074 6865 6972 2064 6966 6665 7265 6e74   their different
-00001270: 6961 6c20 6469 6167 6e6f 7369 732a 2a20  ial diagnosis** 
-00001280: 6261 7365 6420 6f6e 2074 6865 2070 6174  based on the pat
-00001290: 6965 6e74 5c27 7320 7068 656e 6f74 7970  ient\'s phenotyp
-000012a0: 652e 0a36 2e20 4578 616d 706c 6520 6f66  e..6. Example of
-000012b0: 2074 6865 2063 6c69 6e69 6361 6c20 6461   the clinical da
-000012c0: 7461 2070 726f 7669 6465 6420 6174 205b  ta provided at [
-000012d0: 436c 696e 6963 616c 2049 6e66 6f72 6d61  Clinical Informa
-000012e0: 7469 6f6e 2045 7861 6d70 6c65 2073 6563  tion Example sec
-000012f0: 7469 6f6e 5d28 2363 6c69 6e69 6361 6c2d  tion](#clinical-
-00001300: 696e 666f 726d 6174 696f 6e2d 6578 616d  information-exam
-00001310: 706c 6529 0a0a 3c21 2d2d 2065 6e64 2074  ple)..<!-- end t
-00001320: 6167 6c69 6e65 202d 2d3e 0a0a 3c70 2061  agline -->..<p a
-00001330: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00001340: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00001350: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
-00001360: 7661 6e77 696c 6c69 616d 6d64 2f69 6465  vanwilliammd/ide
-00001370: 7261 7265 2d70 6865 6e6f 2f61 6374 696f  rare-pheno/actio
-00001380: 6e73 223e 0a20 2020 2020 2020 203c 696d  ns">.        <im
-00001390: 6720 616c 743d 2243 4922 2073 7263 3d22  g alt="CI" src="
-000013a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000013b0: 6f6d 2f69 7661 6e77 696c 6c69 616d 6d64  om/ivanwilliammd
-000013c0: 2f69 6465 7261 7265 2d70 6865 6e6f 2f77  /iderare-pheno/w
-000013d0: 6f72 6b66 6c6f 7773 2f4d 6169 6e2f 6261  orkflows/Main/ba
-000013e0: 6467 652e 7376 6722 3e0a 2020 2020 3c2f  dge.svg">.    </
-000013f0: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
-00001400: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00001410: 2f70 726f 6a65 6374 2f69 6465 7261 7265  /project/iderare
-00001420: 5f70 6865 6e6f 2f22 3e0a 2020 2020 2020  _pheno/">.      
-00001430: 2020 3c69 6d67 2061 6c74 3d22 5079 5049    <img alt="PyPI
-00001440: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00001450: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00001460: 7069 2f76 2f69 6465 7261 7265 5f70 6865  pi/v/iderare_phe
-00001470: 6e6f 223e 0a20 2020 203c 2f61 3e0a 2020  no">.    </a>.  
-00001480: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00001490: 3a2f 2f69 6465 7261 7265 2d70 6865 6e6f  ://iderare-pheno
-000014a0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000014b0: 656e 2f6c 6174 6573 742f 3f62 6164 6765  en/latest/?badge
-000014c0: 3d6c 6174 6573 7422 3e0a 2020 2020 2020  =latest">.      
-000014d0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-000014e0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
-000014f0: 6f72 672f 7072 6f6a 6563 7473 2f69 6465  org/projects/ide
-00001500: 7261 7265 2d70 6865 6e6f 2f62 6164 6765  rare-pheno/badge
-00001510: 2f3f 7665 7273 696f 6e3d 6c61 7465 7374  /?version=latest
-00001520: 2220 616c 743d 2244 6f63 756d 656e 7461  " alt="Documenta
-00001530: 7469 6f6e 2053 7461 7475 7322 202f 3e0a  tion Status" />.
-00001540: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
-00001550: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001560: 7468 7562 2e63 6f6d 2f69 7661 6e77 696c  thub.com/ivanwil
-00001570: 6c69 616d 6d64 2f69 6465 7261 7265 2d70  liammd/iderare-p
-00001580: 6865 6e6f 2f62 6c6f 622f 6d61 696e 2f4c  heno/blob/main/L
-00001590: 4943 454e 5345 223e 0a20 2020 2020 2020  ICENSE">.       
-000015a0: 203c 696d 6720 616c 743d 224c 6963 656e   <img alt="Licen
-000015b0: 7365 2220 7372 633d 2268 7474 7073 3a2f  se" src="https:/
-000015c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000015d0: 6769 7468 7562 2f6c 6963 656e 7365 2f69  github/license/i
-000015e0: 7661 6e77 696c 6c69 616d 6d64 2f69 6465  vanwilliammd/ide
-000015f0: 7261 7265 2d70 6865 6e6f 2e73 7667 3f63  rare-pheno.svg?c
-00001600: 6f6c 6f72 3d62 6c75 6526 6361 6368 6564  olor=blue&cached
-00001610: 726f 7022 3e0a 2020 2020 3c2f 613e 0a20  rop">.    </a>. 
-00001620: 2020 203c 6272 2f3e 0a3c 2f70 3e0a 0a23     <br/>.</p>..#
-00001630: 2320 5175 6963 6b20 6c69 6e6b 730a 0a2d  # Quick links..-
-00001640: 205b 446f 6375 6d65 6e74 6174 696f 6e5d   [Documentation]
-00001650: 2868 7474 7073 3a2f 2f69 6465 7261 7265  (https://iderare
-00001660: 2d70 6865 6e6f 2e72 6561 6474 6865 646f  -pheno.readthedo
-00001670: 6373 2e69 6f2f 290a 2d20 5b50 7950 4920  cs.io/).- [PyPI 
-00001680: 5061 636b 6167 655d 2868 7474 7073 3a2f  Package](https:/
-00001690: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-000016a0: 742f 6964 6572 6172 652d 7068 656e 6f2f  t/iderare-pheno/
-000016b0: 290a 2d20 5b4c 6963 656e 7365 5d28 6874  ).- [License](ht
-000016c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000016d0: 2f69 7661 6e77 696c 6c69 616d 6d64 2f69  /ivanwilliammd/i
-000016e0: 6465 7261 7265 2d70 6865 6e6f 2f62 6c6f  derare-pheno/blo
-000016f0: 622f 6d61 696e 2f4c 4943 454e 5345 290a  b/main/LICENSE).
-00001700: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00001710: 0a0a 3c21 2d2d 2073 7461 7274 2070 7920  ..<!-- start py 
-00001720: 7665 7273 696f 6e20 2d2d 3e0a 0a2a 2a69  version -->..**i
-00001730: 6465 7261 7265 2d70 6865 6e6f 2a2a 2072  derare-pheno** r
-00001740: 6571 7569 7265 7320 5079 7468 6f6e 2033  equires Python 3
-00001750: 2e38 206f 7220 6c61 7465 722e 0a0a 3c21  .8 or later...<!
-00001760: 2d2d 2065 6e64 2070 7920 7665 7273 696f  -- end py versio
-00001770: 6e20 2d2d 3e0a 0a23 2323 2049 6e73 7461  n -->..### Insta
-00001780: 6c6c 696e 6720 7769 7468 2060 7069 7060  lling with `pip`
-00001790: 0a0a 3c21 2d2d 2073 7461 7274 2069 6e73  ..<!-- start ins
-000017a0: 7461 6c6c 2070 6970 202d 2d3e 0a0a 2a2a  tall pip -->..**
-000017b0: 6964 6572 6172 652d 7068 656e 6f2a 2a20  iderare-pheno** 
-000017c0: 6973 2061 7661 696c 6162 6c65 205b 6f6e  is available [on
-000017d0: 2050 7950 495d 2868 7474 7073 3a2f 2f70   PyPI](https://p
-000017e0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-000017f0: 6964 6572 6172 652d 7068 656e 6f2f 292e  iderare-pheno/).
-00001800: 204a 7573 7420 7275 6e0a 0a60 6060 6261   Just run..```ba
-00001810: 7368 0a70 6970 2069 6e73 7461 6c6c 2069  sh.pip install i
-00001820: 6465 7261 7265 2d70 6865 6e6f 0a60 6060  derare-pheno.```
-00001830: 0a0a 3c21 2d2d 2065 6e64 2069 6e73 7461  ..<!-- end insta
-00001840: 6c6c 2070 6970 202d 2d3e 0a0a 2323 2320  ll pip -->..### 
-00001850: 496e 7374 616c 6c69 6e67 2066 726f 6d20  Installing from 
-00001860: 736f 7572 6365 0a0a 3c21 2d2d 2073 7461  source..<!-- sta
-00001870: 7274 2069 6e73 7461 6c6c 2073 6f75 7263  rt install sourc
-00001880: 6520 2d2d 3e0a 0a54 6f20 696e 7374 616c  e -->..To instal
-00001890: 6c20 2a2a 6964 6572 6172 652d 7068 656e  l **iderare-phen
-000018a0: 6f2a 2a20 6672 6f6d 2073 6f75 7263 652c  o** from source,
-000018b0: 2066 6972 7374 2063 6c6f 6e65 205b 7468   first clone [th
-000018c0: 6520 7265 706f 7369 746f 7279 5d28 6874  e repository](ht
-000018d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000018e0: 2f69 7661 6e77 696c 6c69 616d 6d64 2f69  /ivanwilliammd/i
-000018f0: 6465 7261 7265 2d70 6865 6e6f 293a 0a0a  derare-pheno):..
-00001900: 6060 6062 6173 680a 6769 7420 636c 6f6e  ```bash.git clon
-00001910: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-00001920: 2e63 6f6d 2f69 7661 6e77 696c 6c69 616d  .com/ivanwilliam
-00001930: 6d64 2f69 6465 7261 7265 2d70 6865 6e6f  md/iderare-pheno
-00001940: 2e67 6974 0a63 6420 6964 6572 6172 655f  .git.cd iderare_
-00001950: 7068 656e 6f0a 6060 600a 0a54 6865 6e20  pheno.```..Then 
-00001960: 7275 6e0a 0a60 6060 6261 7368 0a70 6970  run..```bash.pip
-00001970: 2069 6e73 7461 6c6c 202d 6520 2e0a 6060   install -e ..``
-00001980: 600a 0a3c 212d 2d20 656e 6420 696e 7374  `..<!-- end inst
-00001990: 616c 6c20 736f 7572 6365 202d 2d3e 0a0a  all source -->..
-000019a0: 2323 2055 7361 6765 0a0a 6060 6070 7974  ## Usage..```pyt
-000019b0: 686f 6e0a 6672 6f6d 2069 6465 7261 7265  hon.from iderare
-000019c0: 5f70 6865 6e6f 2069 6d70 6f72 7420 6964  _pheno import id
-000019d0: 6572 6172 655f 7068 656e 6f0a 6060 600a  erare_pheno.```.
-000019e0: 0a23 2320 5465 616d 0a0a 3c21 2d2d 2073  .## Team..<!-- s
-000019f0: 7461 7274 2074 6561 6d20 2d2d 3e0a 0a2a  tart team -->..*
-00001a00: 2a69 6465 7261 7265 2d70 6865 6e6f 2a2a  *iderare-pheno**
-00001a10: 2069 7320 6465 7665 6c6f 7065 6420 616e   is developed an
-00001a20: 6420 6d61 696e 7461 696e 6564 2062 7920  d maintained by 
-00001a30: 7468 6520 6175 7468 6f72 2873 292c 2054  the author(s), T
-00001a40: 6f20 6c65 6172 6e20 6d6f 7265 2061 626f  o learn more abo
-00001a50: 7574 2077 686f 2073 7065 6369 6669 6361  ut who specifica
-00001a60: 6c6c 7920 636f 6e74 7269 6275 7465 6420  lly contributed 
-00001a70: 746f 2074 6869 7320 636f 6465 6261 7365  to this codebase
-00001a80: 2c20 7365 6520 5b6f 7572 2063 6f6e 7472  , see [our contr
-00001a90: 6962 7574 6f72 735d 2868 7474 7073 3a2f  ibutors](https:/
-00001aa0: 2f67 6974 6875 622e 636f 6d2f 6976 616e  /github.com/ivan
-00001ab0: 7769 6c6c 6961 6d6d 642f 6964 6572 6172  williammd/iderar
-00001ac0: 652d 7068 656e 6f2f 6772 6170 6873 2f63  e-pheno/graphs/c
-00001ad0: 6f6e 7472 6962 7574 6f72 7329 2070 6167  ontributors) pag
-00001ae0: 652e 0a0a 3c21 2d2d 2065 6e64 2074 6561  e...<!-- end tea
-00001af0: 6d20 2d2d 3e0a 0a23 2320 4c69 6365 6e73  m -->..## Licens
-00001b00: 650a 0a3c 212d 2d20 7374 6172 7420 6c69  e..<!-- start li
-00001b10: 6365 6e73 6520 2d2d 3e0a 0a2a 2a69 6465  cense -->..**ide
-00001b20: 7261 7265 2d70 6865 6e6f 2a2a 206c 6963  rare-pheno** lic
-00001b30: 656e 7365 2069 7320 6465 7269 7665 6420  ense is derived 
-00001b40: 6672 6f6d 205b 4944 6552 6172 655d 2868  from [IDeRare](h
-00001b50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001b60: 6d2f 6976 616e 7769 6c6c 6961 6d6d 642f  m/ivanwilliammd/
-00001b70: 6964 6572 6172 6529 0a0a 3c21 2d2d 2065  iderare)..<!-- e
-00001b80: 6e64 206c 6963 656e 7365 202d 2d3e 0a    nd license -->.
+00000e00: 0a3c 212d 2d20 656e 6420 7461 676c 696e  .<!-- end taglin
+00000e10: 6520 2d2d 3e0a 0a3c 7020 616c 6967 6e3d  e -->..<p align=
+00000e20: 2263 656e 7465 7222 3e0a 2020 2020 3c61  "center">.    <a
+00000e30: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000e40: 6974 6875 622e 636f 6d2f 6976 616e 7769  ithub.com/ivanwi
+00000e50: 6c6c 6961 6d6d 642f 6964 6572 6172 652d  lliammd/iderare-
+00000e60: 7068 656e 6f2f 6163 7469 6f6e 7322 3e0a  pheno/actions">.
+00000e70: 2020 2020 2020 2020 3c69 6d67 2061 6c74          <img alt
+00000e80: 3d22 4349 2220 7372 633d 2268 7474 7073  ="CI" src="https
+00000e90: 3a2f 2f67 6974 6875 622e 636f 6d2f 6976  ://github.com/iv
+00000ea0: 616e 7769 6c6c 6961 6d6d 642f 6964 6572  anwilliammd/ider
+00000eb0: 6172 652d 7068 656e 6f2f 776f 726b 666c  are-pheno/workfl
+00000ec0: 6f77 732f 4d61 696e 2f62 6164 6765 2e73  ows/Main/badge.s
+00000ed0: 7667 223e 0a20 2020 203c 2f61 3e0a 2020  vg">.    </a>.  
+00000ee0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000ef0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000f00: 6563 742f 6964 6572 6172 655f 7068 656e  ect/iderare_phen
+00000f10: 6f2f 223e 0a20 2020 2020 2020 203c 696d  o/">.        <im
+00000f20: 6720 616c 743d 2250 7950 4922 2073 7263  g alt="PyPI" src
+00000f30: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000f40: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000f50: 6964 6572 6172 655f 7068 656e 6f22 3e0a  iderare_pheno">.
+00000f60: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
+00000f70: 6872 6566 3d22 6874 7470 733a 2f2f 6964  href="https://id
+00000f80: 6572 6172 652d 7068 656e 6f2e 7265 6164  erare-pheno.read
+00000f90: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000fa0: 7465 7374 2f3f 6261 6467 653d 6c61 7465  test/?badge=late
+00000fb0: 7374 223e 0a20 2020 2020 2020 203c 696d  st">.        <im
+00000fc0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00000fd0: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
+00000fe0: 726f 6a65 6374 732f 6964 6572 6172 652d  rojects/iderare-
+00000ff0: 7068 656e 6f2f 6261 6467 652f 3f76 6572  pheno/badge/?ver
+00001000: 7369 6f6e 3d6c 6174 6573 7422 2061 6c74  sion=latest" alt
+00001010: 3d22 446f 6375 6d65 6e74 6174 696f 6e20  ="Documentation 
+00001020: 5374 6174 7573 2220 2f3e 0a20 2020 203c  Status" />.    <
+00001030: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+00001040: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001050: 636f 6d2f 6976 616e 7769 6c6c 6961 6d6d  com/ivanwilliamm
+00001060: 642f 6964 6572 6172 652d 7068 656e 6f2f  d/iderare-pheno/
+00001070: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00001080: 4522 3e0a 2020 2020 2020 2020 3c69 6d67  E">.        <img
+00001090: 2061 6c74 3d22 4c69 6365 6e73 6522 2073   alt="License" s
+000010a0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000010b0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+000010c0: 622f 6c69 6365 6e73 652f 6976 616e 7769  b/license/ivanwi
+000010d0: 6c6c 6961 6d6d 642f 6964 6572 6172 652d  lliammd/iderare-
+000010e0: 7068 656e 6f2e 7376 673f 636f 6c6f 723d  pheno.svg?color=
+000010f0: 626c 7565 2663 6163 6865 6472 6f70 223e  blue&cachedrop">
+00001100: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
+00001110: 2068 7265 663d 2268 7474 7073 3a2f 2f62   href="https://b
+00001120: 696f 696e 666f 726d 6174 6963 732d 6976  ioinformatics-iv
+00001130: 616e 7769 6c6c 6961 6d68 6172 736f 6e6f  anwilliamharsono
+00001140: 2e73 7472 6561 6d6c 6974 2e61 7070 2f49  .streamlit.app/I
+00001150: 4465 5261 7265 5f50 6865 6e6f 223e 0a20  DeRare_Pheno">. 
+00001160: 2020 2020 2020 203c 696d 6720 616c 743d         <img alt=
+00001170: 2253 7472 6561 6d6c 6974 2220 7372 633d  "Streamlit" src=
+00001180: 2268 7474 7073 3a2f 2f73 7461 7469 632e  "https://static.
+00001190: 7374 7265 616d 6c69 742e 696f 2f62 6164  streamlit.io/bad
+000011a0: 6765 732f 7374 7265 616d 6c69 745f 6261  ges/streamlit_ba
+000011b0: 6467 655f 626c 6163 6b5f 7768 6974 652e  dge_black_white.
+000011c0: 7376 6722 3e0a 2020 2020 3c62 722f 3e0a  svg">.    <br/>.
+000011d0: 3c2f 703e 0a0a 2323 2051 7569 636b 206c  </p>..## Quick l
+000011e0: 696e 6b73 0a0a 2d20 5b44 6f63 756d 656e  inks..- [Documen
+000011f0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00001200: 6964 6572 6172 652d 7068 656e 6f2e 7265  iderare-pheno.re
+00001210: 6164 7468 6564 6f63 732e 696f 2f29 0a2d  adthedocs.io/).-
+00001220: 205b 5079 5049 2050 6163 6b61 6765 5d28   [PyPI Package](
+00001230: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00001240: 2f70 726f 6a65 6374 2f69 6465 7261 7265  /project/iderare
+00001250: 2d70 6865 6e6f 2f29 0a2d 205b 4c69 6365  -pheno/).- [Lice
+00001260: 6e73 655d 2868 7474 7073 3a2f 2f67 6974  nse](https://git
+00001270: 6875 622e 636f 6d2f 6976 616e 7769 6c6c  hub.com/ivanwill
+00001280: 6961 6d6d 642f 6964 6572 6172 652d 7068  iammd/iderare-ph
+00001290: 656e 6f2f 626c 6f62 2f6d 6169 6e2f 4c49  eno/blob/main/LI
+000012a0: 4345 4e53 4529 0a2d 2049 6e74 6572 6163  CENSE).- Interac
+000012b0: 7469 7665 2057 6562 6170 7073 2049 6d70  tive Webapps Imp
+000012c0: 6c65 6d65 6e74 6174 696f 6e20 6f66 2061  lementation of a
+000012d0: 7420 5b53 7472 6561 6d6c 6974 5d28 6874  t [Streamlit](ht
+000012e0: 7470 733a 2f2f 6269 6f69 6e66 6f72 6d61  tps://bioinforma
+000012f0: 7469 6373 2d69 7661 6e77 696c 6c69 616d  tics-ivanwilliam
+00001300: 6861 7273 6f6e 6f2e 7374 7265 616d 6c69  harsono.streamli
+00001310: 7461 7070 2e63 6f6d 2f49 4465 5261 7265  tapp.com/IDeRare
+00001320: 5f50 6865 6e6f 290a 0a0a 2323 2057 6861  _Pheno)...## Wha
+00001330: 7420 646f 6573 2069 7420 646f 3f0a 0a54  t does it do?..T
+00001340: 6869 7320 7363 7269 7074 2069 7320 7265  his script is re
+00001350: 636f 6d6d 656e 6465 6420 6966 2079 6f75  commended if you
+00001360: 2077 6f75 6c64 206c 696b 6520 746f 2064   would like to d
+00001370: 6f20 636f 6e76 6572 7369 6f6e 2c20 6c69  o conversion, li
+00001380: 6e6b 6167 6520 616e 616c 7973 6973 2c20  nkage analysis, 
+00001390: 7369 6d69 6c61 7269 7479 2073 636f 7269  similarity scori
+000013a0: 6e67 2c20 616e 6420 6765 6e65 2d64 6973  ng, and gene-dis
+000013b0: 6561 7365 2072 6563 6f6d 6d65 6e64 6174  ease recommendat
+000013c0: 696f 6e20 6261 7365 6420 6f6e 2074 6865  ion based on the
+000013d0: 2070 6865 6e6f 7479 7065 2064 6174 6120   phenotype data 
+000013e0: 7072 6f76 6964 6564 2061 7420 5b63 6c69  provided at [cli
+000013f0: 6e69 6361 6c5f 6461 7461 2e74 7874 5d28  nical_data.txt](
+00001400: 636c 696e 6963 616c 5f64 6174 612e 7478  clinical_data.tx
+00001410: 7429 2e20 4675 6c6c 2066 6561 7475 7265  t). Full feature
+00001420: 203a 200a 312e 2043 6f6e 7665 7274 2074   : .1. Convert t
+00001430: 6865 2070 6865 6e6f 7479 7065 2064 6174  he phenotype dat
+00001440: 6120 746f 2048 504f 2063 6f64 6520 2861  a to HPO code (a
+00001450: 6363 6570 7420 6d69 7865 6420 534e 4f4d  ccept mixed SNOM
+00001460: 4544 2c20 4c4f 494e 432c 2061 6e64 2048  ED, LOINC, and H
+00001470: 504f 2063 6f64 6529 0a32 2e20 5369 6d69  PO code).2. Simi
+00001480: 6c61 7269 7479 2073 636f 7269 6e67 206f  larity scoring o
+00001490: 6620 6469 6666 6572 656e 7469 616c 2064  f differential d
+000014a0: 6961 676e 6f73 6973 0a33 2e20 4c69 6e6b  iagnosis.3. Link
+000014b0: 6167 6520 616e 616c 7973 6973 206f 6620  age analysis of 
+000014c0: 6469 6666 6572 656e 7469 616c 2064 6961  differential dia
+000014d0: 676e 6f73 6973 2028 6163 6365 7074 206d  gnosis (accept m
+000014e0: 6978 6564 2053 4e4f 4d45 442c 2049 4344  ixed SNOMED, ICD
+000014f0: 2d31 302c 204f 5250 4841 2c20 4f4d 494d  -10, ORPHA, OMIM
+00001500: 2063 6f64 6529 2c20 696e 636c 7564 6520   code), include 
+00001510: 6465 6e64 726f 6772 616d 2074 7265 6520  dendrogram tree 
+00001520: 7669 7375 616c 697a 6174 696f 6e2e 0a20  visualization.. 
+00001530: 2020 202d 2054 6869 7320 7368 6f75 6c64     - This should
+00001540: 2068 656c 7020 636c 696e 6963 6961 6e20   help clinician 
+00001550: 746f 202a 2a73 7973 7465 6d61 7469 6361  to **systematica
+00001560: 6c6c 7920 646f 696e 6720 776f 726b 2d75  lly doing work-u
+00001570: 7020 616e 6420 6578 636c 7564 696e 6720  p and excluding 
+00001580: 7369 6d69 6c61 7220 6469 6167 6e6f 7369  similar diagnosi
+00001590: 7320 746f 6765 7468 6572 2a2a 2062 6173  s together** bas
+000015a0: 6564 206f 6e20 7468 6520 7061 7469 656e  ed on the patien
+000015b0: 745c 2773 2070 6865 6e6f 7479 7065 2e0a  t\'s phenotype..
+000015c0: 342e 2047 656e 6520 616e 6420 6469 7365  4. Gene and dise
+000015d0: 6173 6520 7265 636f 6d6d 656e 6461 7469  ase recommendati
+000015e0: 6f6e 2062 6173 6564 206f 6e20 7468 6520  on based on the 
+000015f0: 7068 656e 6f74 7970 6520 6461 7461 2073  phenotype data s
+00001600: 696d 696c 6172 6974 7920 7363 6f72 696e  imilarity scorin
+00001610: 6720 6265 7477 6565 6e20 2a2a 7068 656e  g between **phen
+00001620: 6f74 7970 652a 2a20 616e 6420 4f4d 494d  otype** and OMIM
+00001630: 2067 656e 6520 616e 6420 6469 7365 6173   gene and diseas
+00001640: 6520 6461 7461 6261 6e6b 2e0a 352e 204c  e databank..5. L
+00001650: 696e 6b61 6765 2061 6e61 6c79 7369 7320  inkage analysis 
+00001660: 6f66 2072 6563 6f6d 6d65 6e64 6564 2063  of recommended c
+00001670: 6175 7361 7469 7665 2067 656e 6520 616e  ausative gene an
+00001680: 6420 6469 7365 6173 6520 6261 7365 6420  d disease based 
+00001690: 6f6e 2070 6865 6e6f 7479 7065 2064 6174  on phenotype dat
+000016a0: 6120 2869 6e63 6c75 6465 2064 656e 6472  a (include dendr
+000016b0: 6f67 7261 6d20 7472 6565 2076 6973 7561  ogram tree visua
+000016c0: 6c69 7a61 7469 6f6e 292e 0a20 2020 202d  lization)..    -
+000016d0: 2054 6869 7320 7368 6f75 6c64 2068 656c   This should hel
+000016e0: 7020 636c 696e 6963 6961 6e20 746f 202a  p clinician to *
+000016f0: 2a65 7870 6c6f 7265 202f 2065 6e72 6963  *explore / enric
+00001700: 6820 7468 6569 7220 6469 6666 6572 656e  h their differen
+00001710: 7469 616c 2064 6961 676e 6f73 6973 2a2a  tial diagnosis**
+00001720: 2062 6173 6564 206f 6e20 7468 6520 7061   based on the pa
+00001730: 7469 656e 745c 2773 2070 6865 6e6f 7479  tient\'s phenoty
+00001740: 7065 2e0a 362e 2045 7861 6d70 6c65 206f  pe..6. Example o
+00001750: 6620 7468 6520 636c 696e 6963 616c 2064  f the clinical d
+00001760: 6174 6120 7072 6f76 6964 6564 2061 7420  ata provided at 
+00001770: 5b43 6c69 6e69 6361 6c20 496e 666f 726d  [Clinical Inform
+00001780: 6174 696f 6e20 4578 616d 706c 6520 7365  ation Example se
+00001790: 6374 696f 6e5d 2823 636c 696e 6963 616c  ction](#clinical
+000017a0: 2d69 6e66 6f72 6d61 7469 6f6e 2d65 7861  -information-exa
+000017b0: 6d70 6c65 290a 0a0a 2323 2049 6e73 7461  mple)...## Insta
+000017c0: 6c6c 6174 696f 6e0a 0a3c 212d 2d20 7374  llation..<!-- st
+000017d0: 6172 7420 7079 2076 6572 7369 6f6e 202d  art py version -
+000017e0: 2d3e 0a0a 2a2a 6964 6572 6172 652d 7068  ->..**iderare-ph
+000017f0: 656e 6f2a 2a20 7265 7175 6972 6573 2050  eno** requires P
+00001800: 7974 686f 6e20 332e 3820 6f72 206c 6174  ython 3.8 or lat
+00001810: 6572 2e0a 0a3c 212d 2d20 656e 6420 7079  er...<!-- end py
+00001820: 2076 6572 7369 6f6e 202d 2d3e 0a0a 2323   version -->..##
+00001830: 2320 496e 7374 616c 6c69 6e67 2077 6974  # Installing wit
+00001840: 6820 6070 6970 600a 0a3c 212d 2d20 7374  h `pip`..<!-- st
+00001850: 6172 7420 696e 7374 616c 6c20 7069 7020  art install pip 
+00001860: 2d2d 3e0a 0a2a 2a69 6465 7261 7265 2d70  -->..**iderare-p
+00001870: 6865 6e6f 2a2a 2069 7320 6176 6169 6c61  heno** is availa
+00001880: 626c 6520 5b6f 6e20 5079 5049 5d28 6874  ble [on PyPI](ht
+00001890: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000018a0: 726f 6a65 6374 2f69 6465 7261 7265 2d70  roject/iderare-p
+000018b0: 6865 6e6f 2f29 2e20 4a75 7374 2072 756e  heno/). Just run
+000018c0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+000018d0: 7374 616c 6c20 6964 6572 6172 652d 7068  stall iderare-ph
+000018e0: 656e 6f0a 6060 600a 0a3c 212d 2d20 656e  eno.```..<!-- en
+000018f0: 6420 696e 7374 616c 6c20 7069 7020 2d2d  d install pip --
+00001900: 3e0a 0a23 2323 2049 6e73 7461 6c6c 696e  >..### Installin
+00001910: 6720 6672 6f6d 2073 6f75 7263 650a 0a3c  g from source..<
+00001920: 212d 2d20 7374 6172 7420 696e 7374 616c  !-- start instal
+00001930: 6c20 736f 7572 6365 202d 2d3e 0a0a 546f  l source -->..To
+00001940: 2069 6e73 7461 6c6c 202a 2a69 6465 7261   install **idera
+00001950: 7265 2d70 6865 6e6f 2a2a 2066 726f 6d20  re-pheno** from 
+00001960: 736f 7572 6365 2c20 6669 7273 7420 636c  source, first cl
+00001970: 6f6e 6520 5b74 6865 2072 6570 6f73 6974  one [the reposit
+00001980: 6f72 795d 2868 7474 7073 3a2f 2f67 6974  ory](https://git
+00001990: 6875 622e 636f 6d2f 6976 616e 7769 6c6c  hub.com/ivanwill
+000019a0: 6961 6d6d 642f 6964 6572 6172 652d 7068  iammd/iderare-ph
+000019b0: 656e 6f29 3a0a 0a60 6060 6261 7368 0a67  eno):..```bash.g
+000019c0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+000019d0: 2f67 6974 6875 622e 636f 6d2f 6976 616e  /github.com/ivan
+000019e0: 7769 6c6c 6961 6d6d 642f 6964 6572 6172  williammd/iderar
+000019f0: 652d 7068 656e 6f2e 6769 740a 6364 2069  e-pheno.git.cd i
+00001a00: 6465 7261 7265 5f70 6865 6e6f 0a60 6060  derare_pheno.```
+00001a10: 0a0a 5468 656e 2072 756e 0a0a 6060 6062  ..Then run..```b
+00001a20: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+00001a30: 2d65 202e 0a60 6060 0a0a 3c21 2d2d 2065  -e ..```..<!-- e
+00001a40: 6e64 2069 6e73 7461 6c6c 2073 6f75 7263  nd install sourc
+00001a50: 6520 2d2d 3e0a 0a23 2320 5573 6167 650a  e -->..## Usage.
+00001a60: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00001a70: 6964 6572 6172 655f 7068 656e 6f20 696d  iderare_pheno im
+00001a80: 706f 7274 2069 6465 7261 7265 5f70 6865  port iderare_phe
+00001a90: 6e6f 0a60 6060 0a0a 2323 2054 6561 6d0a  no.```..## Team.
+00001aa0: 0a3c 212d 2d20 7374 6172 7420 7465 616d  .<!-- start team
+00001ab0: 202d 2d3e 0a0a 2a2a 6964 6572 6172 652d   -->..**iderare-
+00001ac0: 7068 656e 6f2a 2a20 6973 2064 6576 656c  pheno** is devel
+00001ad0: 6f70 6564 2061 6e64 206d 6169 6e74 6169  oped and maintai
+00001ae0: 6e65 6420 6279 2074 6865 2061 7574 686f  ned by the autho
+00001af0: 7228 7329 2c20 546f 206c 6561 726e 206d  r(s), To learn m
+00001b00: 6f72 6520 6162 6f75 7420 7768 6f20 7370  ore about who sp
+00001b10: 6563 6966 6963 616c 6c79 2063 6f6e 7472  ecifically contr
+00001b20: 6962 7574 6564 2074 6f20 7468 6973 2063  ibuted to this c
+00001b30: 6f64 6562 6173 652c 2073 6565 205b 6f75  odebase, see [ou
+00001b40: 7220 636f 6e74 7269 6275 746f 7273 5d28  r contributors](
+00001b50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001b60: 6f6d 2f69 7661 6e77 696c 6c69 616d 6d64  om/ivanwilliammd
+00001b70: 2f69 6465 7261 7265 2d70 6865 6e6f 2f67  /iderare-pheno/g
+00001b80: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
+00001b90: 7273 2920 7061 6765 2e0a 0a3c 212d 2d20  rs) page...<!-- 
+00001ba0: 656e 6420 7465 616d 202d 2d3e 0a0a 2323  end team -->..##
+00001bb0: 204c 6963 656e 7365 0a0a 3c21 2d2d 2073   License..<!-- s
+00001bc0: 7461 7274 206c 6963 656e 7365 202d 2d3e  tart license -->
+00001bd0: 0a0a 2a2a 6964 6572 6172 652d 7068 656e  ..**iderare-phen
+00001be0: 6f2a 2a20 6c69 6365 6e73 6520 6973 2064  o** license is d
+00001bf0: 6572 6976 6564 2066 726f 6d20 5b49 4465  erived from [IDe
+00001c00: 5261 7265 5d28 6874 7470 733a 2f2f 6769  Rare](https://gi
+00001c10: 7468 7562 2e63 6f6d 2f69 7661 6e77 696c  thub.com/ivanwil
+00001c20: 6c69 616d 6d64 2f69 6465 7261 7265 290a  liammd/iderare).
+00001c30: 0a3c 212d 2d20 656e 6420 6c69 6365 6e73  .<!-- end licens
+00001c40: 6520 2d2d 3e0a                           e -->.
```

### Comparing `iderare-pheno-0.1.7/README.md` & `iderare-pheno-0.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-# [IDeRare-pheno](https://iderare-pheno.readthedocs.io/)
+# [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/)
 
 <!-- start tagline -->
 
 IDeRare or "Indonesia Exome Rare Disease Variant Discovery Pipeline" is simple and ready to use variant discovery pipeline to discover rare disease variants from exome sequencing data.
-
-Interactive Webapps Implementation of **iderare_pheno.py** hosted at [Streamlit](https://bioinformatics-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno)
-
-This script is recommended if you would like to do conversion, linkage analysis, similarity scoring, and gene-disease recommendation based on the phenotype data provided at [clinical_data.txt](clinical_data.txt). Full feature : 
-1. Convert the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code)
-2. Similarity scoring of differential diagnosis
-3. Linkage analysis of differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include dendrogram tree visualization.
-    - This should help clinician to **systematically doing work-up and excluding similar diagnosis together** based on the patient\'s phenotype.
-4. Gene and disease recommendation based on the phenotype data similarity scoring between **phenotype** and OMIM gene and disease databank.
-5. Linkage analysis of recommended causative gene and disease based on phenotype data (include dendrogram tree visualization).
-    - This should help clinician to **explore / enrich their differential diagnosis** based on the patient\'s phenotype.
-6. Example of the clinical data provided at [Clinical Information Example section](#clinical-information-example)
-
 <!-- end tagline -->
 
 <p align="center">
     <a href="https://github.com/ivanwilliammd/iderare-pheno/actions">
         <img alt="CI" src="https://github.com/ivanwilliammd/iderare-pheno/workflows/Main/badge.svg">
     </a>
     <a href="https://pypi.org/project/iderare_pheno/">
@@ -27,22 +14,39 @@
     </a>
     <a href="https://iderare-pheno.readthedocs.io/en/latest/?badge=latest">
         <img src="https://readthedocs.org/projects/iderare-pheno/badge/?version=latest" alt="Documentation Status" />
     </a>
     <a href="https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE">
         <img alt="License" src="https://img.shields.io/github/license/ivanwilliammd/iderare-pheno.svg?color=blue&cachedrop">
     </a>
+    <a href="https://bioinformatics-ivanwilliamharsono.streamlit.app/IDeRare_Pheno">
+        <img alt="Streamlit" src="https://static.streamlit.io/badges/streamlit_badge_black_white.svg">
     <br/>
 </p>
 
 ## Quick links
 
 - [Documentation](https://iderare-pheno.readthedocs.io/)
 - [PyPI Package](https://pypi.org/project/iderare-pheno/)
 - [License](https://github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE)
+- Interactive Webapps Implementation of at [Streamlit](https://bioinformatics-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno)
+
+
+## What does it do?
+
+This script is recommended if you would like to do conversion, linkage analysis, similarity scoring, and gene-disease recommendation based on the phenotype data provided at [clinical_data.txt](clinical_data.txt). Full feature : 
+1. Convert the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code)
+2. Similarity scoring of differential diagnosis
+3. Linkage analysis of differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include dendrogram tree visualization.
+    - This should help clinician to **systematically doing work-up and excluding similar diagnosis together** based on the patient\'s phenotype.
+4. Gene and disease recommendation based on the phenotype data similarity scoring between **phenotype** and OMIM gene and disease databank.
+5. Linkage analysis of recommended causative gene and disease based on phenotype data (include dendrogram tree visualization).
+    - This should help clinician to **explore / enrich their differential diagnosis** based on the patient\'s phenotype.
+6. Example of the clinical data provided at [Clinical Information Example section](#clinical-information-example)
+
 
 ## Installation
 
 <!-- start py version -->
 
 **iderare-pheno** requires Python 3.8 or later.
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-# [IDeRare-pheno](https://iderare-pheno.readthedocs.io/) IDeRare or "Indonesia
+# [IDeRare-Pheno](https://iderare-pheno.readthedocs.io/) IDeRare or "Indonesia
 Exome Rare Disease Variant Discovery Pipeline" is simple and ready to use
 variant discovery pipeline to discover rare disease variants from exome
-sequencing data. Interactive Webapps Implementation of **iderare_pheno.py**
-hosted at [Streamlit](https://bioinformatics-
-ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) This script is recommended
-if you would like to do conversion, linkage analysis, similarity scoring, and
-gene-disease recommendation based on the phenotype data provided at
-[clinical_data.txt](clinical_data.txt). Full feature : 1. Convert the phenotype
-data to HPO code (accept mixed SNOMED, LOINC, and HPO code) 2. Similarity
-scoring of differential diagnosis 3. Linkage analysis of differential diagnosis
-(accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include dendrogram tree
-visualization. - This should help clinician to **systematically doing work-up
-and excluding similar diagnosis together** based on the patient\'s phenotype.
-4. Gene and disease recommendation based on the phenotype data similarity
-scoring between **phenotype** and OMIM gene and disease databank. 5. Linkage
-analysis of recommended causative gene and disease based on phenotype data
-(include dendrogram tree visualization). - This should help clinician to
-**explore / enrich their differential diagnosis** based on the patient\'s
-phenotype. 6. Example of the clinical data provided at [Clinical Information
-Example section](#clinical-information-example)
-                   _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]
+sequencing data.
+             _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
 ## Quick links - [Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI
 Package](https://pypi.org/project/iderare-pheno/) - [License](https://
-github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) ## Installation
+github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) - Interactive Webapps
+Implementation of at [Streamlit](https://bioinformatics-
+ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
+script is recommended if you would like to do conversion, linkage analysis,
+similarity scoring, and gene-disease recommendation based on the phenotype data
+provided at [clinical_data.txt](clinical_data.txt). Full feature : 1. Convert
+the phenotype data to HPO code (accept mixed SNOMED, LOINC, and HPO code) 2.
+Similarity scoring of differential diagnosis 3. Linkage analysis of
+differential diagnosis (accept mixed SNOMED, ICD-10, ORPHA, OMIM code), include
+dendrogram tree visualization. - This should help clinician to **systematically
+doing work-up and excluding similar diagnosis together** based on the
+patient\'s phenotype. 4. Gene and disease recommendation based on the phenotype
+data similarity scoring between **phenotype** and OMIM gene and disease
+databank. 5. Linkage analysis of recommended causative gene and disease based
+on phenotype data (include dendrogram tree visualization). - This should help
+clinician to **explore / enrich their differential diagnosis** based on the
+patient\'s phenotype. 6. Example of the clinical data provided at [Clinical
+Information Example section](#clinical-information-example) ## Installation
 **iderare-pheno** requires Python 3.8 or later. ### Installing with `pip`
 **iderare-pheno** is available [on PyPI](https://pypi.org/project/iderare-
 pheno/). Just run ```bash pip install iderare-pheno ``` ### Installing from
 source To install **iderare-pheno** from source, first clone [the repository]
 (https://github.com/ivanwilliammd/iderare-pheno): ```bash git clone https://
 github.com/ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run
 ```bash pip install -e . ``` ## Usage ```python from iderare_pheno import
```

### Comparing `iderare-pheno-0.1.7/iderare_pheno.egg-info/PKG-INFO` & `iderare-pheno-0.1.8/iderare_pheno.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6964 6572  : 2.1.Name: ider
 00000020: 6172 652d 7068 656e 6f0a 5665 7273 696f  are-pheno.Versio
-00000030: 6e3a 2030 2e31 2e37 0a41 7574 686f 722d  n: 0.1.7.Author-
+00000030: 6e3a 2030 2e31 2e38 0a41 7574 686f 722d  n: 0.1.8.Author-
 00000040: 656d 6169 6c3a 2049 7661 6e20 5769 6c6c  email: Ivan Will
 00000050: 6961 6d20 4861 7273 6f6e 6f20 3c63 6f6e  iam Harsono <con
 00000060: 7461 6374 4069 7661 6e77 696c 6c69 616d  tact@ivanwilliam
 00000070: 6d64 2e6f 7267 3e0a 4c69 6365 6e73 653a  md.org>.License:
 00000080: 2042 5344 2033 2d43 6c61 7573 6520 4c69   BSD 3-Clause Li
 00000090: 6365 6e73 650a 2020 2020 2020 2020 0a20  cense.        . 
 000000a0: 2020 2020 2020 2043 6f70 7972 6967 6874         Copyright
@@ -202,15 +202,15 @@
 00000c90: 6972 6573 2d44 6973 743a 2073 7068 696e  ires-Dist: sphin
 00000ca0: 782d 6175 746f 646f 632d 7479 7065 6869  x-autodoc-typehi
 00000cb0: 6e74 733d 3d31 2e32 332e 333b 2065 7874  nts==1.23.3; ext
 00000cc0: 7261 203d 3d20 2264 6576 220a 5265 7175  ra == "dev".Requ
 00000cd0: 6972 6573 2d44 6973 743a 2070 6163 6b61  ires-Dist: packa
 00000ce0: 6769 6e67 3b20 6578 7472 6120 3d3d 2022  ging; extra == "
 00000cf0: 6465 7622 0a0a 2320 5b49 4465 5261 7265  dev"..# [IDeRare
-00000d00: 2d70 6865 6e6f 5d28 6874 7470 733a 2f2f  -pheno](https://
+00000d00: 2d50 6865 6e6f 5d28 6874 7470 733a 2f2f  -Pheno](https://
 00000d10: 6964 6572 6172 652d 7068 656e 6f2e 7265  iderare-pheno.re
 00000d20: 6164 7468 6564 6f63 732e 696f 2f29 0a0a  adthedocs.io/)..
 00000d30: 3c21 2d2d 2073 7461 7274 2074 6167 6c69  <!-- start tagli
 00000d40: 6e65 202d 2d3e 0a0a 4944 6552 6172 6520  ne -->..IDeRare 
 00000d50: 6f72 2022 496e 646f 6e65 7369 6120 4578  or "Indonesia Ex
 00000d60: 6f6d 6520 5261 7265 2044 6973 6561 7365  ome Rare Disease
 00000d70: 2056 6172 6961 6e74 2044 6973 636f 7665   Variant Discove
@@ -218,224 +218,236 @@
 00000d90: 7369 6d70 6c65 2061 6e64 2072 6561 6479  simple and ready
 00000da0: 2074 6f20 7573 6520 7661 7269 616e 7420   to use variant 
 00000db0: 6469 7363 6f76 6572 7920 7069 7065 6c69  discovery pipeli
 00000dc0: 6e65 2074 6f20 6469 7363 6f76 6572 2072  ne to discover r
 00000dd0: 6172 6520 6469 7365 6173 6520 7661 7269  are disease vari
 00000de0: 616e 7473 2066 726f 6d20 6578 6f6d 6520  ants from exome 
 00000df0: 7365 7175 656e 6369 6e67 2064 6174 612e  sequencing data.
-00000e00: 0a0a 496e 7465 7261 6374 6976 6520 5765  ..Interactive We
-00000e10: 6261 7070 7320 496d 706c 656d 656e 7461  bapps Implementa
-00000e20: 7469 6f6e 206f 6620 2a2a 6964 6572 6172  tion of **iderar
-00000e30: 655f 7068 656e 6f2e 7079 2a2a 2068 6f73  e_pheno.py** hos
-00000e40: 7465 6420 6174 205b 5374 7265 616d 6c69  ted at [Streamli
-00000e50: 745d 2868 7474 7073 3a2f 2f62 696f 696e  t](https://bioin
-00000e60: 666f 726d 6174 6963 732d 6976 616e 7769  formatics-ivanwi
-00000e70: 6c6c 6961 6d68 6172 736f 6e6f 2e73 7472  lliamharsono.str
-00000e80: 6561 6d6c 6974 6170 702e 636f 6d2f 4944  eamlitapp.com/ID
-00000e90: 6552 6172 655f 5068 656e 6f29 0a0a 5468  eRare_Pheno)..Th
-00000ea0: 6973 2073 6372 6970 7420 6973 2072 6563  is script is rec
-00000eb0: 6f6d 6d65 6e64 6564 2069 6620 796f 7520  ommended if you 
-00000ec0: 776f 756c 6420 6c69 6b65 2074 6f20 646f  would like to do
-00000ed0: 2063 6f6e 7665 7273 696f 6e2c 206c 696e   conversion, lin
-00000ee0: 6b61 6765 2061 6e61 6c79 7369 732c 2073  kage analysis, s
-00000ef0: 696d 696c 6172 6974 7920 7363 6f72 696e  imilarity scorin
-00000f00: 672c 2061 6e64 2067 656e 652d 6469 7365  g, and gene-dise
-00000f10: 6173 6520 7265 636f 6d6d 656e 6461 7469  ase recommendati
-00000f20: 6f6e 2062 6173 6564 206f 6e20 7468 6520  on based on the 
-00000f30: 7068 656e 6f74 7970 6520 6461 7461 2070  phenotype data p
-00000f40: 726f 7669 6465 6420 6174 205b 636c 696e  rovided at [clin
-00000f50: 6963 616c 5f64 6174 612e 7478 745d 2863  ical_data.txt](c
-00000f60: 6c69 6e69 6361 6c5f 6461 7461 2e74 7874  linical_data.txt
-00000f70: 292e 2046 756c 6c20 6665 6174 7572 6520  ). Full feature 
-00000f80: 3a20 0a31 2e20 436f 6e76 6572 7420 7468  : .1. Convert th
-00000f90: 6520 7068 656e 6f74 7970 6520 6461 7461  e phenotype data
-00000fa0: 2074 6f20 4850 4f20 636f 6465 2028 6163   to HPO code (ac
-00000fb0: 6365 7074 206d 6978 6564 2053 4e4f 4d45  cept mixed SNOME
-00000fc0: 442c 204c 4f49 4e43 2c20 616e 6420 4850  D, LOINC, and HP
-00000fd0: 4f20 636f 6465 290a 322e 2053 696d 696c  O code).2. Simil
-00000fe0: 6172 6974 7920 7363 6f72 696e 6720 6f66  arity scoring of
-00000ff0: 2064 6966 6665 7265 6e74 6961 6c20 6469   differential di
-00001000: 6167 6e6f 7369 730a 332e 204c 696e 6b61  agnosis.3. Linka
-00001010: 6765 2061 6e61 6c79 7369 7320 6f66 2064  ge analysis of d
-00001020: 6966 6665 7265 6e74 6961 6c20 6469 6167  ifferential diag
-00001030: 6e6f 7369 7320 2861 6363 6570 7420 6d69  nosis (accept mi
-00001040: 7865 6420 534e 4f4d 4544 2c20 4943 442d  xed SNOMED, ICD-
-00001050: 3130 2c20 4f52 5048 412c 204f 4d49 4d20  10, ORPHA, OMIM 
-00001060: 636f 6465 292c 2069 6e63 6c75 6465 2064  code), include d
-00001070: 656e 6472 6f67 7261 6d20 7472 6565 2076  endrogram tree v
-00001080: 6973 7561 6c69 7a61 7469 6f6e 2e0a 2020  isualization..  
-00001090: 2020 2d20 5468 6973 2073 686f 756c 6420    - This should 
-000010a0: 6865 6c70 2063 6c69 6e69 6369 616e 2074  help clinician t
-000010b0: 6f20 2a2a 7379 7374 656d 6174 6963 616c  o **systematical
-000010c0: 6c79 2064 6f69 6e67 2077 6f72 6b2d 7570  ly doing work-up
-000010d0: 2061 6e64 2065 7863 6c75 6469 6e67 2073   and excluding s
-000010e0: 696d 696c 6172 2064 6961 676e 6f73 6973  imilar diagnosis
-000010f0: 2074 6f67 6574 6865 722a 2a20 6261 7365   together** base
-00001100: 6420 6f6e 2074 6865 2070 6174 6965 6e74  d on the patient
-00001110: 5c27 7320 7068 656e 6f74 7970 652e 0a34  \'s phenotype..4
-00001120: 2e20 4765 6e65 2061 6e64 2064 6973 6561  . Gene and disea
-00001130: 7365 2072 6563 6f6d 6d65 6e64 6174 696f  se recommendatio
-00001140: 6e20 6261 7365 6420 6f6e 2074 6865 2070  n based on the p
-00001150: 6865 6e6f 7479 7065 2064 6174 6120 7369  henotype data si
-00001160: 6d69 6c61 7269 7479 2073 636f 7269 6e67  milarity scoring
-00001170: 2062 6574 7765 656e 202a 2a70 6865 6e6f   between **pheno
-00001180: 7479 7065 2a2a 2061 6e64 204f 4d49 4d20  type** and OMIM 
-00001190: 6765 6e65 2061 6e64 2064 6973 6561 7365  gene and disease
-000011a0: 2064 6174 6162 616e 6b2e 0a35 2e20 4c69   databank..5. Li
-000011b0: 6e6b 6167 6520 616e 616c 7973 6973 206f  nkage analysis o
-000011c0: 6620 7265 636f 6d6d 656e 6465 6420 6361  f recommended ca
-000011d0: 7573 6174 6976 6520 6765 6e65 2061 6e64  usative gene and
-000011e0: 2064 6973 6561 7365 2062 6173 6564 206f   disease based o
-000011f0: 6e20 7068 656e 6f74 7970 6520 6461 7461  n phenotype data
-00001200: 2028 696e 636c 7564 6520 6465 6e64 726f   (include dendro
-00001210: 6772 616d 2074 7265 6520 7669 7375 616c  gram tree visual
-00001220: 697a 6174 696f 6e29 2e0a 2020 2020 2d20  ization)..    - 
-00001230: 5468 6973 2073 686f 756c 6420 6865 6c70  This should help
-00001240: 2063 6c69 6e69 6369 616e 2074 6f20 2a2a   clinician to **
-00001250: 6578 706c 6f72 6520 2f20 656e 7269 6368  explore / enrich
-00001260: 2074 6865 6972 2064 6966 6665 7265 6e74   their different
-00001270: 6961 6c20 6469 6167 6e6f 7369 732a 2a20  ial diagnosis** 
-00001280: 6261 7365 6420 6f6e 2074 6865 2070 6174  based on the pat
-00001290: 6965 6e74 5c27 7320 7068 656e 6f74 7970  ient\'s phenotyp
-000012a0: 652e 0a36 2e20 4578 616d 706c 6520 6f66  e..6. Example of
-000012b0: 2074 6865 2063 6c69 6e69 6361 6c20 6461   the clinical da
-000012c0: 7461 2070 726f 7669 6465 6420 6174 205b  ta provided at [
-000012d0: 436c 696e 6963 616c 2049 6e66 6f72 6d61  Clinical Informa
-000012e0: 7469 6f6e 2045 7861 6d70 6c65 2073 6563  tion Example sec
-000012f0: 7469 6f6e 5d28 2363 6c69 6e69 6361 6c2d  tion](#clinical-
-00001300: 696e 666f 726d 6174 696f 6e2d 6578 616d  information-exam
-00001310: 706c 6529 0a0a 3c21 2d2d 2065 6e64 2074  ple)..<!-- end t
-00001320: 6167 6c69 6e65 202d 2d3e 0a0a 3c70 2061  agline -->..<p a
-00001330: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00001340: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-00001350: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f69  s://github.com/i
-00001360: 7661 6e77 696c 6c69 616d 6d64 2f69 6465  vanwilliammd/ide
-00001370: 7261 7265 2d70 6865 6e6f 2f61 6374 696f  rare-pheno/actio
-00001380: 6e73 223e 0a20 2020 2020 2020 203c 696d  ns">.        <im
-00001390: 6720 616c 743d 2243 4922 2073 7263 3d22  g alt="CI" src="
-000013a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000013b0: 6f6d 2f69 7661 6e77 696c 6c69 616d 6d64  om/ivanwilliammd
-000013c0: 2f69 6465 7261 7265 2d70 6865 6e6f 2f77  /iderare-pheno/w
-000013d0: 6f72 6b66 6c6f 7773 2f4d 6169 6e2f 6261  orkflows/Main/ba
-000013e0: 6467 652e 7376 6722 3e0a 2020 2020 3c2f  dge.svg">.    </
-000013f0: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
-00001400: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00001410: 2f70 726f 6a65 6374 2f69 6465 7261 7265  /project/iderare
-00001420: 5f70 6865 6e6f 2f22 3e0a 2020 2020 2020  _pheno/">.      
-00001430: 2020 3c69 6d67 2061 6c74 3d22 5079 5049    <img alt="PyPI
-00001440: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
-00001450: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00001460: 7069 2f76 2f69 6465 7261 7265 5f70 6865  pi/v/iderare_phe
-00001470: 6e6f 223e 0a20 2020 203c 2f61 3e0a 2020  no">.    </a>.  
-00001480: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00001490: 3a2f 2f69 6465 7261 7265 2d70 6865 6e6f  ://iderare-pheno
-000014a0: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-000014b0: 656e 2f6c 6174 6573 742f 3f62 6164 6765  en/latest/?badge
-000014c0: 3d6c 6174 6573 7422 3e0a 2020 2020 2020  =latest">.      
-000014d0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-000014e0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
-000014f0: 6f72 672f 7072 6f6a 6563 7473 2f69 6465  org/projects/ide
-00001500: 7261 7265 2d70 6865 6e6f 2f62 6164 6765  rare-pheno/badge
-00001510: 2f3f 7665 7273 696f 6e3d 6c61 7465 7374  /?version=latest
-00001520: 2220 616c 743d 2244 6f63 756d 656e 7461  " alt="Documenta
-00001530: 7469 6f6e 2053 7461 7475 7322 202f 3e0a  tion Status" />.
-00001540: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
-00001550: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00001560: 7468 7562 2e63 6f6d 2f69 7661 6e77 696c  thub.com/ivanwil
-00001570: 6c69 616d 6d64 2f69 6465 7261 7265 2d70  liammd/iderare-p
-00001580: 6865 6e6f 2f62 6c6f 622f 6d61 696e 2f4c  heno/blob/main/L
-00001590: 4943 454e 5345 223e 0a20 2020 2020 2020  ICENSE">.       
-000015a0: 203c 696d 6720 616c 743d 224c 6963 656e   <img alt="Licen
-000015b0: 7365 2220 7372 633d 2268 7474 7073 3a2f  se" src="https:/
-000015c0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000015d0: 6769 7468 7562 2f6c 6963 656e 7365 2f69  github/license/i
-000015e0: 7661 6e77 696c 6c69 616d 6d64 2f69 6465  vanwilliammd/ide
-000015f0: 7261 7265 2d70 6865 6e6f 2e73 7667 3f63  rare-pheno.svg?c
-00001600: 6f6c 6f72 3d62 6c75 6526 6361 6368 6564  olor=blue&cached
-00001610: 726f 7022 3e0a 2020 2020 3c2f 613e 0a20  rop">.    </a>. 
-00001620: 2020 203c 6272 2f3e 0a3c 2f70 3e0a 0a23     <br/>.</p>..#
-00001630: 2320 5175 6963 6b20 6c69 6e6b 730a 0a2d  # Quick links..-
-00001640: 205b 446f 6375 6d65 6e74 6174 696f 6e5d   [Documentation]
-00001650: 2868 7474 7073 3a2f 2f69 6465 7261 7265  (https://iderare
-00001660: 2d70 6865 6e6f 2e72 6561 6474 6865 646f  -pheno.readthedo
-00001670: 6373 2e69 6f2f 290a 2d20 5b50 7950 4920  cs.io/).- [PyPI 
-00001680: 5061 636b 6167 655d 2868 7474 7073 3a2f  Package](https:/
-00001690: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-000016a0: 742f 6964 6572 6172 652d 7068 656e 6f2f  t/iderare-pheno/
-000016b0: 290a 2d20 5b4c 6963 656e 7365 5d28 6874  ).- [License](ht
-000016c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000016d0: 2f69 7661 6e77 696c 6c69 616d 6d64 2f69  /ivanwilliammd/i
-000016e0: 6465 7261 7265 2d70 6865 6e6f 2f62 6c6f  derare-pheno/blo
-000016f0: 622f 6d61 696e 2f4c 4943 454e 5345 290a  b/main/LICENSE).
-00001700: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00001710: 0a0a 3c21 2d2d 2073 7461 7274 2070 7920  ..<!-- start py 
-00001720: 7665 7273 696f 6e20 2d2d 3e0a 0a2a 2a69  version -->..**i
-00001730: 6465 7261 7265 2d70 6865 6e6f 2a2a 2072  derare-pheno** r
-00001740: 6571 7569 7265 7320 5079 7468 6f6e 2033  equires Python 3
-00001750: 2e38 206f 7220 6c61 7465 722e 0a0a 3c21  .8 or later...<!
-00001760: 2d2d 2065 6e64 2070 7920 7665 7273 696f  -- end py versio
-00001770: 6e20 2d2d 3e0a 0a23 2323 2049 6e73 7461  n -->..### Insta
-00001780: 6c6c 696e 6720 7769 7468 2060 7069 7060  lling with `pip`
-00001790: 0a0a 3c21 2d2d 2073 7461 7274 2069 6e73  ..<!-- start ins
-000017a0: 7461 6c6c 2070 6970 202d 2d3e 0a0a 2a2a  tall pip -->..**
-000017b0: 6964 6572 6172 652d 7068 656e 6f2a 2a20  iderare-pheno** 
-000017c0: 6973 2061 7661 696c 6162 6c65 205b 6f6e  is available [on
-000017d0: 2050 7950 495d 2868 7474 7073 3a2f 2f70   PyPI](https://p
-000017e0: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-000017f0: 6964 6572 6172 652d 7068 656e 6f2f 292e  iderare-pheno/).
-00001800: 204a 7573 7420 7275 6e0a 0a60 6060 6261   Just run..```ba
-00001810: 7368 0a70 6970 2069 6e73 7461 6c6c 2069  sh.pip install i
-00001820: 6465 7261 7265 2d70 6865 6e6f 0a60 6060  derare-pheno.```
-00001830: 0a0a 3c21 2d2d 2065 6e64 2069 6e73 7461  ..<!-- end insta
-00001840: 6c6c 2070 6970 202d 2d3e 0a0a 2323 2320  ll pip -->..### 
-00001850: 496e 7374 616c 6c69 6e67 2066 726f 6d20  Installing from 
-00001860: 736f 7572 6365 0a0a 3c21 2d2d 2073 7461  source..<!-- sta
-00001870: 7274 2069 6e73 7461 6c6c 2073 6f75 7263  rt install sourc
-00001880: 6520 2d2d 3e0a 0a54 6f20 696e 7374 616c  e -->..To instal
-00001890: 6c20 2a2a 6964 6572 6172 652d 7068 656e  l **iderare-phen
-000018a0: 6f2a 2a20 6672 6f6d 2073 6f75 7263 652c  o** from source,
-000018b0: 2066 6972 7374 2063 6c6f 6e65 205b 7468   first clone [th
-000018c0: 6520 7265 706f 7369 746f 7279 5d28 6874  e repository](ht
-000018d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000018e0: 2f69 7661 6e77 696c 6c69 616d 6d64 2f69  /ivanwilliammd/i
-000018f0: 6465 7261 7265 2d70 6865 6e6f 293a 0a0a  derare-pheno):..
-00001900: 6060 6062 6173 680a 6769 7420 636c 6f6e  ```bash.git clon
-00001910: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-00001920: 2e63 6f6d 2f69 7661 6e77 696c 6c69 616d  .com/ivanwilliam
-00001930: 6d64 2f69 6465 7261 7265 2d70 6865 6e6f  md/iderare-pheno
-00001940: 2e67 6974 0a63 6420 6964 6572 6172 655f  .git.cd iderare_
-00001950: 7068 656e 6f0a 6060 600a 0a54 6865 6e20  pheno.```..Then 
-00001960: 7275 6e0a 0a60 6060 6261 7368 0a70 6970  run..```bash.pip
-00001970: 2069 6e73 7461 6c6c 202d 6520 2e0a 6060   install -e ..``
-00001980: 600a 0a3c 212d 2d20 656e 6420 696e 7374  `..<!-- end inst
-00001990: 616c 6c20 736f 7572 6365 202d 2d3e 0a0a  all source -->..
-000019a0: 2323 2055 7361 6765 0a0a 6060 6070 7974  ## Usage..```pyt
-000019b0: 686f 6e0a 6672 6f6d 2069 6465 7261 7265  hon.from iderare
-000019c0: 5f70 6865 6e6f 2069 6d70 6f72 7420 6964  _pheno import id
-000019d0: 6572 6172 655f 7068 656e 6f0a 6060 600a  erare_pheno.```.
-000019e0: 0a23 2320 5465 616d 0a0a 3c21 2d2d 2073  .## Team..<!-- s
-000019f0: 7461 7274 2074 6561 6d20 2d2d 3e0a 0a2a  tart team -->..*
-00001a00: 2a69 6465 7261 7265 2d70 6865 6e6f 2a2a  *iderare-pheno**
-00001a10: 2069 7320 6465 7665 6c6f 7065 6420 616e   is developed an
-00001a20: 6420 6d61 696e 7461 696e 6564 2062 7920  d maintained by 
-00001a30: 7468 6520 6175 7468 6f72 2873 292c 2054  the author(s), T
-00001a40: 6f20 6c65 6172 6e20 6d6f 7265 2061 626f  o learn more abo
-00001a50: 7574 2077 686f 2073 7065 6369 6669 6361  ut who specifica
-00001a60: 6c6c 7920 636f 6e74 7269 6275 7465 6420  lly contributed 
-00001a70: 746f 2074 6869 7320 636f 6465 6261 7365  to this codebase
-00001a80: 2c20 7365 6520 5b6f 7572 2063 6f6e 7472  , see [our contr
-00001a90: 6962 7574 6f72 735d 2868 7474 7073 3a2f  ibutors](https:/
-00001aa0: 2f67 6974 6875 622e 636f 6d2f 6976 616e  /github.com/ivan
-00001ab0: 7769 6c6c 6961 6d6d 642f 6964 6572 6172  williammd/iderar
-00001ac0: 652d 7068 656e 6f2f 6772 6170 6873 2f63  e-pheno/graphs/c
-00001ad0: 6f6e 7472 6962 7574 6f72 7329 2070 6167  ontributors) pag
-00001ae0: 652e 0a0a 3c21 2d2d 2065 6e64 2074 6561  e...<!-- end tea
-00001af0: 6d20 2d2d 3e0a 0a23 2320 4c69 6365 6e73  m -->..## Licens
-00001b00: 650a 0a3c 212d 2d20 7374 6172 7420 6c69  e..<!-- start li
-00001b10: 6365 6e73 6520 2d2d 3e0a 0a2a 2a69 6465  cense -->..**ide
-00001b20: 7261 7265 2d70 6865 6e6f 2a2a 206c 6963  rare-pheno** lic
-00001b30: 656e 7365 2069 7320 6465 7269 7665 6420  ense is derived 
-00001b40: 6672 6f6d 205b 4944 6552 6172 655d 2868  from [IDeRare](h
-00001b50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001b60: 6d2f 6976 616e 7769 6c6c 6961 6d6d 642f  m/ivanwilliammd/
-00001b70: 6964 6572 6172 6529 0a0a 3c21 2d2d 2065  iderare)..<!-- e
-00001b80: 6e64 206c 6963 656e 7365 202d 2d3e 0a    nd license -->.
+00000e00: 0a3c 212d 2d20 656e 6420 7461 676c 696e  .<!-- end taglin
+00000e10: 6520 2d2d 3e0a 0a3c 7020 616c 6967 6e3d  e -->..<p align=
+00000e20: 2263 656e 7465 7222 3e0a 2020 2020 3c61  "center">.    <a
+00000e30: 2068 7265 663d 2268 7474 7073 3a2f 2f67   href="https://g
+00000e40: 6974 6875 622e 636f 6d2f 6976 616e 7769  ithub.com/ivanwi
+00000e50: 6c6c 6961 6d6d 642f 6964 6572 6172 652d  lliammd/iderare-
+00000e60: 7068 656e 6f2f 6163 7469 6f6e 7322 3e0a  pheno/actions">.
+00000e70: 2020 2020 2020 2020 3c69 6d67 2061 6c74          <img alt
+00000e80: 3d22 4349 2220 7372 633d 2268 7474 7073  ="CI" src="https
+00000e90: 3a2f 2f67 6974 6875 622e 636f 6d2f 6976  ://github.com/iv
+00000ea0: 616e 7769 6c6c 6961 6d6d 642f 6964 6572  anwilliammd/ider
+00000eb0: 6172 652d 7068 656e 6f2f 776f 726b 666c  are-pheno/workfl
+00000ec0: 6f77 732f 4d61 696e 2f62 6164 6765 2e73  ows/Main/badge.s
+00000ed0: 7667 223e 0a20 2020 203c 2f61 3e0a 2020  vg">.    </a>.  
+00000ee0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000ef0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000f00: 6563 742f 6964 6572 6172 655f 7068 656e  ect/iderare_phen
+00000f10: 6f2f 223e 0a20 2020 2020 2020 203c 696d  o/">.        <im
+00000f20: 6720 616c 743d 2250 7950 4922 2073 7263  g alt="PyPI" src
+00000f30: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000f40: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000f50: 6964 6572 6172 655f 7068 656e 6f22 3e0a  iderare_pheno">.
+00000f60: 2020 2020 3c2f 613e 0a20 2020 203c 6120      </a>.    <a 
+00000f70: 6872 6566 3d22 6874 7470 733a 2f2f 6964  href="https://id
+00000f80: 6572 6172 652d 7068 656e 6f2e 7265 6164  erare-pheno.read
+00000f90: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000fa0: 7465 7374 2f3f 6261 6467 653d 6c61 7465  test/?badge=late
+00000fb0: 7374 223e 0a20 2020 2020 2020 203c 696d  st">.        <im
+00000fc0: 6720 7372 633d 2268 7474 7073 3a2f 2f72  g src="https://r
+00000fd0: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
+00000fe0: 726f 6a65 6374 732f 6964 6572 6172 652d  rojects/iderare-
+00000ff0: 7068 656e 6f2f 6261 6467 652f 3f76 6572  pheno/badge/?ver
+00001000: 7369 6f6e 3d6c 6174 6573 7422 2061 6c74  sion=latest" alt
+00001010: 3d22 446f 6375 6d65 6e74 6174 696f 6e20  ="Documentation 
+00001020: 5374 6174 7573 2220 2f3e 0a20 2020 203c  Status" />.    <
+00001030: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+00001040: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00001050: 636f 6d2f 6976 616e 7769 6c6c 6961 6d6d  com/ivanwilliamm
+00001060: 642f 6964 6572 6172 652d 7068 656e 6f2f  d/iderare-pheno/
+00001070: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
+00001080: 4522 3e0a 2020 2020 2020 2020 3c69 6d67  E">.        <img
+00001090: 2061 6c74 3d22 4c69 6365 6e73 6522 2073   alt="License" s
+000010a0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000010b0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+000010c0: 622f 6c69 6365 6e73 652f 6976 616e 7769  b/license/ivanwi
+000010d0: 6c6c 6961 6d6d 642f 6964 6572 6172 652d  lliammd/iderare-
+000010e0: 7068 656e 6f2e 7376 673f 636f 6c6f 723d  pheno.svg?color=
+000010f0: 626c 7565 2663 6163 6865 6472 6f70 223e  blue&cachedrop">
+00001100: 0a20 2020 203c 2f61 3e0a 2020 2020 3c61  .    </a>.    <a
+00001110: 2068 7265 663d 2268 7474 7073 3a2f 2f62   href="https://b
+00001120: 696f 696e 666f 726d 6174 6963 732d 6976  ioinformatics-iv
+00001130: 616e 7769 6c6c 6961 6d68 6172 736f 6e6f  anwilliamharsono
+00001140: 2e73 7472 6561 6d6c 6974 2e61 7070 2f49  .streamlit.app/I
+00001150: 4465 5261 7265 5f50 6865 6e6f 223e 0a20  DeRare_Pheno">. 
+00001160: 2020 2020 2020 203c 696d 6720 616c 743d         <img alt=
+00001170: 2253 7472 6561 6d6c 6974 2220 7372 633d  "Streamlit" src=
+00001180: 2268 7474 7073 3a2f 2f73 7461 7469 632e  "https://static.
+00001190: 7374 7265 616d 6c69 742e 696f 2f62 6164  streamlit.io/bad
+000011a0: 6765 732f 7374 7265 616d 6c69 745f 6261  ges/streamlit_ba
+000011b0: 6467 655f 626c 6163 6b5f 7768 6974 652e  dge_black_white.
+000011c0: 7376 6722 3e0a 2020 2020 3c62 722f 3e0a  svg">.    <br/>.
+000011d0: 3c2f 703e 0a0a 2323 2051 7569 636b 206c  </p>..## Quick l
+000011e0: 696e 6b73 0a0a 2d20 5b44 6f63 756d 656e  inks..- [Documen
+000011f0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+00001200: 6964 6572 6172 652d 7068 656e 6f2e 7265  iderare-pheno.re
+00001210: 6164 7468 6564 6f63 732e 696f 2f29 0a2d  adthedocs.io/).-
+00001220: 205b 5079 5049 2050 6163 6b61 6765 5d28   [PyPI Package](
+00001230: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00001240: 2f70 726f 6a65 6374 2f69 6465 7261 7265  /project/iderare
+00001250: 2d70 6865 6e6f 2f29 0a2d 205b 4c69 6365  -pheno/).- [Lice
+00001260: 6e73 655d 2868 7474 7073 3a2f 2f67 6974  nse](https://git
+00001270: 6875 622e 636f 6d2f 6976 616e 7769 6c6c  hub.com/ivanwill
+00001280: 6961 6d6d 642f 6964 6572 6172 652d 7068  iammd/iderare-ph
+00001290: 656e 6f2f 626c 6f62 2f6d 6169 6e2f 4c49  eno/blob/main/LI
+000012a0: 4345 4e53 4529 0a2d 2049 6e74 6572 6163  CENSE).- Interac
+000012b0: 7469 7665 2057 6562 6170 7073 2049 6d70  tive Webapps Imp
+000012c0: 6c65 6d65 6e74 6174 696f 6e20 6f66 2061  lementation of a
+000012d0: 7420 5b53 7472 6561 6d6c 6974 5d28 6874  t [Streamlit](ht
+000012e0: 7470 733a 2f2f 6269 6f69 6e66 6f72 6d61  tps://bioinforma
+000012f0: 7469 6373 2d69 7661 6e77 696c 6c69 616d  tics-ivanwilliam
+00001300: 6861 7273 6f6e 6f2e 7374 7265 616d 6c69  harsono.streamli
+00001310: 7461 7070 2e63 6f6d 2f49 4465 5261 7265  tapp.com/IDeRare
+00001320: 5f50 6865 6e6f 290a 0a0a 2323 2057 6861  _Pheno)...## Wha
+00001330: 7420 646f 6573 2069 7420 646f 3f0a 0a54  t does it do?..T
+00001340: 6869 7320 7363 7269 7074 2069 7320 7265  his script is re
+00001350: 636f 6d6d 656e 6465 6420 6966 2079 6f75  commended if you
+00001360: 2077 6f75 6c64 206c 696b 6520 746f 2064   would like to d
+00001370: 6f20 636f 6e76 6572 7369 6f6e 2c20 6c69  o conversion, li
+00001380: 6e6b 6167 6520 616e 616c 7973 6973 2c20  nkage analysis, 
+00001390: 7369 6d69 6c61 7269 7479 2073 636f 7269  similarity scori
+000013a0: 6e67 2c20 616e 6420 6765 6e65 2d64 6973  ng, and gene-dis
+000013b0: 6561 7365 2072 6563 6f6d 6d65 6e64 6174  ease recommendat
+000013c0: 696f 6e20 6261 7365 6420 6f6e 2074 6865  ion based on the
+000013d0: 2070 6865 6e6f 7479 7065 2064 6174 6120   phenotype data 
+000013e0: 7072 6f76 6964 6564 2061 7420 5b63 6c69  provided at [cli
+000013f0: 6e69 6361 6c5f 6461 7461 2e74 7874 5d28  nical_data.txt](
+00001400: 636c 696e 6963 616c 5f64 6174 612e 7478  clinical_data.tx
+00001410: 7429 2e20 4675 6c6c 2066 6561 7475 7265  t). Full feature
+00001420: 203a 200a 312e 2043 6f6e 7665 7274 2074   : .1. Convert t
+00001430: 6865 2070 6865 6e6f 7479 7065 2064 6174  he phenotype dat
+00001440: 6120 746f 2048 504f 2063 6f64 6520 2861  a to HPO code (a
+00001450: 6363 6570 7420 6d69 7865 6420 534e 4f4d  ccept mixed SNOM
+00001460: 4544 2c20 4c4f 494e 432c 2061 6e64 2048  ED, LOINC, and H
+00001470: 504f 2063 6f64 6529 0a32 2e20 5369 6d69  PO code).2. Simi
+00001480: 6c61 7269 7479 2073 636f 7269 6e67 206f  larity scoring o
+00001490: 6620 6469 6666 6572 656e 7469 616c 2064  f differential d
+000014a0: 6961 676e 6f73 6973 0a33 2e20 4c69 6e6b  iagnosis.3. Link
+000014b0: 6167 6520 616e 616c 7973 6973 206f 6620  age analysis of 
+000014c0: 6469 6666 6572 656e 7469 616c 2064 6961  differential dia
+000014d0: 676e 6f73 6973 2028 6163 6365 7074 206d  gnosis (accept m
+000014e0: 6978 6564 2053 4e4f 4d45 442c 2049 4344  ixed SNOMED, ICD
+000014f0: 2d31 302c 204f 5250 4841 2c20 4f4d 494d  -10, ORPHA, OMIM
+00001500: 2063 6f64 6529 2c20 696e 636c 7564 6520   code), include 
+00001510: 6465 6e64 726f 6772 616d 2074 7265 6520  dendrogram tree 
+00001520: 7669 7375 616c 697a 6174 696f 6e2e 0a20  visualization.. 
+00001530: 2020 202d 2054 6869 7320 7368 6f75 6c64     - This should
+00001540: 2068 656c 7020 636c 696e 6963 6961 6e20   help clinician 
+00001550: 746f 202a 2a73 7973 7465 6d61 7469 6361  to **systematica
+00001560: 6c6c 7920 646f 696e 6720 776f 726b 2d75  lly doing work-u
+00001570: 7020 616e 6420 6578 636c 7564 696e 6720  p and excluding 
+00001580: 7369 6d69 6c61 7220 6469 6167 6e6f 7369  similar diagnosi
+00001590: 7320 746f 6765 7468 6572 2a2a 2062 6173  s together** bas
+000015a0: 6564 206f 6e20 7468 6520 7061 7469 656e  ed on the patien
+000015b0: 745c 2773 2070 6865 6e6f 7479 7065 2e0a  t\'s phenotype..
+000015c0: 342e 2047 656e 6520 616e 6420 6469 7365  4. Gene and dise
+000015d0: 6173 6520 7265 636f 6d6d 656e 6461 7469  ase recommendati
+000015e0: 6f6e 2062 6173 6564 206f 6e20 7468 6520  on based on the 
+000015f0: 7068 656e 6f74 7970 6520 6461 7461 2073  phenotype data s
+00001600: 696d 696c 6172 6974 7920 7363 6f72 696e  imilarity scorin
+00001610: 6720 6265 7477 6565 6e20 2a2a 7068 656e  g between **phen
+00001620: 6f74 7970 652a 2a20 616e 6420 4f4d 494d  otype** and OMIM
+00001630: 2067 656e 6520 616e 6420 6469 7365 6173   gene and diseas
+00001640: 6520 6461 7461 6261 6e6b 2e0a 352e 204c  e databank..5. L
+00001650: 696e 6b61 6765 2061 6e61 6c79 7369 7320  inkage analysis 
+00001660: 6f66 2072 6563 6f6d 6d65 6e64 6564 2063  of recommended c
+00001670: 6175 7361 7469 7665 2067 656e 6520 616e  ausative gene an
+00001680: 6420 6469 7365 6173 6520 6261 7365 6420  d disease based 
+00001690: 6f6e 2070 6865 6e6f 7479 7065 2064 6174  on phenotype dat
+000016a0: 6120 2869 6e63 6c75 6465 2064 656e 6472  a (include dendr
+000016b0: 6f67 7261 6d20 7472 6565 2076 6973 7561  ogram tree visua
+000016c0: 6c69 7a61 7469 6f6e 292e 0a20 2020 202d  lization)..    -
+000016d0: 2054 6869 7320 7368 6f75 6c64 2068 656c   This should hel
+000016e0: 7020 636c 696e 6963 6961 6e20 746f 202a  p clinician to *
+000016f0: 2a65 7870 6c6f 7265 202f 2065 6e72 6963  *explore / enric
+00001700: 6820 7468 6569 7220 6469 6666 6572 656e  h their differen
+00001710: 7469 616c 2064 6961 676e 6f73 6973 2a2a  tial diagnosis**
+00001720: 2062 6173 6564 206f 6e20 7468 6520 7061   based on the pa
+00001730: 7469 656e 745c 2773 2070 6865 6e6f 7479  tient\'s phenoty
+00001740: 7065 2e0a 362e 2045 7861 6d70 6c65 206f  pe..6. Example o
+00001750: 6620 7468 6520 636c 696e 6963 616c 2064  f the clinical d
+00001760: 6174 6120 7072 6f76 6964 6564 2061 7420  ata provided at 
+00001770: 5b43 6c69 6e69 6361 6c20 496e 666f 726d  [Clinical Inform
+00001780: 6174 696f 6e20 4578 616d 706c 6520 7365  ation Example se
+00001790: 6374 696f 6e5d 2823 636c 696e 6963 616c  ction](#clinical
+000017a0: 2d69 6e66 6f72 6d61 7469 6f6e 2d65 7861  -information-exa
+000017b0: 6d70 6c65 290a 0a0a 2323 2049 6e73 7461  mple)...## Insta
+000017c0: 6c6c 6174 696f 6e0a 0a3c 212d 2d20 7374  llation..<!-- st
+000017d0: 6172 7420 7079 2076 6572 7369 6f6e 202d  art py version -
+000017e0: 2d3e 0a0a 2a2a 6964 6572 6172 652d 7068  ->..**iderare-ph
+000017f0: 656e 6f2a 2a20 7265 7175 6972 6573 2050  eno** requires P
+00001800: 7974 686f 6e20 332e 3820 6f72 206c 6174  ython 3.8 or lat
+00001810: 6572 2e0a 0a3c 212d 2d20 656e 6420 7079  er...<!-- end py
+00001820: 2076 6572 7369 6f6e 202d 2d3e 0a0a 2323   version -->..##
+00001830: 2320 496e 7374 616c 6c69 6e67 2077 6974  # Installing wit
+00001840: 6820 6070 6970 600a 0a3c 212d 2d20 7374  h `pip`..<!-- st
+00001850: 6172 7420 696e 7374 616c 6c20 7069 7020  art install pip 
+00001860: 2d2d 3e0a 0a2a 2a69 6465 7261 7265 2d70  -->..**iderare-p
+00001870: 6865 6e6f 2a2a 2069 7320 6176 6169 6c61  heno** is availa
+00001880: 626c 6520 5b6f 6e20 5079 5049 5d28 6874  ble [on PyPI](ht
+00001890: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+000018a0: 726f 6a65 6374 2f69 6465 7261 7265 2d70  roject/iderare-p
+000018b0: 6865 6e6f 2f29 2e20 4a75 7374 2072 756e  heno/). Just run
+000018c0: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+000018d0: 7374 616c 6c20 6964 6572 6172 652d 7068  stall iderare-ph
+000018e0: 656e 6f0a 6060 600a 0a3c 212d 2d20 656e  eno.```..<!-- en
+000018f0: 6420 696e 7374 616c 6c20 7069 7020 2d2d  d install pip --
+00001900: 3e0a 0a23 2323 2049 6e73 7461 6c6c 696e  >..### Installin
+00001910: 6720 6672 6f6d 2073 6f75 7263 650a 0a3c  g from source..<
+00001920: 212d 2d20 7374 6172 7420 696e 7374 616c  !-- start instal
+00001930: 6c20 736f 7572 6365 202d 2d3e 0a0a 546f  l source -->..To
+00001940: 2069 6e73 7461 6c6c 202a 2a69 6465 7261   install **idera
+00001950: 7265 2d70 6865 6e6f 2a2a 2066 726f 6d20  re-pheno** from 
+00001960: 736f 7572 6365 2c20 6669 7273 7420 636c  source, first cl
+00001970: 6f6e 6520 5b74 6865 2072 6570 6f73 6974  one [the reposit
+00001980: 6f72 795d 2868 7474 7073 3a2f 2f67 6974  ory](https://git
+00001990: 6875 622e 636f 6d2f 6976 616e 7769 6c6c  hub.com/ivanwill
+000019a0: 6961 6d6d 642f 6964 6572 6172 652d 7068  iammd/iderare-ph
+000019b0: 656e 6f29 3a0a 0a60 6060 6261 7368 0a67  eno):..```bash.g
+000019c0: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+000019d0: 2f67 6974 6875 622e 636f 6d2f 6976 616e  /github.com/ivan
+000019e0: 7769 6c6c 6961 6d6d 642f 6964 6572 6172  williammd/iderar
+000019f0: 652d 7068 656e 6f2e 6769 740a 6364 2069  e-pheno.git.cd i
+00001a00: 6465 7261 7265 5f70 6865 6e6f 0a60 6060  derare_pheno.```
+00001a10: 0a0a 5468 656e 2072 756e 0a0a 6060 6062  ..Then run..```b
+00001a20: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
+00001a30: 2d65 202e 0a60 6060 0a0a 3c21 2d2d 2065  -e ..```..<!-- e
+00001a40: 6e64 2069 6e73 7461 6c6c 2073 6f75 7263  nd install sourc
+00001a50: 6520 2d2d 3e0a 0a23 2320 5573 6167 650a  e -->..## Usage.
+00001a60: 0a60 6060 7079 7468 6f6e 0a66 726f 6d20  .```python.from 
+00001a70: 6964 6572 6172 655f 7068 656e 6f20 696d  iderare_pheno im
+00001a80: 706f 7274 2069 6465 7261 7265 5f70 6865  port iderare_phe
+00001a90: 6e6f 0a60 6060 0a0a 2323 2054 6561 6d0a  no.```..## Team.
+00001aa0: 0a3c 212d 2d20 7374 6172 7420 7465 616d  .<!-- start team
+00001ab0: 202d 2d3e 0a0a 2a2a 6964 6572 6172 652d   -->..**iderare-
+00001ac0: 7068 656e 6f2a 2a20 6973 2064 6576 656c  pheno** is devel
+00001ad0: 6f70 6564 2061 6e64 206d 6169 6e74 6169  oped and maintai
+00001ae0: 6e65 6420 6279 2074 6865 2061 7574 686f  ned by the autho
+00001af0: 7228 7329 2c20 546f 206c 6561 726e 206d  r(s), To learn m
+00001b00: 6f72 6520 6162 6f75 7420 7768 6f20 7370  ore about who sp
+00001b10: 6563 6966 6963 616c 6c79 2063 6f6e 7472  ecifically contr
+00001b20: 6962 7574 6564 2074 6f20 7468 6973 2063  ibuted to this c
+00001b30: 6f64 6562 6173 652c 2073 6565 205b 6f75  odebase, see [ou
+00001b40: 7220 636f 6e74 7269 6275 746f 7273 5d28  r contributors](
+00001b50: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001b60: 6f6d 2f69 7661 6e77 696c 6c69 616d 6d64  om/ivanwilliammd
+00001b70: 2f69 6465 7261 7265 2d70 6865 6e6f 2f67  /iderare-pheno/g
+00001b80: 7261 7068 732f 636f 6e74 7269 6275 746f  raphs/contributo
+00001b90: 7273 2920 7061 6765 2e0a 0a3c 212d 2d20  rs) page...<!-- 
+00001ba0: 656e 6420 7465 616d 202d 2d3e 0a0a 2323  end team -->..##
+00001bb0: 204c 6963 656e 7365 0a0a 3c21 2d2d 2073   License..<!-- s
+00001bc0: 7461 7274 206c 6963 656e 7365 202d 2d3e  tart license -->
+00001bd0: 0a0a 2a2a 6964 6572 6172 652d 7068 656e  ..**iderare-phen
+00001be0: 6f2a 2a20 6c69 6365 6e73 6520 6973 2064  o** license is d
+00001bf0: 6572 6976 6564 2066 726f 6d20 5b49 4465  erived from [IDe
+00001c00: 5261 7265 5d28 6874 7470 733a 2f2f 6769  Rare](https://gi
+00001c10: 7468 7562 2e63 6f6d 2f69 7661 6e77 696c  thub.com/ivanwil
+00001c20: 6c69 616d 6d64 2f69 6465 7261 7265 290a  liammd/iderare).
+00001c30: 0a3c 212d 2d20 656e 6420 6c69 6365 6e73  .<!-- end licens
+00001c40: 6520 2d2d 3e0a                           e -->.
```

### Comparing `iderare-pheno-0.1.7/pyproject.toml` & `iderare-pheno-0.1.8/pyproject.toml`

 * *Files identical despite different names*

