# Comparing `tmp/aligned_textgrid-0.6.4.tar.gz` & `tmp/aligned_textgrid-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned_textgrid-0.6.4.tar", max compression
+gzip compressed data, was "aligned_textgrid-0.6.5.tar", max compression
```

## Comparing `aligned_textgrid-0.6.4.tar` & `aligned_textgrid-0.6.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-02-14 13:52:58.923117 aligned_textgrid-0.6.4/LICENSE
--rw-r--r--   0        0        0     5072 2024-02-21 15:37:23.947449 aligned_textgrid-0.6.4/README.md
--rw-r--r--   0        0        0     1225 2024-03-01 18:43:02.496961 aligned_textgrid-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      707 2024-02-21 15:37:23.962773 aligned_textgrid-0.6.4/src/aligned_textgrid/__init__.py
--rw-r--r--   0        0        0    17084 2024-03-01 18:43:02.497159 aligned_textgrid-0.6.4/src/aligned_textgrid/aligned_textgrid.py
--rw-r--r--   0        0        0     5194 2024-02-21 15:37:23.963303 aligned_textgrid-0.6.4/src/aligned_textgrid/custom_classes.py
--rw-r--r--   0        0        0        0 2024-02-21 15:37:23.963335 aligned_textgrid-0.6.4/src/aligned_textgrid/mixins/__init__.py
--rw-r--r--   0        0        0     5833 2024-02-21 15:37:23.963622 aligned_textgrid-0.6.4/src/aligned_textgrid/mixins/mixins.py
--rw-r--r--   0        0        0     4727 2024-02-21 15:37:23.963912 aligned_textgrid-0.6.4/src/aligned_textgrid/mixins/tiermixins.py
--rw-r--r--   0        0        0     1367 2024-02-21 15:37:23.964010 aligned_textgrid-0.6.4/src/aligned_textgrid/mixins/within.py
--rw-r--r--   0        0        0        0 2024-02-21 15:37:23.964048 aligned_textgrid-0.6.4/src/aligned_textgrid/outputs/__init__.py
--rw-r--r--   0        0        0     3927 2024-02-21 15:37:23.964350 aligned_textgrid-0.6.4/src/aligned_textgrid/outputs/to_dataframe.py
--rw-r--r--   0        0        0        0 2024-02-21 15:37:23.964386 aligned_textgrid-0.6.4/src/aligned_textgrid/points/__init__.py
--rw-r--r--   0        0        0     4986 2024-02-21 15:37:23.964691 aligned_textgrid-0.6.4/src/aligned_textgrid/points/points.py
--rw-r--r--   0        0        0     6521 2024-02-21 15:37:23.964969 aligned_textgrid-0.6.4/src/aligned_textgrid/points/tiers.py
--rw-r--r--   0        0        0        0 2024-02-21 15:37:23.965007 aligned_textgrid-0.6.4/src/aligned_textgrid/polar/__init__.py
--rw-r--r--   0        0        0     5280 2024-02-21 15:37:23.965238 aligned_textgrid-0.6.4/src/aligned_textgrid/polar/polar_classes.py
--rw-r--r--   0        0        0     1544 2024-02-21 15:37:23.965376 aligned_textgrid-0.6.4/src/aligned_textgrid/polar/polar_grid.py
--rw-r--r--   0        0        0        0 2023-11-16 18:05:47.275381 aligned_textgrid-0.6.4/src/aligned_textgrid/sequences/__init__.py
--rw-r--r--   0        0        0    18666 2024-02-21 15:37:23.965756 aligned_textgrid-0.6.4/src/aligned_textgrid/sequences/sequences.py
--rw-r--r--   0        0        0    10613 2024-02-21 15:37:23.966162 aligned_textgrid-0.6.4/src/aligned_textgrid/sequences/tiers.py
--rw-r--r--   0        0        0     2338 2024-02-21 15:37:23.966335 aligned_textgrid-0.6.4/src/aligned_textgrid/sequences/word_and_phone.py
--rw-r--r--   0        0        0     6183 1970-01-01 00:00:00.000000 aligned_textgrid-0.6.4/setup.py
--rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 aligned_textgrid-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-14 13:52:58.923117 aligned_textgrid-0.6.5/LICENSE
+-rw-r--r--   0        0        0     5072 2024-02-21 15:37:23.947449 aligned_textgrid-0.6.5/README.md
+-rw-r--r--   0        0        0     1225 2024-04-06 21:18:00.270105 aligned_textgrid-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-02-21 15:37:23.962773 aligned_textgrid-0.6.5/src/aligned_textgrid/__init__.py
+-rw-r--r--   0        0        0    17084 2024-04-06 21:10:14.820768 aligned_textgrid-0.6.5/src/aligned_textgrid/aligned_textgrid.py
+-rw-r--r--   0        0        0     5194 2024-02-21 15:37:23.963303 aligned_textgrid-0.6.5/src/aligned_textgrid/custom_classes.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:37:23.963335 aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/__init__.py
+-rw-r--r--   0        0        0     5833 2024-02-21 15:37:23.963622 aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/mixins.py
+-rw-r--r--   0        0        0     4727 2024-02-21 15:37:23.963912 aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/tiermixins.py
+-rw-r--r--   0        0        0     1367 2024-02-21 15:37:23.964010 aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/within.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:37:23.964048 aligned_textgrid-0.6.5/src/aligned_textgrid/outputs/__init__.py
+-rw-r--r--   0        0        0     3927 2024-02-21 15:37:23.964350 aligned_textgrid-0.6.5/src/aligned_textgrid/outputs/to_dataframe.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:37:23.964386 aligned_textgrid-0.6.5/src/aligned_textgrid/points/__init__.py
+-rw-r--r--   0        0        0     4986 2024-04-06 21:09:59.872257 aligned_textgrid-0.6.5/src/aligned_textgrid/points/points.py
+-rw-r--r--   0        0        0     6521 2024-04-06 21:09:59.873124 aligned_textgrid-0.6.5/src/aligned_textgrid/points/tiers.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:37:23.965007 aligned_textgrid-0.6.5/src/aligned_textgrid/polar/__init__.py
+-rw-r--r--   0        0        0     5280 2024-02-21 15:37:23.965238 aligned_textgrid-0.6.5/src/aligned_textgrid/polar/polar_classes.py
+-rw-r--r--   0        0        0     1544 2024-02-21 15:37:23.965376 aligned_textgrid-0.6.5/src/aligned_textgrid/polar/polar_grid.py
+-rw-r--r--   0        0        0        0 2023-11-16 18:05:47.275381 aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/__init__.py
+-rw-r--r--   0        0        0    18666 2024-04-06 21:09:59.874411 aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/sequences.py
+-rw-r--r--   0        0        0    10613 2024-04-06 21:09:59.875723 aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/tiers.py
+-rw-r--r--   0        0        0     2338 2024-02-21 15:37:23.966335 aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/word_and_phone.py
+-rw-r--r--   0        0        0     6183 1970-01-01 00:00:00.000000 aligned_textgrid-0.6.5/setup.py
+-rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 aligned_textgrid-0.6.5/PKG-INFO
```

### Comparing `aligned_textgrid-0.6.4/LICENSE` & `aligned_textgrid-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/README.md` & `aligned_textgrid-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/pyproject.toml` & `aligned_textgrid-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aligned_textgrid"
-version = "0.6.4"
+version = "0.6.5"
 description = "Classes for defining sequential information from TextGrids"
 authors = ["JoFrhwld <JoFrhwld@gmail.com>", "chrisbrickhouse <brickhouse@stanford.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "aligned_textgrid", from="src"}]
 exclude = [
     "notebooks/",
@@ -14,15 +14,15 @@
 homepage = "https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/"
 repository = "https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 praatio = "^6.0.0"
 numpy = "^1.24.2"
-polars = "^0.19.14"
+polars = "^0.20.18"
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 pytest = "^7.2.1"
 importlib = "^1.0.4"
 pytest-cov = "^4.0.0"
 pytest-html = "^3.2.0"
```

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/__init__.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/aligned_textgrid.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/aligned_textgrid.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/custom_classes.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/custom_classes.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/mixins/mixins.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/mixins.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/mixins/tiermixins.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/tiermixins.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/mixins/within.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/within.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/outputs/to_dataframe.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/outputs/to_dataframe.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/points/points.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/points/points.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/points/tiers.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/points/tiers.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/polar/polar_classes.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/polar/polar_classes.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/polar/polar_grid.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/polar/polar_grid.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/sequences/sequences.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/sequences.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/sequences/tiers.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/tiers.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/src/aligned_textgrid/sequences/word_and_phone.py` & `aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/word_and_phone.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.4/setup.py` & `aligned_textgrid-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
  'aligned_textgrid.polar',
  'aligned_textgrid.sequences']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.24.2,<2.0.0', 'polars>=0.19.14,<0.20.0', 'praatio>=6.0.0,<7.0.0']
+['numpy>=1.24.2,<2.0.0', 'polars>=0.20.18,<0.21.0', 'praatio>=6.0.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'aligned-textgrid',
-    'version': '0.6.4',
+    'version': '0.6.5',
     'description': 'Classes for defining sequential information from TextGrids',
     'long_description': "# Aligned TextGrid\n\n![PyPI](https://img.shields.io/pypi/v/aligned-textgrid.png)\n![lint_and_test](https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/actions/workflows/test_and_run.yml/badge.svg?event=pull_request&branch=main)\n[![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/branch/dev/graph/badge.svg?token=27YSOQ5ZEL)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid)\n[![Maintainability](https://api.codeclimate.com/v1/badges/2387cd247bd8f1211323/maintainability.png)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/maintainability)\n[![Build\nDocs](https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/actions/workflows/build-docs.yml/badge.svg)](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/)\n[![DOI](https://zenodo.org/badge/552633207.svg)](https://zenodo.org/badge/latestdoi/552633207)\n\nThe aligned-textgrid package provides a python interface for\nrepresenting and operating on TextGrids produced by forced aligners like\n[FAVE](https://github.com/JoFrhwld/FAVE) or the [Montreal Forced\nAligner](https://montreal-forced-aligner.readthedocs.io/en/latest/).\nClasses provided by aligned-textgrid represent hierarchical and\nprecedence relationships among data stored in TextGrid formats allowing\nfor simplified and more accessible analysis of aligned speech data.\n\n## Example Use Cases\n\n- You want to quickly loop through the Phone tier of a Textgrid, and\n  *also* access information about the word it is a part of.\n- You want to quickly loop over the Word tier of a Textgrid and quickly\n  count how many phones it has.\n- You want to programmatically merge together adjacent Textgrid\n  intervals.\n\nFor examples on how to use the pacakge, see the [Usage](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage) pages.\n\n## Installation\n\n<!-- TODO: documnet other package managers like conda -CB 14 March 2023 -->\n\nTo install aligned-textgrid using pip, run the following command in your\nterminal:\n\n``` bash\npip install aligned-textgrid\n```\n\n## Not another TextGrid implementation\n\nThere are several other packages that parse Praat Textgrids, including\n\n- [praatio](http://timmahrt.github.io/praatIO/praatio.html)\n- [textgrid](https://github.com/kylebgorman/textgrid)\n\n`aligned-textgrid`’s goal is to capture hierarchical and sequential\nrelationships represented in many TextGrids, and to make them easilly\naccessible to users via an intuitive interface. The goal is that from\nany arbitrary location within a TextGrid, users can easilly access\ninformation with minimally defensive coding.\n\n![](doc_src/usage/resources/diagrams/hierarchy_precedence.svg)\n\n### Example\n\nAs an example, we’ll read in a textgrid produced with forced alignment\nthat contains a single speaker with a word and phone tier.\n\n``` python\nfrom aligned_textgrid import AlignedTextGrid, Word, Phone\ntg = AlignedTextGrid(\n    textgrid_path='doc_src/usage/resources/josef-fruehwald_speaker.TextGrid', \n    entry_classes=[Word, Phone]\n    )\n```\n\nThen, we can access an arbitrary phone interval.\n\n``` python\narbitrary_interval = tg[0].Phone[20]\n```\n\nFrom this aribitrary interval, we can access information about the\nintervals preceding and following with the `.prev` and `.fol`\nattributes.\n\n``` python\nprint(arbitrary_interval.prev.label)\nprint(arbitrary_interval.label)\nprint(arbitrary_interval.fol.label)\n```\n\n    R\n    EY1\n    N\n\nWe can also access information about the word this interval is nested\nwithin with the `.inword` attribute.\n\n``` python\nprint(arbitrary_interval.inword.label)\n```\n\n    raindrops\n\nThe object returned by `.inword` is just another interval, meaning we\ncan access informaton about *it’s* context with the `.prev` and `.fol`\nattributes as well.\n\n``` python\nprint(arbitrary_interval.inword.prev.label)\nprint(arbitrary_interval.inword.label)\nprint(arbitrary_interval.inword.fol.label)\n```\n\n    strikes\n    raindrops\n    in\n\n## For more\n\n- To start jumping in, check out [the\n  quickstart](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/)\n- To learn more about navigating TextGrids and intervals, check out the\n  usage pages on [navigating\n  TextGrids](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/01_TextGrids/01_tg-nav.html)\n  and [navgiating\n  sequences](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/02_Sequences/00_sequence_structure.html)\n- To learn more about the attributes you can access from textgrids and\n  sequences, see the usage pages on [TextGrid\n  attributes](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/01_TextGrids/02_tg-info.html)\n  and [interval\n  attributes](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/02_Sequences/02_sequence_properties.html)\n\nYou can also directly read up on [the function and class\nreferences](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/reference/).\n",
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/',
```

### Comparing `aligned_textgrid-0.6.4/PKG-INFO` & `aligned_textgrid-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: aligned-textgrid
-Version: 0.6.4
+Version: 0.6.5
 Summary: Classes for defining sequential information from TextGrids
 Home-page: https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/
 License: GPL-3.0-or-later
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: polars (>=0.19.14,<0.20.0)
+Requires-Dist: polars (>=0.20.18,<0.21.0)
 Requires-Dist: praatio (>=6.0.0,<7.0.0)
 Project-URL: Repository, https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid
 Description-Content-Type: text/markdown
 
 # Aligned TextGrid
 
 ![PyPI](https://img.shields.io/pypi/v/aligned-textgrid.png)
```

