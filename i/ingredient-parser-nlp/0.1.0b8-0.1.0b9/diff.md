# Comparing `tmp/ingredient_parser_nlp-0.1.0b8.tar.gz` & `tmp/ingredient_parser_nlp-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingredient_parser_nlp-0.1.0b8.tar", last modified: Sat Jan 27 11:13:05 2024, max compression
+gzip compressed data, was "ingredient_parser_nlp-0.1.0b9.tar", last modified: Sat Apr  6 15:10:08 2024, max compression
```

## Comparing `ingredient_parser_nlp-0.1.0b8.tar` & `ingredient_parser_nlp-0.1.0b9.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-01-27 11:13:05.027554 ingredient_parser_nlp-0.1.0b8/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1073 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       99 2023-09-04 19:01:18.000000 ingredient_parser_nlp-0.1.0b8/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     4415 2024-01-27 11:13:05.027554 ingredient_parser_nlp-0.1.0b8/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     2195 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-01-27 11:13:05.023554 ingredient_parser_nlp-0.1.0b8/ingredient_parser/
--rw-rw-r--   0 tom       (1000) tom       (1000)     5312 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/ModelCard.md
--rw-rw-r--   0 tom       (1000) tom       (1000)      434 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7531 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/_constants.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2567 2023-11-21 20:36:27.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)   986140 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/model.crfsuite
--rw-rw-r--   0 tom       (1000) tom       (1000)     4603 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/parsers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-01-27 11:13:05.023554 ingredient_parser_nlp-0.1.0b8/ingredient_parser/postprocess/
--rw-rw-r--   0 tom       (1000) tom       (1000)      302 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/postprocess/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5810 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/postprocess/dataclasses.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    31237 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/postprocess/postprocess.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-01-27 11:13:05.023554 ingredient_parser_nlp-0.1.0b8/ingredient_parser/preprocess/
--rw-rw-r--   0 tom       (1000) tom       (1000)      132 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/preprocess/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1904 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/preprocess/funcs.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    27228 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/preprocess/preprocess.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2261 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser/preprocess/regex.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-01-27 11:13:05.027554 ingredient_parser_nlp-0.1.0b8/ingredient_parser_nlp.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     4415 2024-01-27 11:13:05.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser_nlp.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      763 2024-01-27 11:13:05.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser_nlp.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-01-27 11:13:05.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser_nlp.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       21 2024-01-27 11:13:05.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser_nlp.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       18 2024-01-27 11:13:05.000000 ingredient_parser_nlp-0.1.0b8/ingredient_parser_nlp.egg-info/top_level.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     2118 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b8/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-01-27 11:13:05.027554 ingredient_parser_nlp-0.1.0b8/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-01-27 11:13:05.027554 ingredient_parser_nlp-0.1.0b8/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1389 2023-10-08 18:02:46.000000 ingredient_parser_nlp-0.1.0b8/tests/test_utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-06 15:10:08.299509 ingredient_parser_nlp-0.1.0b9/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1073 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b9/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)      123 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     4578 2024-04-06 15:10:08.299509 ingredient_parser_nlp-0.1.0b9/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2338 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/README.md
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-06 15:10:08.295509 ingredient_parser_nlp-0.1.0b9/ingredient_parser/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5367 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/ModelCard.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)      434 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7863 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/_constants.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5692 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1688272 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/model.en.crfsuite
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7598 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/parsers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-06 15:10:08.295509 ingredient_parser_nlp-0.1.0b9/ingredient_parser/postprocess/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      302 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/postprocess/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     7849 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/postprocess/dataclasses.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    34666 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/postprocess/postprocess.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-06 15:10:08.295509 ingredient_parser_nlp-0.1.0b9/ingredient_parser/preprocess/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      132 2024-01-27 11:12:33.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/preprocess/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1902 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/preprocess/funcs.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    32629 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/preprocess/preprocess.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3744 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/preprocess/regex.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)        0 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser/py.typed
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-06 15:10:08.295509 ingredient_parser_nlp-0.1.0b9/ingredient_parser_nlp.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4578 2024-04-06 15:10:08.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser_nlp.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      773 2024-04-06 15:10:08.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser_nlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-06 15:10:08.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser_nlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       26 2024-04-06 15:10:08.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser_nlp.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       18 2024-04-06 15:10:08.000000 ingredient_parser_nlp-0.1.0b9/ingredient_parser_nlp.egg-info/top_level.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2091 2024-04-06 15:06:37.000000 ingredient_parser_nlp-0.1.0b9/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-06 15:10:08.299509 ingredient_parser_nlp-0.1.0b9/setup.cfg
```

### Comparing `ingredient_parser_nlp-0.1.0b8/LICENSE` & `ingredient_parser_nlp-0.1.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `ingredient_parser_nlp-0.1.0b8/PKG-INFO` & `ingredient_parser_nlp-0.1.0b9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_parser_nlp
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: A Python package to parse structured information from recipe ingredient sentences
 Author-email: Tom Strange <tpstrange@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2024 Tom Strange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: <=3.12,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nltk
 Requires-Dist: python-crfsuite
+Requires-Dist: pint
 
 # Ingredient Parser
 
 The Ingredient Parser package is a Python package for parsing structured information out of recipe ingredient sentences.
 
 ![](docs/source/_static/logo.png)
 
@@ -52,49 +53,54 @@
 
 Import the ```parse_ingredient``` function and pass it an ingredient sentence.
 
 ```python
 >>> from ingredient_parser import parse_ingredient
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks")
 ParsedIngredient(
-    name=IngredientText(text='pork shoulder', confidence=0.999196),
+    name=IngredientText(text='pork shoulder', confidence=0.999193),
+    size=None,
     amount=[IngredientAmount(quantity='3',
-                             unit='pounds',
+                             unit=<Unit('pound')>,
                              text='3 pounds',
-                             confidence=0.998769,
+                             confidence=0.999906,,
                              APPROXIMATE=False,
                              SINGULAR=False)],
-    preparation=IngredientText(text='cut into 2 inch chunks', confidence=0.995614),
+    preparation=IngredientText(text='cut into 2 inch chunks', confidence=0.999193),
     comment=None,
     sentence='3 pounds pork shoulder, cut into 2-inch chunks'
 )
 ```
 
 ## Model accuracy
 
 The model used for labelling tokens in sentences, provided in the ```ingredient-parser/``` directory, has the following accuracy on a test data set of 25% of the total  data used:
 
 ```
 Sentence-level results:
-	Total: 14982
-	Correct: 14021
-	Incorrect: 961
-	-> 93.59% correct
+	Accuracy: 94.24%
 
 Word-level results:
-	Total: 105360
-	Correct: 102741
-	Incorrect: 2619
-	-> 97.51% correct
+	Accuracy 97.73%
+	Precision (micro) 97.72%
+	Recall (micro) 97.73%
+	F1 score (micro) 97.72%
 ```
 
 ## Development
 
 The development dependencies are in the ```requirements-dev.txt``` file. Details on the training process can be found in the [Model Guide](https://ingredient-parser.readthedocs.io/en/latest/guide/index.html) documentation.
 
+Before committing anything, install [pre-commit](https://pre-commit.com/) and run
+```
+pre-commit install
+```
+
+to install the pre-commit hooks.
+
 There is a simple web app for testing the parser with ingredient sentences and showing the parsed output. To run the web app, run the command
 
 ```bash
 $ flask --app webapp run
 ```
 
 ![Screen shot of web app](docs/source/_static/app-screenshot.png)
```

### Comparing `ingredient_parser_nlp-0.1.0b8/README.md` & `ingredient_parser_nlp-0.1.0b9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -18,49 +18,54 @@
 
 Import the ```parse_ingredient``` function and pass it an ingredient sentence.
 
 ```python
 >>> from ingredient_parser import parse_ingredient
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks")
 ParsedIngredient(
-    name=IngredientText(text='pork shoulder', confidence=0.999196),
+    name=IngredientText(text='pork shoulder', confidence=0.999193),
+    size=None,
     amount=[IngredientAmount(quantity='3',
-                             unit='pounds',
+                             unit=<Unit('pound')>,
                              text='3 pounds',
-                             confidence=0.998769,
+                             confidence=0.999906,,
                              APPROXIMATE=False,
                              SINGULAR=False)],
-    preparation=IngredientText(text='cut into 2 inch chunks', confidence=0.995614),
+    preparation=IngredientText(text='cut into 2 inch chunks', confidence=0.999193),
     comment=None,
     sentence='3 pounds pork shoulder, cut into 2-inch chunks'
 )
 ```
 
 ## Model accuracy
 
 The model used for labelling tokens in sentences, provided in the ```ingredient-parser/``` directory, has the following accuracy on a test data set of 25% of the total  data used:
 
 ```
 Sentence-level results:
-	Total: 14982
-	Correct: 14021
-	Incorrect: 961
-	-> 93.59% correct
+	Accuracy: 94.24%
 
 Word-level results:
-	Total: 105360
-	Correct: 102741
-	Incorrect: 2619
-	-> 97.51% correct
+	Accuracy 97.73%
+	Precision (micro) 97.72%
+	Recall (micro) 97.73%
+	F1 score (micro) 97.72%
 ```
 
 ## Development
 
 The development dependencies are in the ```requirements-dev.txt``` file. Details on the training process can be found in the [Model Guide](https://ingredient-parser.readthedocs.io/en/latest/guide/index.html) documentation.
 
+Before committing anything, install [pre-commit](https://pre-commit.com/) and run
+```
+pre-commit install
+```
+
+to install the pre-commit hooks.
+
 There is a simple web app for testing the parser with ingredient sentences and showing the parsed output. To run the web app, run the command
 
 ```bash
 $ flask --app webapp run
 ```
 
 ![Screen shot of web app](docs/source/_static/app-screenshot.png)
```

### Comparing `ingredient_parser_nlp-0.1.0b8/ingredient_parser/ModelCard.md` & `ingredient_parser_nlp-0.1.0b9/ingredient_parser/ModelCard.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 ### Person or Organisation
 
 <https://github.com/strangetom>
 
 ### Model Date and Version
 
-Date: December 2023
+Date: April 2024
 
 Version: The model version is the same has the `ingredient_parser_nlp` package version.
 
+Filename: model.en.crfsuite
+
 ### Model Type
 
 Natural language model for labelling tokens in a recipe ingredient sentence.
 
 The model is a Conditional Random Fields (CRF) model, implemented using [pycrfsuite](https://github.com/scrapinghub/python-crfsuite). A pre-processing step is required before a sentence can be presented to the model, which performs a number of text normalisation operations. See [preprocess.py](https://github.com/strangetom/ingredient-parser/blob/master/ingredient_parser/preprocess.py). A postprocesing step takes the model output and interprets the tokens and labels to generate a structured representation of the ingredient sentence.
 
 ### License
@@ -32,14 +34,15 @@
 
 ### Primary Intended Uses
 
 - Label tokens in English language recipe ingredient sentences with one of the following labels:
   - QTY: Quantity of ingredient
   - UNIT: Unit of ingredient
   - NAME: Name of ingredient
+  - SIZE: Size of ingredient
   - PREP: Preparation notes for the ingredient
   - COMMENT: Comment in ingredient sentence
   - OTHER, for text that cannot be classified into one of the above labels
 
 ### Primary Intended Users
 
 - Developers and users of recipe management software or services
@@ -90,15 +93,15 @@
 
 ## Quantitative Analysis
 
 The model has the following performance metrics:
 
 | Word level accuracy | Sentence level accuracy |
 | ------------------- | ----------------------- |
-| 97.51±0.28%         | 93.59±0.62%             |
+| 97.73 ± 0.33%       | 94.24 ± 0.59%           |
 
 These metrics were determined by executing 20 training/evaluation cycles and calculating the mean and standard deviation for the two metrics across all cycles. The uncertainty values provided represent the 99.7% confidence bounds (i.e. 3x standard deviation). The uncertainty is due to the randomisation of the selection of training and evaluation data whenever the model is trained.
 
 ## Ethical Considerations
 
 There are no known ethical considerations related to this model.
```

### Comparing `ingredient_parser_nlp-0.1.0b8/ingredient_parser/_constants.py` & `ingredient_parser_nlp-0.1.0b9/ingredient_parser/_constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 
 import re
+from itertools import chain
 
 # Plural and singular units
 UNITS = {
     "bags": "bag",
     "bars": "bar",
     "baskets": "basket",
     "batches": "batch",
@@ -12,29 +13,31 @@
     "bottles": "bottle",
     "boxes": "box",
     "branches": "branch",
     "bulbs": "bulb",
     "bunches": "bunch",
     "bundles": "bundle",
     "cans": "can",
-    "chops": "chop",
     "chunks": "chunk",
     "cloves": "clove",
     "clusters": "cluster",
+    "cl": "cl",
+    "cL": "cL",
     "cm": "cm",
     "cubes": "cube",
     "cups": "cup",
     "cutlets": "cutlet",
     "dashes": "dash",
     "dessertspoons": "dessertspoon",
     "dollops": "dollop",
     "drops": "drop",
     "ears": "ear",
     "envelopes": "envelope",
     "feet": "foot",
+    "fl": "fl",
     "g": "g",
     "gallons": "gallon",
     "glasses": "glass",
     "grams": "gram",
     "grinds": "grind",
     "handfuls": "handful",
     "heads": "head",
@@ -48,28 +51,32 @@
     "lengths": "length",
     "links": "link",
     "l": "l",
     "liters": "liter",
     "litres": "litre",
     "loaves": "loaf",
     "milliliters": "milliliter",
+    "millilitres": "millilitre",
     "ml": "ml",
+    "mL": "mL",
+    "mm": "mm",
     "mugs": "mug",
     "ounces": "ounce",
     "oz": "oz",
     "packs": "pack",
     "packages": "package",
     "packets": "packet",
     "pairs": "pair",
     "pieces": "piece",
     "pinches": "pinch",
     "pints": "pint",
     "pods": "pod",
     "pounds": "pound",
     "pts": "pt",
+    "punnets": "punnet",
     "racks": "rack",
     "rashers": "rasher",
     "recipes": "recipe",
     "rectangles": "rectangle",
     "ribs": "rib",
     "quarts": "quart",
     "sachets": "sachet",
@@ -98,14 +105,17 @@
     "wheels": "wheel",
 }
 # Generate capitalized version of each entry in the UNITS dictionary
 _capitalized_units = {}
 for plural, singular in UNITS.items():
     _capitalized_units[plural.capitalize()] = singular.capitalize()
 UNITS = UNITS | _capitalized_units
+# Create a flattened list of all keys and values in UNITS dict
+# since we need this in a few places
+FLATTENED_UNITS_LIST = list(chain.from_iterable(UNITS.items()))
 
 # Words that can modify a unit
 UNIT_MODIFIERS = [
     "big",
     "fat",
     "generous",
     "healthy",
@@ -137,14 +147,15 @@
     _ambiguous_units_alt_forms.append(UNITS[amb_unit.capitalize()])
 
 AMBIGUOUS_UNITS.extend(_ambiguous_units_alt_forms)
 
 
 # Strings and their numeric representation
 STRING_NUMBERS = {
+    "one-half": "1/2",
     "one": "1",
     "two": "2",
     "three": "3",
     "four": "4",
     "five": "5",
     "six": "6",
     "seven": "7",
```

### Comparing `ingredient_parser_nlp-0.1.0b8/ingredient_parser/postprocess/postprocess.py` & `ingredient_parser_nlp-0.1.0b9/ingredient_parser/postprocess/postprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 #!/usr/bin/env python3
 
 import re
+from functools import cached_property
 from itertools import chain, groupby
 from operator import itemgetter
 from statistics import mean
 from typing import Any, Generator, Iterator
 
-from ingredient_parser._constants import APPROXIMATE_TOKENS, SINGULAR_TOKENS, STOP_WORDS
-from ingredient_parser._utils import consume
+from ingredient_parser._constants import (
+    APPROXIMATE_TOKENS,
+    SINGULAR_TOKENS,
+    STOP_WORDS,
+)
+from ingredient_parser._utils import consume, convert_to_pint_unit
 
 from .dataclasses import (
     CompositeIngredientAmount,
     IngredientAmount,
     IngredientText,
     ParsedIngredient,
     _PartialIngredientAmount,
 )
 
 WORD_CHAR = re.compile(r"\w")
 
 
 class PostProcessor:
-
     """Recipe ingredient sentence PostProcessor class.
 
     Performs the necessary postprocessing on the sentence tokens and labels and scores
     for the tokens after tagging with the CRF model in order to return a coherent
     structure of parsed information.
 
     Attributes
@@ -36,33 +40,46 @@
         Confidence associated with the label for each token.
     sentence : str
         Original ingredient sentence.
     tokens : list[str]
         List of tokens for original ingredient sentence.
     discard_isolated_stop_words : bool
         If True, isolated stop words are discarded from the name, preparation or
-        comment fields. Default value is True
+        comment fields. Default value is True.
+    string_units : bool
+        If True, return all IngredientAmount units as strings.
+        If False, convert IngredientAmount units to pint.Unit objects where possible.
+        Dfault is False.
+    imperial_units : bool
+        If True, use imperial units instead of US customary units for pint.Unit objects
+        for the the following units: fluid ounce, cup, pint, quart, gallon.
+        Default is False, which results in US customary units being used.
+        This has no effect if string_units=True.
     consumed : list[int]
         List of indices of tokens consumed as part of setting the APPROXIMATE and
         SINGULAR flags. These tokens should not end up in the parsed output.
     """
 
     def __init__(
         self,
         sentence: str,
         tokens: list[str],
         labels: list[str],
         scores: list[float],
         discard_isolated_stop_words: bool = True,
+        string_units: bool = False,
+        imperial_units: bool = False,
     ):
         self.sentence = sentence
         self.tokens = tokens
         self.labels = labels
         self.scores = scores
         self.discard_isolated_stop_words = discard_isolated_stop_words
+        self.string_units = string_units
+        self.imperial_units = imperial_units
         self.consumed = []
 
     def __repr__(self) -> str:
         """__repr__ method
 
         Returns
         -------
@@ -81,33 +98,36 @@
         """
         _str = [
             "Post-processed recipe ingredient sentence",
             f"\t{list(zip(self.tokens, self.labels))}",
         ]
         return "\n".join(_str)
 
+    @cached_property
     def parsed(self) -> ParsedIngredient:
         """Return parsed ingredient data
 
         Returns
         -------
         ParsedIngredient
             Object containing structured data from sentence.
         """
         amounts = self._postprocess_amounts()
+        size = self._postprocess("SIZE")
         name = self._postprocess("NAME")
         preparation = self._postprocess("PREP")
         comment = self._postprocess("COMMENT")
 
         return ParsedIngredient(
-            sentence=self.sentence,
-            amount=amounts,
             name=name,
+            size=size,
+            amount=amounts,
             preparation=preparation,
             comment=comment,
+            sentence=self.sentence,
         )
 
     def _postprocess(self, selected: str) -> IngredientText | None:
         """Process tokens, labels and scores with selected label into an
         IngredientText object.
 
         Parameters
@@ -121,15 +141,15 @@
             Object containing ingredient comment text and confidence
         """
         # Select indices of tokens, labels and scores for selected label
         # Do not include tokens, labels and scores in self.consumed
         idx = [
             i
             for i, label in enumerate(self.labels)
-            if label == selected and i not in self.consumed
+            if label in [selected, "PUNC"] and i not in self.consumed
         ]
 
         # Join consecutive tokens together and average their score
         parts = []
         confidence_parts = []
         for group in self._group_consecutive_idx(idx):
             idx = list(group)
@@ -167,14 +187,15 @@
         """Process tokens, labels and scores into IngredientAmount objects, by combining
         QTY labels with any following UNIT labels, up to the next QTY label.
 
         The confidence is the average confidence of all labels in the IngredientGroup.
 
         A number of special cases are considered before the default processing:
         1. "sizable unit" pattern
+        2. "composite amounts" pattern
 
         Returns
         -------
         list[IngredientAmount]
             List of IngredientAmount objects
         """
 
@@ -232,25 +253,24 @@
         >>> p._fix_punctuation(", some words ( inside ),")
         "some words (inside)"
 
         >>> p = PostProcessor("", [], [], [])
         >>> p._fix_punctuation("(unmatched parenthesis (inside)(")
         "unmatched parenthesis (inside)"
         """
-        # Remove leading comma
-        if text.startswith(", "):
-            text = text[2:]
-
-        # Remove trailing comma
-        if text.endswith(","):
-            text = text[:-1]
+        if text == "":
+            return text
 
         # Correct space following open parens or before close parens
         text = text.replace("( ", "(").replace(" )", ")")
 
+        # Correct space preceeding various punctuation
+        for punc in [",", ":", ";"]:
+            text = text.replace(f" {punc}", punc)
+
         # Remove parentheses that aren't part of a matching pair
         idx_to_remove = []
         stack = []
         for i, char in enumerate(text):
             if char in ["(", "["]:
                 # Add index to stack when we find an opening parens
                 stack.append(i)
@@ -262,15 +282,23 @@
                     # Remove last added index from stack when we find a closing parens
                     stack.pop()
 
         # Insert anything left in stack into idx_to_remove
         idx_to_remove.extend(stack)
         text = "".join(char for i, char in enumerate(text) if i not in idx_to_remove)
 
-        return text
+        # Remove leading comma, colon, semi-colon, hyphen
+        while text[0] in [",", ";", ":", "-"]:
+            text = text[1:].strip()
+
+        # Remove trailing comma, colon, semi-colon, hypehn
+        while text[-1] in [",", ";", ":", "-"]:
+            text = text[:-1].strip()
+
+        return text.strip()
 
     def _remove_isolated_punctuation_and_duplicate_indices(
         self, parts: list[str]
     ) -> list[int]:
         """Find elements in list that comprise a single punctuation character or are a
         duplicate of the previous element and discard their indices.
 
@@ -383,14 +411,15 @@
             "box",
             "can",
             "envelope",
             "jar",
             "package",
             "packet",
             "piece",
+            "sachet",
             "slice",
             "tin",
         ]
 
         amounts = []
         for pattern in patterns:
             for match in self._match_pattern(labels, pattern, ignore_other_labels=True):
@@ -403,17 +432,29 @@
 
                     # Keep track of indices of matching elements so we don't use them
                     # again elsewhere
                     self.consumed.extend([idx[i] for i in match])
 
                     # The first amount is made up of the first and last items
                     # Note that this cannot be singular, but may be approximate
+                    quantity = matching_tokens.pop(0)
+                    unit = matching_tokens.pop(-1)
+                    text = " ".join((quantity, unit)).strip()
+
+                    if not self.string_units:
+                        # If the unit is recognised in the pint unit registry, use
+                        # a pint.Unit object instead of a string. This has the benefit
+                        # of simplifying alternative unit representations into a single
+                        # common representation
+                        unit = convert_to_pint_unit(unit, self.imperial_units)
+
                     first = IngredientAmount(
-                        quantity=matching_tokens.pop(0),
-                        unit=matching_tokens.pop(-1),
+                        quantity=quantity,
+                        unit=unit,
+                        text=text,
                         confidence=round(
                             mean([matching_scores.pop(0), matching_scores.pop(-1)]), 6
                         ),
                         starting_index=idx[match[0]],
                         APPROXIMATE=self._is_approximate(match[0], tokens, labels, idx),
                     )
                     amounts.append(first)
@@ -422,21 +463,27 @@
                     _ = match.pop(-1)
 
                     # Now create the IngredientAmount objects for the pairs in between
                     # the first and last items
                     for i in range(0, len(matching_tokens), 2):
                         quantity = matching_tokens[i]
                         unit = matching_tokens[i + 1]
+                        text = " ".join((quantity, unit)).strip()
                         confidence = mean(matching_scores[i : i + 1])
 
+                        if not self.string_units:
+                            # Conver to pint.Unit if appropriate
+                            unit = convert_to_pint_unit(unit, self.imperial_units)
+
                         # If the first amount (e.g. 1 can) is approximate, so are all
                         # the pairs in between
                         amount = IngredientAmount(
                             quantity=quantity,
                             unit=unit,
+                            text=text,
                             confidence=round(confidence, 6),
                             starting_index=idx[match[i]],
                             SINGULAR=True,
                             APPROXIMATE=first.APPROXIMATE,
                         )
                         amounts.append(amount)
 
@@ -498,24 +545,40 @@
                 first_unit_idx = match[1]
                 last_unit_idx = match[-1]
                 if (
                     tokens[first_unit_idx] in first_unit
                     and tokens[last_unit_idx] in last_unit
                 ):
                     # First amount
+                    quantity_1 = tokens[match[0]]
+                    unit_1 = tokens[match[1]]
+                    text_1 = " ".join((quantity_1, unit_1)).strip()
+                    if not self.string_units:
+                        # Convert to pint.Unit if appropriate
+                        unit_1 = convert_to_pint_unit(unit_1, self.imperial_units)
+
                     first_amount = IngredientAmount(
-                        quantity=tokens[match[0]],
-                        unit=tokens[match[1]],
+                        quantity=quantity_1,
+                        unit=unit_1,
+                        text=text_1,
                         confidence=round(mean([scores[i] for i in match[0:2]]), 6),
                         starting_index=idx[first_unit_idx - 1],
                     )
                     # Second amount
+                    quantity_2 = tokens[match[2]]
+                    unit_2 = " ".join([tokens[i] for i in match[3:]])
+                    text_2 = " ".join((quantity_2, unit_2)).strip()
+                    if not self.string_units:
+                        # Convert to pint.Unit if appropriate
+                        unit_2 = convert_to_pint_unit(unit_2, self.imperial_units)
+
                     second_amount = IngredientAmount(
-                        quantity=tokens[match[2]],
-                        unit=" ".join([tokens[i] for i in match[3:]]),
+                        quantity=quantity_2,
+                        unit=unit_2,
+                        text=text_2,
                         confidence=round(mean([scores[i] for i in match[3:]]), 6),
                         starting_index=idx[last_unit_idx - 1],
                     )
                     composite_amounts.append(
                         CompositeIngredientAmount(
                             amounts=[first_amount, second_amount],
                             join="",
@@ -661,17 +724,17 @@
                             quantity="",
                             unit=[],
                             confidence=[score],
                             _starting_index=idx[i],
                         )
                     )
 
-                if i > 0 and labels[i - 1] == "COMMA":
-                    # If previous token was a comma, append to unit
-                    # of last IngredientAmount
+                if i > 0 and tokens[i - 1] == "," and amounts[-1].unit != []:
+                    # If the previous token was a comma, and the last amount has a unit,
+                    # append comma to unit of last IngredientAmount
                     amounts[-1].unit.append(",")
 
                 # Append token and score for unit to last IngredientAmount
                 amounts[-1].unit.append(token)
                 amounts[-1].confidence.append(score)
 
             # Check if any flags should be set
@@ -690,19 +753,30 @@
 
         # Loop through amounts list to fix unit and confidence
         # Unit needs converting to a string
         # Confidence needs averaging
         # Then convert to IngredientAmount object
         processed_amounts = []
         for amount in amounts:
+            unit = " ".join(amount.unit)
+            text = " ".join((amount.quantity, unit)).strip()
+
+            if not self.string_units:
+                # If the unit is recognised in the pint unit registry, use
+                # a pint.Unit object instead of a string. This has the benefit of
+                # simplifying alternative unit representations into a single
+                # common representation
+                unit = convert_to_pint_unit(unit, self.imperial_units)
+
             # Convert to an IngredientAmount object for returning
             processed_amounts.append(
                 IngredientAmount(
                     quantity=amount.quantity,
-                    unit=" ".join(amount.unit),
+                    unit=unit,
+                    text=text,
                     confidence=round(mean(amount.confidence), 6),
                     starting_index=amount._starting_index,
                     APPROXIMATE=amount.APPROXIMATE,
                     SINGULAR=amount.SINGULAR,
                 )
             )
```

### Comparing `ingredient_parser_nlp-0.1.0b8/ingredient_parser/preprocess/funcs.py` & `ingredient_parser_nlp-0.1.0b9/ingredient_parser/preprocess/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 STEMMER = PorterStemmer()
 
 # Define regular expressions used by tokenizer.
 # Matches one or more whitespace characters
 WHITESPACE_TOKENISER = re.compile(r"\S+")
 # Matches and captures one of the following: ( ) [ ] { } , " / : ;
-PUNCTUATION_TOKENISER = re.compile(r"([\(\)\[\]\{\}\,\"/:;])")
+PUNCTUATION_TOKENISER = re.compile(r"([\(\)\[\]\{\}\,/:;])")
 
 
 def tokenize(sentence: str) -> list[str]:
     """Tokenise an ingredient sentence.
     The sentence is split on whitespace characters into a list of tokens.
     If any of these tokens contains of the punctuation marks captured by
     PUNCTUATION_TOKENISER, these are then split and isolated as a seperate
```

### Comparing `ingredient_parser_nlp-0.1.0b8/ingredient_parser/preprocess/preprocess.py` & `ingredient_parser_nlp-0.1.0b9/ingredient_parser/preprocess/preprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 #!/usr/bin/env python3
 
+import re
+import string
 from fractions import Fraction
 from html import unescape
 
 from nltk.tag import pos_tag
 
 from ingredient_parser._constants import (
     AMBIGUOUS_UNITS,
+    FLATTENED_UNITS_LIST,
+    STRING_NUMBERS,
     STRING_NUMBERS_REGEXES,
     UNICODE_FRACTIONS,
     UNITS,
 )
 
 from .funcs import stem, tokenize
 from .regex import (
@@ -25,15 +29,14 @@
     STRING_RANGE_PATTERN,
     UNITS_HYPHEN_QUANTITY_PATTERN,
     UNITS_QUANTITY_PATTERN,
 )
 
 
 class PreProcessor:
-
     """Recipe ingredient sentence PreProcessor class.
 
     Performs the necessary preprocessing on a sentence to generate the features
     required for the ingredient parser model.
 
     Each input sentence goes through a cleaning process to tidy up the input into a
     standardised form.
@@ -45,15 +48,15 @@
 
     1. | Replace all en-dashes and em-dashes with hyphens.
     2. | Replace numbers given as words with the numeric equivalent.
        | e.g. one >> 1
     3. | Replace fractions given in html markup with the unicode representation.
        | e.g. &frac12; >> ½
     4. | Replace unicode fractions with the equivalent decimal form. Decimals are
-       | rounded to 3 a maximum of decimal places.
+       | rounded to a maximum of 3 decimal places.
        | e.g. ½ >> 0.5
     5. | Replace "fake" fractions represented by 1/2, 2/3 etc. with the equivalent
        | decimal form
        | e.g. 1/2 >> 0.5
     6. | A space is enforced between quantities and units
     7. | Remove trailing periods from units
        | e.g. tsp. >> tsp
@@ -254,18 +257,54 @@
         "12 bonbons"
         """
 
         # STRING_NUMBER_REGEXES is a dict where the values are a tuple of the compiled
         # regular expression for matching a string number e.g. 'one', 'two' and the
         # substitution numerical value for that string number.
         for regex, substitution in STRING_NUMBERS_REGEXES.values():
-            sentence = regex.sub(rf"{substitution}", sentence)
+            # Find matches for current string number
+            for match in regex.finditer(sentence):
+                if self._valid_string_number_replacement(match, sentence):
+                    sentence = regex.sub(rf"{substitution}", sentence)
 
         return sentence
 
+    def _valid_string_number_replacement(self, match: re.Match, sentence: str) -> bool:
+        """Check if it's valid to do a string number replacement for the given Match
+        in the given sentence
+
+        Parameters
+        ----------
+        match : re.Match
+            Match object for matching string number in sentence
+        sentence : str
+            Sentence
+
+        Returns
+        -------
+        bool
+        """
+        # Check the character following the match, If it's not a hyphen, or we're at
+        # the end of the sentence, the replacement is valid.
+        next_char_idx = match.span()[-1]
+        if next_char_idx >= len(sentence) or sentence[next_char_idx] != "-":
+            return True
+
+        # If the next character is a hyphen, if the hyphen is followed by
+        # a unit or another string number, then also do the substitution.
+        sub_sentence = sentence[next_char_idx + 1 :]
+        units_and_numbers = FLATTENED_UNITS_LIST + list(STRING_NUMBERS.keys())
+        for unit_or_num in units_and_numbers:
+            # Add a space to end of unit_or_num to make sure we don't incorrectly
+            # get a substring match e.g. matching "g" when unit_or_num is grain.
+            if sub_sentence.startswith(unit_or_num + " "):
+                return True
+
+        return False
+
     def _replace_html_fractions(self, sentence: str) -> str:
         """Replace html fractions e.g. &frac12; with unicode equivalents
 
         Parameters
         ----------
         sentence : str
             Ingredient sentence
@@ -542,14 +581,18 @@
             return sentence
 
         for full_match, quantity1, unit1, quantity2, unit2 in matches:
             # We are only interested if the both captured units are the same
             if unit1 != unit2:
                 continue
 
+            # If capture unit not in units list, abort
+            if unit1 not in FLATTENED_UNITS_LIST:
+                continue
+
             sentence = sentence.replace(full_match, f"{quantity1}-{quantity2} {unit1}")
 
         return sentence
 
     def _merge_quantity_x(self, sentence: str) -> str:
         """Merge any quantity followed by "x" into a single token e.g. 1 x can -> 1x can
 
@@ -675,14 +718,39 @@
 
         >>> p = PreProcessor("")
         >>> p._is_unit("beef")
         False
         """
         return token.lower() in UNITS.values()
 
+    def _is_punc(self, token: str) -> bool:
+        """Return True if token is a punctuation mark
+
+        Parameters
+        ----------
+        token : str
+            Token to check
+
+        Returns
+        -------
+        bool
+            True if token is a punctuation mark, else False
+
+        Examples
+        --------
+        >>> p = PreProcessor("")
+        >>> p._is_unit("/")
+        True
+
+        >>> p = PreProcessor("")
+        >>> p._is_unit("beef")
+        False
+        """
+        return token in string.punctuation
+
     def _is_numeric(self, token: str) -> bool:
         """Return True if token is numeric
 
         Parameters
         ----------
         token : str
             Token to check
@@ -795,15 +863,15 @@
             True if index is inside parentheses or is parenthesis, else False
         """
         # If it's "(" or ")", return True
         if self.tokenized_sentence[index] in ["(", ")", "[", "]"]:
             return True
 
         open_parens, closed_parens = [], []
-        for i, token in enumerate((self.tokenized_sentence)):
+        for i, token in enumerate(self.tokenized_sentence):
             if token == "(" or token == "[":
                 open_parens.append(i)
             elif token == ")" or token == "]":
                 closed_parens.append(i)
 
         for start, end in zip(open_parens, closed_parens):
             if start < index < end:
@@ -851,41 +919,98 @@
         Returns
         -------
         dict[str, str | bool]
             Dictionary of features for token at index
         """
         token = self.tokenized_sentence[index]
         features = {
+            "bias": "",
             "stem": stem(token),
             "pos": self.pos_tags[index],
             "is_capitalised": self._is_capitalised(token),
             "is_numeric": self._is_numeric(token),
             "is_unit": self._is_unit(token),
+            "is_punc": self._is_punc(token),
             "is_ambiguous": self._is_ambiguous_unit(token),
             "is_in_parens": self._is_inside_parentheses(index),
             "is_after_comma": self._follows_comma(index),
             "is_after_plus": self._follows_plus(index),
             "is_short_phrase": len(self.tokenized_sentence) < 3,
         }
 
+        if token != stem(token):
+            features["token"] = token
+
         if index > 0:
-            features["prev_pos"] = self.pos_tags[index - 1]
-            features["prev_word"] = stem(self.tokenized_sentence[index - 1])
+            prev_token = self.tokenized_sentence[index - 1]
+            features["prev_pos"] = "+".join(
+                (self.pos_tags[index - 1], self.pos_tags[index])
+            )
+            features["prev_stem"] = stem(prev_token)
+            features["prev_is_capitalised"] = self._is_capitalised(prev_token)
+            features["prev_is_numeric"] = self._is_numeric(prev_token)
+            features["prev_is_unit"] = self._is_unit(prev_token)
+            features["prev_is_punc"] = self._is_punc(prev_token)
+            features["prev_is_ambiguous"] = self._is_ambiguous_unit(prev_token)
+            features["prev_is_in_parens"] = self._is_inside_parentheses(index - 1)
+            features["prev_is_after_comma"] = self._follows_comma(index - 1)
+            features["prev_is_after_plus"] = self._follows_plus(index - 1)
 
         if index > 1:
-            features["prev_pos2"] = self.pos_tags[index - 2]
-            features["prev_word2"] = stem(self.tokenized_sentence[index - 2])
+            prev_token2 = self.tokenized_sentence[index - 2]
+            features["prev_pos2"] = "+".join(
+                (
+                    self.pos_tags[index - 2],
+                    self.pos_tags[index - 1],
+                    self.pos_tags[index],
+                )
+            )
+            features["prev_stem2"] = stem(prev_token2)
+            features["prev_is_capitalised2"] = self._is_capitalised(prev_token2)
+            features["prev_is_numeric2"] = self._is_numeric(prev_token2)
+            features["prev_is_unit2"] = self._is_unit(prev_token2)
+            features["prev_is_punc2"] = self._is_punc(prev_token2)
+            features["prev_is_ambiguous2"] = self._is_ambiguous_unit(prev_token2)
+            features["prev_is_in_parens2"] = self._is_inside_parentheses(index - 2)
+            features["prev_is_after_comma2"] = self._follows_comma(index - 2)
+            features["prev_is_after_plus2"] = self._follows_plus(index - 2)
 
         if index < len(self.tokenized_sentence) - 1:
-            features["next_pos"] = self.pos_tags[index + 1]
-            features["next_word"] = stem(self.tokenized_sentence[index + 1])
+            next_token = self.tokenized_sentence[index + 1]
+            features["next_pos"] = "+".join(
+                (self.pos_tags[index], self.pos_tags[index + 1])
+            )
+            features["next_stem"] = stem(next_token)
+            features["next_is_capitalised"] = self._is_capitalised(next_token)
+            features["next_is_numeric"] = self._is_numeric(next_token)
+            features["next_is_unit"] = self._is_unit(next_token)
+            features["next_is_punc"] = self._is_punc(next_token)
+            features["next_is_ambiguous"] = self._is_ambiguous_unit(next_token)
+            features["next_is_in_parens"] = self._is_inside_parentheses(index + 1)
+            features["next_is_after_comma"] = self._follows_comma(index + 1)
+            features["next_is_after_plus"] = self._follows_plus(index + 1)
 
         if index < len(self.tokenized_sentence) - 2:
-            features["next_pos2"] = self.pos_tags[index + 2]
-            features["next_word2"] = stem(self.tokenized_sentence[index + 2])
+            next_token2 = self.tokenized_sentence[index + 2]
+            features["next_pos2"] = "+".join(
+                (
+                    self.pos_tags[index + 2],
+                    self.pos_tags[index + 1],
+                    self.pos_tags[index],
+                )
+            )
+            features["next_stem2"] = stem(next_token2)
+            features["next_is_capitalised2"] = self._is_capitalised(next_token2)
+            features["next_is_numeric2"] = self._is_numeric(next_token2)
+            features["next_is_unit2"] = self._is_unit(next_token2)
+            features["next_is_punc2"] = self._is_punc(next_token2)
+            features["next_is_ambiguous2"] = self._is_ambiguous_unit(next_token2)
+            features["next_is_in_parens2"] = self._is_inside_parentheses(index + 2)
+            features["next_is_after_comma2"] = self._follows_comma(index + 2)
+            features["next_is_after_plus2"] = self._follows_plus(index + 2)
 
         return features
 
     def sentence_features(self) -> list[dict[str, str | bool]]:
         """Return features for all tokens in sentence
 
         Returns
```

### Comparing `ingredient_parser_nlp-0.1.0b8/ingredient_parser_nlp.egg-info/PKG-INFO` & `ingredient_parser_nlp-0.1.0b9/ingredient_parser_nlp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingredient_parser_nlp
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: A Python package to parse structured information from recipe ingredient sentences
 Author-email: Tom Strange <tpstrange@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2024 Tom Strange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -27,14 +27,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: <=3.12,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nltk
 Requires-Dist: python-crfsuite
+Requires-Dist: pint
 
 # Ingredient Parser
 
 The Ingredient Parser package is a Python package for parsing structured information out of recipe ingredient sentences.
 
 ![](docs/source/_static/logo.png)
 
@@ -52,49 +53,54 @@
 
 Import the ```parse_ingredient``` function and pass it an ingredient sentence.
 
 ```python
 >>> from ingredient_parser import parse_ingredient
 >>> parse_ingredient("3 pounds pork shoulder, cut into 2-inch chunks")
 ParsedIngredient(
-    name=IngredientText(text='pork shoulder', confidence=0.999196),
+    name=IngredientText(text='pork shoulder', confidence=0.999193),
+    size=None,
     amount=[IngredientAmount(quantity='3',
-                             unit='pounds',
+                             unit=<Unit('pound')>,
                              text='3 pounds',
-                             confidence=0.998769,
+                             confidence=0.999906,,
                              APPROXIMATE=False,
                              SINGULAR=False)],
-    preparation=IngredientText(text='cut into 2 inch chunks', confidence=0.995614),
+    preparation=IngredientText(text='cut into 2 inch chunks', confidence=0.999193),
     comment=None,
     sentence='3 pounds pork shoulder, cut into 2-inch chunks'
 )
 ```
 
 ## Model accuracy
 
 The model used for labelling tokens in sentences, provided in the ```ingredient-parser/``` directory, has the following accuracy on a test data set of 25% of the total  data used:
 
 ```
 Sentence-level results:
-	Total: 14982
-	Correct: 14021
-	Incorrect: 961
-	-> 93.59% correct
+	Accuracy: 94.24%
 
 Word-level results:
-	Total: 105360
-	Correct: 102741
-	Incorrect: 2619
-	-> 97.51% correct
+	Accuracy 97.73%
+	Precision (micro) 97.72%
+	Recall (micro) 97.73%
+	F1 score (micro) 97.72%
 ```
 
 ## Development
 
 The development dependencies are in the ```requirements-dev.txt``` file. Details on the training process can be found in the [Model Guide](https://ingredient-parser.readthedocs.io/en/latest/guide/index.html) documentation.
 
+Before committing anything, install [pre-commit](https://pre-commit.com/) and run
+```
+pre-commit install
+```
+
+to install the pre-commit hooks.
+
 There is a simple web app for testing the parser with ingredient sentences and showing the parsed output. To run the web app, run the command
 
 ```bash
 $ flask --app webapp run
 ```
 
 ![Screen shot of web app](docs/source/_static/app-screenshot.png)
```

### Comparing `ingredient_parser_nlp-0.1.0b8/ingredient_parser_nlp.egg-info/SOURCES.txt` & `ingredient_parser_nlp-0.1.0b9/ingredient_parser_nlp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 MANIFEST.in
 README.md
 pyproject.toml
 ingredient_parser/ModelCard.md
 ingredient_parser/__init__.py
 ingredient_parser/_constants.py
 ingredient_parser/_utils.py
-ingredient_parser/model.crfsuite
+ingredient_parser/model.en.crfsuite
 ingredient_parser/parsers.py
+ingredient_parser/py.typed
 ingredient_parser/postprocess/__init__.py
 ingredient_parser/postprocess/dataclasses.py
 ingredient_parser/postprocess/postprocess.py
 ingredient_parser/preprocess/__init__.py
 ingredient_parser/preprocess/funcs.py
 ingredient_parser/preprocess/preprocess.py
 ingredient_parser/preprocess/regex.py
 ingredient_parser_nlp.egg-info/PKG-INFO
 ingredient_parser_nlp.egg-info/SOURCES.txt
 ingredient_parser_nlp.egg-info/dependency_links.txt
 ingredient_parser_nlp.egg-info/requires.txt
-ingredient_parser_nlp.egg-info/top_level.txt
-tests/test_utils.py
+ingredient_parser_nlp.egg-info/top_level.txt
```

### Comparing `ingredient_parser_nlp-0.1.0b8/pyproject.toml` & `ingredient_parser_nlp-0.1.0b9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Text Processing :: Linguistic",
 ]
 dependencies = [
     "nltk",
     "python-crfsuite",
+    "pint",
 ]
 
 [project.urls]
 Homepage = "https://github.com/strangetom/ingredient-parser/"
 Documentation = "https://ingredient-parser.readthedocs.io/en/latest/"
 Source = "https://github.com/strangetom/ingredient-parser"
 
@@ -54,31 +55,31 @@
 
 [tool.coverage.run]
 branch = true
 omit = [
     "tests/*"
 ]
 
-[tool.black]
-target-version = ["py310", "py311", "py312"]
-include = "\\.py$"
-extend-exclude = "\\.ipynb$"
-
 [tool.ruff]
-select = ["E", "F", "I"]
-ignore = ["E402"]
 exclude = [
     "**/__pycache__",
     ".git",
     "venv"
 ]
 line-length = 88
 
+[tool.ruff.lint]
+select = ["E", "F", "I"]
+ignore = ["E402"]
+
+[tool.ruff.format]
+docstring-code-format = true
+
 [tool.pyright]
 include = ["ingredient_parser"]
 exclude = ["**/__pycache__"]
 reportUnusedImport = true
 reportUnusedClass = true
 reportUnuedFunction = true
 reportUnusedVariable = true
 reportWildcardImportFromLibrary = true
-reportPrivateUsage = true
+reportPrivateUsage = true
```

