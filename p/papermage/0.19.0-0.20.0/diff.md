# Comparing `tmp/papermage-0.19.0.tar.gz` & `tmp/papermage-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papermage-0.19.0.tar", last modified: Mon Apr  1 22:58:11 2024, max compression
+gzip compressed data, was "papermage-0.20.0.tar", last modified: Fri Apr  5 22:30:08 2024, max compression
```

## Comparing `papermage-0.19.0.tar` & `papermage-0.20.0.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.850811 papermage-0.19.0/
--rw-r--r--   0 kylel      (502) staff       (20)    11358 2023-07-20 23:26:15.000000 papermage-0.19.0/LICENSE
--rw-r--r--   0 kylel      (502) staff       (20)     9255 2024-04-01 22:58:11.850426 papermage-0.19.0/PKG-INFO
--rw-r--r--   0 kylel      (502) staff       (20)     6438 2024-02-15 16:04:56.000000 papermage-0.19.0/README.md
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.821384 papermage-0.19.0/examples/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.19.0/examples/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1424 2023-09-07 22:51:15.000000 papermage-0.19.0/examples/how_predictors_help_each_other.py
--rw-r--r--   0 kylel      (502) staff       (20)      578 2024-02-04 00:54:44.000000 papermage-0.19.0/examples/improving_sections.py
--rw-r--r--   0 kylel      (502) staff       (20)     2480 2024-03-21 20:28:43.000000 papermage-0.19.0/examples/visualize_a_doc.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.822156 papermage-0.19.0/papermage/
--rw-r--r--   0 kylel      (502) staff       (20)       93 2023-08-07 08:19:36.000000 papermage-0.19.0/papermage/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.828074 papermage-0.19.0/papermage/magelib/
--rw-r--r--   0 kylel      (502) staff       (20)     1802 2024-03-14 22:28:04.000000 papermage-0.19.0/papermage/magelib/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     5054 2024-02-15 16:04:44.000000 papermage-0.19.0/papermage/magelib/box.py
--rw-r--r--   0 kylel      (502) staff       (20)     6858 2024-03-14 22:28:04.000000 papermage-0.19.0/papermage/magelib/document.py
--rw-r--r--   0 kylel      (502) staff       (20)     7641 2024-03-17 22:30:35.000000 papermage-0.19.0/papermage/magelib/entity.py
--rw-r--r--   0 kylel      (502) staff       (20)     3963 2023-10-11 15:02:41.000000 papermage-0.19.0/papermage/magelib/image.py
--rw-r--r--   0 kylel      (502) staff       (20)     6250 2023-10-10 23:43:41.000000 papermage-0.19.0/papermage/magelib/indexer.py
--rw-r--r--   0 kylel      (502) staff       (20)     4263 2024-03-14 22:28:04.000000 papermage-0.19.0/papermage/magelib/layer.py
--rw-r--r--   0 kylel      (502) staff       (20)    15532 2023-08-06 02:20:53.000000 papermage-0.19.0/papermage/magelib/metadata.py
--rw-r--r--   0 kylel      (502) staff       (20)      877 2024-03-14 22:28:04.000000 papermage-0.19.0/papermage/magelib/names.py
--rw-r--r--   0 kylel      (502) staff       (20)     2051 2023-09-11 13:01:19.000000 papermage-0.19.0/papermage/magelib/span.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.829239 papermage-0.19.0/papermage/parsers/
--rw-r--r--   0 kylel      (502) staff       (20)      102 2023-07-20 23:36:48.000000 papermage-0.19.0/papermage/parsers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)    14955 2023-10-14 07:16:14.000000 papermage-0.19.0/papermage/parsers/grobid_parser.py
--rw-r--r--   0 kylel      (502) staff       (20)      595 2023-08-06 02:20:53.000000 papermage-0.19.0/papermage/parsers/parser.py
--rw-r--r--   0 kylel      (502) staff       (20)    18459 2023-08-06 21:43:49.000000 papermage-0.19.0/papermage/parsers/pdfplumber_parser.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.831787 papermage-0.19.0/papermage/predictors/
--rw-r--r--   0 kylel      (502) staff       (20)      982 2023-11-30 05:00:36.000000 papermage-0.19.0/papermage/predictors/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.835762 papermage-0.19.0/papermage/predictors/base_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-09-21 21:40:36.000000 papermage-0.19.0/papermage/predictors/base_predictors/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)       17 2023-09-21 21:40:36.000000 papermage-0.19.0/papermage/predictors/base_predictors/api_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     1351 2023-11-30 05:00:36.000000 papermage-0.19.0/papermage/predictors/base_predictors/base_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)    18228 2023-10-14 19:10:01.000000 papermage-0.19.0/papermage/predictors/base_predictors/hf_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     3528 2023-11-30 05:00:36.000000 papermage-0.19.0/papermage/predictors/base_predictors/lp_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)       17 2023-09-21 21:40:36.000000 papermage-0.19.0/papermage/predictors/base_predictors/sklearn_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)       17 2023-09-21 21:40:36.000000 papermage-0.19.0/papermage/predictors/base_predictors/spacy_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)      448 2023-09-21 21:40:36.000000 papermage-0.19.0/papermage/predictors/block_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)      436 2023-09-21 21:40:36.000000 papermage-0.19.0/papermage/predictors/formula_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     3463 2023-10-10 23:43:41.000000 papermage-0.19.0/papermage/predictors/sentence_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     3831 2023-10-14 07:16:14.000000 papermage-0.19.0/papermage/predictors/span_qa_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     1742 2023-09-21 21:40:36.000000 papermage-0.19.0/papermage/predictors/token_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     9228 2024-03-14 22:28:04.000000 papermage-0.19.0/papermage/predictors/vila_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)    22885 2023-10-14 07:16:14.000000 papermage-0.19.0/papermage/predictors/word_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-08-06 21:43:49.000000 papermage-0.19.0/papermage/py.typed
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.836261 papermage-0.19.0/papermage/rasterizers/
--rw-r--r--   0 kylel      (502) staff       (20)      105 2023-07-21 03:02:56.000000 papermage-0.19.0/papermage/rasterizers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     2042 2023-10-14 07:16:14.000000 papermage-0.19.0/papermage/rasterizers/rasterizer.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.837677 papermage-0.19.0/papermage/recipes/
--rw-r--r--   0 kylel      (502) staff       (20)      305 2024-04-01 22:33:01.000000 papermage-0.19.0/papermage/recipes/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     5697 2024-03-14 22:28:04.000000 papermage-0.19.0/papermage/recipes/core_recipe.py
--rw-r--r--   0 kylel      (502) staff       (20)     2690 2024-04-01 22:47:51.000000 papermage-0.19.0/papermage/recipes/minimal_pdf_recipe.py
--rw-r--r--   0 kylel      (502) staff       (20)     1299 2023-09-11 12:41:20.000000 papermage-0.19.0/papermage/recipes/recipe.py
--rw-r--r--   0 kylel      (502) staff       (20)     1178 2023-10-14 07:16:14.000000 papermage-0.19.0/papermage/recipes/text_recipe.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.838031 papermage-0.19.0/papermage/trainers/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-31 09:58:28.000000 papermage-0.19.0/papermage/trainers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)    21793 2023-10-10 23:43:41.000000 papermage-0.19.0/papermage/trainers/bio_tagger_predictor_trainer.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.839483 papermage-0.19.0/papermage/utils/
--rw-r--r--   0 kylel      (502) staff       (20)      171 2023-08-07 08:19:36.000000 papermage-0.19.0/papermage/utils/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1883 2023-10-10 23:43:41.000000 papermage-0.19.0/papermage/utils/annotate.py
--rw-r--r--   0 kylel      (502) staff       (20)     3720 2023-09-11 13:01:19.000000 papermage-0.19.0/papermage/utils/merge.py
--rw-r--r--   0 kylel      (502) staff       (20)      307 2023-08-06 21:43:49.000000 papermage-0.19.0/papermage/utils/text.py
--rw-r--r--   0 kylel      (502) staff       (20)     1025 2023-08-06 21:43:49.000000 papermage-0.19.0/papermage/utils/version.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.839947 papermage-0.19.0/papermage/visualizers/
--rw-r--r--   0 kylel      (502) staff       (20)       83 2023-08-08 22:07:02.000000 papermage-0.19.0/papermage/visualizers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1812 2024-03-13 22:23:41.000000 papermage-0.19.0/papermage/visualizers/visualizer.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.848239 papermage-0.19.0/papermage.egg-info/
--rw-r--r--   0 kylel      (502) staff       (20)     9255 2024-04-01 22:58:11.000000 papermage-0.19.0/papermage.egg-info/PKG-INFO
--rw-r--r--   0 kylel      (502) staff       (20)     3469 2024-04-01 22:58:11.000000 papermage-0.19.0/papermage.egg-info/SOURCES.txt
--rw-r--r--   0 kylel      (502) staff       (20)        1 2024-04-01 22:58:11.000000 papermage-0.19.0/papermage.egg-info/dependency_links.txt
--rw-r--r--   0 kylel      (502) staff       (20)      588 2024-04-01 22:58:11.000000 papermage-0.19.0/papermage.egg-info/requires.txt
--rw-r--r--   0 kylel      (502) staff       (20)       49 2024-04-01 22:58:11.000000 papermage-0.19.0/papermage.egg-info/top_level.txt
--rw-r--r--   0 kylel      (502) staff       (20)     4015 2024-04-01 22:55:04.000000 papermage-0.19.0/pyproject.toml
--rw-r--r--   0 kylel      (502) staff       (20)       33 2023-09-07 02:55:51.000000 papermage-0.19.0/requirements.txt
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.840405 papermage-0.19.0/scripts/
--rw-r--r--   0 kylel      (502) staff       (20)     5027 2023-10-14 07:16:14.000000 papermage-0.19.0/scripts/evaluation.py
--rw-r--r--   0 kylel      (502) staff       (20)      802 2023-11-30 22:47:38.000000 papermage-0.19.0/scripts/get_thumbnails_for_papers.py
--rw-r--r--   0 kylel      (502) staff       (20)       38 2024-04-01 22:58:11.850886 papermage-0.19.0/setup.cfg
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.840662 papermage-0.19.0/tests/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.19.0/tests/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.842670 papermage-0.19.0/tests/test_magelib/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-08-06 02:20:53.000000 papermage-0.19.0/tests/test_magelib/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     4929 2023-08-06 02:20:53.000000 papermage-0.19.0/tests/test_magelib/test_box.py
--rw-r--r--   0 kylel      (502) staff       (20)    11905 2024-03-17 22:30:35.000000 papermage-0.19.0/tests/test_magelib/test_document.py
--rw-r--r--   0 kylel      (502) staff       (20)     4073 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_magelib/test_entity.py
--rw-r--r--   0 kylel      (502) staff       (20)     2535 2023-08-06 02:20:53.000000 papermage-0.19.0/tests/test_magelib/test_image.py
--rw-r--r--   0 kylel      (502) staff       (20)     4378 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_magelib/test_indexer.py
--rw-r--r--   0 kylel      (502) staff       (20)     1152 2023-10-10 23:43:41.000000 papermage-0.19.0/tests/test_magelib/test_layer.py
--rw-r--r--   0 kylel      (502) staff       (20)     1853 2023-08-06 02:20:53.000000 papermage-0.19.0/tests/test_magelib/test_metadata.py
--rw-r--r--   0 kylel      (502) staff       (20)     1938 2023-09-11 13:01:19.000000 papermage-0.19.0/tests/test_magelib/test_span.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.843032 papermage-0.19.0/tests/test_parsers/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.19.0/tests/test_parsers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     8971 2023-08-06 02:20:53.000000 papermage-0.19.0/tests/test_parsers/test_pdf_plumber_parser.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.844600 papermage-0.19.0/tests/test_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.19.0/tests/test_predictors/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.844925 papermage-0.19.0/tests/test_predictors/test_base_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-09-21 21:40:36.000000 papermage-0.19.0/tests/test_predictors/test_base_predictors/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1771 2023-09-21 21:40:36.000000 papermage-0.19.0/tests/test_predictors/test_base_predictors/test_lp_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     5151 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_predictors/test_bio_tagger_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)      421 2023-09-21 21:40:36.000000 papermage-0.19.0/tests/test_predictors/test_block_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)      411 2023-09-21 21:40:36.000000 papermage-0.19.0/tests/test_predictors/test_formula_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     3293 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_predictors/test_sentence_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     4010 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_predictors/test_span_qa_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     2636 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_predictors/test_vila_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     2220 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_predictors/test_whitespace_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     4957 2023-09-21 21:40:36.000000 papermage-0.19.0/tests/test_predictors/test_word_predictor.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.845259 papermage-0.19.0/tests/test_rasterizers/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.19.0/tests/test_rasterizers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1048 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_rasterizers/test_pdf2image_rasterizer.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.846069 papermage-0.19.0/tests/test_recipes/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-08-06 02:20:53.000000 papermage-0.19.0/tests/test_recipes/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1096 2023-12-18 19:03:22.000000 papermage-0.19.0/tests/test_recipes/test_core_recipe.py
--rw-r--r--   0 kylel      (502) staff       (20)     1899 2024-04-01 22:54:31.000000 papermage-0.19.0/tests/test_recipes/test_minimal_pdf_recipe.py
--rw-r--r--   0 kylel      (502) staff       (20)      746 2023-09-11 12:41:20.000000 papermage-0.19.0/tests/test_recipes/test_text_recipe.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.846284 papermage-0.19.0/tests/test_trainers/
--rw-r--r--   0 kylel      (502) staff       (20)     7683 2023-10-14 07:16:14.000000 papermage-0.19.0/tests/test_trainers/test_entity_classification_predictor_trainer.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.846588 papermage-0.19.0/tests/test_utils/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-09-11 13:01:19.000000 papermage-0.19.0/tests/test_utils/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     3492 2023-09-11 13:01:19.000000 papermage-0.19.0/tests/test_utils/test_merge.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-01 22:58:11.846933 papermage-0.19.0/tests/test_visualizers/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2023-08-06 02:20:53.000000 papermage-0.19.0/tests/test_visualizers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)      890 2023-08-06 02:20:53.000000 papermage-0.19.0/tests/test_visualizers/test_visualizer.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.530238 papermage-0.20.0/
+-rw-r--r--   0 kylel      (502) staff       (20)    11358 2023-07-20 23:26:15.000000 papermage-0.20.0/LICENSE
+-rw-r--r--   0 kylel      (502) staff       (20)     9280 2024-04-05 22:30:08.529802 papermage-0.20.0/PKG-INFO
+-rw-r--r--   0 kylel      (502) staff       (20)     6438 2024-02-15 16:04:56.000000 papermage-0.20.0/README.md
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.498789 papermage-0.20.0/examples/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.20.0/examples/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1424 2023-09-07 22:51:15.000000 papermage-0.20.0/examples/how_predictors_help_each_other.py
+-rw-r--r--   0 kylel      (502) staff       (20)      578 2024-02-04 00:54:44.000000 papermage-0.20.0/examples/improving_sections.py
+-rw-r--r--   0 kylel      (502) staff       (20)     2480 2024-03-21 20:28:43.000000 papermage-0.20.0/examples/visualize_a_doc.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.499749 papermage-0.20.0/papermage/
+-rw-r--r--   0 kylel      (502) staff       (20)       93 2023-08-07 08:19:36.000000 papermage-0.20.0/papermage/__init__.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.504004 papermage-0.20.0/papermage/magelib/
+-rw-r--r--   0 kylel      (502) staff       (20)     1802 2024-03-14 22:28:04.000000 papermage-0.20.0/papermage/magelib/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     5054 2024-02-15 16:04:44.000000 papermage-0.20.0/papermage/magelib/box.py
+-rw-r--r--   0 kylel      (502) staff       (20)     6858 2024-03-14 22:28:04.000000 papermage-0.20.0/papermage/magelib/document.py
+-rw-r--r--   0 kylel      (502) staff       (20)     7641 2024-03-17 22:30:35.000000 papermage-0.20.0/papermage/magelib/entity.py
+-rw-r--r--   0 kylel      (502) staff       (20)     3963 2023-10-11 15:02:41.000000 papermage-0.20.0/papermage/magelib/image.py
+-rw-r--r--   0 kylel      (502) staff       (20)     6250 2023-10-10 23:43:41.000000 papermage-0.20.0/papermage/magelib/indexer.py
+-rw-r--r--   0 kylel      (502) staff       (20)     4263 2024-03-14 22:28:04.000000 papermage-0.20.0/papermage/magelib/layer.py
+-rw-r--r--   0 kylel      (502) staff       (20)    15532 2023-08-06 02:20:53.000000 papermage-0.20.0/papermage/magelib/metadata.py
+-rw-r--r--   0 kylel      (502) staff       (20)      877 2024-03-14 22:28:04.000000 papermage-0.20.0/papermage/magelib/names.py
+-rw-r--r--   0 kylel      (502) staff       (20)     2051 2023-09-11 13:01:19.000000 papermage-0.20.0/papermage/magelib/span.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.505180 papermage-0.20.0/papermage/parsers/
+-rw-r--r--   0 kylel      (502) staff       (20)      102 2023-07-20 23:36:48.000000 papermage-0.20.0/papermage/parsers/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)    14955 2023-10-14 07:16:14.000000 papermage-0.20.0/papermage/parsers/grobid_parser.py
+-rw-r--r--   0 kylel      (502) staff       (20)      595 2023-08-06 02:20:53.000000 papermage-0.20.0/papermage/parsers/parser.py
+-rw-r--r--   0 kylel      (502) staff       (20)    18459 2023-08-06 21:43:49.000000 papermage-0.20.0/papermage/parsers/pdfplumber_parser.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.507918 papermage-0.20.0/papermage/predictors/
+-rw-r--r--   0 kylel      (502) staff       (20)      987 2024-04-05 19:21:52.000000 papermage-0.20.0/papermage/predictors/__init__.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.509987 papermage-0.20.0/papermage/predictors/base_predictors/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-09-21 21:40:36.000000 papermage-0.20.0/papermage/predictors/base_predictors/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)       17 2023-09-21 21:40:36.000000 papermage-0.20.0/papermage/predictors/base_predictors/api_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1351 2023-11-30 05:00:36.000000 papermage-0.20.0/papermage/predictors/base_predictors/base_predictor.py
+-rw-r--r--   0 kylel      (502) staff       (20)    18228 2023-10-14 19:10:01.000000 papermage-0.20.0/papermage/predictors/base_predictors/hf_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     3528 2023-11-30 05:00:36.000000 papermage-0.20.0/papermage/predictors/base_predictors/lp_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)       17 2023-09-21 21:40:36.000000 papermage-0.20.0/papermage/predictors/base_predictors/sklearn_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)       17 2023-09-21 21:40:36.000000 papermage-0.20.0/papermage/predictors/base_predictors/spacy_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)      448 2023-09-21 21:40:36.000000 papermage-0.20.0/papermage/predictors/block_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)      436 2023-09-21 21:40:36.000000 papermage-0.20.0/papermage/predictors/formula_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     3463 2023-10-10 23:43:41.000000 papermage-0.20.0/papermage/predictors/sentence_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     3831 2023-10-14 07:16:14.000000 papermage-0.20.0/papermage/predictors/span_qa_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1742 2023-09-21 21:40:36.000000 papermage-0.20.0/papermage/predictors/token_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     9228 2024-03-14 22:28:04.000000 papermage-0.20.0/papermage/predictors/vila_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)    22885 2023-10-14 07:16:14.000000 papermage-0.20.0/papermage/predictors/word_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-08-06 21:43:49.000000 papermage-0.20.0/papermage/py.typed
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.514084 papermage-0.20.0/papermage/rasterizers/
+-rw-r--r--   0 kylel      (502) staff       (20)      105 2023-07-21 03:02:56.000000 papermage-0.20.0/papermage/rasterizers/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     2042 2023-10-14 07:16:14.000000 papermage-0.20.0/papermage/rasterizers/rasterizer.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.515757 papermage-0.20.0/papermage/recipes/
+-rw-r--r--   0 kylel      (502) staff       (20)      305 2024-04-01 22:58:27.000000 papermage-0.20.0/papermage/recipes/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     5697 2024-03-14 22:28:04.000000 papermage-0.20.0/papermage/recipes/core_recipe.py
+-rw-r--r--   0 kylel      (502) staff       (20)     2690 2024-04-01 22:58:27.000000 papermage-0.20.0/papermage/recipes/minimal_pdf_recipe.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1299 2023-09-11 12:41:20.000000 papermage-0.20.0/papermage/recipes/recipe.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1178 2023-10-14 07:16:14.000000 papermage-0.20.0/papermage/recipes/text_recipe.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.516078 papermage-0.20.0/papermage/trainers/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-31 09:58:28.000000 papermage-0.20.0/papermage/trainers/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)    21793 2023-10-10 23:43:41.000000 papermage-0.20.0/papermage/trainers/bio_tagger_predictor_trainer.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.517717 papermage-0.20.0/papermage/utils/
+-rw-r--r--   0 kylel      (502) staff       (20)      171 2023-08-07 08:19:36.000000 papermage-0.20.0/papermage/utils/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1883 2023-10-10 23:43:41.000000 papermage-0.20.0/papermage/utils/annotate.py
+-rw-r--r--   0 kylel      (502) staff       (20)     3720 2023-09-11 13:01:19.000000 papermage-0.20.0/papermage/utils/merge.py
+-rw-r--r--   0 kylel      (502) staff       (20)      307 2023-08-06 21:43:49.000000 papermage-0.20.0/papermage/utils/text.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1025 2023-08-06 21:43:49.000000 papermage-0.20.0/papermage/utils/version.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.518247 papermage-0.20.0/papermage/visualizers/
+-rw-r--r--   0 kylel      (502) staff       (20)       83 2023-08-08 22:07:02.000000 papermage-0.20.0/papermage/visualizers/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1812 2024-03-13 22:23:41.000000 papermage-0.20.0/papermage/visualizers/visualizer.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.528103 papermage-0.20.0/papermage.egg-info/
+-rw-r--r--   0 kylel      (502) staff       (20)     9280 2024-04-05 22:30:08.000000 papermage-0.20.0/papermage.egg-info/PKG-INFO
+-rw-r--r--   0 kylel      (502) staff       (20)     3469 2024-04-05 22:30:08.000000 papermage-0.20.0/papermage.egg-info/SOURCES.txt
+-rw-r--r--   0 kylel      (502) staff       (20)        1 2024-04-05 22:30:08.000000 papermage-0.20.0/papermage.egg-info/dependency_links.txt
+-rw-r--r--   0 kylel      (502) staff       (20)      601 2024-04-05 22:30:08.000000 papermage-0.20.0/papermage.egg-info/requires.txt
+-rw-r--r--   0 kylel      (502) staff       (20)       49 2024-04-05 22:30:08.000000 papermage-0.20.0/papermage.egg-info/top_level.txt
+-rw-r--r--   0 kylel      (502) staff       (20)     4030 2024-04-05 17:31:05.000000 papermage-0.20.0/pyproject.toml
+-rw-r--r--   0 kylel      (502) staff       (20)       33 2023-09-07 02:55:51.000000 papermage-0.20.0/requirements.txt
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.518742 papermage-0.20.0/scripts/
+-rw-r--r--   0 kylel      (502) staff       (20)     5027 2023-10-14 07:16:14.000000 papermage-0.20.0/scripts/evaluation.py
+-rw-r--r--   0 kylel      (502) staff       (20)      802 2023-11-30 22:47:38.000000 papermage-0.20.0/scripts/get_thumbnails_for_papers.py
+-rw-r--r--   0 kylel      (502) staff       (20)       38 2024-04-05 22:30:08.530315 papermage-0.20.0/setup.cfg
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.519034 papermage-0.20.0/tests/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.20.0/tests/__init__.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.521497 papermage-0.20.0/tests/test_magelib/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-08-06 02:20:53.000000 papermage-0.20.0/tests/test_magelib/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     4929 2023-08-06 02:20:53.000000 papermage-0.20.0/tests/test_magelib/test_box.py
+-rw-r--r--   0 kylel      (502) staff       (20)    11905 2024-03-17 22:30:35.000000 papermage-0.20.0/tests/test_magelib/test_document.py
+-rw-r--r--   0 kylel      (502) staff       (20)     4073 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_magelib/test_entity.py
+-rw-r--r--   0 kylel      (502) staff       (20)     2535 2023-08-06 02:20:53.000000 papermage-0.20.0/tests/test_magelib/test_image.py
+-rw-r--r--   0 kylel      (502) staff       (20)     4378 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_magelib/test_indexer.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1152 2023-10-10 23:43:41.000000 papermage-0.20.0/tests/test_magelib/test_layer.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1853 2023-08-06 02:20:53.000000 papermage-0.20.0/tests/test_magelib/test_metadata.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1938 2023-09-11 13:01:19.000000 papermage-0.20.0/tests/test_magelib/test_span.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.521961 papermage-0.20.0/tests/test_parsers/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.20.0/tests/test_parsers/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     8971 2023-08-06 02:20:53.000000 papermage-0.20.0/tests/test_parsers/test_pdf_plumber_parser.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.524125 papermage-0.20.0/tests/test_predictors/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.20.0/tests/test_predictors/__init__.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.524555 papermage-0.20.0/tests/test_predictors/test_base_predictors/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-09-21 21:40:36.000000 papermage-0.20.0/tests/test_predictors/test_base_predictors/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1771 2023-09-21 21:40:36.000000 papermage-0.20.0/tests/test_predictors/test_base_predictors/test_lp_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     5151 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_predictors/test_bio_tagger_predictor.py
+-rw-r--r--   0 kylel      (502) staff       (20)      421 2023-09-21 21:40:36.000000 papermage-0.20.0/tests/test_predictors/test_block_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)      411 2023-09-21 21:40:36.000000 papermage-0.20.0/tests/test_predictors/test_formula_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     3293 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_predictors/test_sentence_predictor.py
+-rw-r--r--   0 kylel      (502) staff       (20)     4010 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_predictors/test_span_qa_predictors.py
+-rw-r--r--   0 kylel      (502) staff       (20)     2636 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_predictors/test_vila_predictor.py
+-rw-r--r--   0 kylel      (502) staff       (20)     2220 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_predictors/test_whitespace_predictor.py
+-rw-r--r--   0 kylel      (502) staff       (20)     4957 2023-09-21 21:40:36.000000 papermage-0.20.0/tests/test_predictors/test_word_predictor.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.524924 papermage-0.20.0/tests/test_rasterizers/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-07-20 23:26:15.000000 papermage-0.20.0/tests/test_rasterizers/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1048 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_rasterizers/test_pdf2image_rasterizer.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.526045 papermage-0.20.0/tests/test_recipes/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-08-06 02:20:53.000000 papermage-0.20.0/tests/test_recipes/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1096 2023-12-18 19:03:22.000000 papermage-0.20.0/tests/test_recipes/test_core_recipe.py
+-rw-r--r--   0 kylel      (502) staff       (20)     1899 2024-04-01 22:58:27.000000 papermage-0.20.0/tests/test_recipes/test_minimal_pdf_recipe.py
+-rw-r--r--   0 kylel      (502) staff       (20)      746 2023-09-11 12:41:20.000000 papermage-0.20.0/tests/test_recipes/test_text_recipe.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.526366 papermage-0.20.0/tests/test_trainers/
+-rw-r--r--   0 kylel      (502) staff       (20)     7683 2023-10-14 07:16:14.000000 papermage-0.20.0/tests/test_trainers/test_entity_classification_predictor_trainer.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.526880 papermage-0.20.0/tests/test_utils/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-09-11 13:01:19.000000 papermage-0.20.0/tests/test_utils/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)     3492 2023-09-11 13:01:19.000000 papermage-0.20.0/tests/test_utils/test_merge.py
+drwxr-xr-x   0 kylel      (502) staff       (20)        0 2024-04-05 22:30:08.527269 papermage-0.20.0/tests/test_visualizers/
+-rw-r--r--   0 kylel      (502) staff       (20)        0 2023-08-06 02:20:53.000000 papermage-0.20.0/tests/test_visualizers/__init__.py
+-rw-r--r--   0 kylel      (502) staff       (20)      890 2023-08-06 02:20:53.000000 papermage-0.20.0/tests/test_visualizers/test_visualizer.py
```

### Comparing `papermage-0.19.0/LICENSE` & `papermage-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/PKG-INFO` & `papermage-0.20.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papermage
-Version: 0.19.0
+Version: 0.20.0
 Summary: Papermage. Casting magic over scientific PDFs.
 Author-email: Kyle Lo <kylel@allenai.org>, Luca Soldaini <luca@soldaini.net>, Shannon Zejiang Shen <zejiangshen@gmail.com>, Ben Newman <blnewman@stanford.edu>, Russell Authur <russell.authur@gmail.com>, Stefan Candra <stefanc@allenai.org>, Yoganand Chandrasekhar <yogic@allenai.org>, Regan Huff <reganh@allenai.org>, Amanpreet Singh <amans@allenai.org>, Chris Wilhelm <chrisw@allenai.org>, Angele Zamarron <angelez@allenai.org>
 Maintainer-email: Kyle Lo <kylel@allenai.org>, Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://www.github.com/allenai/papermage
 Project-URL: Repository, https://www.github.com/allenai/papermage
 Project-URL: Bug Tracker, https://www.github.com/allenai/papermage/issues
@@ -45,16 +45,17 @@
 Requires-Dist: transformers==4.31.0; extra == "predictors"
 Requires-Dist: smashed==0.1.10; extra == "predictors"
 Requires-Dist: pytorch-lightning>=2.0.5; extra == "predictors"
 Requires-Dist: springs==1.13.0; extra == "predictors"
 Requires-Dist: wandb>=0.15.7; extra == "predictors"
 Requires-Dist: seqeval==1.2.2; extra == "predictors"
 Requires-Dist: effdet==0.3.0; extra == "predictors"
-Requires-Dist: decontext==0.1.6; extra == "predictors"
 Requires-Dist: vila==0.5.0; extra == "predictors"
+Provides-Extra: decontext
+Requires-Dist: decontext==0.1.6; extra == "decontext"
 Provides-Extra: production
 Requires-Dist: optimum[onnxruntime]==1.10.0; extra == "production"
 
 # papermage
 
 ### Setup
```

### Comparing `papermage-0.19.0/README.md` & `papermage-0.20.0/README.md`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/examples/how_predictors_help_each_other.py` & `papermage-0.20.0/examples/how_predictors_help_each_other.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/examples/improving_sections.py` & `papermage-0.20.0/examples/improving_sections.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/examples/visualize_a_doc.py` & `papermage-0.20.0/examples/visualize_a_doc.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/__init__.py` & `papermage-0.20.0/papermage/magelib/__init__.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/box.py` & `papermage-0.20.0/papermage/magelib/box.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/document.py` & `papermage-0.20.0/papermage/magelib/document.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/entity.py` & `papermage-0.20.0/papermage/magelib/entity.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/image.py` & `papermage-0.20.0/papermage/magelib/image.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/indexer.py` & `papermage-0.20.0/papermage/magelib/indexer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/layer.py` & `papermage-0.20.0/papermage/magelib/layer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/metadata.py` & `papermage-0.20.0/papermage/magelib/metadata.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/names.py` & `papermage-0.20.0/papermage/magelib/names.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/magelib/span.py` & `papermage-0.20.0/papermage/magelib/span.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/parsers/grobid_parser.py` & `papermage-0.20.0/papermage/parsers/grobid_parser.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/parsers/parser.py` & `papermage-0.20.0/papermage/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/parsers/pdfplumber_parser.py` & `papermage-0.20.0/papermage/parsers/pdfplumber_parser.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/predictors/__init__.py` & `papermage-0.20.0/papermage/predictors/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from papermage.predictors.base_predictors.base_predictor import BasePredictor
 from papermage.predictors.base_predictors.hf_predictors import HFBIOTaggerPredictor
 from papermage.predictors.block_predictors import LPEffDetPubLayNetBlockPredictor
 from papermage.predictors.formula_predictors import LPEffDetFormulaPredictor
 from papermage.predictors.sentence_predictors import PysbdSentencePredictor
-from papermage.predictors.span_qa_predictors import APISpanQAPredictor
+
+# from papermage.predictors.span_qa_predictors import APISpanQAPredictor
 from papermage.predictors.token_predictors import HFWhitspaceTokenPredictor
 from papermage.predictors.vila_predictors import IVILATokenClassificationPredictor
 from papermage.predictors.word_predictors import SVMWordPredictor
 
 __all__ = [
     "HFBIOTaggerPredictor",
     "IVILATokenClassificationPredictor",
     "HFWhitspaceTokenPredictor",
     "SVMWordPredictor",
     "PysbdSentencePredictor",
     "LPEffDetPubLayNetBlockPredictor",
     "LPEffDetFormulaPredictor",
-    "APISpanQAPredictor",
+    # "APISpanQAPredictor",
     "BasePredictor",
 ]
```

### Comparing `papermage-0.19.0/papermage/predictors/base_predictors/base_predictor.py` & `papermage-0.20.0/papermage/predictors/base_predictors/base_predictor.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/predictors/base_predictors/hf_predictors.py` & `papermage-0.20.0/papermage/predictors/base_predictors/hf_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/predictors/base_predictors/lp_predictors.py` & `papermage-0.20.0/papermage/predictors/base_predictors/lp_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/predictors/sentence_predictors.py` & `papermage-0.20.0/papermage/predictors/sentence_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/predictors/span_qa_predictors.py` & `papermage-0.20.0/papermage/predictors/span_qa_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/predictors/token_predictors.py` & `papermage-0.20.0/papermage/predictors/token_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/predictors/vila_predictors.py` & `papermage-0.20.0/papermage/predictors/vila_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/predictors/word_predictors.py` & `papermage-0.20.0/papermage/predictors/word_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/rasterizers/rasterizer.py` & `papermage-0.20.0/papermage/rasterizers/rasterizer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/recipes/core_recipe.py` & `papermage-0.20.0/papermage/recipes/core_recipe.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/recipes/minimal_pdf_recipe.py` & `papermage-0.20.0/papermage/recipes/minimal_pdf_recipe.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/recipes/recipe.py` & `papermage-0.20.0/papermage/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/recipes/text_recipe.py` & `papermage-0.20.0/papermage/recipes/text_recipe.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/trainers/bio_tagger_predictor_trainer.py` & `papermage-0.20.0/papermage/trainers/bio_tagger_predictor_trainer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/utils/annotate.py` & `papermage-0.20.0/papermage/utils/annotate.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/utils/merge.py` & `papermage-0.20.0/papermage/utils/merge.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/utils/version.py` & `papermage-0.20.0/papermage/utils/version.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage/visualizers/visualizer.py` & `papermage-0.20.0/papermage/visualizers/visualizer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/papermage.egg-info/PKG-INFO` & `papermage-0.20.0/papermage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: papermage
-Version: 0.19.0
+Version: 0.20.0
 Summary: Papermage. Casting magic over scientific PDFs.
 Author-email: Kyle Lo <kylel@allenai.org>, Luca Soldaini <luca@soldaini.net>, Shannon Zejiang Shen <zejiangshen@gmail.com>, Ben Newman <blnewman@stanford.edu>, Russell Authur <russell.authur@gmail.com>, Stefan Candra <stefanc@allenai.org>, Yoganand Chandrasekhar <yogic@allenai.org>, Regan Huff <reganh@allenai.org>, Amanpreet Singh <amans@allenai.org>, Chris Wilhelm <chrisw@allenai.org>, Angele Zamarron <angelez@allenai.org>
 Maintainer-email: Kyle Lo <kylel@allenai.org>, Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://www.github.com/allenai/papermage
 Project-URL: Repository, https://www.github.com/allenai/papermage
 Project-URL: Bug Tracker, https://www.github.com/allenai/papermage/issues
@@ -45,16 +45,17 @@
 Requires-Dist: transformers==4.31.0; extra == "predictors"
 Requires-Dist: smashed==0.1.10; extra == "predictors"
 Requires-Dist: pytorch-lightning>=2.0.5; extra == "predictors"
 Requires-Dist: springs==1.13.0; extra == "predictors"
 Requires-Dist: wandb>=0.15.7; extra == "predictors"
 Requires-Dist: seqeval==1.2.2; extra == "predictors"
 Requires-Dist: effdet==0.3.0; extra == "predictors"
-Requires-Dist: decontext==0.1.6; extra == "predictors"
 Requires-Dist: vila==0.5.0; extra == "predictors"
+Provides-Extra: decontext
+Requires-Dist: decontext==0.1.6; extra == "decontext"
 Provides-Extra: production
 Requires-Dist: optimum[onnxruntime]==1.10.0; extra == "production"
 
 # papermage
 
 ### Setup
```

### Comparing `papermage-0.19.0/papermage.egg-info/SOURCES.txt` & `papermage-0.20.0/papermage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/pyproject.toml` & `papermage-0.20.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'papermage'
-version = '0.19.0'
+version = '0.20.0'
 description = 'Papermage. Casting magic over scientific PDFs.'
 license = {text = 'Apache-2.0'}
 readme = 'README.md'
 requires-python = '>=3.8'
 dependencies = [
         'tqdm',
         'pdf2image',
@@ -127,17 +127,19 @@
     'transformers==4.31.0',
     'smashed==0.1.10',
     'pytorch-lightning>=2.0.5',
     'springs==1.13.0',
     'wandb>=0.15.7',
     'seqeval==1.2.2',
     'effdet==0.3.0',
-    'decontext==0.1.6',
     'vila==0.5.0'
 ]
+decontext = [
+    'decontext==0.1.6'
+]
 production = [
     'optimum[onnxruntime]==1.10.0'
 ]
 
 [tool.pytest.ini_options]
 addopts = '-n auto --cov=.'
 testpaths = ['tests/']
```

### Comparing `papermage-0.19.0/scripts/evaluation.py` & `papermage-0.20.0/scripts/evaluation.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/scripts/get_thumbnails_for_papers.py` & `papermage-0.20.0/scripts/get_thumbnails_for_papers.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_magelib/test_box.py` & `papermage-0.20.0/tests/test_magelib/test_box.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_magelib/test_document.py` & `papermage-0.20.0/tests/test_magelib/test_document.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_magelib/test_entity.py` & `papermage-0.20.0/tests/test_magelib/test_entity.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_magelib/test_image.py` & `papermage-0.20.0/tests/test_magelib/test_image.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_magelib/test_indexer.py` & `papermage-0.20.0/tests/test_magelib/test_indexer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_magelib/test_layer.py` & `papermage-0.20.0/tests/test_magelib/test_layer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_magelib/test_metadata.py` & `papermage-0.20.0/tests/test_magelib/test_metadata.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_magelib/test_span.py` & `papermage-0.20.0/tests/test_magelib/test_span.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_parsers/test_pdf_plumber_parser.py` & `papermage-0.20.0/tests/test_parsers/test_pdf_plumber_parser.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_predictors/test_base_predictors/test_lp_predictors.py` & `papermage-0.20.0/tests/test_predictors/test_base_predictors/test_lp_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_predictors/test_bio_tagger_predictor.py` & `papermage-0.20.0/tests/test_predictors/test_bio_tagger_predictor.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_predictors/test_sentence_predictor.py` & `papermage-0.20.0/tests/test_predictors/test_sentence_predictor.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_predictors/test_span_qa_predictors.py` & `papermage-0.20.0/tests/test_predictors/test_span_qa_predictors.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_predictors/test_vila_predictor.py` & `papermage-0.20.0/tests/test_predictors/test_vila_predictor.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_predictors/test_whitespace_predictor.py` & `papermage-0.20.0/tests/test_predictors/test_whitespace_predictor.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_predictors/test_word_predictor.py` & `papermage-0.20.0/tests/test_predictors/test_word_predictor.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_rasterizers/test_pdf2image_rasterizer.py` & `papermage-0.20.0/tests/test_rasterizers/test_pdf2image_rasterizer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_recipes/test_core_recipe.py` & `papermage-0.20.0/tests/test_recipes/test_core_recipe.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_recipes/test_minimal_pdf_recipe.py` & `papermage-0.20.0/tests/test_recipes/test_minimal_pdf_recipe.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_recipes/test_text_recipe.py` & `papermage-0.20.0/tests/test_recipes/test_text_recipe.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_trainers/test_entity_classification_predictor_trainer.py` & `papermage-0.20.0/tests/test_trainers/test_entity_classification_predictor_trainer.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_utils/test_merge.py` & `papermage-0.20.0/tests/test_utils/test_merge.py`

 * *Files identical despite different names*

### Comparing `papermage-0.19.0/tests/test_visualizers/test_visualizer.py` & `papermage-0.20.0/tests/test_visualizers/test_visualizer.py`

 * *Files identical despite different names*

