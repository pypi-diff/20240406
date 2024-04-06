# Comparing `tmp/iderare-pheno-0.3.0.tar.gz` & `tmp/iderare-pheno-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iderare-pheno-0.3.0.tar", last modified: Sat Apr  6 17:24:54 2024, max compression
+gzip compressed data, was "iderare-pheno-0.3.2.tar", last modified: Sat Apr  6 18:15:20 2024, max compression
```

## Comparing `iderare-pheno-0.3.0.tar` & `iderare-pheno-0.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:24:54.244353 iderare-pheno-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-06 17:24:54.244353 iderare-pheno-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:24:54.240353 iderare-pheno-0.3.0/iderare_pheno/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/simrec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/iderare_pheno/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:24:54.240353 iderare-pheno-0.3.0/iderare_pheno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 17:24:54.000000 iderare-pheno-0.3.0/iderare_pheno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-06 17:24:01.000000 iderare-pheno-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:24:54.244353 iderare-pheno-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:15:20.126692 iderare-pheno-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 18:14:58.000000 iderare-pheno-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-06 18:15:20.126692 iderare-pheno-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-06 18:14:58.000000 iderare-pheno-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:15:20.122692 iderare-pheno-0.3.2/iderare_pheno/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 18:14:58.000000 iderare-pheno-0.3.2/iderare_pheno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-06 18:14:58.000000 iderare-pheno-0.3.2/iderare_pheno/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/iderare_pheno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/iderare_pheno/simrec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/iderare_pheno/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/iderare_pheno/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:15:20.122692 iderare-pheno-0.3.2/iderare_pheno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 18:15:20.000000 iderare-pheno-0.3.2/iderare_pheno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-06 18:14:59.000000 iderare-pheno-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:15:20.126692 iderare-pheno-0.3.2/setup.cfg
```

### Comparing `iderare-pheno-0.3.0/LICENSE` & `iderare-pheno-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.0/PKG-INFO` & `iderare-pheno-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.3.0
+Version: 0.3.2
 Author-email: Ivan William Harsono <contact@ivanwilliammd.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -154,15 +154,17 @@
 ```
 
 <!-- end install source -->
 
 ## Usage
 
 ```python
-from iderare_pheno import iderare_pheno
+from iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
+from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name
+from iderare_pheno.utils import linkage_dendrogram, list2tsv
 ```
 
 ## Team
 
 <!-- start team -->
 
 **iderare-pheno** is developed and maintained by the author(s), To learn more about who specifically contributed to this codebase, see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.0 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.2 Author-email: Ivan
 William Harsono
 ivanwilliammd.org> License: BSD 3-Clause License Copyright (c) 2024, Ivan
 William Harsono Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
@@ -69,13 +69,16 @@
 Information Example section](#clinical-information-example) ## Installation
 **iderare-pheno** requires Python 3.8 or later. ### Installing with `pip`
 **iderare-pheno** is available [on PyPI](https://pypi.org/project/iderare-
 pheno/). Just run ```bash pip install iderare-pheno ``` ### Installing from
 source To install **iderare-pheno** from source, first clone [the repository]
 (https://github.com/ivanwilliammd/iderare-pheno): ```bash git clone https://
 github.com/ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run
-```bash pip install -e . ``` ## Usage ```python from iderare_pheno import
-iderare_pheno ``` ## Team **iderare-pheno** is developed and maintained by the
-author(s), To learn more about who specifically contributed to this codebase,
-see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/
-contributors) page. ## License **iderare-pheno** license is derived from
-[IDeRare](https://github.com/ivanwilliammd/iderare)
+```bash pip install -e . ``` ## Usage ```python from iderare_pheno.converter
+import term2omim, term2orpha, term2hpo, batchconvert from iderare_pheno.simrec
+import hpo2omim_similarity, omim_recommendation, hpo2name from
+iderare_pheno.utils import linkage_dendrogram, list2tsv ``` ## Team **iderare-
+pheno** is developed and maintained by the author(s), To learn more about who
+specifically contributed to this codebase, see [our contributors](https://
+github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License
+**iderare-pheno** license is derived from [IDeRare](https://github.com/
+ivanwilliammd/iderare)
```

### Comparing `iderare-pheno-0.3.0/README.md` & `iderare-pheno-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,17 @@
 ```
 
 <!-- end install source -->
 
 ## Usage
 
 ```python
-from iderare_pheno import iderare_pheno
+from iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
+from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name
+from iderare_pheno.utils import linkage_dendrogram, list2tsv
 ```
 
 ## Team
 
 <!-- start team -->
 
 **iderare-pheno** is developed and maintained by the author(s), To learn more about who specifically contributed to this codebase, see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page.
```

#### html2text {}

```diff
@@ -25,13 +25,16 @@
 Information Example section](#clinical-information-example) ## Installation
 **iderare-pheno** requires Python 3.8 or later. ### Installing with `pip`
 **iderare-pheno** is available [on PyPI](https://pypi.org/project/iderare-
 pheno/). Just run ```bash pip install iderare-pheno ``` ### Installing from
 source To install **iderare-pheno** from source, first clone [the repository]
 (https://github.com/ivanwilliammd/iderare-pheno): ```bash git clone https://
 github.com/ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run
-```bash pip install -e . ``` ## Usage ```python from iderare_pheno import
-iderare_pheno ``` ## Team **iderare-pheno** is developed and maintained by the
-author(s), To learn more about who specifically contributed to this codebase,
-see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/
-contributors) page. ## License **iderare-pheno** license is derived from
-[IDeRare](https://github.com/ivanwilliammd/iderare)
+```bash pip install -e . ``` ## Usage ```python from iderare_pheno.converter
+import term2omim, term2orpha, term2hpo, batchconvert from iderare_pheno.simrec
+import hpo2omim_similarity, omim_recommendation, hpo2name from
+iderare_pheno.utils import linkage_dendrogram, list2tsv ``` ## Team **iderare-
+pheno** is developed and maintained by the author(s), To learn more about who
+specifically contributed to this codebase, see [our contributors](https://
+github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License
+**iderare-pheno** license is derived from [IDeRare](https://github.com/
+ivanwilliammd/iderare)
```

### Comparing `iderare-pheno-0.3.0/iderare_pheno/converter.py` & `iderare-pheno-0.3.2/iderare_pheno/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+import os
+
 import pandas as pd
 
 # Declare the folder path for phenotype data source
-phenotype_folder = "phenotype/subset"
+phenotype_folder = os.path.dirname(__file__)
 
 # Declare database useds for mapping
-icd10omim = "icd102omim_subset.tsv"
-loinc2hpo = "loinc2hpo_standardized.tsv"
-orpha2omim = "orpha2omim_subset.tsv"
-omim2hpo = "omim2hpo_subset.tsv"
-snomed2hpo = "snomed2hpo_subset.tsv"
-snomed2orpha = "snomed2orpha_subset.tsv"
+icd10omim = os.path.join(phenotype_folder, "phenotype", "subset", "icd102omim_subset.tsv")
+loinc2hpo = os.path.join(phenotype_folder, "phenotype", "subset", "loinc2hpo_standardized.tsv")
+orpha2omim = os.path.join(phenotype_folder, "phenotype", "subset", "orpha2omim_subset.tsv")
+omim2hpo = os.path.join(phenotype_folder, "phenotype", "subset", "omim2hpo_subset.tsv")
+snomed2hpo = os.path.join(phenotype_folder, "phenotype", "subset", "snomed2hpo_subset.tsv")
+snomed2orpha = os.path.join(phenotype_folder, "phenotype", "subset", "snomed2orpha_subset.tsv")
 
 # iderare yaml configuration file
 yaml_file = "iderare.yaml"
 
 # Clinical data dummy in txt format separated with new line
 clinical_data = "clinical_data.txt"
 
 # Read the clinical data and parse the data
-icd10omim_df = pd.read_csv(phenotype_folder + "/" + icd10omim, sep="\t")
-loinc2hpo_df = pd.read_csv(phenotype_folder + "/" + loinc2hpo, sep="\t")
-orpha2omim_df = pd.read_csv(phenotype_folder + "/" + orpha2omim, sep="\t")
-omim2hpo_df = pd.read_csv(phenotype_folder + "/" + omim2hpo, sep="\t")
-snomed2hpo_df = pd.read_csv(phenotype_folder + "/" + snomed2hpo, sep="\t")
-snomed2orpha_df = pd.read_csv(phenotype_folder + "/" + snomed2orpha, sep="\t")
+icd10omim_df = pd.read_csv(icd10omim, sep="\t")
+loinc2hpo_df = pd.read_csv(loinc2hpo, sep="\t")
+orpha2omim_df = pd.read_csv(orpha2omim, sep="\t")
+omim2hpo_df = pd.read_csv(omim2hpo, sep="\t")
+snomed2hpo_df = pd.read_csv(snomed2hpo, sep="\t")
+snomed2orpha_df = pd.read_csv(snomed2orpha, sep="\t")
 
 
 # Convert SNOMED to ORPHA First
 def term2orpha(clinical_data):
     print("Trying to parse ORPHA from SNOMEDCT", clinical_data)
 
     if "SNOMEDCT:" in clinical_data:
```

### Comparing `iderare-pheno-0.3.0/iderare_pheno/simrec.py` & `iderare-pheno-0.3.2/iderare_pheno/simrec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import os
+
 from pyhpo import HPOSet, Omim, Ontology, stats
 
-Ontology("phenotype/rawdl_20240310")
+Ontology(os.path.join(os.path.dirname(__file__), "phenotype", "data"))
 
 
 # Convert OMIM code to OMIM Class Object
 def omim2object(omim_set):
     omim_object = []
     for item in list(set(omim_set)):
         try:
```

### Comparing `iderare-pheno-0.3.0/iderare_pheno/utils.py` & `iderare-pheno-0.3.2/iderare_pheno/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ):
     if sim_score is None:
         data = {"id": term_id, "name": name}
     else:
         rank = [i + 1 for i in range(len(name))]
         data = {"rank": rank, "id": term_id, "name": name, "score": sim_score}
     df = pd.DataFrame(data)
-    df.to_csv("output/{}.tsv".format(filename), index=False, sep="\t")
+    df.to_csv("{}.tsv".format(filename), index=False, sep="\t")
     return df
 
 
 # Print the dendrogram tree
 def linkage_dendrogram(linkage, labels, title="Similarity", threshold=0.3, path_to_save=None):
     if len(linkage) == 0:
         print("Linkage is empty. The data not possible due to blank linkage information.")
```

### Comparing `iderare-pheno-0.3.0/iderare_pheno.egg-info/PKG-INFO` & `iderare-pheno-0.3.2/iderare_pheno.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.3.0
+Version: 0.3.2
 Author-email: Ivan William Harsono <contact@ivanwilliammd.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -154,15 +154,17 @@
 ```
 
 <!-- end install source -->
 
 ## Usage
 
 ```python
-from iderare_pheno import iderare_pheno
+from iderare_pheno.converter import term2omim, term2orpha, term2hpo, batchconvert
+from iderare_pheno.simrec import hpo2omim_similarity, omim_recommendation, hpo2name
+from iderare_pheno.utils import linkage_dendrogram, list2tsv
 ```
 
 ## Team
 
 <!-- start team -->
 
 **iderare-pheno** is developed and maintained by the author(s), To learn more about who specifically contributed to this codebase, see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.0 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.2 Author-email: Ivan
 William Harsono
 ivanwilliammd.org> License: BSD 3-Clause License Copyright (c) 2024, Ivan
 William Harsono Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
 binary form must reproduce the above copyright notice, this list of conditions
@@ -69,13 +69,16 @@
 Information Example section](#clinical-information-example) ## Installation
 **iderare-pheno** requires Python 3.8 or later. ### Installing with `pip`
 **iderare-pheno** is available [on PyPI](https://pypi.org/project/iderare-
 pheno/). Just run ```bash pip install iderare-pheno ``` ### Installing from
 source To install **iderare-pheno** from source, first clone [the repository]
 (https://github.com/ivanwilliammd/iderare-pheno): ```bash git clone https://
 github.com/ivanwilliammd/iderare-pheno.git cd iderare_pheno ``` Then run
-```bash pip install -e . ``` ## Usage ```python from iderare_pheno import
-iderare_pheno ``` ## Team **iderare-pheno** is developed and maintained by the
-author(s), To learn more about who specifically contributed to this codebase,
-see [our contributors](https://github.com/ivanwilliammd/iderare-pheno/graphs/
-contributors) page. ## License **iderare-pheno** license is derived from
-[IDeRare](https://github.com/ivanwilliammd/iderare)
+```bash pip install -e . ``` ## Usage ```python from iderare_pheno.converter
+import term2omim, term2orpha, term2hpo, batchconvert from iderare_pheno.simrec
+import hpo2omim_similarity, omim_recommendation, hpo2name from
+iderare_pheno.utils import linkage_dendrogram, list2tsv ``` ## Team **iderare-
+pheno** is developed and maintained by the author(s), To learn more about who
+specifically contributed to this codebase, see [our contributors](https://
+github.com/ivanwilliammd/iderare-pheno/graphs/contributors) page. ## License
+**iderare-pheno** license is derived from [IDeRare](https://github.com/
+ivanwilliammd/iderare)
```

### Comparing `iderare-pheno-0.3.0/pyproject.toml` & `iderare-pheno-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     "*.tests",
     "*.tests.*",
     "tests.*",
     "tests",
     "docs*",
     "scripts*"
 ]
-include = ["iderare_pheno", "phenotype", "phenotype.*"]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 iderare_pheno = ["py.typed"]
```

