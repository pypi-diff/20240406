# Comparing `tmp/brahmai-0.0.1.0.1a3.tar.gz` & `tmp/brahmai-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brahmai-0.0.1.0.1a3.tar", last modified: Sat Apr  6 21:37:23 2024, max compression
+gzip compressed data, was "brahmai-0.0.1a1.tar", last modified: Sat Apr  6 21:41:20 2024, max compression
```

## Comparing `brahmai-0.0.1.0.1a3.tar` & `brahmai-0.0.1a1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.667366 brahmai-0.0.1.0.1a3/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2080 2024-04-06 21:37:23.667366 brahmai-0.0.1.0.1a3/PKG-INFO
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1883 2024-03-29 23:03:15.000000 brahmai-0.0.1.0.1a3/README.md
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.655365 brahmai-0.0.1.0.1a3/brahmai/
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.655365 brahmai-0.0.1.0.1a3/brahmai/ZeroShot/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)       24 2024-04-06 21:19:12.000000 brahmai-0.0.1.0.1a3/brahmai/ZeroShot/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-05 12:27:00.000000 brahmai-0.0.1.0.1a3/brahmai/ZeroShot/image.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1391 2024-04-06 09:36:49.000000 brahmai-0.0.1.0.1a3/brahmai/ZeroShot/text.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1551 2024-04-06 09:26:16.000000 brahmai-0.0.1.0.1a3/brahmai/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      157 2024-04-06 17:37:18.000000 brahmai-0.0.1.0.1a3/brahmai/_globals.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2692 2024-04-06 09:32:43.000000 brahmai-0.0.1.0.1a3/brahmai/chat.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)        0 2024-03-26 22:41:17.000000 brahmai-0.0.1.0.1a3/brahmai/embeddings.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)       82 2024-03-26 22:40:10.000000 brahmai-0.0.1.0.1a3/brahmai/errors.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1148 2024-04-04 23:44:37.000000 brahmai-0.0.1.0.1a3/brahmai/moderations.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.659366 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1757 2024-03-29 17:52:35.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2323 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/analysis_explanation.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)    13921 2024-03-29 17:55:18.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/analyzer_engine.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1457 2024-03-29 17:55:27.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/analyzer_request.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2605 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/analyzer_utils.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      970 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/app_tracer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     5143 2024-03-29 17:56:06.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/batch_analyzer_engine.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.659366 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/context_aware_enhancers/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      222 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/context_aware_enhancers/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2490 2024-03-29 17:58:19.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/context_aware_enhancers/context_aware_enhancer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)    13153 2024-03-29 17:58:38.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/context_aware_enhancers/lemma_context_aware_enhancer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      981 2024-03-29 17:56:18.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/dict_analyzer_result.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     6546 2024-03-29 17:56:29.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/entity_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      186 2024-03-29 17:56:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/local_recognizer.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.659366 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      572 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4627 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/ner_model_configuration.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2802 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/nlp_artifacts.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1501 2024-03-29 17:59:06.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/nlp_engine.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4838 2024-03-29 17:58:58.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/nlp_engine_provider.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     8487 2024-03-29 17:59:16.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/spacy_nlp_engine.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1694 2024-03-29 17:59:22.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/stanza_nlp_engine.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4671 2024-03-29 17:59:29.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/transformers_nlp_engine.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1259 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/pattern.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     9550 2024-03-29 17:56:49.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/pattern_recognizer.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.663365 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3083 2024-03-29 18:04:42.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2594 2024-03-29 17:59:39.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/aba_routing_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3386 2024-03-29 17:59:49.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/au_abn_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3160 2024-03-29 17:59:56.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/au_acn_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3250 2024-03-29 18:00:02.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/au_medicare_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3370 2024-03-29 18:00:09.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/au_tfn_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     6160 2024-03-29 18:00:21.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/azure_ai_language.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2837 2024-03-29 18:00:30.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/credit_card_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4983 2024-03-29 18:00:39.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/crypto_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3062 2024-03-29 18:00:45.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/date_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1458 2024-03-29 18:00:51.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/email_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2084 2024-03-29 18:00:58.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/es_nif_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     8399 2024-03-29 16:16:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/iban_patterns.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     7845 2024-03-29 18:01:17.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/iban_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2612 2024-03-29 18:01:27.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/in_aadhaar_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2359 2024-03-29 18:01:34.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/in_pan_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)    18520 2024-03-29 18:01:53.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/in_vehicle_registration_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2537 2024-03-29 18:01:59.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/ip_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1322 2024-03-29 18:02:05.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_driver_license_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4790 2024-03-29 18:02:11.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_fiscal_code_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2350 2024-03-29 18:02:18.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_identity_card_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1358 2024-03-29 18:02:23.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_passport_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3136 2024-03-29 18:02:29.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_vat_code.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2760 2024-03-29 18:02:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/medical_license_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3482 2024-03-29 18:02:48.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/phone_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1602 2024-03-29 18:02:54.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/pl_pesel_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1395 2024-03-29 18:03:01.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/sg_fin_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     5428 2024-03-29 18:03:07.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/sg_uen_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4748 2024-03-29 18:03:14.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/spacy_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      508 2024-03-29 18:03:22.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/stanza_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      954 2024-03-29 18:03:28.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/transformers_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2633 2024-03-29 18:03:35.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/uk_nhs_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3350 2024-03-29 18:03:42.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/url_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1382 2024-03-29 18:03:47.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_bank_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2327 2024-03-29 18:03:55.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_driver_license_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1675 2024-03-29 18:04:02.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_itin_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1336 2024-03-29 18:04:07.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_passport_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2797 2024-03-29 18:04:14.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_ssn_recognizer.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)    11734 2024-03-29 17:57:10.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/recognizer_registry.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     5910 2024-03-29 17:54:34.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/recognizer_result.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1654 2024-03-29 17:57:22.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/remote_recognizer.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.663365 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      820 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     9933 2024-03-29 18:06:26.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/anonymizer_engine.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3357 2024-03-29 18:06:45.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/batch_anonymizer_engine.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.663365 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/core/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      172 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/core/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4142 2024-03-29 18:10:02.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/core/engine_base.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2245 2024-03-29 18:10:06.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/core/text_replace_builder.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1998 2024-03-29 18:06:54.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/deanonymize_engine.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.667366 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      724 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      675 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/conflict_resolution_strategy.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.667366 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      220 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1027 2024-03-29 18:08:59.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/dict_recognizer_result.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1692 2024-03-29 18:09:06.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/operator_config.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1882 2024-03-29 18:09:19.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/pii_entity.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4136 2024-03-29 18:09:22.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/recognizer_result.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.667366 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/result/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      200 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/result/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1841 2024-03-29 18:09:33.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/result/engine_result.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2009 2024-03-29 18:09:37.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/result/operator_result.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      332 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/invalid_exception.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.667366 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      656 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1701 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/aes_cipher.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1237 2024-03-29 18:07:41.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/custom.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      536 2024-03-29 18:07:45.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/deanonymize_keep.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1373 2024-03-29 18:07:59.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/decrypt.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2022 2024-03-29 18:08:03.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/encrypt.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1528 2024-03-29 18:08:06.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/hash.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1052 2024-03-29 18:08:10.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/keep.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2646 2024-03-29 18:08:15.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/mask.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      972 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/operator.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     5048 2024-03-29 18:08:23.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/operators_factory.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      686 2024-03-29 18:08:26.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/redact.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      945 2024-03-29 18:08:30.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/replace.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.667366 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/services/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)       21 2024-03-29 16:16:36.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/services/__init__.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2189 2024-03-29 18:07:11.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/services/app_entities_convertor.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3255 2024-03-29 18:07:18.000000 brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/services/validators.py
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2791 2024-03-29 18:50:16.000000 brahmai-0.0.1.0.1a3/brahmai/skynet.py
-drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:37:23.655365 brahmai-0.0.1.0.1a3/brahmai.egg-info/
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2080 2024-04-06 21:37:23.000000 brahmai-0.0.1.0.1a3/brahmai.egg-info/PKG-INFO
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     6133 2024-04-06 21:37:23.000000 brahmai-0.0.1.0.1a3/brahmai.egg-info/SOURCES.txt
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)        1 2024-04-06 21:37:23.000000 brahmai-0.0.1.0.1a3/brahmai.egg-info/dependency_links.txt
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      159 2024-04-06 21:37:23.000000 brahmai-0.0.1.0.1a3/brahmai.egg-info/requires.txt
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)        8 2024-04-06 21:37:23.000000 brahmai-0.0.1.0.1a3/brahmai.egg-info/top_level.txt
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)       38 2024-04-06 21:37:23.667366 brahmai-0.0.1.0.1a3/setup.cfg
--rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      638 2024-04-06 21:37:14.000000 brahmai-0.0.1.0.1a3/setup.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.581940 brahmai-0.0.1a1/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2076 2024-04-06 21:41:20.581940 brahmai-0.0.1a1/PKG-INFO
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1883 2024-03-29 23:03:15.000000 brahmai-0.0.1a1/README.md
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.569939 brahmai-0.0.1a1/brahmai/
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.569939 brahmai-0.0.1a1/brahmai/ZeroShot/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)       24 2024-04-06 21:19:12.000000 brahmai-0.0.1a1/brahmai/ZeroShot/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-05 12:27:00.000000 brahmai-0.0.1a1/brahmai/ZeroShot/image.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1391 2024-04-06 09:36:49.000000 brahmai-0.0.1a1/brahmai/ZeroShot/text.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1551 2024-04-06 09:26:16.000000 brahmai-0.0.1a1/brahmai/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      157 2024-04-06 17:37:18.000000 brahmai-0.0.1a1/brahmai/_globals.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2692 2024-04-06 09:32:43.000000 brahmai-0.0.1a1/brahmai/chat.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)        0 2024-03-26 22:41:17.000000 brahmai-0.0.1a1/brahmai/embeddings.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)       82 2024-03-26 22:40:10.000000 brahmai-0.0.1a1/brahmai/errors.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1148 2024-04-04 23:44:37.000000 brahmai-0.0.1a1/brahmai/moderations.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.573939 brahmai-0.0.1a1/brahmai/secnet_analyzer/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1757 2024-03-29 17:52:35.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2323 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/analysis_explanation.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)    13921 2024-03-29 17:55:18.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/analyzer_engine.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1457 2024-03-29 17:55:27.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/analyzer_request.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2605 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/analyzer_utils.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      970 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/app_tracer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     5143 2024-03-29 17:56:06.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/batch_analyzer_engine.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.573939 brahmai-0.0.1a1/brahmai/secnet_analyzer/context_aware_enhancers/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      222 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/context_aware_enhancers/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2490 2024-03-29 17:58:19.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/context_aware_enhancers/context_aware_enhancer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)    13153 2024-03-29 17:58:38.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/context_aware_enhancers/lemma_context_aware_enhancer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      981 2024-03-29 17:56:18.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/dict_analyzer_result.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     6546 2024-03-29 17:56:29.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/entity_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      186 2024-03-29 17:56:36.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/local_recognizer.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.573939 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      572 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4627 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/ner_model_configuration.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2802 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/nlp_artifacts.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1501 2024-03-29 17:59:06.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/nlp_engine.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4838 2024-03-29 17:58:58.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/nlp_engine_provider.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     8487 2024-03-29 17:59:16.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/spacy_nlp_engine.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1694 2024-03-29 17:59:22.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/stanza_nlp_engine.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4671 2024-03-29 17:59:29.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/transformers_nlp_engine.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1259 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/pattern.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     9550 2024-03-29 17:56:49.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/pattern_recognizer.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.577940 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3083 2024-03-29 18:04:42.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2594 2024-03-29 17:59:39.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/aba_routing_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3386 2024-03-29 17:59:49.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/au_abn_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3160 2024-03-29 17:59:56.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/au_acn_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3250 2024-03-29 18:00:02.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/au_medicare_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3370 2024-03-29 18:00:09.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/au_tfn_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     6160 2024-03-29 18:00:21.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/azure_ai_language.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2837 2024-03-29 18:00:30.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/credit_card_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4983 2024-03-29 18:00:39.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/crypto_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3062 2024-03-29 18:00:45.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/date_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1458 2024-03-29 18:00:51.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/email_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2084 2024-03-29 18:00:58.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/es_nif_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     8399 2024-03-29 16:16:15.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/iban_patterns.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     7845 2024-03-29 18:01:17.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/iban_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2612 2024-03-29 18:01:27.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/in_aadhaar_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2359 2024-03-29 18:01:34.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/in_pan_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)    18520 2024-03-29 18:01:53.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/in_vehicle_registration_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2537 2024-03-29 18:01:59.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/ip_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1322 2024-03-29 18:02:05.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_driver_license_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4790 2024-03-29 18:02:11.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_fiscal_code_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2350 2024-03-29 18:02:18.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_identity_card_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1358 2024-03-29 18:02:23.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_passport_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3136 2024-03-29 18:02:29.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_vat_code.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2760 2024-03-29 18:02:36.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/medical_license_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3482 2024-03-29 18:02:48.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/phone_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1602 2024-03-29 18:02:54.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/pl_pesel_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1395 2024-03-29 18:03:01.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/sg_fin_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     5428 2024-03-29 18:03:07.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/sg_uen_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4748 2024-03-29 18:03:14.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/spacy_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      508 2024-03-29 18:03:22.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/stanza_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      954 2024-03-29 18:03:28.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/transformers_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2633 2024-03-29 18:03:35.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/uk_nhs_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3350 2024-03-29 18:03:42.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/url_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1382 2024-03-29 18:03:47.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_bank_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2327 2024-03-29 18:03:55.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_driver_license_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1675 2024-03-29 18:04:02.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_itin_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1336 2024-03-29 18:04:07.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_passport_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2797 2024-03-29 18:04:14.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_ssn_recognizer.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)    11734 2024-03-29 17:57:10.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/recognizer_registry.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     5910 2024-03-29 17:54:34.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/recognizer_result.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1654 2024-03-29 17:57:22.000000 brahmai-0.0.1a1/brahmai/secnet_analyzer/remote_recognizer.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.577940 brahmai-0.0.1a1/brahmai/secnet_anonymizer/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      820 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     9933 2024-03-29 18:06:26.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/anonymizer_engine.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3357 2024-03-29 18:06:45.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/batch_anonymizer_engine.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.577940 brahmai-0.0.1a1/brahmai/secnet_anonymizer/core/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      172 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/core/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4142 2024-03-29 18:10:02.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/core/engine_base.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2245 2024-03-29 18:10:06.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/core/text_replace_builder.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1998 2024-03-29 18:06:54.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/deanonymize_engine.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.577940 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      724 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      675 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/conflict_resolution_strategy.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.577940 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      220 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1027 2024-03-29 18:08:59.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/dict_recognizer_result.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1692 2024-03-29 18:09:06.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/operator_config.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1882 2024-03-29 18:09:19.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/pii_entity.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     4136 2024-03-29 18:09:22.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/recognizer_result.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.577940 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/result/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      200 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/result/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1841 2024-03-29 18:09:33.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/result/engine_result.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2009 2024-03-29 18:09:37.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/result/operator_result.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      332 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/invalid_exception.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.581940 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      656 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1701 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/aes_cipher.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1237 2024-03-29 18:07:41.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/custom.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      536 2024-03-29 18:07:45.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/deanonymize_keep.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1373 2024-03-29 18:07:59.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/decrypt.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2022 2024-03-29 18:08:03.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/encrypt.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1528 2024-03-29 18:08:06.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/hash.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     1052 2024-03-29 18:08:10.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/keep.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2646 2024-03-29 18:08:15.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/mask.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      972 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/operator.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     5048 2024-03-29 18:08:23.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/operators_factory.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      686 2024-03-29 18:08:26.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/redact.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      945 2024-03-29 18:08:30.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/replace.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.581940 brahmai-0.0.1a1/brahmai/secnet_anonymizer/services/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)       21 2024-03-29 16:16:36.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/services/__init__.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2189 2024-03-29 18:07:11.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/services/app_entities_convertor.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     3255 2024-03-29 18:07:18.000000 brahmai-0.0.1a1/brahmai/secnet_anonymizer/services/validators.py
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2791 2024-03-29 18:50:16.000000 brahmai-0.0.1a1/brahmai/skynet.py
+drwxrwxr-x   0 kstyagi   (1000) kstyagi   (1000)        0 2024-04-06 21:41:20.569939 brahmai-0.0.1a1/brahmai.egg-info/
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     2076 2024-04-06 21:41:20.000000 brahmai-0.0.1a1/brahmai.egg-info/PKG-INFO
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)     6133 2024-04-06 21:41:20.000000 brahmai-0.0.1a1/brahmai.egg-info/SOURCES.txt
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)        1 2024-04-06 21:41:20.000000 brahmai-0.0.1a1/brahmai.egg-info/dependency_links.txt
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      159 2024-04-06 21:41:20.000000 brahmai-0.0.1a1/brahmai.egg-info/requires.txt
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)        8 2024-04-06 21:41:20.000000 brahmai-0.0.1a1/brahmai.egg-info/top_level.txt
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)       38 2024-04-06 21:41:20.581940 brahmai-0.0.1a1/setup.cfg
+-rw-rw-r--   0 kstyagi   (1000) kstyagi   (1000)      634 2024-04-06 21:40:57.000000 brahmai-0.0.1a1/setup.py
```

### Comparing `brahmai-0.0.1.0.1a3/PKG-INFO` & `brahmai-0.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brahmai
-Version: 0.0.1.0.1a3
+Version: 0.0.1a1
 Summary: Python SDK to interact with BRAHMAI APIs.
 Author: BRAHMAI
 Author-email: hello@brahmai.in
 Description-Content-Type: text/markdown
 
 ![BRAHMAI](https://brahmai.in/brahmai-banner.png)
 ## Enhancing A.I. Technology for the Betterment of All.
```

### Comparing `brahmai-0.0.1.0.1a3/README.md` & `brahmai-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/ZeroShot/text.py` & `brahmai-0.0.1a1/brahmai/ZeroShot/text.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/__init__.py` & `brahmai-0.0.1a1/brahmai/__init__.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/chat.py` & `brahmai-0.0.1a1/brahmai/chat.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/moderations.py` & `brahmai-0.0.1a1/brahmai/moderations.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/__init__.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/analysis_explanation.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/analysis_explanation.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/analyzer_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/analyzer_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/analyzer_request.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/analyzer_request.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/analyzer_utils.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/analyzer_utils.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/app_tracer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/app_tracer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/batch_analyzer_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/batch_analyzer_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/context_aware_enhancers/context_aware_enhancer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/context_aware_enhancers/context_aware_enhancer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/context_aware_enhancers/lemma_context_aware_enhancer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/context_aware_enhancers/lemma_context_aware_enhancer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/dict_analyzer_result.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/dict_analyzer_result.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/entity_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/entity_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/__init__.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/ner_model_configuration.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/ner_model_configuration.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/nlp_artifacts.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/nlp_artifacts.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/nlp_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/nlp_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/nlp_engine_provider.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/nlp_engine_provider.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/spacy_nlp_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/spacy_nlp_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/stanza_nlp_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/stanza_nlp_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/nlp_engine/transformers_nlp_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/nlp_engine/transformers_nlp_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/pattern.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/pattern.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/pattern_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/pattern_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/__init__.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/__init__.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/aba_routing_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/aba_routing_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/au_abn_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/au_abn_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/au_acn_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/au_acn_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/au_medicare_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/au_medicare_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/au_tfn_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/au_tfn_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/azure_ai_language.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/azure_ai_language.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/credit_card_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/credit_card_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/crypto_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/crypto_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/date_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/date_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/email_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/email_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/es_nif_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/es_nif_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/iban_patterns.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/iban_patterns.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/iban_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/iban_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/in_aadhaar_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/in_aadhaar_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/in_pan_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/in_pan_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/in_vehicle_registration_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/in_vehicle_registration_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/ip_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/ip_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_driver_license_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_driver_license_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_fiscal_code_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_fiscal_code_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_identity_card_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_identity_card_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_passport_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_passport_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/it_vat_code.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/it_vat_code.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/medical_license_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/medical_license_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/phone_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/phone_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/pl_pesel_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/pl_pesel_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/sg_fin_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/sg_fin_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/sg_uen_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/sg_uen_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/spacy_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/spacy_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/transformers_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/transformers_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/uk_nhs_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/uk_nhs_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/url_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/url_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_bank_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_bank_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_driver_license_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_driver_license_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_itin_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_itin_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_passport_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_passport_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/predefined_recognizers/us_ssn_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/predefined_recognizers/us_ssn_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/recognizer_registry.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/recognizer_registry.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/recognizer_result.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/recognizer_result.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_analyzer/remote_recognizer.py` & `brahmai-0.0.1a1/brahmai/secnet_analyzer/remote_recognizer.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/__init__.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/__init__.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/anonymizer_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/anonymizer_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/batch_anonymizer_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/batch_anonymizer_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/core/engine_base.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/core/engine_base.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/core/text_replace_builder.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/core/text_replace_builder.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/deanonymize_engine.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/deanonymize_engine.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/__init__.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/conflict_resolution_strategy.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/conflict_resolution_strategy.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/dict_recognizer_result.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/dict_recognizer_result.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/operator_config.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/operator_config.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/pii_entity.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/pii_entity.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/recognizer_result.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/recognizer_result.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/result/engine_result.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/result/engine_result.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/entities/engine/result/operator_result.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/entities/engine/result/operator_result.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/__init__.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/aes_cipher.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/aes_cipher.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/custom.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/custom.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/deanonymize_keep.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/deanonymize_keep.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/decrypt.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/decrypt.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/encrypt.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/encrypt.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/hash.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/hash.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/keep.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/keep.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/mask.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/mask.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/operator.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/operator.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/operators_factory.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/operators_factory.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/redact.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/redact.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/operators/replace.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/operators/replace.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/services/app_entities_convertor.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/services/app_entities_convertor.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/secnet_anonymizer/services/validators.py` & `brahmai-0.0.1a1/brahmai/secnet_anonymizer/services/validators.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai/skynet.py` & `brahmai-0.0.1a1/brahmai/skynet.py`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/brahmai.egg-info/PKG-INFO` & `brahmai-0.0.1a1/brahmai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brahmai
-Version: 0.0.1.0.1a3
+Version: 0.0.1a1
 Summary: Python SDK to interact with BRAHMAI APIs.
 Author: BRAHMAI
 Author-email: hello@brahmai.in
 Description-Content-Type: text/markdown
 
 ![BRAHMAI](https://brahmai.in/brahmai-banner.png)
 ## Enhancing A.I. Technology for the Betterment of All.
```

### Comparing `brahmai-0.0.1.0.1a3/brahmai.egg-info/SOURCES.txt` & `brahmai-0.0.1a1/brahmai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brahmai-0.0.1.0.1a3/setup.py` & `brahmai-0.0.1a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="brahmai",
-    version="0.0.1.0.1-alpha-3",
+    version="0.0.1-alpha-1",
     author="BRAHMAI",
     author_email="hello@brahmai.in",
     packages=find_packages(),
     install_requires=[
         "spacy-loggers==1.0.5",
         "transformers==4.39.2",
         "tldextract==5.1.2",
```

